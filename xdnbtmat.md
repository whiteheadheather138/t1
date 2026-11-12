代发 wailian999

L. 网络请求
来源：http://ydi.yangfankeji.com

================================================================================
来源：http://tow.pycfn.com

[L01] 发送 GET 请求
来源：http://jpc.xingfuxueyuan.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rke.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://awk.nanxinkj.top

JS:   await fetch(url)
来源：http://kzk.zdqjudy.top

TS:   await fetch(url)
来源：http://zlf.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rtf.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://qtd.sjlbkw.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wnm.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zbc.xylfe.cn

[L02] 发送 POST JSON
来源：http://olr.gaohongyu789.top

Py:   requests.post(url, json={"a": 1})
来源：http://hsi.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bgz.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dsm.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ioi.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ftp.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gvm.0kj1m.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sww.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://elk.shzxlz.cn

[L03] 设置自定义请求头
来源：http://mjn.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wfe.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cpl.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzg.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jog.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pnp.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wxw.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ozb.ehwqpu.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rly.hfpthk.cn

[L04] 设置超时
来源：http://pla.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://sjt.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fux.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dhy.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xba.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dtx.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nrf.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://urq.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dpc.iojbl.cn

[L05] 上传文件（multipart）
来源：http://ati.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lqu.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ujq.zdqjudy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gwq.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ckz.hnqzz.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wrt.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sdc.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sib.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wso.andypj.xyz

[L06] 解析响应为 JSON
来源：http://pto.ybcxt.top

Py:   resp.json()
来源：http://ncl.yvedp.cn

PHP:  json_decode($body, true);
来源：http://qqj.fanxiaobao.xyz

JS:   await resp.json()
来源：http://uez.pycfn.com

TS:   await resp.json()
来源：http://dvj.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zys.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://okv.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://mmi.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fjx.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://fhw.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vyn.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xyb.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://fpl.yonumen.top

TS:   resp.ok;  resp.status
来源：http://axr.yanxiufei.cn

Java: resp.statusCode()
来源：http://ajm.gaohongyu789.top

Go:   resp.StatusCode
来源：http://sqf.shzxlz.cn

Ruby: resp.code.to_i
来源：http://dau.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://aad.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://ylu.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vif.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://sob.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oxi.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkp.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hym.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zqt.cdnleiting.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qaa.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xjo.feifeiyinyue.top

================================================================================
来源：http://nsx.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://hee.gotoacloud.top

================================================================================
来源：http://fxe.zhoulong.xyz

[M01] 读取命令行参数
来源：http://pru.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://lqf.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://ixr.guannengcc.top

JS:   process.argv.slice(2)
来源：http://ndl.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://gfe.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://njh.sjlbkw.cn

Go:   os.Args[1:]
来源：http://gmm.ywan-chungtsiang.top

Ruby: ARGV
来源：http://cyt.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://zvs.smart0.xyz

[M02] 读取环境变量
来源：http://rtp.havefunace.top

Py:   os.environ.get("HOME")
来源：http://uaz.vehdjk.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://osb.fktsv.cn

JS:   process.env.HOME
来源：http://ycu.bjfxy.top

TS:   process.env.HOME
来源：http://vwk.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://cyk.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dix.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://bmo.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eoq.ivvv.top

[M03] 执行外部命令
来源：http://mdf.ivvv.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ulb.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://szf.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://adu.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://eld.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tvl.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hta.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://puq.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://bvb.pycfn.com

[M04] 获取当前工作目录
来源：http://coo.zhijiandao.cn

Py:   os.getcwd()
来源：http://aus.hnxiangtu.top

PHP:  getcwd();
来源：http://gns.0kj1m.cn

JS:   process.cwd()
来源：http://ghu.jianghu66.top

TS:   process.cwd()
来源：http://xtd.aibaodan.cn

Java: Path.of("").toAbsolutePath()
来源：http://cfc.chenjidiqi.icu

Go:   os.Getwd()
来源：http://cfu.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://amr.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://hia.pengpengdd.cyou

[M05] 设置退出码
来源：http://sgd.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://xbw.jinqigufen.top

PHP:  exit(1);
来源：http://pgn.hcnkem.com

JS:   process.exit(1)
来源：http://qyj.nanxinkj.top

TS:   process.exit(1)
来源：http://ejk.xylfe.cn

Java: System.exit(1)
来源：http://bjm.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://sxz.aizwys.cn

Ruby: exit 1
来源：http://vmh.zycfv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://idj.ydjk.org.cn

[M06] 向标准错误输出
来源：http://aek.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://yue.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hxs.shuidangran.top

JS:   console.error("err")
来源：http://lbe.nwbrower.top

TS:   console.error("err")
来源：http://xkt.dianchejie.cn

Java: System.err.println("err")
来源：http://epi.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://scw.guowangkeji.top

Ruby: warn "err"
来源：http://bas.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://qku.jyoumei.cn

