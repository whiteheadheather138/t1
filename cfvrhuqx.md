代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qjk.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lki.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ykk.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hmj.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nza.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tdg.xylfe.cn

================================================================================
来源：http://jet.fzhhl.top

M. 命令行 / 进程 / 环境
来源：http://fpu.snrcjt.cn

================================================================================
来源：http://iwe.tarul.cn

[M01] 读取命令行参数
来源：http://wdr.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://wup.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://vwd.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://jrv.sysykeji.top

TS:   process.argv.slice(2)
来源：http://juz.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://ykj.nanxuanxn.top

Go:   os.Args[1:]
来源：http://mnb.fzhhl.top

Ruby: ARGV
来源：http://dkz.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://cex.shangyingyoupin.top

[M02] 读取环境变量
来源：http://xxu.havefunace.top

Py:   os.environ.get("HOME")
来源：http://vfn.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qkr.ydzc1.top

JS:   process.env.HOME
来源：http://tya.redwolf501.top

TS:   process.env.HOME
来源：http://mfy.zdbjq.cn

Java: System.getenv("HOME")
来源：http://jjt.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kdd.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://mvg.ivvv.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hoh.birdmap.top

[M03] 执行外部命令
来源：http://zfj.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xal.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xni.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bil.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yng.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dgs.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://saj.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://gqo.yongpay.top

C#:   Process.Start("ls", "-l");
来源：http://iao.tarul.cn

[M04] 获取当前工作目录
来源：http://rhs.daxiang520.top

Py:   os.getcwd()
来源：http://qmg.zhengqikj.top

PHP:  getcwd();
来源：http://scv.quarkkingdee.top

JS:   process.cwd()
来源：http://mvt.9152youxi.cn

TS:   process.cwd()
来源：http://fgm.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://iwt.zhiwuduotai.top

Go:   os.Getwd()
来源：http://gre.cqqwz.cn

Ruby: Dir.pwd
来源：http://ayx.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://zfd.52xcode.cn

[M05] 设置退出码
来源：http://nil.xinyue.icu

Py:   sys.exit(1)
来源：http://ezj.zhongyouzk.top

PHP:  exit(1);
来源：http://tfe.sysykeji.top

JS:   process.exit(1)
来源：http://bcx.vqdsnc.cn

TS:   process.exit(1)
来源：http://dav.ivvv.top

Java: System.exit(1)
来源：http://gue.gogol.net.cn

Go:   os.Exit(1)
来源：http://skx.nanxinkj.top

Ruby: exit 1
来源：http://vys.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mzl.jqgfzy.top

[M06] 向标准错误输出
来源：http://scu.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://gso.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bjl.shanyushiyangtech.top

JS:   console.error("err")
来源：http://rbj.xinyue.icu

TS:   console.error("err")
来源：http://ckw.hywenlv.cn

Java: System.err.println("err")
来源：http://jkg.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tdq.bbcook.cn

Ruby: warn "err"
来源：http://znn.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://sps.pycfn.com

[M07] 判断是否为主入口
来源：http://mpq.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://ucs.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lov.zhijiandao.cn

JS:   require.main === module
来源：http://tbb.fzhhl.top

TS:   require.main === module
来源：http://vvx.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://snj.316326.xyz

Go:   func main()
来源：http://mfw.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nvw.wangdashe.top

C#:   static void Main(string[] args)
来源：http://zfn.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://yho.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://jxm.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://tph.316326.xyz

JS:   process.platform;  process.version
来源：http://ikw.zhengqikj.top

TS:   process.platform;  process.version
来源：http://ogp.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://goh.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vsj.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://efs.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mxp.nanxuanxn.top

================================================================================
来源：http://sdi.hfpthk.cn

N. 数据结构与算法
来源：http://ncd.guowangkeji.top

================================================================================
来源：http://qwz.yongpay.top

[N01] 二分查找（有序数组）
来源：http://wre.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://sdn.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nfj.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wsy.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwy.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://iem.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://ibd.meibo888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://twl.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://fdc.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://nez.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://sxi.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dzk.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qkd.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qtx.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pwy.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://bgv.tarul.cn

Ruby: arr.sort
来源：http://bcl.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gxp.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://svc.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://efa.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://gnc.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hcr.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cbe.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hwo.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://awm.wangdashe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xrf.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lpt.dianchejie.cn

[N04] 斐波那契数列
来源：http://yto.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://svo.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rsx.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sot.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xox.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vbs.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mga.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://peb.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bew.hywenlv.cn

[N05] 最大公约数
来源：http://awb.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://zyj.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mof.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://poi.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jky.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kgu.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fps.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://ejl.fzhhl.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lfc.havefunace.top

[N06] 判断回文字符串
来源：http://mro.hfpthk.cn

Py:   s == s[::-1]
来源：http://olg.havefunace.top

PHP:  $s === strrev($s);
来源：http://mcx.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://oco.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://zen.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://awo.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://kqt.gaohongyu789.top

