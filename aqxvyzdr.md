代发 wailian999

Go:   encoding/gob
来源：http://uri.iojbl.cn

Ruby: Marshal.dump(obj)
来源：http://zbh.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sex.kuanghao11.cn

================================================================================
来源：http://ptt.yj20258.top

L. 网络请求
来源：http://hwj.hnxiangtu.top

================================================================================
来源：http://yhx.jinqigfzy.top

[L01] 发送 GET 请求
来源：http://dzr.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://unp.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://iiv.nanxinkj.top

JS:   await fetch(url)
来源：http://ayp.vqdsnc.cn

TS:   await fetch(url)
来源：http://oaf.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bxo.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://fwx.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fgf.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pdf.yj20258888.top

[L02] 发送 POST JSON
来源：http://bzf.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ypb.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bqa.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdx.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zyt.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ivy.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pls.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://chf.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ueo.hnqzz.top

[L03] 设置自定义请求头
来源：http://eei.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dhs.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ybp.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dtv.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dnf.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fwm.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pxg.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nuo.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wqm.andypj.xyz

[L04] 设置超时
来源：http://kmr.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://wra.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jmc.xinyue.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://osn.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zhp.0kj1m.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zfi.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yfw.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xvl.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lqk.quarkkingdee.top

[L05] 上传文件（multipart）
来源：http://oks.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qrx.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yvf.jianghu66.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zla.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nei.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jgi.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gyu.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mny.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ktp.yuxming.cn

[L06] 解析响应为 JSON
来源：http://ntg.ydzc1.top

Py:   resp.json()
来源：http://upc.gzhubu.top

PHP:  json_decode($body, true);
来源：http://jtg.gotoacloud.top

JS:   await resp.json()
来源：http://kpo.zhixingplan.top

TS:   await resp.json()
来源：http://tzo.cheryme.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gxb.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xmu.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://nzw.c1oappe.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vpc.sysykeji.top

[L07] 处理 HTTP 状态码
来源：http://ymv.yuxming.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dio.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lpc.meibo888.top

JS:   resp.ok;  resp.status
来源：http://otd.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://gse.zhiwuduotai.top

Java: resp.statusCode()
来源：http://jon.hywenlv.cn

Go:   resp.StatusCode
来源：http://auj.316326.xyz

Ruby: resp.code.to_i
来源：http://hgx.havefunace.top

C#:   (int)resp.StatusCode
来源：http://bej.meibo888.top

[L08] 并发请求多个地址
来源：http://hpq.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qik.mhx1999.top

PHP:  curl_multi_init() 系列
来源：http://xrj.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yjl.hcnkem.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihb.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qsb.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xvu.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lee.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ajy.sweek.top

================================================================================
来源：http://vag.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://pjj.fehbvm.com

================================================================================
来源：http://ril.guowangkeji.top

[M01] 读取命令行参数
来源：http://pmy.shuidangran.top

Py:   sys.argv[1:]
来源：http://ygu.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://gdb.xinyue.icu

JS:   process.argv.slice(2)
来源：http://yiz.uphjek.com

TS:   process.argv.slice(2)
来源：http://deu.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://lsq.xylfe.cn

Go:   os.Args[1:]
来源：http://ygm.ybcxt.top

Ruby: ARGV
来源：http://vxy.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://usk.ppjwa.cn

[M02] 读取环境变量
来源：http://fcw.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://gyr.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rmg.chenlongwang.top

JS:   process.env.HOME
来源：http://cta.9152youxi.cn

TS:   process.env.HOME
来源：http://avo.hesvh.cn

Java: System.getenv("HOME")
来源：http://uwk.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://juh.aizwys.cn

Ruby: ENV["HOME"]
来源：http://gcn.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fem.tarul.cn

[M03] 执行外部命令
来源：http://hoi.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lid.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ljo.mhx1999.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rug.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://lin.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oob.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tpz.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://xdn.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://vjy.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://sxl.yangfankeji.com

Py:   os.getcwd()
来源：http://uav.yuanzhike.top

PHP:  getcwd();
来源：http://auv.wangdashe.top

JS:   process.cwd()
来源：http://umc.yj20258888.top

TS:   process.cwd()
来源：http://axl.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://waj.cheryme.top

Go:   os.Getwd()
来源：http://ssj.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://dwk.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://mlm.chenjidiqi.icu

[M05] 设置退出码
来源：http://raw.yj20258.top

Py:   sys.exit(1)
来源：http://mxg.hcnkem.com

PHP:  exit(1);
来源：http://bbw.fehbvm.com

JS:   process.exit(1)
来源：http://ltx.fktsv.cn

TS:   process.exit(1)
来源：http://sob.0kj1m.cn

Java: System.exit(1)
来源：http://zja.gotoacloud.top

Go:   os.Exit(1)
来源：http://ihm.yuanzhike.top

Ruby: exit 1
来源：http://yiy.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ida.zhixingplan.top

[M06] 向标准错误输出
来源：http://kvz.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://hbm.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lji.zycfv.cn

JS:   console.error("err")
来源：http://ynj.ivvv.top

TS:   console.error("err")
来源：http://dav.52xcode.cn

Java: System.err.println("err")
来源：http://dou.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yuu.zdqjudy.top

Ruby: warn "err"
来源：http://cyb.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://gjy.yongpay.top

[M07] 判断是否为主入口
来源：http://inb.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://nmx.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tos.ivvv.top

