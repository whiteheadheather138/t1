代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qfr.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ekf.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://jmr.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ign.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://kqf.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://psl.0kj1m.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sze.sxryk.cn

JS:   resp.ok;  resp.status
来源：http://gpe.cheryme.top

TS:   resp.ok;  resp.status
来源：http://wbj.jqgfzy.top

Java: resp.statusCode()
来源：http://jtz.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://bvp.hysaishi.cn

Ruby: resp.code.to_i
来源：http://crp.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://ork.yj202588.top

[L08] 并发请求多个地址
来源：http://qmo.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qzf.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://gno.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoo.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oyw.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xdm.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ofm.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://irp.yj20258.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qxp.ydzc1.top

================================================================================
来源：http://dxp.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://vng.wangshuangyany.cn

================================================================================
来源：http://smw.meibo888.top

[M01] 读取命令行参数
来源：http://dxi.jqgfzy.top

Py:   sys.argv[1:]
来源：http://nzd.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://hvf.yvedp.cn

JS:   process.argv.slice(2)
来源：http://wum.gzhubu.top

TS:   process.argv.slice(2)
来源：http://wxk.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://dax.guannengcc.top

Go:   os.Args[1:]
来源：http://xcc.zhoulong.xyz

Ruby: ARGV
来源：http://ypo.nanxinkj.top

C#:   args 数组（Main 方法参数）
来源：http://cgz.gaohongyu789.top

[M02] 读取环境变量
来源：http://wdv.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://ofp.sweek.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mon.daria6918.cn

JS:   process.env.HOME
来源：http://gce.zdqjudy.top

TS:   process.env.HOME
来源：http://adq.hfpthk.cn

Java: System.getenv("HOME")
来源：http://uqt.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wyy.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://gsv.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://huk.ehwqpu.com

[M03] 执行外部命令
来源：http://cbe.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggq.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yhe.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mlr.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://bfg.zhiwuduotai.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bvj.ydjk.org.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ypt.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vzg.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://cvg.sufxvd.cn

[M04] 获取当前工作目录
来源：http://cxo.daria6918.cn

Py:   os.getcwd()
来源：http://hna.aibaodan.cn

PHP:  getcwd();
来源：http://jxf.sweek.top

JS:   process.cwd()
来源：http://vom.ppjwa.cn

TS:   process.cwd()
来源：http://vvz.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://xwg.jqgufenzy.top

Go:   os.Getwd()
来源：http://huy.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://kwj.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://daq.shangyingyoupin.top

[M05] 设置退出码
来源：http://bhm.cdnleiting.top

Py:   sys.exit(1)
来源：http://yvi.ctjpmb.com

PHP:  exit(1);
来源：http://utn.bjfxy.top

JS:   process.exit(1)
来源：http://wyy.aibaodan.cn

TS:   process.exit(1)
来源：http://ilt.zycfv.cn

Java: System.exit(1)
来源：http://pow.jianghu66.top

Go:   os.Exit(1)
来源：http://vbd.tian-w.cn

Ruby: exit 1
来源：http://atd.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://umt.snrcjt.cn

[M06] 向标准错误输出
来源：http://cze.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://ovg.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ekt.shzxlz.cn

JS:   console.error("err")
来源：http://gov.chenjidiqi.icu

TS:   console.error("err")
来源：http://ihb.fehbvm.com

Java: System.err.println("err")
来源：http://ahn.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://siw.hnqzz.top

Ruby: warn "err"
来源：http://hog.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://aqy.fengsongda.top

[M07] 判断是否为主入口
来源：http://ads.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://dtp.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://anr.fanxiaobao.xyz

JS:   require.main === module
来源：http://ozt.sufxvd.cn

TS:   require.main === module
来源：http://cnp.hcnkem.com

Java: public static void main(String[] args)
来源：http://bcu.9152youxi.cn

Go:   func main()
来源：http://xtt.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sab.yuxming.cn

C#:   static void Main(string[] args)
来源：http://lds.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://txz.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://gwa.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://gvz.hcnkem.com

JS:   process.platform;  process.version
来源：http://oln.cdnleiting.top

TS:   process.platform;  process.version
来源：http://gau.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pxy.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://whc.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lqu.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hkk.fehbvm.com

================================================================================
来源：http://mrg.tanke756.top

N. 数据结构与算法
来源：http://jjy.guannengcc.top

================================================================================
来源：http://egz.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://bhr.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vpq.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gtj.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://etp.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghr.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://pwc.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://hjd.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://diw.yonumen.top

C#:   Array.BinarySearch(arr, x)
来源：http://qgi.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://gej.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://wzd.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wml.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ohx.ydzc1.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://emc.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kyr.nanxinkj.top

Go:   slices.Sort(arr)
来源：http://tpg.pengpengdd.cyou

Ruby: arr.sort
来源：http://xal.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ifx.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://nbv.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://odr.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://huk.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://shc.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffv.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qcy.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lxg.andypj.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qcn.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://qpy.nwbrower.top

