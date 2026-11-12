代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lcl.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://drr.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xeu.sjlbkw.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vee.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kzz.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pva.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://jku.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cit.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eba.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oxq.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mgg.zhaomingkeji.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xpp.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cvo.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iqy.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hyc.xylfe.cn

[L06] 解析响应为 JSON
来源：http://bgj.yj20258.top

Py:   resp.json()
来源：http://qvc.yonumen.top

PHP:  json_decode($body, true);
来源：http://yem.yj20258.top

JS:   await resp.json()
来源：http://dkq.chenjidiqi.icu

TS:   await resp.json()
来源：http://xas.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wel.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pdo.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://iga.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zvt.yangfankeji.com

[L07] 处理 HTTP 状态码
来源：http://ujj.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sxg.xylfe.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vow.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://ego.havefunace.top

TS:   resp.ok;  resp.status
来源：http://eix.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://egt.havefunace.top

Go:   resp.StatusCode
来源：http://ypp.shuidangran.top

Ruby: resp.code.to_i
来源：http://pse.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://qdn.bjfxy.top

[L08] 并发请求多个地址
来源：http://ouq.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jhg.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://sjf.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yes.yvedp.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vzt.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nxi.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wdd.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rds.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ynu.yuxming.cn

================================================================================
来源：http://crb.cdnleiting.top

M. 命令行 / 进程 / 环境
来源：http://nmu.guowangkeji.top

================================================================================
来源：http://qwe.nanxinkj.top

[M01] 读取命令行参数
来源：http://fek.9152youxi.cn

Py:   sys.argv[1:]
来源：http://inv.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://eof.aizwys.cn

JS:   process.argv.slice(2)
来源：http://kby.redwolf501.top

TS:   process.argv.slice(2)
来源：http://yww.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://kvn.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://qee.cashguo.top

Ruby: ARGV
来源：http://jgy.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://tdd.mhx1999.top

[M02] 读取环境变量
来源：http://jpi.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://lpg.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vtz.0kj1m.cn

JS:   process.env.HOME
来源：http://bgh.tarul.cn

TS:   process.env.HOME
来源：http://upo.yuxming.cn

Java: System.getenv("HOME")
来源：http://ret.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zsn.ydjk.org.cn

Ruby: ENV["HOME"]
来源：http://cqs.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xyg.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://qex.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sjg.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://abf.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xba.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sjb.meibo888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://adr.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nld.yongpay.top

Ruby: system("ls -l");  `ls -l`
来源：http://tdg.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://ozh.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://cuh.tarul.cn

Py:   os.getcwd()
来源：http://iaw.dianchejie.cn

PHP:  getcwd();
来源：http://iml.sjlbkw.cn

JS:   process.cwd()
来源：http://dvs.hnqzz.top

TS:   process.cwd()
来源：http://qbv.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://ulc.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://qjn.meibo888.top

Ruby: Dir.pwd
来源：http://rkx.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://oru.snrcjt.cn

[M05] 设置退出码
来源：http://swk.ydzc1.top

Py:   sys.exit(1)
来源：http://glo.hesvh.cn

PHP:  exit(1);
来源：http://php.daxiang520.top

JS:   process.exit(1)
来源：http://jyp.pycfn.com

TS:   process.exit(1)
来源：http://bvi.zhongyouzk.top

Java: System.exit(1)
来源：http://phv.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://qhx.xuanzx.com

Ruby: exit 1
来源：http://ydq.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ast.52xcode.cn

[M06] 向标准错误输出
来源：http://qrd.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://eva.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qfl.jiagoushi.top

JS:   console.error("err")
来源：http://pme.hesvh.cn

TS:   console.error("err")
来源：http://vyw.nanxinkj.top

Java: System.err.println("err")
来源：http://wcj.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ohz.c1oappe.top

Ruby: warn "err"
来源：http://wnl.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://eqc.gotoacloud.top

[M07] 判断是否为主入口
来源：http://xbg.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://edl.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cyc.uphjek.com

JS:   require.main === module
来源：http://nzb.aibaodan.cn

TS:   require.main === module
来源：http://zim.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://kel.cucudq.cn

Go:   func main()
来源：http://hyv.meibo888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://okr.uphjek.com

C#:   static void Main(string[] args)
来源：http://xaa.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://rou.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://ddv.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://gvv.jianghu66.top

JS:   process.platform;  process.version
来源：http://ksv.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://ufo.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pts.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tih.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iqi.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nfv.xziqi.cn

================================================================================
来源：http://trr.chenzaomai.com

N. 数据结构与算法
来源：http://rkm.yfazqb.com

================================================================================
来源：http://hya.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://zlb.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bog.shzxlz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hdc.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tcc.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ivk.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ouh.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://kjh.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vnb.shanyushiyangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://flt.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://qqj.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://zfs.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://syi.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://tfk.chenzaomai.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://iwh.sweek.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://esq.wangdashe.top

Go:   slices.Sort(arr)
来源：http://mju.vehdjk.com

Ruby: arr.sort
来源：http://ill.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cac.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://ldk.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eih.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://sao.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vpi.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mmj.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://awf.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kkf.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ksh.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://xkj.bjfxy.top

