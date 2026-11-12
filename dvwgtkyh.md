代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mea.sjlbkw.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ejj.fehbvm.com

================================================================================
来源：http://ods.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://mhq.ehwqpu.com

================================================================================
来源：http://sak.jqgufenzy.top

[M01] 读取命令行参数
来源：http://yej.sxryk.cn

Py:   sys.argv[1:]
来源：http://web.cdnleiting.top

PHP:  $argv;  $argc;
来源：http://mjg.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://yrd.sxryk.cn

TS:   process.argv.slice(2)
来源：http://rnp.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://bbj.daria6918.cn

Go:   os.Args[1:]
来源：http://etb.vehdjk.com

Ruby: ARGV
来源：http://hnr.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://oqn.fehbvm.com

[M02] 读取环境变量
来源：http://sql.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://xel.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pwj.yfazqb.com

JS:   process.env.HOME
来源：http://jvn.kuanghao11.cn

TS:   process.env.HOME
来源：http://wku.iojbl.cn

Java: System.getenv("HOME")
来源：http://lwi.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wnm.tarul.cn

Ruby: ENV["HOME"]
来源：http://xnn.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qsc.nanxuanxn.top

[M03] 执行外部命令
来源：http://hjm.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://otg.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oeg.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ejk.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ylt.hesvh.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://keu.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eka.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://sug.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://cmb.svipenyu.cn

[M04] 获取当前工作目录
来源：http://jpd.daxiang520.top

Py:   os.getcwd()
来源：http://izw.havefunace.top

PHP:  getcwd();
来源：http://ahv.9152youxi.cn

JS:   process.cwd()
来源：http://ndx.ehwqpu.com

TS:   process.cwd()
来源：http://akl.havefunace.top

Java: Path.of("").toAbsolutePath()
来源：http://ifc.hysaishi.cn

Go:   os.Getwd()
来源：http://vpq.jinqigufen.top

Ruby: Dir.pwd
来源：http://pfw.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://emw.dianchejie.cn

[M05] 设置退出码
来源：http://hwf.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://sie.jinqigufen.top

PHP:  exit(1);
来源：http://bgz.cucudq.cn

JS:   process.exit(1)
来源：http://tzf.316326.xyz

TS:   process.exit(1)
来源：http://voq.ehwqpu.com

Java: System.exit(1)
来源：http://jzf.sweek.top

Go:   os.Exit(1)
来源：http://wyp.hongshengwenyu.top

Ruby: exit 1
来源：http://hfr.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ymc.jyoumei.cn

[M06] 向标准错误输出
来源：http://qcb.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://cdc.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rhi.ivvv.top

JS:   console.error("err")
来源：http://xio.bjfxy.top

TS:   console.error("err")
来源：http://adg.vqdsnc.cn

Java: System.err.println("err")
来源：http://oiy.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qsc.tianlin.xyz

Ruby: warn "err"
来源：http://smf.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://uvt.cheryme.top

[M07] 判断是否为主入口
来源：http://hoo.tarul.cn

Py:   if __name__ == "__main__":
来源：http://oxx.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tlf.jlsjyb.cn

JS:   require.main === module
来源：http://tad.havefunace.top

TS:   require.main === module
来源：http://ser.zhixingplan.top

Java: public static void main(String[] args)
来源：http://muo.yfazqb.com

Go:   func main()
来源：http://stw.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vgy.shanyushiyangkeji.top

C#:   static void Main(string[] args)
来源：http://jnn.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://qie.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://ldk.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://lir.zdqjudy.top

JS:   process.platform;  process.version
来源：http://mlv.guowangkeji.top

TS:   process.platform;  process.version
来源：http://xvu.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vjc.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://swk.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ofv.nanxinkj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zkr.yuxming.cn

================================================================================
来源：http://tna.yfazqb.com

N. 数据结构与算法
来源：http://hyd.pycfn.com

================================================================================
来源：http://wlt.birdmap.top

[N01] 二分查找（有序数组）
来源：http://pzo.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jhi.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rpl.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eik.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://erf.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://kge.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://ogt.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hun.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://apg.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://rvt.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://lcy.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cgq.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://whh.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jfh.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vld.iojbl.cn

Go:   slices.Sort(arr)
来源：http://sda.hfpthk.cn

Ruby: arr.sort
来源：http://ttp.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lqv.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://gsd.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://boc.cucudq.cn

PHP:  // 递归实现，或用 usort
来源：http://tvj.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wab.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ydz.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ubp.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qel.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tnq.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rkk.tarul.cn

[N04] 斐波那契数列
来源：http://ccq.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eft.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gyn.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bbw.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fno.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jee.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tqs.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kig.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kao.fktsv.cn

[N05] 最大公约数
来源：http://flw.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://jkb.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hrs.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kkq.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyt.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://syu.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rhi.ehwqpu.com

Ruby: a.gcd(b)
来源：http://abj.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hhr.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://muu.9152youxi.cn

Py:   s == s[::-1]
来源：http://rml.smart0.xyz

PHP:  $s === strrev($s);
来源：http://yut.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://bzd.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://gbr.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yft.nanxuanxn.top

