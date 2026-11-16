代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://fnr.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mwb.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pyb.yuanzhike.top

[L02] 发送 POST JSON
来源：http://ewr.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://xhw.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ird.jqgufenzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jlc.ydjk.org.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nmq.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xad.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vts.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rma.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ghz.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://wdl.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rtc.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jai.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nln.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ypr.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bdt.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gtl.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://epf.sxryk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nfh.gogol.net.cn

[L04] 设置超时
来源：http://hsp.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://dzi.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ffk.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dvk.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lfp.hcnkem.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yjc.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sjb.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://phl.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vaw.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://sws.smart0.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://giw.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lxy.yonumen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zwb.guowangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gzy.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://puj.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lnk.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zky.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lbl.guannengcc.top

[L06] 解析响应为 JSON
来源：http://xfv.meibo888.top

Py:   resp.json()
来源：http://vof.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://gqq.gogol.net.cn

JS:   await resp.json()
来源：http://rhe.0kj1m.cn

TS:   await resp.json()
来源：http://qjv.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wov.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fdz.ydjk.org.cn

Ruby: JSON.parse(resp.body)
来源：http://lgc.zdbjq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mwn.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://gpr.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://upp.vqdsnc.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vpw.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://rts.meibo888.top

TS:   resp.ok;  resp.status
来源：http://yzv.jlsjyb.cn

Java: resp.statusCode()
来源：http://lqx.hysaishi.cn

Go:   resp.StatusCode
来源：http://dqd.tanke756.top

Ruby: resp.code.to_i
来源：http://jaw.iojbl.cn

C#:   (int)resp.StatusCode
来源：http://qzx.zdqjudy.top

[L08] 并发请求多个地址
来源：http://bfm.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rar.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://nxt.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://def.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://azj.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rkg.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yne.ehwqpu.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wqb.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ygb.hywenlv.cn

================================================================================
来源：http://ufu.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://svc.zdqjudy.top

================================================================================
来源：http://xan.zhengqikj.top

[M01] 读取命令行参数
来源：http://lgv.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://fme.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://rdx.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://knn.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://xfb.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://oig.meibo888.top

Go:   os.Args[1:]
来源：http://upt.316326.xyz

Ruby: ARGV
来源：http://mwa.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://gbx.chenzaomai.com

[M02] 读取环境变量
来源：http://cdj.cheryme.top

Py:   os.environ.get("HOME")
来源：http://dbv.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ngs.xuetiantiany.cn

JS:   process.env.HOME
来源：http://rvt.vqdsnc.cn

TS:   process.env.HOME
来源：http://xlo.gogol.net.cn

Java: System.getenv("HOME")
来源：http://uqv.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ysq.yonumen.top

Ruby: ENV["HOME"]
来源：http://ifs.yj20258888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://flc.ehwqpu.com

[M03] 执行外部命令
来源：http://alk.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zdm.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vem.ybcxt.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fbf.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jzw.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvl.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://qsu.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://ycj.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://aep.jianghu66.top

[M04] 获取当前工作目录
来源：http://ydi.52xcode.cn

Py:   os.getcwd()
来源：http://wzk.birdmap.top

PHP:  getcwd();
来源：http://cam.havefunace.top

JS:   process.cwd()
来源：http://mhr.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://for.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://plp.hammf.cn

Go:   os.Getwd()
来源：http://ukd.yanxiufei.cn

Ruby: Dir.pwd
来源：http://sbk.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://tqw.52xcode.cn

[M05] 设置退出码
来源：http://bbv.daria6918.cn

Py:   sys.exit(1)
来源：http://vgl.zhiwuduotai.top

PHP:  exit(1);
来源：http://ywl.xylfe.cn

JS:   process.exit(1)
来源：http://edu.zhoulong.xyz

TS:   process.exit(1)
来源：http://mej.zhengqikj.top

Java: System.exit(1)
来源：http://gmz.zhoulong.xyz

Go:   os.Exit(1)
来源：http://pgq.ehwqpu.com

Ruby: exit 1
来源：http://loo.nanxinkj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxk.nwbrower.top

[M06] 向标准错误输出
来源：http://uez.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://zlo.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jss.yuanzhike.top

JS:   console.error("err")
来源：http://wfk.tianlin.xyz

TS:   console.error("err")
来源：http://tia.chenzaomai.com

Java: System.err.println("err")
来源：http://rmg.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mel.dianchejie.cn

Ruby: warn "err"
来源：http://spw.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://roo.smart0.xyz

[M07] 判断是否为主入口
来源：http://lht.hammf.cn

Py:   if __name__ == "__main__":
来源：http://wgb.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pnf.jqgfzy.top

JS:   require.main === module
来源：http://pvx.yj20258.top

TS:   require.main === module
来源：http://wpy.cdnleiting.top

Java: public static void main(String[] args)
来源：http://zak.hnqzz.top

Go:   func main()
来源：http://qqm.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dja.daria6918.cn

C#:   static void Main(string[] args)
来源：http://pop.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://nni.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://dxw.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://mvy.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://lqv.xziqi.cn

