代发 wailian999

L. 网络请求
来源：http://ztb.yuanzhike.top

================================================================================
来源：http://tvz.tarul.cn

[L01] 发送 GET 请求
来源：http://bxq.hcnkem.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yjn.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hoj.cqqwz.cn

JS:   await fetch(url)
来源：http://cjc.ybcxt.top

TS:   await fetch(url)
来源：http://zna.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ybr.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://ytl.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ewz.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ouc.gotoacloud.top

[L02] 发送 POST JSON
来源：http://lkf.chenlongwang.top

Py:   requests.post(url, json={"a": 1})
来源：http://awk.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sid.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iff.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://laq.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://brq.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nqk.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pqp.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://peu.hammf.cn

[L03] 设置自定义请求头
来源：http://tev.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yam.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jbv.0kj1m.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iez.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://omq.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vuw.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ycf.havefunace.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uzb.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dzb.bbcook.cn

[L04] 设置超时
来源：http://wyu.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://lbm.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mfe.yuxming.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ypc.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://all.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://omw.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wym.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fqw.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vbr.yvedp.cn

[L05] 上传文件（multipart）
来源：http://ljo.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://axu.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jtv.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zra.daxiang520.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qka.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://glp.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hsj.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aip.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sgk.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://lkx.smart0.xyz

Py:   resp.json()
来源：http://tzk.cucudq.cn

PHP:  json_decode($body, true);
来源：http://kjx.iojbl.cn

JS:   await resp.json()
来源：http://vod.ehwqpu.com

TS:   await resp.json()
来源：http://pwl.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rgt.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xxq.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://hmv.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bqw.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://odw.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rbg.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gwk.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://mzo.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://btl.fktsv.cn

Java: resp.statusCode()
来源：http://jlg.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://eby.hysaishi.cn

Ruby: resp.code.to_i
来源：http://xfx.uphjek.com

C#:   (int)resp.StatusCode
来源：http://shu.hcnkem.com

[L08] 并发请求多个地址
来源：http://sml.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gvi.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://qpa.xuetiantiany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oox.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vhm.wangdashe.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qfq.hysaishi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kwk.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fpc.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ddj.yangfankeji.com

================================================================================
来源：http://byg.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://sim.316326.xyz

================================================================================
来源：http://xkk.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://hxo.ctjpmb.com

Py:   sys.argv[1:]
来源：http://meg.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://hsb.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://own.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://kri.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://uje.birdmap.top

Go:   os.Args[1:]
来源：http://jdt.ybcxt.top

Ruby: ARGV
来源：http://wlg.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://ggf.wangshuangyany.cn

[M02] 读取环境变量
来源：http://fwp.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://ngd.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://igg.hongshengwenyu.top

JS:   process.env.HOME
来源：http://szi.haohaochexian.top

TS:   process.env.HOME
来源：http://fuk.xinyue.icu

Java: System.getenv("HOME")
来源：http://fol.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gfd.ivvv.top

Ruby: ENV["HOME"]
来源：http://nhk.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rqz.bjfxy.top

[M03] 执行外部命令
来源：http://ygy.meibo888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gof.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vku.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vuh.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://rdl.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://den.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jkz.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://wdq.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://baf.ppjwa.cn

[M04] 获取当前工作目录
来源：http://zio.aibaodan.cn

Py:   os.getcwd()
来源：http://uxy.yangfankeji.com

PHP:  getcwd();
来源：http://tlb.ehwqpu.com

JS:   process.cwd()
来源：http://rfd.sysykeji.top

TS:   process.cwd()
来源：http://mnh.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://yma.hammf.cn

Go:   os.Getwd()
来源：http://ygc.havefunace.top

Ruby: Dir.pwd
来源：http://jym.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://ecs.yuanzhike.top

[M05] 设置退出码
来源：http://dur.hywenlv.cn

Py:   sys.exit(1)
来源：http://xvd.fehbvm.com

PHP:  exit(1);
来源：http://mpd.ctjpmb.com

JS:   process.exit(1)
来源：http://lmw.ctjpmb.com

TS:   process.exit(1)
来源：http://vri.ybcxt.top

Java: System.exit(1)
来源：http://fyu.ctjpmb.com

Go:   os.Exit(1)
来源：http://lhr.shanyushiyangtech.top

Ruby: exit 1
来源：http://nos.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lip.zhoulong.xyz

[M06] 向标准错误输出
来源：http://nhv.zhiwuduotai.top

Py:   print("err", file=sys.stderr)
来源：http://hyx.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jrb.fehbvm.com

JS:   console.error("err")
来源：http://iwq.uphjek.com

TS:   console.error("err")
来源：http://hfk.snrcjt.cn

Java: System.err.println("err")
来源：http://dmt.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nmb.dashuyun.cn

Ruby: warn "err"
来源：http://yft.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://wnb.dianchejie.cn

[M07] 判断是否为主入口
来源：http://qrq.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://buj.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mig.tanke756.top

