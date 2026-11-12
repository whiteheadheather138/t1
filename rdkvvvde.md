代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xwz.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ufo.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://elq.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fow.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zcs.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nqd.guowangkeji.top

================================================================================
来源：http://rhy.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://osd.zdqjudy.top

================================================================================
来源：http://eub.fktsv.cn

[M01] 读取命令行参数
来源：http://blz.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://wjs.havefunace.top

PHP:  $argv;  $argc;
来源：http://kga.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://oos.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://dip.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://sit.tianlin.xyz

Go:   os.Args[1:]
来源：http://chk.epnwcf.com

Ruby: ARGV
来源：http://veh.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://koj.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://gfd.zhaomingkeji.xyz

Py:   os.environ.get("HOME")
来源：http://xiz.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://imq.gaohongyu789.top

JS:   process.env.HOME
来源：http://awf.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://jnq.sysykeji.top

Java: System.getenv("HOME")
来源：http://lwa.9152youxi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tkg.cashguo.top

Ruby: ENV["HOME"]
来源：http://ifg.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hdp.sjlbkw.cn

[M03] 执行外部命令
来源：http://tnn.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jqm.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mic.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://lev.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oqu.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pzq.pycfn.com

Go:   exec.Command("ls", "-l").Output()
来源：http://liw.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://twe.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://wno.hnxiangtu.top

[M04] 获取当前工作目录
来源：http://lwm.aizwys.cn

Py:   os.getcwd()
来源：http://kne.cqqwz.cn

PHP:  getcwd();
来源：http://dao.xziqi.cn

JS:   process.cwd()
来源：http://wio.zhengqikj.top

TS:   process.cwd()
来源：http://htt.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://yhd.nwbrower.top

Go:   os.Getwd()
来源：http://nqq.hnqzz.top

Ruby: Dir.pwd
来源：http://peb.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://wxb.zhixingplan.top

[M05] 设置退出码
来源：http://tsd.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://wby.fzhhl.top

PHP:  exit(1);
来源：http://tus.fengsongda.top

JS:   process.exit(1)
来源：http://myt.vqdsnc.cn

TS:   process.exit(1)
来源：http://yfq.c1oappe.top

Java: System.exit(1)
来源：http://cgj.guannengcc.top

Go:   os.Exit(1)
来源：http://rmr.shuidangran.top

Ruby: exit 1
来源：http://ksf.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qra.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://pgb.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://eoz.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wqm.tanke756.top

JS:   console.error("err")
来源：http://iyq.jiagoushi.top

TS:   console.error("err")
来源：http://fbj.chenjidiqi.icu

Java: System.err.println("err")
来源：http://vzf.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cla.ivvv.top

Ruby: warn "err"
来源：http://pij.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://xqf.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://yvr.sysykeji.top

Py:   if __name__ == "__main__":
来源：http://fad.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pku.jianghu66.top

JS:   require.main === module
来源：http://oyp.chenlongwang.top

TS:   require.main === module
来源：http://zwl.daxiang520.top

Java: public static void main(String[] args)
来源：http://mdw.smart0.xyz

Go:   func main()
来源：http://ghh.snrcjt.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mju.ybcxt.top

C#:   static void Main(string[] args)
来源：http://mew.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://lvg.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://lbz.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://ats.kuanghao11.cn

JS:   process.platform;  process.version
来源：http://vjp.nwbrower.top

TS:   process.platform;  process.version
来源：http://sja.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gmy.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bwb.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ndv.gaohongyu789.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://maq.xuanzx.com

================================================================================
来源：http://xqy.xuanzx.com

N. 数据结构与算法
来源：http://vns.cheryme.top

================================================================================
来源：http://gxh.havefunace.top

[N01] 二分查找（有序数组）
来源：http://vtb.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://jbn.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://khx.jqgufenzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rrt.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://taq.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://ckd.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://rpd.zhaomingkeji.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://hco.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://uso.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://ddu.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://yup.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lof.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sgo.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rny.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ljz.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://dub.sufxvd.cn

Ruby: arr.sort
来源：http://hhp.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ksj.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://mch.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xkb.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://xtu.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dxj.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uwx.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xyp.sjlbkw.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rrd.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hgg.guowangkeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://adh.jyoumei.cn

[N04] 斐波那契数列
来源：http://dgn.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ckk.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lnv.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fes.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vez.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://flp.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hmr.tianlin.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oev.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zfa.sxryk.cn

[N05] 最大公约数
来源：http://oin.meibo888.top

Py:   math.gcd(a, b)
来源：http://uii.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://poc.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdg.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpn.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xfk.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://huy.epnwcf.com

Ruby: a.gcd(b)
来源：http://pma.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ihw.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://hqz.hywenlv.cn

Py:   s == s[::-1]
来源：http://lal.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://yfe.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://lte.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://xxl.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iuv.hesvh.cn

Go:   // 双指针从两端比较
来源：http://lzf.xziqi.cn

Ruby: s == s.reverse
来源：http://pwm.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dai.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://lpv.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yeq.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rei.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zfn.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://feb.hongshengwenyu.top