Go:   // 双指针从两端比较
来源：http://psl.yj20258.top

Ruby: s == s.reverse
来源：http://pfb.ydjk.org.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://trc.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://dnj.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vot.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://okz.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ywr.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://rsi.iojbl.cn

Java: // 手写 HashMap
来源：http://dhg.tarul.cn

Go:   // 手写 map[int]int
来源：http://qbx.ppjwa.cn

Ruby: // 手写 Hash
来源：http://zob.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lxa.gogol.net.cn

[N08] 生成全排列
来源：http://pqv.316326.xyz

Py:   itertools.permutations(arr)
来源：http://lhz.daxiang520.top

PHP:  // 手写递归交换
来源：http://foi.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://wab.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://wpt.zhongyouzk.top

Java: // 手写回溯递归
来源：http://pjk.gzhubu.top

Go:   // 手写回溯递归
来源：http://fiq.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://ozv.hywenlv.cn

C#:   // 手写回溯递归
来源：http://mml.smart0.xyz

[N09] 栈与队列
来源：http://vht.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ezc.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tzt.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bdr.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xmc.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bnm.jianghu66.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tex.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eto.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://umj.hammf.cn

[N10] 链表节点定义
来源：http://bqe.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mwr.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://prt.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wta.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jvp.yj202588.top

Java: class Node { int v; Node next; }
来源：http://lzy.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://cqn.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://aqa.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jpx.guannengcc.top

[N11] 二叉树中序遍历
来源：http://kht.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zpz.tanke756.top

PHP:  // 手写递归函数
来源：http://zxw.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bnt.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ufm.yongpay.top

Java: // 手写递归
来源：http://pks.jqgfzy.top

Go:   // 手写递归
来源：http://uzh.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mkr.zdqjudy.top

C#:   // 手写递归
来源：http://uzv.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://exi.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lbd.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fqp.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nff.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgd.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sdn.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cbu.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://udd.hnqzz.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nha.hfpthk.cn

================================================================================
来源：http://sln.wangshuangyany.cn

O. 并发与异步
来源：http://plr.hongshengwenyu.top

================================================================================
来源：http://ewa.hammf.cn

[O01] 启动一个线程
来源：http://ghu.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://msg.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fjg.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rxf.hnxiangtu.top

TS:   // 同 JS
来源：http://sti.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://wew.cucudq.cn

Go:   go f()
来源：http://gxt.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://nph.gzhubu.top

C#:   Task.Run(() => F());
来源：http://cgq.fanxiaobao.xyz

[O02] 使用线程池
来源：http://rpx.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ihk.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hep.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://jxv.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://wfj.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://nez.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tsc.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fvm.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dce.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://nrp.guannengcc.top

Py:   with lock: shared += 1
来源：http://hli.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://jzp.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://prv.shuidangran.top

TS:   // 同 JS
来源：http://nbq.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://nux.fzhhl.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cpz.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nng.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://eoo.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://cdm.sweek.top

Py:   async def f():⏎    await g()
来源：http://tih.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gur.hcnkem.com

JS:   async function f() { await g(); }
来源：http://bqs.zhiwuduotai.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bbr.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://liz.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dle.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://phi.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://csb.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://wfr.dianchejie.cn

Py:   asyncio.gather(*tasks)
来源：http://zgf.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dox.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://nmm.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://chj.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ofw.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ayj.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://yao.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jwi.haohaochexian.top

[O06] 使用进程池
来源：http://jfs.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://crl.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lyb.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://stt.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://ypl.bbcook.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jty.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://knu.yuxming.cn

Ruby: // fork 块
来源：http://fow.fktsv.cn

C#:   Parallel.For
来源：http://brn.zdqjudy.top

================================================================================
来源：http://nkn.ybcxt.top

P. 常用工具函数
来源：http://xxo.xuetiantiany.cn

================================================================================
来源：http://ljn.yj20258888.top

[P01] 生成 UUID
来源：http://sun.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://ovh.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ddl.yfazqb.com

JS:   crypto.randomUUID()
来源：http://eay.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://fql.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://cna.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://hcr.yongpay.top

Ruby: SecureRandom.uuid
来源：http://jjd.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://dej.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://chj.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tiq.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wfu.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bxs.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sjo.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wcn.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ert.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hlk.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xpw.guowangkeji.top

[P03] 生成短随机字符串
来源：http://tbm.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://shz.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://khq.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezd.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://glh.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dwz.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nry.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wvz.tanke756.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oce.c1oappe.top

[P04] 求长度
来源：http://ebe.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cvr.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lbg.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://anz.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iew.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://tsj.ybcxt.top

Go:   len(arr);  len(m)
来源：http://pnp.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://jkh.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wrb.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://izn.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cja.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cvx.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ogt.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xsb.cqqwz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xxs.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://shi.fengsongda.top

Ruby: a == b
来源：http://qqi.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zff.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://whp.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aib.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://ekx.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jad.guowangkeji.top

TS:   if (x == null) {}
来源：http://gfu.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jdr.redwolf501.top

Go:   if x == nil {}
来源：http://nml.vqdsnc.cn


<!-- 参考信息 -->