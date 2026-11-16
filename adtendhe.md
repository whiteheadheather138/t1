代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wiu.yangfankeji.com

JS:   await fetch(url)
来源：http://njl.gogol.net.cn

TS:   await fetch(url)
来源：http://cdr.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sna.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://rko.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://cxs.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ysv.svipenyu.cn

[L02] 发送 POST JSON
来源：http://iuz.zhaomingkeji.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://egg.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ars.fzhhl.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cms.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pvo.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wmd.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nnd.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wqg.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://prv.tarul.cn

[L03] 设置自定义请求头
来源：http://opc.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ctg.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://djh.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://srq.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jkt.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ayt.vqdsnc.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vbj.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ogv.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mgb.wangdashe.top

[L04] 设置超时
来源：http://njy.zhaomingkeji.xyz

Py:   requests.get(url, timeout=5)
来源：http://wjp.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hed.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cij.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wid.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://flm.ydjk.org.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zfm.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vou.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://orz.shuidangran.top

[L05] 上传文件（multipart）
来源：http://mrm.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zzj.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xxa.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tnl.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wsd.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://cvy.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tsg.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jme.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wsk.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://alt.sxryk.cn

Py:   resp.json()
来源：http://uew.xziqi.cn

PHP:  json_decode($body, true);
来源：http://uyf.sweek.top

JS:   await resp.json()
来源：http://jsl.c1oappe.top

TS:   await resp.json()
来源：http://zko.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zob.yanxiufei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uqm.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://yjg.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fmd.sweek.top

[L07] 处理 HTTP 状态码
来源：http://fla.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://byb.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://khh.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://duy.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://gbp.bjfxy.top

Java: resp.statusCode()
来源：http://kbz.cdnleiting.top

Go:   resp.StatusCode
来源：http://rkj.yvedp.cn

Ruby: resp.code.to_i
来源：http://yed.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://vgi.bjfxy.top

[L08] 并发请求多个地址
来源：http://ctk.dianchejie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nul.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://hrg.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rba.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hwi.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://roq.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zwx.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rdw.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iuu.cdnleiting.top

================================================================================
来源：http://ogt.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://epe.yonumen.top

================================================================================
来源：http://bgq.shanyushiyangtech.top

[M01] 读取命令行参数
来源：http://tqd.ydzc1.top

Py:   sys.argv[1:]
来源：http://ihr.yj20258.top

PHP:  $argv;  $argc;
来源：http://ofz.xinyue.icu

JS:   process.argv.slice(2)
来源：http://hut.mhx1999.top

TS:   process.argv.slice(2)
来源：http://phx.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://xyi.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://afi.c1oappe.top

Ruby: ARGV
来源：http://cce.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://ace.aibaodan.cn

[M02] 读取环境变量
来源：http://duh.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://pxr.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://one.bbcook.cn

JS:   process.env.HOME
来源：http://dqj.pycfn.com

TS:   process.env.HOME
来源：http://pxg.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://uvs.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://slc.wangdashe.top

Ruby: ENV["HOME"]
来源：http://ffu.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://njn.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://zpy.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kgq.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lit.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nop.gaohongyu789.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jel.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iya.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vmz.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vac.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://iuu.gogol.net.cn

[M04] 获取当前工作目录
来源：http://ecz.uphjek.com

Py:   os.getcwd()
来源：http://stf.52xcode.cn

PHP:  getcwd();
来源：http://kxw.jinqigfzy.top

JS:   process.cwd()
来源：http://spy.pycfn.com

TS:   process.cwd()
来源：http://fhl.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://avv.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://yrm.ctjpmb.com

Ruby: Dir.pwd
来源：http://jzu.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tce.yj20258888.top

[M05] 设置退出码
来源：http://xbo.fzhhl.top

Py:   sys.exit(1)
来源：http://oil.ehwqpu.com

PHP:  exit(1);
来源：http://lno.ivvv.top

JS:   process.exit(1)
来源：http://avf.nwbrower.top

TS:   process.exit(1)
来源：http://tec.cashguo.top

Java: System.exit(1)
来源：http://atn.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://rac.sxryk.cn

Ruby: exit 1
来源：http://zqp.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hvb.cdnleiting.top

[M06] 向标准错误输出
来源：http://tgw.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://xyw.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wxn.pengpengdd.cyou

JS:   console.error("err")
来源：http://ehq.fengsongda.top

TS:   console.error("err")
来源：http://pwo.sysykeji.top

Java: System.err.println("err")
来源：http://zbd.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mlo.cheryme.top

Ruby: warn "err"
来源：http://gck.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://msq.shzxlz.cn

[M07] 判断是否为主入口
来源：http://gkh.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://umm.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://idt.yj20258888.top

JS:   require.main === module
来源：http://ags.nanxuanxn.top

TS:   require.main === module
来源：http://yxm.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://elb.shzxlz.cn

Go:   func main()
来源：http://rsa.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wsb.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://axe.yj202588.top

