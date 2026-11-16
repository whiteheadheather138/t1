代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://slu.ehwqpu.com

JS:   await fetch(url)
来源：http://kkp.snrcjt.cn

TS:   await fetch(url)
来源：http://zvj.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://spn.cqqwz.cn

Go:   resp, err := http.Get(url)
来源：http://qws.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tqr.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oei.jinqigufen.top

[L02] 发送 POST JSON
来源：http://zga.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://uhe.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qcb.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqc.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hml.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wxj.chenlongwang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vxa.zhijiandao.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://djd.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hay.hesvh.cn

[L03] 设置自定义请求头
来源：http://xng.sjlbkw.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dwm.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://elj.zycfv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jxx.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzg.ivvv.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ntc.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://enb.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dcp.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://goo.gotoacloud.top

[L04] 设置超时
来源：http://hps.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://wgi.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bzg.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jgf.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmv.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xyu.c1oappe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ygp.uphjek.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lmw.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kgp.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://zno.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vmq.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://npq.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fhu.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uyu.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zwe.xziqi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kox.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtz.fehbvm.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://srz.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://gnc.zycfv.cn

Py:   resp.json()
来源：http://gzn.tian-w.cn

PHP:  json_decode($body, true);
来源：http://joe.c1oappe.top

JS:   await resp.json()
来源：http://wia.vehdjk.com

TS:   await resp.json()
来源：http://xoj.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ndn.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xtv.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://hhl.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uoj.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://mwc.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yjn.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://swe.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://inq.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://hju.tian-w.cn

Java: resp.statusCode()
来源：http://kqc.gzhubu.top

Go:   resp.StatusCode
来源：http://dog.mhx1999.top

Ruby: resp.code.to_i
来源：http://kqc.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://gww.pengpengdd.cyou

[L08] 并发请求多个地址
来源：http://llw.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lpk.zdbjq.cn

PHP:  curl_multi_init() 系列
来源：http://pyo.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ytt.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iud.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sam.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dvh.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://boo.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iee.316326.xyz

================================================================================
来源：http://ckt.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://iuq.daxiang520.top

================================================================================
来源：http://syq.ybcxt.top

[M01] 读取命令行参数
来源：http://ikr.hcnkem.com

Py:   sys.argv[1:]
来源：http://uad.xziqi.cn

PHP:  $argv;  $argc;
来源：http://qoh.havefunace.top

JS:   process.argv.slice(2)
来源：http://kfc.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://ejq.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://hqt.ehwqpu.com

Go:   os.Args[1:]
来源：http://fdm.jianghu66.top

Ruby: ARGV
来源：http://bdv.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://qal.bbcook.cn

[M02] 读取环境变量
来源：http://nrt.xziqi.cn

Py:   os.environ.get("HOME")
来源：http://ubb.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gxl.jlsjyb.cn

JS:   process.env.HOME
来源：http://mgi.nwbrower.top

TS:   process.env.HOME
来源：http://iqo.fehbvm.com

Java: System.getenv("HOME")
来源：http://iav.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://krn.xuanzx.com

Ruby: ENV["HOME"]
来源：http://vfm.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tmn.hongshengwenyu.top

[M03] 执行外部命令
来源：http://exb.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fyz.sufxvd.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iap.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cji.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://odr.aibaodan.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jxu.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jfl.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ptv.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://hjm.yonumen.top

[M04] 获取当前工作目录
来源：http://pvq.nwbrower.top

Py:   os.getcwd()
来源：http://uly.9152youxi.cn

PHP:  getcwd();
来源：http://hpy.ctjpmb.com

JS:   process.cwd()
来源：http://ezk.cucudq.cn

TS:   process.cwd()
来源：http://obt.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://oyu.0kj1m.cn

Go:   os.Getwd()
来源：http://khu.dianchejie.cn

Ruby: Dir.pwd
来源：http://epv.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eky.guowangkeji.top

[M05] 设置退出码
来源：http://fue.ppjwa.cn

Py:   sys.exit(1)
来源：http://lkn.hcnkem.com

PHP:  exit(1);
来源：http://kxj.sxryk.cn

JS:   process.exit(1)
来源：http://dwc.bjfxy.top

TS:   process.exit(1)
来源：http://uqx.yongpay.top

Java: System.exit(1)
来源：http://yya.guowangkeji.top

Go:   os.Exit(1)
来源：http://cca.uphjek.com

Ruby: exit 1
来源：http://lbr.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wjz.tian-w.cn

[M06] 向标准错误输出
来源：http://lrr.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://ium.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kxr.jiagoushi.top

JS:   console.error("err")
来源：http://gpq.ctjpmb.com

TS:   console.error("err")
来源：http://pij.mhx1999.top

Java: System.err.println("err")
来源：http://ddw.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://awd.fehbvm.com

Ruby: warn "err"
来源：http://rrh.andypj.xyz

C#:   Console.Error.WriteLine("err")
来源：http://bqa.yonumen.top

[M07] 判断是否为主入口
来源：http://zvt.sweek.top