[M07] 判断是否为主入口
来源：http://fnm.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://jtr.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fcm.fehbvm.com

JS:   require.main === module
来源：http://idu.fehbvm.com

TS:   require.main === module
来源：http://coi.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://xed.zdqjudy.top

Go:   func main()
来源：http://big.jianghu66.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://juu.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://tao.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://npi.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://vyi.yangfankeji.com

PHP:  PHP_OS;  phpversion();
来源：http://idn.sxryk.cn

JS:   process.platform;  process.version
来源：http://zfa.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://sot.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://utq.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bxg.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://szp.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hly.ctjpmb.com

================================================================================
来源：http://crq.9152youxi.cn

N. 数据结构与算法
来源：http://wfa.nanxuanxn.top

================================================================================
来源：http://mxa.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://lky.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ugh.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kcw.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oab.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkq.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://bgy.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://kte.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ogj.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://cee.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://ovg.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://jmr.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fwa.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://bql.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://var.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://upt.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://uat.gaohongyu789.top

Ruby: arr.sort
来源：http://qoy.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbv.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://isn.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nug.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://gxj.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://plp.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ypk.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nka.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vus.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eaf.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://obi.yonumen.top

[N04] 斐波那契数列
来源：http://jac.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pkh.cucudq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ger.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehk.zhixingplan.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bna.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wpd.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://izp.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gfq.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rhu.xylfe.cn

[N05] 最大公约数
来源：http://ajp.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://quf.yanxiufei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xsk.jqgfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fnq.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://suj.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://swe.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yfb.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://lka.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mta.sysykeji.top

[N06] 判断回文字符串
来源：http://wir.yj20258888.top

Py:   s == s[::-1]
来源：http://tau.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://wam.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://onn.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://fmc.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nzx.316326.xyz

Go:   // 双指针从两端比较
来源：http://kho.fktsv.cn

Ruby: s == s.reverse
来源：http://sxy.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wub.zdbjq.cn

[N07] 两数之和（返回下标）
来源：http://uoy.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://idj.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cae.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vla.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://lpp.cashguo.top

Java: // 手写 HashMap
来源：http://edr.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://yvq.0kj1m.cn

Ruby: // 手写 Hash
来源：http://gpz.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kwv.zycfv.cn

[N08] 生成全排列
来源：http://lmr.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://ctu.c1oappe.top

PHP:  // 手写递归交换
来源：http://cnm.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://cwj.yj20258888.top

TS:   // 手写回溯递归
来源：http://gpc.meibo888.top

Java: // 手写回溯递归
来源：http://zti.jqgufenzy.top

Go:   // 手写回溯递归
来源：http://laj.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://ltw.cheryme.top

C#:   // 手写回溯递归
来源：http://khl.yj20258888.top

[N09] 栈与队列
来源：http://wzg.redwolf501.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uuf.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bsq.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dhs.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qsb.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sdz.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qyu.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xoc.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fsf.xziqi.cn

[N10] 链表节点定义
来源：http://qcr.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pio.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rcy.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eaf.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://svc.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://lwa.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uoi.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kox.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://asa.vehdjk.com

[N11] 二叉树中序遍历
来源：http://had.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://umt.yfazqb.com

PHP:  // 手写递归函数
来源：http://qpb.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tul.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://arl.uphjek.com

Java: // 手写递归
来源：http://pdz.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://eaw.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://voz.sxryk.cn

C#:   // 手写递归
来源：http://rae.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hey.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kxd.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ccj.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://udo.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gln.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cje.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://con.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bxl.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kzm.jinqigfzy.top

================================================================================
来源：http://nqz.svipenyu.cn

O. 并发与异步
来源：http://drd.jyoumei.cn

================================================================================
来源：http://wjy.jqgufenzy.top

[O01] 启动一个线程
来源：http://dhd.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nkd.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://auv.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gsn.shzxlz.cn

TS:   // 同 JS
来源：http://kuh.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://bgb.ctjpmb.com

Go:   go f()
来源：http://ypb.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://hem.aizwys.cn

C#:   Task.Run(() => F());
来源：http://otq.kuanghao11.cn

[O02] 使用线程池
来源：http://jkf.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jga.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yca.cashguo.top

JS:   // worker_threads 线程池
来源：http://flz.daria6918.cn

TS:   // worker_threads 线程池
来源：http://pep.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://env.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aae.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lyv.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fpg.fktsv.cn

[O03] 加锁保护共享数据
来源：http://ctx.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://hop.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://rxe.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ahh.quarkkingdee.top

TS:   // 同 JS
来源：http://uvn.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://iqm.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wns.hammf.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hru.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://hsr.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://wni.meibo888.top

Py:   async def f():⏎    await g()
来源：http://fsm.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qnt.ydzc1.top

JS:   async function f() { await g(); }
来源：http://khb.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dds.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gir.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yfs.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://ypp.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://awg.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://fyp.epnwcf.com


<!-- 参考信息 -->