[M08] 获取系统与运行时信息
来源：http://mxy.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://kcr.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://for.zdqjudy.top

JS:   process.platform;  process.version
来源：http://kxq.ybcxt.top

TS:   process.platform;  process.version
来源：http://cth.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tga.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://smd.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://csy.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bqt.xziqi.cn

================================================================================
来源：http://zim.wangshuangyany.cn

N. 数据结构与算法
来源：http://jtn.hcnkem.com

================================================================================
来源：http://afu.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://ajw.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://xij.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kay.gogol.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ios.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ozu.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://eve.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://apn.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iqo.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://kjb.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://yot.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://jzr.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://erk.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lty.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ybc.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ofo.ivvv.top

Go:   slices.Sort(arr)
来源：http://qbf.mhx1999.top

Ruby: arr.sort
来源：http://brs.zhaomingkeji.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://lft.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://rpx.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hfx.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://izu.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tkx.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tii.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sfw.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pze.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://drh.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://rhg.nanxuanxn.top

[N04] 斐波那契数列
来源：http://glu.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qih.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hnr.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hpr.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ytp.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ysg.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lbp.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nxe.hnxiangtu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nji.hcnkem.com

[N05] 最大公约数
来源：http://xfa.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://qpw.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ags.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdz.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://klo.tian-w.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jrr.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xpg.shangyingyoupin.top

Ruby: a.gcd(b)
来源：http://osb.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yoh.jlsjyb.cn

[N06] 判断回文字符串
来源：http://xdr.gotoacloud.top

Py:   s == s[::-1]
来源：http://lev.jianghu66.top

PHP:  $s === strrev($s);
来源：http://dcw.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://czd.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://lmx.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nme.bjfxy.top

Go:   // 双指针从两端比较
来源：http://brx.zycfv.cn

Ruby: s == s.reverse
来源：http://wts.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://akx.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://hiq.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://emh.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tlm.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gnj.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://sis.cashguo.top

Java: // 手写 HashMap
来源：http://yez.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://led.dashuyun.cn

Ruby: // 手写 Hash
来源：http://fqp.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://zsh.mhx1999.top

[N08] 生成全排列
来源：http://fut.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://qjo.chenzaomai.com

PHP:  // 手写递归交换
来源：http://cdo.xziqi.cn

JS:   // 手写回溯递归
来源：http://hqw.havefunace.top

TS:   // 手写回溯递归
来源：http://udr.shuidangran.top

Java: // 手写回溯递归
来源：http://nsg.xinyue.icu

Go:   // 手写回溯递归
来源：http://wut.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://nhc.haohaochexian.top

C#:   // 手写回溯递归
来源：http://gvr.zhoulong.xyz

[N09] 栈与队列
来源：http://mkz.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lla.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xze.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tyl.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ayg.uphjek.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kkd.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ipt.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pgj.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ucd.bbcook.cn

[N10] 链表节点定义
来源：http://nzm.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xrg.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rpf.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://alw.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dxv.tian-w.cn

Java: class Node { int v; Node next; }
来源：http://bsm.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://rwz.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://enk.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://hdx.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://esh.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zyx.sufxvd.cn

PHP:  // 手写递归函数
来源：http://pom.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tgk.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpc.tianlin.xyz

Java: // 手写递归
来源：http://rbo.haohaochexian.top

Go:   // 手写递归
来源：http://fqi.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gak.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://cwf.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ocw.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://naf.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vht.feifeiyinyue.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mkl.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uyh.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xnb.daria6918.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ytn.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://own.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xvp.chenzaomai.com

================================================================================
来源：http://one.havefunace.top

O. 并发与异步
来源：http://hcf.0kj1m.cn

================================================================================
来源：http://fse.daxiang520.top

[O01] 启动一个线程
来源：http://opm.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nyr.gzhubu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eyi.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wqm.yongpay.top

TS:   // 同 JS
来源：http://kix.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://oig.zhixingplan.top

Go:   go f()
来源：http://vce.yuxming.cn

Ruby: Thread.new { f }
来源：http://bqm.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://jsj.hongshengwenyu.top

[O02] 使用线程池
来源：http://bth.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wcn.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cmd.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://kah.yvedp.cn

TS:   // worker_threads 线程池
来源：http://vnq.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://zyg.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nac.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://goy.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uzq.mhx1999.top

[O03] 加锁保护共享数据
来源：http://jeo.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://nqo.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://ufs.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kfd.jinghuilouyu.cn

TS:   // 同 JS
来源：http://myn.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://daf.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tjw.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bjt.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://osd.yj202588.top

[O04] 定义异步函数并等待
来源：http://tvv.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://fbt.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://btd.yj20258.top

JS:   async function f() { await g(); }
来源：http://czc.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://axj.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rmy.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wts.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://azz.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://qww.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://zxb.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://kud.zhongyouzk.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xiu.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://ygz.yj20258.top

TS:   await Promise.all(tasks)
来源：http://lim.c1oappe.top


<!-- 参考信息 -->