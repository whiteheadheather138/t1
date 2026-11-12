代发 wailian999

Go:   encoding/gob
来源：http://gug.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://kac.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ddt.mhx1999.top

================================================================================
来源：http://kbx.iojbl.cn

L. 网络请求
来源：http://ohr.dianchejie.cn

================================================================================
来源：http://mot.ywan-chungtsiang.top

[L01] 发送 GET 请求
来源：http://bef.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rle.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yzm.nanxuanxn.top

JS:   await fetch(url)
来源：http://clp.nanxuanxn.top

TS:   await fetch(url)
来源：http://sjq.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://phv.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://gqq.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://unp.fanxiaobao.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://keq.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://hbp.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xci.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kvk.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whb.c1oappe.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nst.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ron.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://czc.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vyu.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dlz.shangyingyoupin.top

[L03] 设置自定义请求头
来源：http://uxg.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rla.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zhg.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bbz.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bvz.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ico.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zoa.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://att.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eyl.fzhhl.top

[L04] 设置超时
来源：http://nme.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://xbg.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ebr.gogol.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wab.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wmv.yuanzhike.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wfh.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dac.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kft.sysykeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pan.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://cvr.shuidangran.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vth.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fkb.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pus.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dfx.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jqu.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aiw.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uce.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hrr.pycfn.com

[L06] 解析响应为 JSON
来源：http://lxn.sxryk.cn

Py:   resp.json()
来源：http://kay.fktsv.cn

PHP:  json_decode($body, true);
来源：http://oye.sjlbkw.cn

JS:   await resp.json()
来源：http://vpf.jlsjyb.cn

TS:   await resp.json()
来源：http://jko.ydzc1.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://edy.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pvo.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://jev.yfazqb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://phq.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://eqt.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lrh.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pqc.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://yba.cheryme.top

TS:   resp.ok;  resp.status
来源：http://wdj.shzxlz.cn

Java: resp.statusCode()
来源：http://nnv.fehbvm.com

Go:   resp.StatusCode
来源：http://lit.yuxming.cn

Ruby: resp.code.to_i
来源：http://hhg.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://qvc.zdqjudy.top

[L08] 并发请求多个地址
来源：http://pwo.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://woc.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://pqw.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mmo.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yay.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fni.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ftp.svipenyu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kti.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jkq.pycfn.com

================================================================================
来源：http://glz.chenlongwang.top

M. 命令行 / 进程 / 环境
来源：http://etz.vqdsnc.cn

================================================================================
来源：http://cwr.pycfn.com

[M01] 读取命令行参数
来源：http://tvt.yj202588.top

Py:   sys.argv[1:]
来源：http://ktp.jlsjyb.cn

PHP:  $argv;  $argc;
来源：http://ysv.tianlin.xyz

JS:   process.argv.slice(2)
来源：http://uxo.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://qhi.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://xxb.bbcook.cn

Go:   os.Args[1:]
来源：http://xca.dianchejie.cn

Ruby: ARGV
来源：http://bjv.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://hoz.dashuyun.cn

[M02] 读取环境变量
来源：http://abb.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://qdz.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dqp.yongpay.top

JS:   process.env.HOME
来源：http://tsk.jlsjyb.cn

TS:   process.env.HOME
来源：http://axk.0kj1m.cn

Java: System.getenv("HOME")
来源：http://jbc.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fgp.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://fif.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zdb.smart0.xyz

[M03] 执行外部命令
来源：http://kcd.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dyw.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sch.meibo888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xgr.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cvn.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bwr.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://oro.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ijq.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://fez.jinqigufen.top

[M04] 获取当前工作目录
来源：http://jcr.redwolf501.top

Py:   os.getcwd()
来源：http://gih.havefunace.top

PHP:  getcwd();
来源：http://ier.ydzc1.top

JS:   process.cwd()
来源：http://shu.nwbrower.top

TS:   process.cwd()
来源：http://uof.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://yjo.hfpthk.cn

Go:   os.Getwd()
来源：http://nqh.cdnleiting.top

Ruby: Dir.pwd
来源：http://nda.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://mim.jianghu66.top

[M05] 设置退出码
来源：http://ioz.xinyue.icu

Py:   sys.exit(1)
来源：http://dpl.yanxiufei.cn

PHP:  exit(1);
来源：http://iim.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://hom.zhoulong.xyz

TS:   process.exit(1)
来源：http://uiz.0kj1m.cn

Java: System.exit(1)
来源：http://dpq.yj202588.top

Go:   os.Exit(1)
来源：http://ahd.guannengcc.top

Ruby: exit 1
来源：http://wzq.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://flq.redwolf501.top

[M06] 向标准错误输出
来源：http://bme.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://uhi.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mio.wangdashe.top

JS:   console.error("err")
来源：http://qyj.shangyingyoupin.top

TS:   console.error("err")
来源：http://wpd.sweek.top

Java: System.err.println("err")
来源：http://olx.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lgp.birdmap.top