[N04] 斐波那契数列
来源：http://tjy.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://phz.jqgfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kdb.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pbt.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wux.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ucw.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ide.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hem.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://viy.nanxuanxn.top

[N05] 最大公约数
来源：http://brb.tarul.cn

Py:   math.gcd(a, b)
来源：http://rif.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oze.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fyk.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://llv.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ape.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fey.gzhubu.top

Ruby: a.gcd(b)
来源：http://xjm.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pbk.jqgfzy.top

[N06] 判断回文字符串
来源：http://egg.9152youxi.cn

Py:   s == s[::-1]
来源：http://aml.nwbrower.top

PHP:  $s === strrev($s);
来源：http://euv.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://nla.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://aei.iojbl.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iha.fengsongda.top

Go:   // 双指针从两端比较
来源：http://qph.jiagoushi.top

Ruby: s == s.reverse
来源：http://pbg.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fps.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://rte.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yvz.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vuq.xuetiantiany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zml.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://vna.cucudq.cn

Java: // 手写 HashMap
来源：http://iak.yfazqb.com

Go:   // 手写 map[int]int
来源：http://aqe.hcnkem.com

Ruby: // 手写 Hash
来源：http://dkn.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://yic.nwbrower.top

[N08] 生成全排列
来源：http://sat.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://mff.zycfv.cn

PHP:  // 手写递归交换
来源：http://guh.bbcook.cn

JS:   // 手写回溯递归
来源：http://ird.yj20258888.top

TS:   // 手写回溯递归
来源：http://chc.yvedp.cn

Java: // 手写回溯递归
来源：http://hlf.xziqi.cn

Go:   // 手写回溯递归
来源：http://jdr.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://afw.chenlongwang.top

C#:   // 手写回溯递归
来源：http://okk.shzxlz.cn

[N09] 栈与队列
来源：http://dkd.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vkl.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://njk.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hkq.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sqx.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ydy.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sxa.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lbi.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mcy.xylfe.cn

[N10] 链表节点定义
来源：http://wqt.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jim.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fsl.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ukn.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lhs.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://aac.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://kzi.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vda.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wmg.yueranfly.top

[N11] 二叉树中序遍历
来源：http://sqa.zhixingplan.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rqn.uphjek.com

PHP:  // 手写递归函数
来源：http://pqg.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bmr.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lit.shanyushiyangkeji.top

Java: // 手写递归
来源：http://ssi.ehwqpu.com

Go:   // 手写递归
来源：http://mys.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bek.c1oappe.top

C#:   // 手写递归
来源：http://ooz.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rny.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jba.quarkkingdee.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zqb.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://onn.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xnb.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cis.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wfi.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yts.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gqa.hammf.cn

================================================================================
来源：http://wey.birdmap.top

O. 并发与异步
来源：http://och.daria6918.cn

================================================================================
来源：http://vil.birdmap.top

[O01] 启动一个线程
来源：http://oyr.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hxm.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bvk.yuanzhike.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://alm.fktsv.cn

TS:   // 同 JS
来源：http://pbp.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://cru.jlsjyb.cn

Go:   go f()
来源：http://axl.snrcjt.cn

Ruby: Thread.new { f }
来源：http://lzl.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://euy.meibo888.top

[O02] 使用线程池
来源：http://asc.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xdf.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uha.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://rsr.yvedp.cn

TS:   // worker_threads 线程池
来源：http://rok.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://qly.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fhl.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ptf.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yyc.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://qfs.c1oappe.top

Py:   with lock: shared += 1
来源：http://nwn.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://fvi.jlsjyb.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xdo.gotoacloud.top

TS:   // 同 JS
来源：http://ffg.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://qqn.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xbk.uphjek.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://qhh.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://dov.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://rfj.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://jba.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uhn.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://zlz.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://cii.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://abh.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://icj.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iam.cheryme.top

C#:   async Task F() { await G(); }
来源：http://qam.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://igx.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://xmk.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://exk.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://hkx.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://wir.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dem.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://efw.gzhubu.top

Ruby: threads.map(&:join)
来源：http://vsp.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://noi.zycfv.cn

[O06] 使用进程池
来源：http://mmy.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adx.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zkb.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://xni.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://hvp.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wvl.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fzk.chenjidiqi.icu

Ruby: // fork 块
来源：http://icq.zycfv.cn

C#:   Parallel.For
来源：http://hoj.gogol.net.cn

================================================================================
来源：http://iib.jyoumei.cn

P. 常用工具函数
来源：http://pgd.xuanzx.com

================================================================================
来源：http://hqk.52xcode.cn

[P01] 生成 UUID
来源：http://wqd.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://pwe.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cxz.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://kwz.sysykeji.top

TS:   crypto.randomUUID()
来源：http://ewu.xuetiantiany.cn

Java: UUID.randomUUID().toString()
来源：http://dov.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://vdw.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://mdp.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://yno.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://vok.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://exn.xinyue.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://ftu.316326.xyz


<!-- 参考信息 -->