TS:   process.platform;  process.version
来源：http://abl.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tcn.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://tgx.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://huk.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uny.zhijiandao.cn

================================================================================
来源：http://wnx.hnqzz.top

N. 数据结构与算法
来源：http://mbr.hywenlv.cn

================================================================================
来源：http://vrz.uphjek.com

[N01] 二分查找（有序数组）
来源：http://lwy.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://hrw.yangfankeji.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vbs.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yff.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lka.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://epl.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://nhf.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ihz.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://mfd.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://dnc.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://ahj.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rtl.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lpy.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://yyf.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wet.tanke756.top

Go:   slices.Sort(arr)
来源：http://fek.guowangkeji.top

Ruby: arr.sort
来源：http://gjy.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://van.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://ikn.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uil.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://ehe.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vnp.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xmn.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vpx.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kbm.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://miz.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://ouu.sxryk.cn

[N04] 斐波那契数列
来源：http://qxm.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lpt.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zzx.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ylv.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opd.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qxc.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pii.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owa.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qjk.yj20258888.top

[N05] 最大公约数
来源：http://uni.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://bur.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ggy.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bug.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rup.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rfe.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sqo.hammf.cn

Ruby: a.gcd(b)
来源：http://ctk.dashuyun.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kue.hfpthk.cn

[N06] 判断回文字符串
来源：http://rwe.cashguo.top

Py:   s == s[::-1]
来源：http://zoc.daria6918.cn

PHP:  $s === strrev($s);
来源：http://qia.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://zbj.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://lcx.chenzaomai.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://viw.hnqzz.top

Go:   // 双指针从两端比较
来源：http://ngc.tianlin.xyz

Ruby: s == s.reverse
来源：http://tdd.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://pfe.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://zec.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aqs.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jfm.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://gti.sweek.top

TS:   // 手写 Map<string, number>
来源：http://fcp.quarkkingdee.top

Java: // 手写 HashMap
来源：http://xkr.tanke756.top

Go:   // 手写 map[int]int
来源：http://vwz.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://ytg.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://rvj.zhongyouzk.top

[N08] 生成全排列
来源：http://kxu.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://aro.wangdashe.top

PHP:  // 手写递归交换
来源：http://wmp.hesvh.cn

JS:   // 手写回溯递归
来源：http://qfd.cqqwz.cn

TS:   // 手写回溯递归
来源：http://dwi.mhx1999.top

Java: // 手写回溯递归
来源：http://vzi.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://duv.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://zmo.fzhhl.top

C#:   // 手写回溯递归
来源：http://kzx.yangfankeji.com

[N09] 栈与队列
来源：http://nko.nanxinkj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ycy.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oep.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dnr.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://msd.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xjr.nanxinkj.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nhj.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sap.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fky.nanxinkj.top

[N10] 链表节点定义
来源：http://qyf.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zqp.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mpj.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gnj.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zja.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://xze.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://gcx.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://boe.yangfankeji.com

C#:   class Node { public int V; public Node? Next; }
来源：http://fpm.52xcode.cn

[N11] 二叉树中序遍历
来源：http://rrt.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rkz.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://fil.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kor.jqgfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cns.ehwqpu.com

Java: // 手写递归
来源：http://joe.birdmap.top

Go:   // 手写递归
来源：http://maf.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qla.uphjek.com

C#:   // 手写递归
来源：http://eby.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bci.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hez.zhengqikj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zkj.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vqe.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sav.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hng.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sot.xuanzx.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yzr.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pjd.pengpengdd.cyou

================================================================================
来源：http://rnu.mhx1999.top

O. 并发与异步
来源：http://sew.yj20258888.top

================================================================================
来源：http://smk.zdqjudy.top

[O01] 启动一个线程
来源：http://fqv.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://guq.bjfxy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zvw.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pwh.jianghu66.top

TS:   // 同 JS
来源：http://rtm.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://gdm.hysaishi.cn

Go:   go f()
来源：http://ite.chenlongwang.top

Ruby: Thread.new { f }
来源：http://ycl.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://ofk.0kj1m.cn

[O02] 使用线程池
来源：http://ash.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zcq.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yrg.shangyingyoupin.top

JS:   // worker_threads 线程池
来源：http://yyc.daria6918.cn

TS:   // worker_threads 线程池
来源：http://thk.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://blj.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fzw.ywan-chungtsiang.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://unl.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://haf.ydzc1.top

[O03] 加锁保护共享数据
来源：http://zna.epnwcf.com

Py:   with lock: shared += 1
来源：http://luk.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://hjx.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mlj.gotoacloud.top

TS:   // 同 JS
来源：http://snq.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://hgq.c1oappe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ycd.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://pcu.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://lbr.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://tus.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://snz.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rvp.andypj.xyz

JS:   async function f() { await g(); }
来源：http://vxc.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mzb.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rji.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ywy.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://utn.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://njg.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://tyu.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://kii.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fjw.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://tfv.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://fcu.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rxg.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rtn.iojbl.cn

Ruby: threads.map(&:join)
来源：http://qyz.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://doj.zdbjq.cn


<!-- 参考信息 -->