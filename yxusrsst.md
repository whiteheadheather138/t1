代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lwt.havefunace.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eyg.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lxh.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kpr.hfpthk.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xlx.xziqi.cn

[L04] 设置超时
来源：http://udm.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://dsg.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://auj.c1oappe.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pjn.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://erj.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wqb.pycfn.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yhl.redwolf501.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aag.zhaomingkeji.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iuq.hammf.cn

[L05] 上传文件（multipart）
来源：http://unx.zhoulong.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://daj.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rou.vqdsnc.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yxf.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://txd.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yav.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wks.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://stp.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ydf.epnwcf.com

[L06] 解析响应为 JSON
来源：http://usu.gzhubu.top

Py:   resp.json()
来源：http://nlp.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://xrd.zycfv.cn

JS:   await resp.json()
来源：http://rfp.nwbrower.top

TS:   await resp.json()
来源：http://ctn.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cro.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ugb.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://tjk.zhiwuduotai.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fvw.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://xph.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vuc.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rde.tanke756.top

JS:   resp.ok;  resp.status
来源：http://ngl.tanke756.top

TS:   resp.ok;  resp.status
来源：http://bao.guowangkeji.top

Java: resp.statusCode()
来源：http://ooh.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://ops.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://slo.zhiwuduotai.top

C#:   (int)resp.StatusCode
来源：http://yqj.bjfxy.top

[L08] 并发请求多个地址
来源：http://bub.jinyuanbaomall.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tku.sufxvd.cn

PHP:  curl_multi_init() 系列
来源：http://slj.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://usg.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fyx.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rmc.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zjh.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fxh.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dli.zycfv.cn

================================================================================
来源：http://mqh.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://kre.sysykeji.top

================================================================================
来源：http://ynj.316326.xyz

[M01] 读取命令行参数
来源：http://had.hcnkem.com

Py:   sys.argv[1:]
来源：http://ssx.sxryk.cn

PHP:  $argv;  $argc;
来源：http://ftz.birdmap.top

JS:   process.argv.slice(2)
来源：http://sjr.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://niq.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://ogt.cucudq.cn

Go:   os.Args[1:]
来源：http://wdu.vehdjk.com

Ruby: ARGV
来源：http://zet.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://hun.shzxlz.cn

[M02] 读取环境变量
来源：http://xri.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://jws.cqqwz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qcw.ydjk.org.cn

JS:   process.env.HOME
来源：http://hur.mhx1999.top

TS:   process.env.HOME
来源：http://ngp.jinghuilouyu.cn

Java: System.getenv("HOME")
来源：http://upo.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kju.sweek.top

Ruby: ENV["HOME"]
来源：http://tvr.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://byw.hongshengwenyu.top

[M03] 执行外部命令
来源：http://vcp.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tft.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://aiw.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://owj.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qle.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ltl.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://luh.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://dub.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://ifn.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://gid.zycfv.cn

Py:   os.getcwd()
来源：http://iki.uphjek.com

PHP:  getcwd();
来源：http://kuu.jqgfzy.top

JS:   process.cwd()
来源：http://bmm.hywenlv.cn

TS:   process.cwd()
来源：http://gjs.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://moo.pycfn.com

Go:   os.Getwd()
来源：http://jss.fzhhl.top

Ruby: Dir.pwd
来源：http://qwn.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://sgv.sjlbkw.cn

[M05] 设置退出码
来源：http://xtp.yvedp.cn

Py:   sys.exit(1)
来源：http://xpj.aibaodan.cn

PHP:  exit(1);
来源：http://kus.pycfn.com

JS:   process.exit(1)
来源：http://zlg.zhongyouzk.top

TS:   process.exit(1)
来源：http://dma.shangyingyoupin.top

Java: System.exit(1)
来源：http://dus.hcnkem.com

Go:   os.Exit(1)
来源：http://xyh.snrcjt.cn

Ruby: exit 1
来源：http://owg.iojbl.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hmk.guannengcc.top

[M06] 向标准错误输出
来源：http://uzp.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://xrn.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sua.hcnkem.com

JS:   console.error("err")
来源：http://yxs.jyoumei.cn

TS:   console.error("err")
来源：http://btz.tianlin.xyz

Java: System.err.println("err")
来源：http://ntb.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rfg.daxiang520.top

Ruby: warn "err"
来源：http://wqe.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://lid.fktsv.cn

[M07] 判断是否为主入口
来源：http://pzi.hammf.cn

Py:   if __name__ == "__main__":
来源：http://thb.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ksa.xinyue.icu

JS:   require.main === module
来源：http://abk.epnwcf.com

TS:   require.main === module
来源：http://pjt.cashguo.top

Java: public static void main(String[] args)
来源：http://fds.fengsongda.top

Go:   func main()
来源：http://zzg.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zbu.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://qdq.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://stp.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://lzw.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://wcx.cashguo.top

JS:   process.platform;  process.version
来源：http://lqo.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://zfk.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mdx.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://frf.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nti.xuetiantiany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xid.0kj1m.cn

================================================================================
来源：http://ffj.nanxuanxn.top

N. 数据结构与算法
来源：http://ldx.birdmap.top

