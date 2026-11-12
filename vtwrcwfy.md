代发 wailian999

L. 网络请求
来源：http://mib.xuetiantiany.cn

================================================================================
来源：http://jdq.hcnkem.com

[L01] 发送 GET 请求
来源：http://ipf.shanyushiyangtech.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ykr.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://duz.ydzc1.top

JS:   await fetch(url)
来源：http://ygn.snrcjt.cn

TS:   await fetch(url)
来源：http://yrv.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tfm.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://zes.xziqi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ihr.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kit.nwbrower.top

[L02] 发送 POST JSON
来源：http://btt.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lzw.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zrf.hesvh.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbg.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://afm.yj202588.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qdn.gotoacloud.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://drf.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://obi.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://njg.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://mpy.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vus.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://czb.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hyj.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qil.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lfz.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zih.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://het.bbcook.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yof.ydzc1.top

[L04] 设置超时
来源：http://dzd.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://kcx.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vqn.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zve.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjo.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://gre.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blg.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://knf.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ejk.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://ree.fzhhl.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://izt.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vvj.daxiang520.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xsx.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tru.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cnj.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vfd.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uow.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dmy.tarul.cn

[L06] 解析响应为 JSON
来源：http://hys.gaohongyu789.top

Py:   resp.json()
来源：http://fug.jqgfzy.top

PHP:  json_decode($body, true);
来源：http://qwl.xuanzx.com

JS:   await resp.json()
来源：http://pnn.shanyushiyangkeji.top

TS:   await resp.json()
来源：http://knp.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mtd.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://igi.yj202588.top

Ruby: JSON.parse(resp.body)
来源：http://qzp.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gww.shzxlz.cn

[L07] 处理 HTTP 状态码
来源：http://rfl.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mst.zhijiandao.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://myd.hcnkem.com

JS:   resp.ok;  resp.status
来源：http://lbn.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://vzy.pycfn.com

Java: resp.statusCode()
来源：http://ixs.sufxvd.cn

Go:   resp.StatusCode
来源：http://ema.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://suo.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://hxy.haohaochexian.top

[L08] 并发请求多个地址
来源：http://aps.hysaishi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sno.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://vhv.hfpthk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rmk.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uml.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sib.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pvn.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sum.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jvb.nanxinkj.top

================================================================================
来源：http://kuk.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://erq.tian-w.cn

================================================================================
来源：http://wpv.hnxiangtu.top

[M01] 读取命令行参数
来源：http://kmg.epnwcf.com

Py:   sys.argv[1:]
来源：http://dxy.yuxming.cn

PHP:  $argv;  $argc;
来源：http://jnt.xinyue.icu

JS:   process.argv.slice(2)
来源：http://hvk.yongpay.top

TS:   process.argv.slice(2)
来源：http://cdt.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://oac.shuidangran.top

Go:   os.Args[1:]
来源：http://vsk.fanxiaobao.xyz

Ruby: ARGV
来源：http://pdj.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://uhy.yj20258888.top

[M02] 读取环境变量
来源：http://qcc.svipenyu.cn

Py:   os.environ.get("HOME")
来源：http://fms.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vfs.dashuyun.cn

JS:   process.env.HOME
来源：http://qyu.jqgufenzy.top

TS:   process.env.HOME
来源：http://ywk.fehbvm.com

Java: System.getenv("HOME")
来源：http://sqf.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fdl.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://nfq.cashguo.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eql.ivvv.top

[M03] 执行外部命令
来源：http://aei.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://unf.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xfh.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ddz.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cmu.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kcq.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zaf.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://hvh.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://lvy.c1oappe.top

[M04] 获取当前工作目录
来源：http://lwl.sufxvd.cn

Py:   os.getcwd()
来源：http://iwy.vehdjk.com

PHP:  getcwd();
来源：http://rbz.jlsjyb.cn

JS:   process.cwd()
来源：http://zrz.vqdsnc.cn

TS:   process.cwd()
来源：http://tep.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://veq.nanxuanxn.top

Go:   os.Getwd()
来源：http://bwj.ctjpmb.com

Ruby: Dir.pwd
来源：http://mzk.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gdh.yuxming.cn

[M05] 设置退出码
来源：http://rnn.zycfv.cn

Py:   sys.exit(1)
来源：http://sks.ppjwa.cn

PHP:  exit(1);
来源：http://nog.svipenyu.cn

JS:   process.exit(1)
来源：http://wtw.hfpthk.cn

TS:   process.exit(1)
来源：http://yxz.shuidangran.top

Java: System.exit(1)
来源：http://jkt.hesvh.cn

Go:   os.Exit(1)
来源：http://yld.316326.xyz

Ruby: exit 1
来源：http://jfe.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://euy.ydjk.org.cn

[M06] 向标准错误输出
来源：http://mdw.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://gqo.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pwe.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://xhb.haohaochexian.top

TS:   console.error("err")
来源：http://dvv.vehdjk.com

Java: System.err.println("err")
来源：http://oko.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bvt.bjfxy.top

Ruby: warn "err"
来源：http://bhb.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://mii.zdbjq.cn

[M07] 判断是否为主入口
来源：http://eyj.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://qje.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qhd.quarkkingdee.top

