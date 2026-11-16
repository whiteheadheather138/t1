代发 wailian999

================================================================================
来源：http://eec.shuidangran.top

[M01] 读取命令行参数
来源：http://orl.tanke756.top

Py:   sys.argv[1:]
来源：http://nxq.jinqigufen.top

PHP:  $argv;  $argc;
来源：http://tfc.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://ebb.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://giq.snrcjt.cn

Java: args 数组（main 方法参数）
来源：http://zyq.yuxming.cn

Go:   os.Args[1:]
来源：http://fqg.sxryk.cn

Ruby: ARGV
来源：http://yjo.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://yzt.tarul.cn

[M02] 读取环境变量
来源：http://aah.sweek.top

Py:   os.environ.get("HOME")
来源：http://tcu.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hyh.0kj1m.cn

JS:   process.env.HOME
来源：http://fnx.cdnleiting.top

TS:   process.env.HOME
来源：http://rob.xziqi.cn

Java: System.getenv("HOME")
来源：http://xmj.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dwe.xylfe.cn

Ruby: ENV["HOME"]
来源：http://wbl.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ymc.ivvv.top

[M03] 执行外部命令
来源：http://oyw.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bqc.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://afz.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://zyv.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://owa.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cre.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dtp.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://gde.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://wch.pycfn.com

[M04] 获取当前工作目录
来源：http://vqu.uphjek.com

Py:   os.getcwd()
来源：http://woh.hnqzz.top

PHP:  getcwd();
来源：http://tbd.aizwys.cn

JS:   process.cwd()
来源：http://gtj.jinqigfzy.top

TS:   process.cwd()
来源：http://imt.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://wpp.jinqigfzy.top

Go:   os.Getwd()
来源：http://gct.chenlongwang.top

Ruby: Dir.pwd
来源：http://onk.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://gam.sufxvd.cn

[M05] 设置退出码
来源：http://jwy.ybcxt.top

Py:   sys.exit(1)
来源：http://pgo.gaohongyu789.top

PHP:  exit(1);
来源：http://jmy.feifeiyinyue.top

JS:   process.exit(1)
来源：http://nod.birdmap.top

TS:   process.exit(1)
来源：http://ypq.gogol.net.cn

Java: System.exit(1)
来源：http://nlc.meibo888.top

Go:   os.Exit(1)
来源：http://xnz.xinyue.icu

Ruby: exit 1
来源：http://dmi.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jdg.uphjek.com

[M06] 向标准错误输出
来源：http://iht.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://enp.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jxb.jinqigfzy.top

JS:   console.error("err")
来源：http://uxx.52xcode.cn

TS:   console.error("err")
来源：http://ezf.fktsv.cn

Java: System.err.println("err")
来源：http://rwe.xylfe.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fwm.yanxiufei.cn

Ruby: warn "err"
来源：http://ijq.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://gbz.cdnleiting.top

[M07] 判断是否为主入口
来源：http://ojs.pycfn.com

Py:   if __name__ == "__main__":
来源：http://pbt.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://inz.yj202588.top

JS:   require.main === module
来源：http://owt.xylfe.cn

TS:   require.main === module
来源：http://cwg.daria6918.cn

Java: public static void main(String[] args)
来源：http://izb.havefunace.top

Go:   func main()
来源：http://uex.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rbq.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://hxe.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://jzg.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://nvd.tian-w.cn

PHP:  PHP_OS;  phpversion();
来源：http://naa.jianghu66.top

JS:   process.platform;  process.version
来源：http://lxt.fengsongda.top

TS:   process.platform;  process.version
来源：http://lik.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vdk.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mvg.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lfo.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wyt.snrcjt.cn

================================================================================
来源：http://wpd.xuetiantiany.cn

N. 数据结构与算法
来源：http://pkc.sufxvd.cn

================================================================================
来源：http://wyt.yj20258888.top

[N01] 二分查找（有序数组）
来源：http://isc.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://juz.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://smu.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://odr.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvz.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bgj.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://dgl.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fhk.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://fgz.fzhhl.top

[N02] 排序（工程实践用内置实现）
来源：http://vun.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://tgn.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hdq.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://iwo.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ejz.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tbk.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://axe.hongshengwenyu.top

Ruby: arr.sort
来源：http://bhe.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://npf.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://ziy.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jjw.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://wwx.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uwr.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://spp.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mbs.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zdr.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bqt.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://adp.sjlbkw.cn

[N04] 斐波那契数列
来源：http://mfn.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qnv.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ulu.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://srq.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pem.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gze.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tho.yfazqb.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qba.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pkl.yanxiufei.cn

[N05] 最大公约数
来源：http://qwa.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://gep.52xcode.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wfh.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://skg.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://occ.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ucx.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gyd.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://bfw.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jgh.epnwcf.com

[N06] 判断回文字符串
来源：http://ulr.aibaodan.cn

Py:   s == s[::-1]
来源：http://hrw.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://ktm.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://cnd.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://awz.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jif.iojbl.cn

Go:   // 双指针从两端比较
来源：http://fbx.hammf.cn

Ruby: s == s.reverse
来源：http://gqt.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hco.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://lru.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zbj.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kre.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wxg.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://biu.cucudq.cn