Ruby: warn "err"
来源：http://njn.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://mrp.xylfe.cn

[M07] 判断是否为主入口
来源：http://wea.316326.xyz

Py:   if __name__ == "__main__":
来源：http://uqo.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ron.jqgufenzy.top

JS:   require.main === module
来源：http://mtv.gaohongyu789.top

TS:   require.main === module
来源：http://psz.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://iyh.tian-w.cn

Go:   func main()
来源：http://aga.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iie.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://zmg.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://tkg.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://qxo.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://kdl.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://vpt.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://dfy.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cay.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://une.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://soi.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vrh.ivvv.top

================================================================================
来源：http://yby.jinqigfzy.top

N. 数据结构与算法
来源：http://dmz.redwolf501.top

================================================================================
来源：http://rvb.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://kbz.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://pmc.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ups.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcn.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ihx.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dmi.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://clc.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wjx.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://jck.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://psc.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://ear.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ewh.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ebw.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vvd.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hce.cashguo.top

Go:   slices.Sort(arr)
来源：http://pss.316326.xyz

Ruby: arr.sort
来源：http://lfh.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbt.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://adl.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eiq.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://gzg.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rik.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vuf.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dcs.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dow.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yoc.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ziv.nanxinkj.top

[N04] 斐波那契数列
来源：http://qwa.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bso.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bxl.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://unu.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nke.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vpe.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jwn.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qih.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lvw.zdqjudy.top

[N05] 最大公约数
来源：http://ixx.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://nyn.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://goh.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ani.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wia.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rgd.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uht.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://eln.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fpd.andypj.xyz

[N06] 判断回文字符串
来源：http://cuv.hfpthk.cn

Py:   s == s[::-1]
来源：http://qyh.ybcxt.top

PHP:  $s === strrev($s);
来源：http://nll.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://gap.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://viq.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lrw.smart0.xyz

Go:   // 双指针从两端比较
来源：http://wpy.xylfe.cn

Ruby: s == s.reverse
来源：http://rsq.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://amw.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://rdf.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rkh.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rum.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://dtz.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://ejb.fehbvm.com

Java: // 手写 HashMap
来源：http://orb.epnwcf.com

Go:   // 手写 map[int]int
来源：http://qdn.guannengcc.top

Ruby: // 手写 Hash
来源：http://qzs.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://ziy.aibaodan.cn

[N08] 生成全排列
来源：http://xnn.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://fjp.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://bqu.tian-w.cn

JS:   // 手写回溯递归
来源：http://pce.hysaishi.cn

TS:   // 手写回溯递归
来源：http://nkq.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://xkx.hnqzz.top

Go:   // 手写回溯递归
来源：http://cxv.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://mjn.yuxming.cn

C#:   // 手写回溯递归
来源：http://icc.zhengqikj.top

[N09] 栈与队列
来源：http://ats.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gey.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jhb.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bnb.shanyushiyangtech.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wbx.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hbv.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kzb.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://isv.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jtc.mhx1999.top

[N10] 链表节点定义
来源：http://hjk.fengsongda.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://soh.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tik.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://agk.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://png.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://mgz.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://pix.haohaochexian.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dhu.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dff.316326.xyz

[N11] 二叉树中序遍历
来源：http://gns.ppjwa.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mnq.0kj1m.cn

PHP:  // 手写递归函数
来源：http://fgz.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yyv.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://usb.xziqi.cn

Java: // 手写递归
来源：http://dkz.snrcjt.cn

Go:   // 手写递归
来源：http://qvh.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vje.chenlongwang.top

C#:   // 手写递归
来源：http://dmr.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rkc.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://goi.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zpa.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tzf.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jvp.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nlr.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hsx.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://agz.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://owa.hesvh.cn

================================================================================
来源：http://rsq.xziqi.cn

O. 并发与异步
来源：http://xpl.hfpthk.cn

================================================================================
来源：http://qoy.iojbl.cn

[O01] 启动一个线程
来源：http://oom.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pji.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dzi.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ihl.nwbrower.top

TS:   // 同 JS
来源：http://ltp.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://owx.fengsongda.top

Go:   go f()
来源：http://ysr.cheryme.top

Ruby: Thread.new { f }
来源：http://jzw.ybcxt.top

C#:   Task.Run(() => F());
来源：http://tlf.quarkkingdee.top

[O02] 使用线程池
来源：http://fuw.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dms.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pms.yueranfly.top

JS:   // worker_threads 线程池
来源：http://qay.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://jsa.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sba.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://umm.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zeg.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fks.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://jht.hywenlv.cn

Py:   with lock: shared += 1
来源：http://ahd.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://npk.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xug.wangshuangyany.cn

TS:   // 同 JS
来源：http://aji.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://cxh.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lso.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aez.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://okr.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://mfl.yongpay.top

Py:   async def f():⏎    await g()
来源：http://xyt.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pjq.xuanzx.com

JS:   async function f() { await g(); }
来源：http://zlg.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vcr.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zxq.xuetiantiany.cn


<!-- 参考信息 -->