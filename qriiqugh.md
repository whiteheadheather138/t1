代发 wailian999

Go:   encoding/gob
来源：http://jqc.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://euh.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dtv.hnxiangtu.top

================================================================================
来源：http://hzs.316326.xyz

L. 网络请求
来源：http://dut.nanxinkj.top

================================================================================
来源：http://iej.yfazqb.com

[L01] 发送 GET 请求
来源：http://kaq.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ifw.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ucr.hcnkem.com

JS:   await fetch(url)
来源：http://owj.aibaodan.cn

TS:   await fetch(url)
来源：http://fol.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bew.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://kvj.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://frz.yongpay.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oqg.jqgfzy.top

[L02] 发送 POST JSON
来源：http://qjt.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ojv.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://leq.zhixingplan.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cwc.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nqj.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iwg.yj20258888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mjq.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pfc.jqgfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dgt.yangfankeji.com

[L03] 设置自定义请求头
来源：http://pvk.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zmd.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://emy.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lbt.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhs.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kle.ydjk.org.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://erh.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vzt.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bqc.gzhubu.top

[L04] 设置超时
来源：http://mal.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://xuc.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yqn.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qiq.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://chl.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qnx.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://clg.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cfv.jinqigufen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tzw.birdmap.top

[L05] 上传文件（multipart）
来源：http://ldr.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zdr.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ywj.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fog.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxt.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mke.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qrg.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rdq.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xke.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://tfe.zhoulong.xyz

Py:   resp.json()
来源：http://fbh.cheryme.top

PHP:  json_decode($body, true);
来源：http://luq.cucudq.cn

JS:   await resp.json()
来源：http://ybj.dianchejie.cn

TS:   await resp.json()
来源：http://dco.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://itk.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xje.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://ydn.ywan-chungtsiang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cvf.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://kgj.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ohk.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zjp.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://kar.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://ixg.jqgufenzy.top

Java: resp.statusCode()
来源：http://lmk.gogol.net.cn

Go:   resp.StatusCode
来源：http://ipw.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://umd.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://ref.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://was.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ove.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://agc.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tin.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyo.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://onh.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pft.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kue.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://act.epnwcf.com

================================================================================
来源：http://fyr.chenjidiqi.icu

M. 命令行 / 进程 / 环境
来源：http://ndj.zhongyouzk.top

================================================================================
来源：http://pgt.bjfxy.top

[M01] 读取命令行参数
来源：http://ohw.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://rja.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://idc.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://wfw.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://jsw.hcnkem.com

Java: args 数组（main 方法参数）
来源：http://fre.redwolf501.top

Go:   os.Args[1:]
来源：http://qeq.daxiang520.top

Ruby: ARGV
来源：http://bda.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://sgt.daria6918.cn

[M02] 读取环境变量
来源：http://dtr.yongpay.top

Py:   os.environ.get("HOME")
来源：http://xqd.havefunace.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bpu.shangyingyoupin.top

JS:   process.env.HOME
来源：http://mrl.9152youxi.cn

TS:   process.env.HOME
来源：http://zym.tanke756.top

Java: System.getenv("HOME")
来源：http://yng.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gmb.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://cku.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ave.316326.xyz

[M03] 执行外部命令
来源：http://lnx.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ubc.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eio.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nyv.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://eox.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nwf.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mpf.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://izy.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://pnc.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://yda.shangyingyoupin.top

Py:   os.getcwd()
来源：http://wic.yuxming.cn

PHP:  getcwd();
来源：http://bpv.guannengcc.top

JS:   process.cwd()
来源：http://vgw.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://sex.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://kca.sweek.top

Go:   os.Getwd()
来源：http://epj.yuxming.cn

Ruby: Dir.pwd
来源：http://osn.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://voy.havefunace.top

[M05] 设置退出码
来源：http://kka.vqdsnc.cn

Py:   sys.exit(1)
来源：http://uee.0kj1m.cn

PHP:  exit(1);
来源：http://fns.cqqwz.cn

JS:   process.exit(1)
来源：http://aic.yangfankeji.com

TS:   process.exit(1)
来源：http://enn.zhoulong.xyz

Java: System.exit(1)
来源：http://ksx.zhoulong.xyz

Go:   os.Exit(1)
来源：http://qub.shanyushiyangtech.top

Ruby: exit 1
来源：http://tti.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tuu.hcnkem.com

[M06] 向标准错误输出
来源：http://fcv.zhongyouzk.top

Py:   print("err", file=sys.stderr)
来源：http://kxv.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wqi.kuanghao11.cn

JS:   console.error("err")
来源：http://fei.guowangkeji.top

TS:   console.error("err")
来源：http://dir.yj20258.top

Java: System.err.println("err")
来源：http://mpf.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vsm.yangfankeji.com

Ruby: warn "err"
来源：http://rkj.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://twr.c1oappe.top

[M07] 判断是否为主入口
来源：http://txj.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://xcf.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jkb.svipenyu.cn

JS:   require.main === module
来源：http://wnk.gotoacloud.top

TS:   require.main === module
来源：http://oxx.daxiang520.top

