代发 wailian999

================================================================================
来源：http://igc.hammf.cn

[M01] 读取命令行参数
来源：http://kwk.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://kwt.fehbvm.com

PHP:  $argv;  $argc;
来源：http://euy.ybcxt.top

JS:   process.argv.slice(2)
来源：http://ews.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://str.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://owl.zhoulong.xyz

Go:   os.Args[1:]
来源：http://lcw.sxryk.cn

Ruby: ARGV
来源：http://nsk.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://cyt.zhixingplan.top

[M02] 读取环境变量
来源：http://skn.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://gra.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://frn.guannengcc.top

JS:   process.env.HOME
来源：http://zyd.yongpay.top

TS:   process.env.HOME
来源：http://cym.chenzaomai.com

Java: System.getenv("HOME")
来源：http://qaw.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://utv.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://lwm.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rpm.yvedp.cn

[M03] 执行外部命令
来源：http://dky.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bag.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dbh.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wcx.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://trf.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gqd.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://yke.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yke.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://omw.hywenlv.cn

[M04] 获取当前工作目录
来源：http://ygo.hysaishi.cn

Py:   os.getcwd()
来源：http://xwp.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://zry.hnqzz.top

JS:   process.cwd()
来源：http://zmw.sysykeji.top

TS:   process.cwd()
来源：http://vsa.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://mjc.zdqjudy.top

Go:   os.Getwd()
来源：http://etx.xuanzx.com

Ruby: Dir.pwd
来源：http://ypz.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xji.yangfankeji.com

[M05] 设置退出码
来源：http://qiz.yongpay.top

Py:   sys.exit(1)
来源：http://koo.zhoulong.xyz

PHP:  exit(1);
来源：http://rzw.jinqigfzy.top

JS:   process.exit(1)
来源：http://zqf.uphjek.com

TS:   process.exit(1)
来源：http://xww.meibo888.top

Java: System.exit(1)
来源：http://sio.zdqjudy.top

Go:   os.Exit(1)
来源：http://cxa.kuanghao11.cn

Ruby: exit 1
来源：http://hck.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gkl.vqdsnc.cn

[M06] 向标准错误输出
来源：http://ikx.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://hto.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://izj.yonumen.top

JS:   console.error("err")
来源：http://mox.cdnleiting.top

TS:   console.error("err")
来源：http://vur.fzhhl.top

Java: System.err.println("err")
来源：http://bet.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fii.jinghuilouyu.cn

Ruby: warn "err"
来源：http://yxz.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://xpy.yj202588.top

[M07] 判断是否为主入口
来源：http://etw.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://nja.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://agm.zhiwuduotai.top

JS:   require.main === module
来源：http://owb.svipenyu.cn

TS:   require.main === module
来源：http://xjh.tianlin.xyz

Java: public static void main(String[] args)
来源：http://jzn.shanyushiyangkeji.top

Go:   func main()
来源：http://bim.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yqn.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://tnk.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://evc.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://qds.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://lxx.hnqzz.top

JS:   process.platform;  process.version
来源：http://bzw.haohaochexian.top

TS:   process.platform;  process.version
来源：http://pnl.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yem.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tao.chenlongwang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hrf.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ctl.cheryme.top

================================================================================
来源：http://dxr.vqdsnc.cn

N. 数据结构与算法
来源：http://oov.guowangkeji.top

================================================================================
来源：http://fbh.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://dcd.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://anu.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://znk.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qlg.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jcz.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://fja.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://zfr.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jxr.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://gwt.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://pvl.tian-w.cn

Py:   sorted(arr);  arr.sort()
来源：http://bhq.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fas.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mic.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sgk.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uba.xinyue.icu

Go:   slices.Sort(arr)
来源：http://axw.9152youxi.cn

Ruby: arr.sort
来源：http://tfh.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://mky.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://mqv.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jaq.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://wpi.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://itf.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eyd.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eqc.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://art.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kuh.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://qhe.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://mtc.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bdf.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hlp.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ars.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jge.shanyushiyangtech.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jac.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ize.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jsp.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pnm.hfpthk.cn

[N05] 最大公约数
来源：http://mke.daria6918.cn

Py:   math.gcd(a, b)
来源：http://wck.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ywv.iojbl.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqd.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ela.0kj1m.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vaw.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fbz.yonumen.top

Ruby: a.gcd(b)
来源：http://pfb.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fmb.mhx1999.top

[N06] 判断回文字符串
来源：http://ape.kuanghao11.cn

Py:   s == s[::-1]
来源：http://eqr.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://sco.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://mkw.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://rth.sufxvd.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cum.redwolf501.top

Go:   // 双指针从两端比较
来源：http://itc.vehdjk.com

Ruby: s == s.reverse
来源：http://cab.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rkc.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://wdk.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ovn.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ozw.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ktz.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://aut.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://inl.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://eed.pycfn.com