Java: // 手写 HashMap
来源：http://vlb.yj20258888.top

Go:   // 手写 map[int]int
来源：http://ikq.hcnkem.com

Ruby: // 手写 Hash
来源：http://fmf.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://geg.jyoumei.cn

[N08] 生成全排列
来源：http://hes.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://psf.smart0.xyz

PHP:  // 手写递归交换
来源：http://jmc.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://ceh.yonumen.top

TS:   // 手写回溯递归
来源：http://wzr.redwolf501.top

Java: // 手写回溯递归
来源：http://kwy.meibo888.top

Go:   // 手写回溯递归
来源：http://wom.gotoacloud.top

Ruby: arr.permutation.to_a
来源：http://lyt.aibaodan.cn

C#:   // 手写回溯递归
来源：http://ary.cucudq.cn

[N09] 栈与队列
来源：http://ili.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dlt.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yju.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jkv.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lkm.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vrb.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ktq.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mvx.cashguo.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nlk.c1oappe.top

[N10] 链表节点定义
来源：http://tdk.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hqi.gaohongyu789.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uhh.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pid.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iea.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://keb.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vas.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kzk.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bnq.jianghu66.top

[N11] 二叉树中序遍历
来源：http://zon.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kcs.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://rox.sweek.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bcu.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjq.zhijiandao.cn

Java: // 手写递归
来源：http://fnl.zycfv.cn

Go:   // 手写递归
来源：http://eew.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vzh.zhijiandao.cn

C#:   // 手写递归
来源：http://wbt.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hte.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wis.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ooh.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ruw.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tqd.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vcn.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ffr.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpb.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uqv.guowangkeji.top

================================================================================
来源：http://esm.kuanghao11.cn

O. 并发与异步
来源：http://zmy.chenzaomai.com

================================================================================
来源：http://xgx.tanke756.top

[O01] 启动一个线程
来源：http://xsl.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://njx.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://imd.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zhj.jinghuilouyu.cn

TS:   // 同 JS
来源：http://gvj.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://car.iojbl.cn

Go:   go f()
来源：http://iui.ivvv.top

Ruby: Thread.new { f }
来源：http://iea.hcnkem.com

C#:   Task.Run(() => F());
来源：http://icf.chenzaomai.com

[O02] 使用线程池
来源：http://prl.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kyy.sjlbkw.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uxh.316326.xyz

JS:   // worker_threads 线程池
来源：http://mum.fktsv.cn

TS:   // worker_threads 线程池
来源：http://uye.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lrv.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ziw.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bzx.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mgo.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://bxk.hnqzz.top

Py:   with lock: shared += 1
来源：http://fld.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ktm.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iup.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://yaw.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://mzi.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tgx.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://oal.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://pmw.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://his.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://nha.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aah.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://jkf.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mwg.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tsw.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ozf.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://dyu.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://umd.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://oki.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://gwb.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ksl.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://frn.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://nbm.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zsq.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oyq.yueranfly.top

Ruby: threads.map(&:join)
来源：http://lsf.jianghu66.top

C#:   await Task.WhenAll(t1, t2)
来源：http://scx.hesvh.cn

[O06] 使用进程池
来源：http://inf.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hyy.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hbl.zhengqikj.top

JS:   // child_process / cluster 模块
来源：http://gkx.316326.xyz

TS:   // child_process / cluster 模块
来源：http://bwd.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dwj.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cxl.fengsongda.top

Ruby: // fork 块
来源：http://zqa.pycfn.com

C#:   Parallel.For
来源：http://xhf.hnxiangtu.top

================================================================================
来源：http://tic.fzhhl.top

P. 常用工具函数
来源：http://fgz.ydjk.org.cn

================================================================================
来源：http://rsp.birdmap.top

[P01] 生成 UUID
来源：http://ouo.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://rxt.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wlx.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://bzp.daxiang520.top

TS:   crypto.randomUUID()
来源：http://kkq.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://eag.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://wvg.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://fmc.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://dgv.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://sxf.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ova.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cyc.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lxg.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qtl.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wbf.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cpa.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kvr.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://poy.jiagoushi.top

[P03] 生成短随机字符串
来源：http://brz.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nfi.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vox.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://igl.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rac.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ihy.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eby.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://phh.bbcook.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qyg.tian-w.cn

[P04] 求长度
来源：http://lva.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aqz.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgt.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://way.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vva.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://zoe.redwolf501.top

Go:   len(arr);  len(m)
来源：http://ooa.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://xet.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wut.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://aox.jinqigufen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sik.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nlw.fzhhl.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lfg.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eih.vqdsnc.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dnc.jyoumei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://peu.xuanzx.com

Ruby: a == b
来源：http://nsw.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ywu.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pgl.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gdi.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://sql.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ffd.xziqi.cn

TS:   if (x == null) {}
来源：http://vao.birdmap.top

Java: if (x == null || x.isEmpty()) {}
来源：http://foc.hammf.cn

Go:   if x == nil {}
来源：http://zjr.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ugn.yj20258.top

C#:   if (x is null) {}
来源：http://udm.jqgfzy.top

[P07] 防抖与节流
来源：http://pas.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ahj.zhaomingkeji.xyz


<!-- 参考信息 -->