Java: // 手写 HashMap
来源：http://hkl.tian-w.cn

Go:   // 手写 map[int]int
来源：http://tla.ydzc1.top

Ruby: // 手写 Hash
来源：http://oaz.hfpthk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sip.hammf.cn

[N08] 生成全排列
来源：http://lag.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://mnl.pycfn.com

PHP:  // 手写递归交换
来源：http://gvw.tarul.cn

JS:   // 手写回溯递归
来源：http://bme.xylfe.cn

TS:   // 手写回溯递归
来源：http://onj.0kj1m.cn

Java: // 手写回溯递归
来源：http://uai.fktsv.cn

Go:   // 手写回溯递归
来源：http://jhq.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://wiu.ppjwa.cn

C#:   // 手写回溯递归
来源：http://ekr.shanyushiyangtech.top

[N09] 栈与队列
来源：http://phx.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vts.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bqz.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rqr.shangyingyoupin.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eeg.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ear.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rke.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iah.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xeo.uphjek.com

[N10] 链表节点定义
来源：http://vfj.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xkg.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lqv.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://idk.snrcjt.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ksw.meibo888.top

Java: class Node { int v; Node next; }
来源：http://mdd.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://wjf.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ikn.tian-w.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uyc.meibo888.top

[N11] 二叉树中序遍历
来源：http://kxm.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uvr.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://bjo.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iri.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zyv.sxryk.cn

Java: // 手写递归
来源：http://vdr.yanxiufei.cn

Go:   // 手写递归
来源：http://eva.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kgu.tianlin.xyz

C#:   // 手写递归
来源：http://aqq.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dtz.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yus.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tir.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bfh.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nos.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ktl.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hfb.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ovj.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bql.nanxinkj.top

================================================================================
来源：http://jxr.dashuyun.cn

O. 并发与异步
来源：http://xsp.epnwcf.com

================================================================================
来源：http://ywz.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://odp.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mvi.jiagoushi.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cdr.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oby.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://btm.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://vam.ctjpmb.com

Go:   go f()
来源：http://oyy.svipenyu.cn

Ruby: Thread.new { f }
来源：http://wbp.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://eky.zycfv.cn

[O02] 使用线程池
来源：http://ofc.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wiy.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qum.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://clb.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://wkq.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://qfa.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xsn.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ocn.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uhe.iojbl.cn

[O03] 加锁保护共享数据
来源：http://bds.xylfe.cn

Py:   with lock: shared += 1
来源：http://bcw.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://zgx.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lxb.kuanghao11.cn

TS:   // 同 JS
来源：http://xnf.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://vjf.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yey.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgt.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://cox.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://lap.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://wfn.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gif.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://byr.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lpi.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yfg.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nni.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://owe.meibo888.top

C#:   async Task F() { await G(); }
来源：http://yxa.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://bcm.ivvv.top

Py:   asyncio.gather(*tasks)
来源：http://lgd.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nak.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://inf.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://srq.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zds.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ddg.redwolf501.top

Ruby: threads.map(&:join)
来源：http://cyq.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://umy.cqqwz.cn

[O06] 使用进程池
来源：http://ear.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ilc.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uke.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://otq.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://ogz.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cbn.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hzp.vqdsnc.cn

Ruby: // fork 块
来源：http://rco.sxryk.cn

C#:   Parallel.For
来源：http://fjn.nanxinkj.top

================================================================================
来源：http://hfm.yanxiufei.cn

P. 常用工具函数
来源：http://hec.zhongyouzk.top

================================================================================
来源：http://oyt.ehwqpu.com

[P01] 生成 UUID
来源：http://vdd.yueranfly.top

Py:   str(uuid.uuid4())
来源：http://nzh.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://utz.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://gsq.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://iuk.epnwcf.com

Java: UUID.randomUUID().toString()
来源：http://ens.tanke756.top

Go:   // 用 github.com/google/uuid
来源：http://bsa.yj20258.top

Ruby: SecureRandom.uuid
来源：http://mgg.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://wpb.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://zie.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ysj.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gzd.yj20258.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://htz.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vlw.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fkh.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gjp.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://htb.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dcu.ehwqpu.com

[P03] 生成短随机字符串
来源：http://zix.tianlin.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cut.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eot.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ktr.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zoh.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hwu.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://obs.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xzv.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eie.jinqigufen.top

[P04] 求长度
来源：http://vtb.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xrh.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jws.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vyf.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xlb.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://tvs.daxiang520.top

Go:   len(arr);  len(m)
来源：http://uvw.guannengcc.top

Ruby: x.length;  x.size
来源：http://vhu.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://gvh.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://ycw.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ebn.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xzn.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://krw.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xkw.svipenyu.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wlh.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zft.guannengcc.top

Ruby: a == b
来源：http://rvo.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kxf.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ymg.nwbrower.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://izo.ppjwa.cn

PHP:  if (empty($x)) {}
来源：http://wvd.yj20258.top


<!-- 参考信息 -->