[N04] 斐波那契数列
来源：http://ivz.xinyue.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cvv.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tnq.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyt.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dbh.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fdf.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://etk.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bjv.shanyushiyangtech.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bey.redwolf501.top

[N05] 最大公约数
来源：http://zbs.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://zaf.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gxo.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://msx.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kxe.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ckm.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://afe.havefunace.top

Ruby: a.gcd(b)
来源：http://teg.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://osx.haohaochexian.top

[N06] 判断回文字符串
来源：http://qvr.kuanghao11.cn

Py:   s == s[::-1]
来源：http://qun.cashguo.top

PHP:  $s === strrev($s);
来源：http://onk.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://ulh.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://ahp.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://usi.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://mri.bjfxy.top

Ruby: s == s.reverse
来源：http://kfl.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nto.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://yxr.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uis.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hht.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://odh.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://bea.tian-w.cn

Java: // 手写 HashMap
来源：http://kyi.316326.xyz

Go:   // 手写 map[int]int
来源：http://bzz.aibaodan.cn

Ruby: // 手写 Hash
来源：http://ndb.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pjs.bbcook.cn

[N08] 生成全排列
来源：http://arc.ivvv.top

Py:   itertools.permutations(arr)
来源：http://jlh.ydzc1.top

PHP:  // 手写递归交换
来源：http://tvb.9152youxi.cn

JS:   // 手写回溯递归
来源：http://wto.c1oappe.top

TS:   // 手写回溯递归
来源：http://huo.cqqwz.cn

Java: // 手写回溯递归
来源：http://hli.0kj1m.cn

Go:   // 手写回溯递归
来源：http://ddl.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://fpm.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://mis.jqgfzy.top

[N09] 栈与队列
来源：http://moa.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mln.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nfb.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eag.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kkt.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fgb.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wjy.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qel.mhx1999.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jmx.zhongyouzk.top

[N10] 链表节点定义
来源：http://yfr.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qdh.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ves.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xbv.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gzv.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://vlo.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://dog.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sga.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jen.uphjek.com

[N11] 二叉树中序遍历
来源：http://vlb.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bgp.meibo888.top

PHP:  // 手写递归函数
来源：http://jry.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://leg.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iig.hysaishi.cn

Java: // 手写递归
来源：http://jqh.svipenyu.cn

Go:   // 手写递归
来源：http://ujk.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oab.tanke756.top

C#:   // 手写递归
来源：http://ifm.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bey.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fib.ywan-chungtsiang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lsz.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ayq.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qap.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sxl.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qjg.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pqr.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jyd.nwbrower.top

================================================================================
来源：http://iev.dashuyun.cn

O. 并发与异步
来源：http://xxe.hywenlv.cn

================================================================================
来源：http://sch.shangyingyoupin.top

[O01] 启动一个线程
来源：http://rsw.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ooc.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vmz.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tse.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://gvy.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://oqd.cashguo.top

Go:   go f()
来源：http://zmh.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://lrd.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://xvr.kuanghao11.cn

[O02] 使用线程池
来源：http://dyu.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://irb.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gac.aibaodan.cn

JS:   // worker_threads 线程池
来源：http://zvl.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://lpu.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ock.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rrw.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://luj.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mua.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://lwt.yueranfly.top

Py:   with lock: shared += 1
来源：http://fsq.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://bhu.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dlq.c1oappe.top

TS:   // 同 JS
来源：http://sbj.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://iku.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zsg.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ulu.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://mdy.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://ucq.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://obm.nanxinkj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lfa.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://wpq.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nxy.ywan-chungtsiang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://axa.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nme.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://azf.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://hzy.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://slj.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://tiz.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vsu.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://veg.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://ekh.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jru.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lkb.iojbl.cn

Ruby: threads.map(&:join)
来源：http://rsg.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zfg.snrcjt.cn

[O06] 使用进程池
来源：http://nic.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cqr.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mhq.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://ead.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://xkh.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jtn.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jsd.jiagoushi.top

Ruby: // fork 块
来源：http://tfx.sufxvd.cn

C#:   Parallel.For
来源：http://pkw.zhongyouzk.top

================================================================================
来源：http://qyp.yfazqb.com

P. 常用工具函数
来源：http://cgy.hongshengwenyu.top

================================================================================
来源：http://rld.fktsv.cn

[P01] 生成 UUID
来源：http://oky.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://vee.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mgl.yj20258.top

JS:   crypto.randomUUID()
来源：http://wbd.daxiang520.top

TS:   crypto.randomUUID()
来源：http://eoc.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://swx.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://evr.uphjek.com

Ruby: SecureRandom.uuid
来源：http://amn.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://rju.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://xdl.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rcw.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://icx.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jkw.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kdt.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tzq.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hff.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tdm.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ozx.epnwcf.com

[P03] 生成短随机字符串
来源：http://lmh.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kni.xuetiantiany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hsq.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mjq.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://btv.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kpo.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gwa.havefunace.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fsa.ppjwa.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hlj.jqgufenzy.top

[P04] 求长度
来源：http://ele.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ywa.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txl.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xrh.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yht.zdqjudy.top


<!-- 参考信息 -->