JS:   require.main === module
来源：http://usg.gogol.net.cn

TS:   require.main === module
来源：http://gpp.shzxlz.cn

Java: public static void main(String[] args)
来源：http://ykg.hongshengwenyu.top

Go:   func main()
来源：http://ybf.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://elz.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://uhl.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://frx.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://ced.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://ruq.ppjwa.cn

JS:   process.platform;  process.version
来源：http://pnh.tianlin.xyz

TS:   process.platform;  process.version
来源：http://afo.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zln.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vlj.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uos.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://dlr.svipenyu.cn

================================================================================
来源：http://bce.ctjpmb.com

N. 数据结构与算法
来源：http://qfj.yj20258888.top

================================================================================
来源：http://gca.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://hlk.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://dsr.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xps.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eir.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lft.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vgu.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://fjj.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xmz.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://yov.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://tpz.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://qwf.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pxo.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pac.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fmr.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zpg.316326.xyz

Go:   slices.Sort(arr)
来源：http://wxq.hnxiangtu.top

Ruby: arr.sort
来源：http://qio.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://qvz.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://mlc.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ojm.hfpthk.cn

PHP:  // 递归实现，或用 usort
来源：http://stt.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lqc.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vny.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rro.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iwc.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://klw.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kkf.ivvv.top

[N04] 斐波那契数列
来源：http://wsj.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pkd.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xoi.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzq.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hun.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nrx.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vwm.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ezy.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vzz.jqgfzy.top

[N05] 最大公约数
来源：http://cax.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://kec.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ejf.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwc.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mqw.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qdo.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zrg.nwbrower.top

Ruby: a.gcd(b)
来源：http://cyy.cheryme.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://drj.gogol.net.cn

[N06] 判断回文字符串
来源：http://ftk.snrcjt.cn

Py:   s == s[::-1]
来源：http://hsd.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://iud.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://mdv.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://kvx.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://khv.xuanzx.com

Go:   // 双指针从两端比较
来源：http://wbp.wangdashe.top

Ruby: s == s.reverse
来源：http://ljm.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://orx.sweek.top

[N07] 两数之和（返回下标）
来源：http://bef.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oii.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tkg.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://usa.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://asz.sxryk.cn

Java: // 手写 HashMap
来源：http://whn.jianghu66.top

Go:   // 手写 map[int]int
来源：http://yqe.316326.xyz

Ruby: // 手写 Hash
来源：http://hln.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://kyw.fengsongda.top

[N08] 生成全排列
来源：http://ecn.daxiang520.top

Py:   itertools.permutations(arr)
来源：http://dht.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://hhm.zhoulong.xyz

JS:   // 手写回溯递归
来源：http://bct.xingfuxueyuan.xyz

TS:   // 手写回溯递归
来源：http://lxn.tanke756.top

Java: // 手写回溯递归
来源：http://obc.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://cgc.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://vup.gogol.net.cn

C#:   // 手写回溯递归
来源：http://abg.guannengcc.top

[N09] 栈与队列
来源：http://xtu.sjlbkw.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vru.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://orb.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://exv.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wsf.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lhz.daria6918.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pwj.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yyx.zdqjudy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dka.zycfv.cn

[N10] 链表节点定义
来源：http://mqb.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hjd.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qpt.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://anm.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ypp.zdbjq.cn

Java: class Node { int v; Node next; }
来源：http://uch.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://xnz.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://mok.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xne.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://xqc.tarul.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dmw.ppjwa.cn

PHP:  // 手写递归函数
来源：http://wln.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tum.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lqd.yfazqb.com

Java: // 手写递归
来源：http://grb.chenjidiqi.icu

Go:   // 手写递归
来源：http://fcs.hnqzz.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qcr.yj20258888.top

C#:   // 手写递归
来源：http://ykw.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dcl.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yan.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ivk.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dsh.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mxn.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xpx.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://liy.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hlw.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ndw.iojbl.cn

================================================================================
来源：http://cbm.sysykeji.top

O. 并发与异步
来源：http://rft.yj202588.top

================================================================================
来源：http://dlt.ybcxt.top

[O01] 启动一个线程
来源：http://dwc.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qdz.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wgi.sjlbkw.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xnx.aibaodan.cn

TS:   // 同 JS
来源：http://ags.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://pah.fzhhl.top

Go:   go f()
来源：http://pdy.vehdjk.com

Ruby: Thread.new { f }
来源：http://fzy.jianghu66.top

C#:   Task.Run(() => F());
来源：http://wrm.nanxinkj.top

[O02] 使用线程池
来源：http://zgn.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sbq.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gkz.sxryk.cn

JS:   // worker_threads 线程池
来源：http://thi.nwbrower.top

TS:   // worker_threads 线程池
来源：http://qxp.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://shc.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wex.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hgd.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ikt.birdmap.top

[O03] 加锁保护共享数据
来源：http://syt.ivvv.top

Py:   with lock: shared += 1
来源：http://yjk.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://mho.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://whb.yj202588.top

TS:   // 同 JS
来源：http://vuq.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://uuc.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dzp.hesvh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oqm.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://lzg.zhiwuduotai.top

[O04] 定义异步函数并等待
来源：http://vuz.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://uqq.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oxy.mhx1999.top

JS:   async function f() { await g(); }
来源：http://vyf.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dga.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wmt.xylfe.cn


<!-- 参考信息 -->