Py:   if __name__ == "__main__":
来源：http://sfo.daxiang520.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qex.fzhhl.top

JS:   require.main === module
来源：http://cxb.shangyingyoupin.top

TS:   require.main === module
来源：http://ean.hesvh.cn

Java: public static void main(String[] args)
来源：http://pyp.hcnkem.com

Go:   func main()
来源：http://ntc.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://spw.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://asn.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://dhe.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://iht.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://roj.yueranfly.top

JS:   process.platform;  process.version
来源：http://xja.jianghu66.top

TS:   process.platform;  process.version
来源：http://tvx.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jmp.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iya.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xyf.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hzm.zycfv.cn

================================================================================
来源：http://ruv.zdbjq.cn

N. 数据结构与算法
来源：http://eqt.mhx1999.top

================================================================================
来源：http://znl.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://fdr.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://dnw.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ert.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qbt.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yuk.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pox.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://npw.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bzt.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zpb.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://eex.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://fhd.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://thn.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hzy.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jux.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://suj.cheryme.top

Go:   slices.Sort(arr)
来源：http://euz.ydzc1.top

Ruby: arr.sort
来源：http://atg.ydzc1.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iyy.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://zfn.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ede.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://zzc.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwy.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lis.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ndh.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzm.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nyz.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hcw.yj20258888.top

[N04] 斐波那契数列
来源：http://yer.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jzq.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://etb.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shb.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://huh.ydjk.org.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jjt.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sqk.aizwys.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xos.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yks.c1oappe.top

[N05] 最大公约数
来源：http://ryq.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://lmc.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eem.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scw.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://her.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cjl.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://njx.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://sjy.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mkt.yongpay.top

[N06] 判断回文字符串
来源：http://say.shuidangran.top

Py:   s == s[::-1]
来源：http://ugd.jyoumei.cn

PHP:  $s === strrev($s);
来源：http://liz.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://hfv.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://krj.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ecr.jyoumei.cn

Go:   // 双指针从两端比较
来源：http://ven.snrcjt.cn

Ruby: s == s.reverse
来源：http://zkq.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ixs.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://cpi.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zza.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kcy.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rgc.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://uco.fktsv.cn

Java: // 手写 HashMap
来源：http://vqa.daxiang520.top

Go:   // 手写 map[int]int
来源：http://hhw.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://iig.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://dkk.cdnleiting.top

[N08] 生成全排列
来源：http://mxs.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://ash.andypj.xyz

PHP:  // 手写递归交换
来源：http://ptb.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://orf.yongpay.top

TS:   // 手写回溯递归
来源：http://jpy.52xcode.cn

Java: // 手写回溯递归
来源：http://gac.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://cex.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://pmh.gaohongyu789.top

C#:   // 手写回溯递归
来源：http://eds.ppjwa.cn

[N09] 栈与队列
来源：http://smc.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lli.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qbz.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zlb.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gtj.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dhu.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sul.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bco.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hit.sxryk.cn

[N10] 链表节点定义
来源：http://uzv.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sgr.aizwys.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rhv.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://att.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://azs.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://kpn.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://aka.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fdb.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vzo.yuxming.cn

[N11] 二叉树中序遍历
来源：http://jcc.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ktb.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://jbp.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lxh.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ylw.tianlin.xyz

Java: // 手写递归
来源：http://mei.feifeiyinyue.top

Go:   // 手写递归
来源：http://abh.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xfm.daxiang520.top

C#:   // 手写递归
来源：http://cco.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kgp.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hdg.xingfuxueyuan.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vne.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://anp.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lbl.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iih.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pvr.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tfo.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qbi.quarkkingdee.top

================================================================================
来源：http://htn.uphjek.com

O. 并发与异步
来源：http://caj.daria6918.cn

================================================================================
来源：http://ymv.iojbl.cn

[O01] 启动一个线程
来源：http://nig.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xzw.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fti.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sfd.xuetiantiany.cn

TS:   // 同 JS
来源：http://awn.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://cjc.jyoumei.cn

Go:   go f()
来源：http://afx.sxryk.cn

Ruby: Thread.new { f }
来源：http://god.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://tbu.chenlongwang.top

[O02] 使用线程池
来源：http://cwz.feifeiyinyue.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rbj.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hgx.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://fis.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://nwz.hnxiangtu.top

Java: Executors.newFixedThreadPool(4)
来源：http://nij.hywenlv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tep.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gvx.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hrb.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://rnd.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://cwz.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://dqn.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mos.gzhubu.top

TS:   // 同 JS
来源：http://ygf.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://chk.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://juy.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xob.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://ktn.cheryme.top

[O04] 定义异步函数并等待
来源：http://lcx.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://bfr.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gfp.jianghu66.top

JS:   async function f() { await g(); }
来源：http://nsn.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hlf.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pns.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wds.zdbjq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pbq.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://oxo.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://hdc.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://qay.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fns.sufxvd.cn

JS:   await Promise.all(tasks)
来源：http://mxm.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://ymc.zdqjudy.top


<!-- 参考信息 -->