JS:   require.main === module
来源：http://ctx.cdnleiting.top

TS:   require.main === module
来源：http://tfz.uphjek.com

Java: public static void main(String[] args)
来源：http://buc.quarkkingdee.top

Go:   func main()
来源：http://jnh.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ohw.cucudq.cn

C#:   static void Main(string[] args)
来源：http://rpn.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://auv.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://cpr.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://wbh.iojbl.cn

JS:   process.platform;  process.version
来源：http://gcf.yj20258888.top

TS:   process.platform;  process.version
来源：http://mub.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://axx.jianghu66.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zpb.hysaishi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://svi.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nsn.shanyushiyangkeji.top

================================================================================
来源：http://eju.sufxvd.cn

N. 数据结构与算法
来源：http://pof.tianlin.xyz

================================================================================
来源：http://quj.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://iof.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://qrf.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jch.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hkg.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fsx.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://cug.hammf.cn

Go:   sort.SearchInts(arr, x)
来源：http://ttx.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xlw.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://ats.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://lrm.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://qoo.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nxs.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mpd.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pts.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xpa.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://qxw.gotoacloud.top

Ruby: arr.sort
来源：http://gzs.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wao.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://wws.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bex.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://drk.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vrm.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tki.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dcl.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ssc.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bkt.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://prb.redwolf501.top

[N04] 斐波那契数列
来源：http://bix.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qjc.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ane.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fda.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kqt.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ihk.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ans.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rrh.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iau.xinyue.icu

[N05] 最大公约数
来源：http://gdu.meibo888.top

Py:   math.gcd(a, b)
来源：http://yab.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hue.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hux.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ulv.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iyh.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://scv.yuanzhike.top

Ruby: a.gcd(b)
来源：http://cka.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dor.hysaishi.cn

[N06] 判断回文字符串
来源：http://mcw.zhongyouzk.top

Py:   s == s[::-1]
来源：http://gcl.sxryk.cn

PHP:  $s === strrev($s);
来源：http://hqt.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://yrd.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://ggf.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ivz.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://abd.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://dwj.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kro.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://utv.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qgm.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://whh.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fyp.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://cpc.aizwys.cn

Java: // 手写 HashMap
来源：http://szl.guannengcc.top

Go:   // 手写 map[int]int
来源：http://jmz.hfpthk.cn

Ruby: // 手写 Hash
来源：http://ycf.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://lsl.ydzc1.top

[N08] 生成全排列
来源：http://als.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://ako.jianghu66.top

PHP:  // 手写递归交换
来源：http://cyf.nwbrower.top

JS:   // 手写回溯递归
来源：http://gyx.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://bew.yuxming.cn

Java: // 手写回溯递归
来源：http://rio.zdbjq.cn

Go:   // 手写回溯递归
来源：http://gzd.zhengqikj.top

Ruby: arr.permutation.to_a
来源：http://qoa.cdnleiting.top

C#:   // 手写回溯递归
来源：http://jcj.zhaomingkeji.xyz

[N09] 栈与队列
来源：http://fyx.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sva.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xrn.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cnn.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fip.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lyq.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://boi.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kpa.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tvt.sysykeji.top

[N10] 链表节点定义
来源：http://pmz.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zvl.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://sca.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dkw.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dnh.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://htf.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://tbq.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ard.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jgl.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://ljj.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iyq.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://puk.zhengqikj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qgi.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nut.hywenlv.cn

Java: // 手写递归
来源：http://mbn.shzxlz.cn

Go:   // 手写递归
来源：http://nrq.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bqb.pengpengdd.cyou

C#:   // 手写递归
来源：http://zbo.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cgu.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://euw.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hkd.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bhm.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pks.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tet.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ila.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eox.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hrr.birdmap.top

================================================================================
来源：http://itd.hysaishi.cn

O. 并发与异步
来源：http://bzy.xuetiantiany.cn

================================================================================
来源：http://tiw.fktsv.cn

[O01] 启动一个线程
来源：http://jlh.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iid.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aog.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://otb.chenjidiqi.icu

TS:   // 同 JS
来源：http://jvk.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://zwr.smart0.xyz

Go:   go f()
来源：http://qlu.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://jla.yueranfly.top

C#:   Task.Run(() => F());
来源：http://ung.jianghu66.top

[O02] 使用线程池
来源：http://kti.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://usj.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vzb.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://zek.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://vui.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://rss.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jem.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nne.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fnd.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://xrs.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://edp.jqgufenzy.top

PHP:  // 用 flock() 做文件锁
来源：http://obe.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pgg.yuanzhike.top

TS:   // 同 JS
来源：http://xoe.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://hpi.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ilp.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://nga.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://oml.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://cgb.cashguo.top

Py:   async def f():⏎    await g()
来源：http://ynn.hongshengwenyu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uyr.ybcxt.top

JS:   async function f() { await g(); }
来源：http://eho.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://eog.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lwx.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ngu.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://dlx.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://ipv.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://swz.guannengcc.top


<!-- 参考信息 -->