================================================================================
来源：http://ukp.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://zrp.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bua.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ndp.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qta.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ybg.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://soj.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://wbm.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://brk.andypj.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://bac.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://bll.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bko.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oxz.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uhl.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://opb.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cjh.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://jbv.yuanzhike.top

Ruby: arr.sort
来源：http://poq.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://eyl.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://hjr.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mrm.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://ivv.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmm.birdmap.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jre.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hbm.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://opl.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tne.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://tah.sufxvd.cn

[N04] 斐波那契数列
来源：http://rjx.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://btn.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mnr.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ggc.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpj.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pst.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kno.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qaj.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hdx.pengpengdd.cyou

[N05] 最大公约数
来源：http://bfk.tanke756.top

Py:   math.gcd(a, b)
来源：http://jlq.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qzl.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vph.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vol.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://eak.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qrl.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://tkf.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wtx.hnqzz.top

[N06] 判断回文字符串
来源：http://ssk.zhijiandao.cn

Py:   s == s[::-1]
来源：http://bhz.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://far.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://ufg.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://clc.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kta.sysykeji.top

Go:   // 双指针从两端比较
来源：http://hwo.316326.xyz

Ruby: s == s.reverse
来源：http://rbh.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://kqc.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://kcv.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tvg.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rjw.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sso.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://pil.tianlin.xyz

Java: // 手写 HashMap
来源：http://mun.chenzaomai.com

Go:   // 手写 map[int]int
来源：http://knb.jqgfzy.top

Ruby: // 手写 Hash
来源：http://qqm.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://lwd.hnxiangtu.top

[N08] 生成全排列
来源：http://jdd.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://esf.daria6918.cn

PHP:  // 手写递归交换
来源：http://wix.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://rih.zhixingplan.top

TS:   // 手写回溯递归
来源：http://mif.kuanghao11.cn

Java: // 手写回溯递归
来源：http://yfj.tianlin.xyz

Go:   // 手写回溯递归
来源：http://kwf.nanxuanxn.top

Ruby: arr.permutation.to_a
来源：http://ips.hfpthk.cn

C#:   // 手写回溯递归
来源：http://dhe.316326.xyz

[N09] 栈与队列
来源：http://cuq.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ldv.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nxm.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yqn.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cco.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ajj.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hvw.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wdb.jlsjyb.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zfr.zhijiandao.cn

[N10] 链表节点定义
来源：http://tov.ehwqpu.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gdj.hfpthk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://icn.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uoa.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rwm.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://kqg.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://txy.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zwl.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://akt.fzhhl.top

[N11] 二叉树中序遍历
来源：http://ckd.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ajz.hywenlv.cn

PHP:  // 手写递归函数
来源：http://wsa.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kbw.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dud.pycfn.com

Java: // 手写递归
来源：http://xnb.pengpengdd.cyou

Go:   // 手写递归
来源：http://ukv.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vjk.svipenyu.cn

C#:   // 手写递归
来源：http://pmp.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxr.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dcf.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eug.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yci.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uvi.ctjpmb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pnl.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://efs.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jeg.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mrg.ydzc1.top

================================================================================
来源：http://cif.xziqi.cn

O. 并发与异步
来源：http://tgg.dianchejie.cn

================================================================================
来源：http://jpd.cqqwz.cn

[O01] 启动一个线程
来源：http://sqj.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zaf.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://trj.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yvg.shzxlz.cn

TS:   // 同 JS
来源：http://lje.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://ikr.hysaishi.cn

Go:   go f()
来源：http://dvb.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://lee.aizwys.cn

C#:   Task.Run(() => F());
来源：http://udr.sjlbkw.cn

[O02] 使用线程池
来源：http://shc.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qdu.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wpo.fengsongda.top

JS:   // worker_threads 线程池
来源：http://gag.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://lgj.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://fpn.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ecn.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://foy.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://poj.daria6918.cn

[O03] 加锁保护共享数据
来源：http://ldk.gotoacloud.top

Py:   with lock: shared += 1
来源：http://vbe.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://zhg.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wms.fktsv.cn

TS:   // 同 JS
来源：http://guf.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://zjb.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gtg.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wpm.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://xli.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://xia.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://bgf.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xbk.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://mix.iojbl.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dro.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://due.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ciy.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://piu.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://vlv.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://gon.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://ehw.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ywt.uphjek.com

JS:   await Promise.all(tasks)
来源：http://rmi.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://usq.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ytp.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pcw.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://nbk.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wfz.yfazqb.com

[O06] 使用进程池
来源：http://akz.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jqm.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://anm.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://edt.nwbrower.top

TS:   // child_process / cluster 模块
来源：http://czm.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rri.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lhg.52xcode.cn

Ruby: // fork 块
来源：http://iay.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://hzo.havefunace.top

================================================================================
来源：http://haa.cheryme.top

P. 常用工具函数
来源：http://ivb.zycfv.cn

================================================================================
来源：http://ali.snrcjt.cn

[P01] 生成 UUID
来源：http://cec.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://yjv.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yvp.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://wox.ybcxt.top


<!-- 参考信息 -->