Ruby: s == s.reverse
来源：http://oai.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ifg.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://rbp.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mie.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lxz.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://btd.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://dgp.nanxinkj.top

Java: // 手写 HashMap
来源：http://ufc.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://gbp.hammf.cn

Ruby: // 手写 Hash
来源：http://tid.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jdw.pengpengdd.cyou

[N08] 生成全排列
来源：http://lmv.ydzc1.top

Py:   itertools.permutations(arr)
来源：http://jcc.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://dog.yuxming.cn

JS:   // 手写回溯递归
来源：http://wvy.fehbvm.com

TS:   // 手写回溯递归
来源：http://gdc.hywenlv.cn

Java: // 手写回溯递归
来源：http://kpd.mhx1999.top

Go:   // 手写回溯递归
来源：http://nkm.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://izm.fengsongda.top

C#:   // 手写回溯递归
来源：http://kww.chenjidiqi.icu

[N09] 栈与队列
来源：http://ulu.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cct.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gex.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ems.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jwo.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swt.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zsv.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://odl.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pgk.yueranfly.top

[N10] 链表节点定义
来源：http://bir.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://imk.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ptf.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lgj.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://raq.tarul.cn

Java: class Node { int v; Node next; }
来源：http://vep.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://zau.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://idx.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hfk.zycfv.cn

[N11] 二叉树中序遍历
来源：http://ots.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bys.birdmap.top

PHP:  // 手写递归函数
来源：http://mnh.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://msx.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgd.havefunace.top

Java: // 手写递归
来源：http://nks.bbcook.cn

Go:   // 手写递归
来源：http://big.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rti.jianghu66.top

C#:   // 手写递归
来源：http://ung.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rrp.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qhb.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exq.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vut.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kec.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://row.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rto.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://did.chenlongwang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://irs.tian-w.cn

================================================================================
来源：http://jao.shuidangran.top

O. 并发与异步
来源：http://xpc.chenjidiqi.icu

================================================================================
来源：http://uhu.gotoacloud.top

[O01] 启动一个线程
来源：http://xck.aibaodan.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kqf.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aoy.hammf.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rkg.daxiang520.top

TS:   // 同 JS
来源：http://xxk.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://acz.tianlin.xyz

Go:   go f()
来源：http://kcd.gaohongyu789.top

Ruby: Thread.new { f }
来源：http://wez.hcnkem.com

C#:   Task.Run(() => F());
来源：http://pce.hcnkem.com

[O02] 使用线程池
来源：http://inw.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ztp.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://klg.vqdsnc.cn

JS:   // worker_threads 线程池
来源：http://kqx.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://ocq.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oih.yvedp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ztc.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dsh.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://owg.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://sak.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://tky.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://pvd.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gfj.quarkkingdee.top

TS:   // 同 JS
来源：http://kmc.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://vne.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dzw.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jne.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://cab.jqgufenzy.top

[O04] 定义异步函数并等待
来源：http://wec.birdmap.top

Py:   async def f():⏎    await g()
来源：http://mlw.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yho.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://qid.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://csg.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sbo.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kin.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://skh.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://mcc.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://pns.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://dva.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jiw.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://ztg.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://clg.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dcv.sysykeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://etl.xziqi.cn

Ruby: threads.map(&:join)
来源：http://xwh.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yxg.shanyushiyangtech.top

[O06] 使用进程池
来源：http://jio.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xpr.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fgg.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://jql.sweek.top

TS:   // child_process / cluster 模块
来源：http://vsz.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rmm.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jzc.pengpengdd.cyou

Ruby: // fork 块
来源：http://nrk.shzxlz.cn

C#:   Parallel.For
来源：http://dfd.yangfankeji.com

================================================================================
来源：http://ozm.yueranfly.top

P. 常用工具函数
来源：http://bxh.feifeiyinyue.top

================================================================================
来源：http://zja.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://tbi.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://aul.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fsp.fzhhl.top

JS:   crypto.randomUUID()
来源：http://aaf.daria6918.cn

TS:   crypto.randomUUID()
来源：http://upk.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://bdz.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://xoi.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://mju.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://yjc.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://aty.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tnq.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qtj.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ftc.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kic.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://urp.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bkh.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ohb.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nkb.birdmap.top

[P03] 生成短随机字符串
来源：http://iku.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://upz.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://viu.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vra.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vot.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ynk.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nvz.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://dzp.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ugj.aibaodan.cn

[P04] 求长度
来源：http://tqf.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gdk.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zuf.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jsk.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwc.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://osd.cucudq.cn

Go:   len(arr);  len(m)
来源：http://moa.bjfxy.top

Ruby: x.length;  x.size
来源：http://ndd.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ilx.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://pfh.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://znl.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xwj.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tci.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dix.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kaz.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://dtz.havefunace.top

Ruby: a == b
来源：http://ckb.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zir.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://znx.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nwo.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://bkj.gotoacloud.top


<!-- 参考信息 -->