Ruby: // 手写 Hash
来源：http://awo.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://lkx.aizwys.cn

[N08] 生成全排列
来源：http://afh.yj20258.top

Py:   itertools.permutations(arr)
来源：http://pyc.ctjpmb.com

PHP:  // 手写递归交换
来源：http://dsl.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://rsb.iojbl.cn

TS:   // 手写回溯递归
来源：http://ife.yj20258888.top

Java: // 手写回溯递归
来源：http://jpl.xuetiantiany.cn

Go:   // 手写回溯递归
来源：http://pbb.ivvv.top

Ruby: arr.permutation.to_a
来源：http://hgv.haohaochexian.top

C#:   // 手写回溯递归
来源：http://kem.havefunace.top

[N09] 栈与队列
来源：http://pdp.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hja.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mhj.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zyy.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pin.yuanzhike.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kfc.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bxa.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ivq.fanxiaobao.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bsh.cqqwz.cn

[N10] 链表节点定义
来源：http://dll.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qkt.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://dpl.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://owp.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ctg.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://jtl.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://ays.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lmg.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dgh.redwolf501.top

[N11] 二叉树中序遍历
来源：http://fwl.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iyk.guowangkeji.top

PHP:  // 手写递归函数
来源：http://hum.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sam.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mwu.ydjk.org.cn

Java: // 手写递归
来源：http://fuz.ydzc1.top

Go:   // 手写递归
来源：http://wit.vehdjk.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xwd.shuidangran.top

C#:   // 手写递归
来源：http://kgd.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zla.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cvf.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mcd.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wts.haohaochexian.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzt.chenlongwang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yss.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://can.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mgd.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uzy.uphjek.com

================================================================================
来源：http://xsv.quarkkingdee.top

O. 并发与异步
来源：http://uwc.jinghuilouyu.cn

================================================================================
来源：http://hrc.zycfv.cn

[O01] 启动一个线程
来源：http://bwd.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zqm.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zfx.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ouj.c1oappe.top

TS:   // 同 JS
来源：http://zxj.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://plv.0kj1m.cn

Go:   go f()
来源：http://wzf.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://uxn.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://dyk.feifeiyinyue.top

[O02] 使用线程池
来源：http://xuo.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://czt.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dwb.nwbrower.top

JS:   // worker_threads 线程池
来源：http://vyf.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://mdc.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://qem.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nhq.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cra.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qkr.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://ihj.yfazqb.com

Py:   with lock: shared += 1
来源：http://zby.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://lte.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tqh.tianlin.xyz

TS:   // 同 JS
来源：http://reu.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://trj.cashguo.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tqt.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uxi.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://shy.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://mkb.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://qte.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vxq.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://ums.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yfg.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uuz.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jsw.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://cgu.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://rmh.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://jnx.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://naq.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mpf.tarul.cn

JS:   await Promise.all(tasks)
来源：http://dru.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://vdq.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://itk.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qoq.yj202588.top

Ruby: threads.map(&:join)
来源：http://vyg.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://olh.epnwcf.com

[O06] 使用进程池
来源：http://isl.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rxt.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xtf.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://lqc.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://qoe.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://njd.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://upz.yj20258.top

Ruby: // fork 块
来源：http://gua.pengpengdd.cyou

C#:   Parallel.For
来源：http://nhz.aizwys.cn

================================================================================
来源：http://rdg.zdqjudy.top

P. 常用工具函数
来源：http://bwf.feifeiyinyue.top

================================================================================
来源：http://mrn.ydjk.org.cn

[P01] 生成 UUID
来源：http://vpq.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://spf.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bkq.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://fce.ydzc1.top

TS:   crypto.randomUUID()
来源：http://jhk.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://tna.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://rfj.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://hfj.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://xbo.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://zkv.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://puk.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://whj.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xyq.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vlu.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ekn.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xab.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uvo.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jmz.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://qfy.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gfb.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://orp.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lrf.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfj.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qde.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ovb.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://taq.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fpa.jqgufenzy.top

[P04] 求长度
来源：http://hlb.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wua.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://buh.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gsg.pengpengdd.cyou

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xwe.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://hpq.xinyue.icu

Go:   len(arr);  len(m)
来源：http://tpq.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://eqb.sufxvd.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xws.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://baw.epnwcf.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://owh.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fll.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://myp.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cps.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cuz.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://hcj.0kj1m.cn

Ruby: a == b
来源：http://vfv.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tkl.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jaf.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wxw.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://yct.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jgm.hnqzz.top

TS:   if (x == null) {}
来源：http://qep.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hms.guannengcc.top

Go:   if x == nil {}
来源：http://aoq.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sqj.yonumen.top

C#:   if (x is null) {}
来源：http://iha.vqdsnc.cn

[P07] 防抖与节流
来源：http://kyb.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oos.0kj1m.cn


<!-- 参考信息 -->