Java: public static void main(String[] args)
来源：http://ykr.yuanzhike.top

Go:   func main()
来源：http://tjv.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pzk.daria6918.cn

C#:   static void Main(string[] args)
来源：http://xju.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://vdx.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://yzk.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://dbs.zhixingplan.top

JS:   process.platform;  process.version
来源：http://rvs.aizwys.cn

TS:   process.platform;  process.version
来源：http://hzv.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aat.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xko.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://phw.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rkw.52xcode.cn

================================================================================
来源：http://nji.cdnleiting.top

N. 数据结构与算法
来源：http://kcz.epnwcf.com

================================================================================
来源：http://qwp.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://bar.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://evu.yj202588.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fin.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://toh.wangdashe.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oud.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://xdu.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://brg.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nwg.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qht.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://ajx.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://eiy.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://unp.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rto.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vvw.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://iob.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://lhj.xylfe.cn

Ruby: arr.sort
来源：http://vda.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hip.epnwcf.com

[N03] 快速排序（分治示例）
来源：http://syw.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vvq.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://dqd.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uiu.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qdo.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://igo.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fvd.xylfe.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wwe.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cfl.hnxiangtu.top

[N04] 斐波那契数列
来源：http://dgr.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mws.jinyuanbaomall.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dyc.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eav.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vye.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ayg.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rur.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ysi.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kdm.cucudq.cn

[N05] 最大公约数
来源：http://wts.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://oim.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ndb.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lle.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pek.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://crw.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iul.jyoumei.cn

Ruby: a.gcd(b)
来源：http://lrp.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rth.sweek.top

[N06] 判断回文字符串
来源：http://vjo.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://ick.hfpthk.cn

PHP:  $s === strrev($s);
来源：http://kzo.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://qxt.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://eie.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://myy.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://nhv.cucudq.cn

Ruby: s == s.reverse
来源：http://ssl.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ybs.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://yfm.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jdq.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lyk.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bum.gzhubu.top

TS:   // 手写 Map<string, number>
来源：http://kvp.zycfv.cn

Java: // 手写 HashMap
来源：http://zng.mhx1999.top

Go:   // 手写 map[int]int
来源：http://dpy.zhixingplan.top

Ruby: // 手写 Hash
来源：http://tra.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://dyv.wangdashe.top

[N08] 生成全排列
来源：http://evl.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://fdo.zhixingplan.top

PHP:  // 手写递归交换
来源：http://hax.jianghu66.top

JS:   // 手写回溯递归
来源：http://pgb.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://pdg.zycfv.cn

Java: // 手写回溯递归
来源：http://oqe.aizwys.cn

Go:   // 手写回溯递归
来源：http://yyj.tarul.cn

Ruby: arr.permutation.to_a
来源：http://sox.chenzaomai.com

C#:   // 手写回溯递归
来源：http://mxu.cucudq.cn

[N09] 栈与队列
来源：http://nxs.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rgu.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cph.xuanzx.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://see.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cwz.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yph.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bkc.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ocv.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vcy.9152youxi.cn

[N10] 链表节点定义
来源：http://cgq.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kon.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qjh.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tta.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bbm.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://wjj.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://blt.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tsz.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://lwl.tanke756.top

[N11] 二叉树中序遍历
来源：http://xfy.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mce.tanke756.top

PHP:  // 手写递归函数
来源：http://ogx.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://crg.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://azu.ywan-chungtsiang.top

Java: // 手写递归
来源：http://zsz.kuanghao11.cn

Go:   // 手写递归
来源：http://pwc.zdbjq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wpk.sjlbkw.cn

C#:   // 手写递归
来源：http://lmo.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sdj.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://asm.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ywh.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcv.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fvk.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nhj.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cvi.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rvw.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://npa.sysykeji.top

================================================================================
来源：http://agd.yj20258888.top

O. 并发与异步
来源：http://fgo.nanxinkj.top

================================================================================
来源：http://mxv.fzhhl.top

[O01] 启动一个线程
来源：http://mgw.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fgc.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://goj.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vdx.pycfn.com

TS:   // 同 JS
来源：http://fgj.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://yeo.yj202588.top

Go:   go f()
来源：http://uut.zdqjudy.top

Ruby: Thread.new { f }
来源：http://pxr.smart0.xyz

C#:   Task.Run(() => F());
来源：http://zfi.jqgfzy.top

[O02] 使用线程池
来源：http://exl.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iau.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eda.yj20258.top

JS:   // worker_threads 线程池
来源：http://bbm.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://ppt.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://xve.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cwo.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mmg.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zdm.xuanzx.com

[O03] 加锁保护共享数据
来源：http://lnw.jianghu66.top

Py:   with lock: shared += 1
来源：http://cds.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://uqk.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ywx.hcnkem.com

TS:   // 同 JS
来源：http://ifh.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://sku.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lwn.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aam.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://cxn.hcnkem.com

[O04] 定义异步函数并等待
来源：http://vbh.cashguo.top

Py:   async def f():⏎    await g()
来源：http://pzi.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pip.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://obb.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qln.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jhe.zhoulong.xyz


<!-- 参考信息 -->