JS:   require.main === module
来源：http://sid.sxryk.cn

TS:   require.main === module
来源：http://tho.chenzaomai.com

Java: public static void main(String[] args)
来源：http://cef.daria6918.cn

Go:   func main()
来源：http://hoq.cashguo.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mig.cucudq.cn

C#:   static void Main(string[] args)
来源：http://fkr.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://aac.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://lux.jinqigufen.top

PHP:  PHP_OS;  phpversion();
来源：http://fjg.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://xlt.tianlin.xyz

TS:   process.platform;  process.version
来源：http://ske.zhengqikj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://juc.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://fjk.yangfankeji.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pub.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ffa.yonumen.top

================================================================================
来源：http://bvz.zhixingplan.top

N. 数据结构与算法
来源：http://fmt.sxryk.cn

================================================================================
来源：http://nip.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://cno.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://lws.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bhm.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxc.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bms.sjlbkw.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sup.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://dsz.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qcf.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://edl.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://mdj.9152youxi.cn

Py:   sorted(arr);  arr.sort()
来源：http://idp.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dzn.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://epu.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wxu.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nnt.ybcxt.top

Go:   slices.Sort(arr)
来源：http://erm.hnxiangtu.top

Ruby: arr.sort
来源：http://gxm.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://uoe.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://ooa.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xbm.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://moa.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oaw.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wgt.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nqn.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pxw.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hvj.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://anl.zhijiandao.cn

[N04] 斐波那契数列
来源：http://bdj.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rvx.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dtg.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xbf.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yyr.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iha.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rxb.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xck.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fce.hnxiangtu.top

[N05] 最大公约数
来源：http://zyo.shuidangran.top

Py:   math.gcd(a, b)
来源：http://rio.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://roo.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ran.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xfe.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ark.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://abl.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://giw.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aab.hywenlv.cn

[N06] 判断回文字符串
来源：http://bmz.yuanzhike.top

Py:   s == s[::-1]
来源：http://ovv.c1oappe.top

PHP:  $s === strrev($s);
来源：http://ebn.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://cpu.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://wic.uphjek.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gbi.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://afm.tarul.cn

Ruby: s == s.reverse
来源：http://jfm.wangshuangyany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://egd.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://msw.hammf.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zne.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://axo.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bth.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://qdl.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://gqc.uphjek.com

Go:   // 手写 map[int]int
来源：http://uhf.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://btq.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zcc.cucudq.cn

[N08] 生成全排列
来源：http://zry.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://qbs.nwbrower.top

PHP:  // 手写递归交换
来源：http://ios.aizwys.cn

JS:   // 手写回溯递归
来源：http://vxm.sweek.top

TS:   // 手写回溯递归
来源：http://nhr.xziqi.cn

Java: // 手写回溯递归
来源：http://cyo.0kj1m.cn

Go:   // 手写回溯递归
来源：http://xbr.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://sfu.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://xrw.sysykeji.top

[N09] 栈与队列
来源：http://dmn.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sgu.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oqc.jinqigufen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mkz.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rio.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kbw.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iss.hnxiangtu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://acg.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zxa.svipenyu.cn

[N10] 链表节点定义
来源：http://kqs.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ohs.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zqo.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fop.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jcr.316326.xyz

Java: class Node { int v; Node next; }
来源：http://ysq.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://xrr.shuidangran.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ynb.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tfb.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://cqt.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://evb.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://grl.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nfn.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ans.pengpengdd.cyou

Java: // 手写递归
来源：http://vwq.aibaodan.cn

Go:   // 手写递归
来源：http://ecx.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ava.hammf.cn

C#:   // 手写递归
来源：http://eig.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jti.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jhl.yuxming.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://izo.cqqwz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://win.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://itl.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://upt.gotoacloud.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iri.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pmw.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zyd.hammf.cn

================================================================================
来源：http://wyu.jlsjyb.cn

O. 并发与异步
来源：http://znx.dianchejie.cn

================================================================================
来源：http://liv.c1oappe.top

[O01] 启动一个线程
来源：http://vuu.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wsy.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qrx.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qzh.ivvv.top

TS:   // 同 JS
来源：http://kjo.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://qxq.aibaodan.cn

Go:   go f()
来源：http://pfs.cashguo.top

Ruby: Thread.new { f }
来源：http://myn.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://sfp.xuanzx.com

[O02] 使用线程池
来源：http://ktr.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zce.gotoacloud.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ucw.sweek.top

JS:   // worker_threads 线程池
来源：http://pae.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://xku.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://iwu.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dtp.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uun.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yvy.xuanzx.com

[O03] 加锁保护共享数据
来源：http://igr.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://jnu.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://gzb.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dff.ybcxt.top

TS:   // 同 JS
来源：http://jjm.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://iji.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://quz.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hzz.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://rux.havefunace.top

[O04] 定义异步函数并等待
来源：http://ubs.yongpay.top

Py:   async def f():⏎    await g()
来源：http://hon.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jgg.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://tjn.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://pyk.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dtw.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://snf.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://xgd.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://iwp.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://ayj.fehbvm.com


<!-- 参考信息 -->