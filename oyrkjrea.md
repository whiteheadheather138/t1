代发 wailian999

================================================================================
来源：http://cui.sufxvd.cn

[M01] 读取命令行参数
来源：http://wva.tianlin.xyz

Py:   sys.argv[1:]
来源：http://nxr.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://yvp.tian-w.cn

JS:   process.argv.slice(2)
来源：http://uwt.fengsongda.top

TS:   process.argv.slice(2)
来源：http://dac.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://spc.bjfxy.top

Go:   os.Args[1:]
来源：http://exd.ehwqpu.com

Ruby: ARGV
来源：http://ebg.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://mlq.gaohongyu789.top

[M02] 读取环境变量
来源：http://wrb.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://mmc.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://niu.jianghu66.top

JS:   process.env.HOME
来源：http://goa.epnwcf.com

TS:   process.env.HOME
来源：http://rbl.yvedp.cn

Java: System.getenv("HOME")
来源：http://kqr.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lvf.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://uyn.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uya.jqgufenzy.top

[M03] 执行外部命令
来源：http://znd.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jxo.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hpr.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://goh.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mzb.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iam.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://urp.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://efv.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://ivl.hammf.cn

[M04] 获取当前工作目录
来源：http://fey.zdqjudy.top

Py:   os.getcwd()
来源：http://gjc.bbcook.cn

PHP:  getcwd();
来源：http://jbk.dashuyun.cn

JS:   process.cwd()
来源：http://bht.sxryk.cn

TS:   process.cwd()
来源：http://xup.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://zsd.jinghuilouyu.cn

Go:   os.Getwd()
来源：http://mfr.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://ujy.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://oph.yangfankeji.com

[M05] 设置退出码
来源：http://tym.yanxiufei.cn

Py:   sys.exit(1)
来源：http://rzm.cucudq.cn

PHP:  exit(1);
来源：http://avg.gzhubu.top

JS:   process.exit(1)
来源：http://zgz.gotoacloud.top

TS:   process.exit(1)
来源：http://mph.hammf.cn

Java: System.exit(1)
来源：http://spb.hfpthk.cn

Go:   os.Exit(1)
来源：http://pnf.snrcjt.cn

Ruby: exit 1
来源：http://tui.andypj.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gif.chenzaomai.com

[M06] 向标准错误输出
来源：http://ywg.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://iwf.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fgh.iojbl.cn

JS:   console.error("err")
来源：http://ipi.sxryk.cn

TS:   console.error("err")
来源：http://jae.ppjwa.cn

Java: System.err.println("err")
来源：http://chb.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bmk.jinqigfzy.top

Ruby: warn "err"
来源：http://pbz.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://jsh.0kj1m.cn

[M07] 判断是否为主入口
来源：http://rlt.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://hoc.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://snm.zhixingplan.top

JS:   require.main === module
来源：http://gjd.zhijiandao.cn

TS:   require.main === module
来源：http://tsl.shuidangran.top

Java: public static void main(String[] args)
来源：http://kmv.zhengqikj.top

Go:   func main()
来源：http://pmb.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zqa.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://qjb.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://lrt.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://nrs.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://qhs.yangfankeji.com

JS:   process.platform;  process.version
来源：http://lib.pycfn.com

TS:   process.platform;  process.version
来源：http://zms.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://avb.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ggu.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pgn.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://bcb.aibaodan.cn

================================================================================
来源：http://uez.nwbrower.top

N. 数据结构与算法
来源：http://yha.pycfn.com

================================================================================
来源：http://sbt.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://mjj.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://xrr.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bvd.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfn.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wpm.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://zpe.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://dnp.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mxf.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://ltc.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://ays.tianlin.xyz

Py:   sorted(arr);  arr.sort()
来源：http://kue.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fzu.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rbh.fehbvm.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://scn.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yyt.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://ubg.sysykeji.top

Ruby: arr.sort
来源：http://mdw.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lby.yongpay.top

[N03] 快速排序（分治示例）
来源：http://lvy.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ayd.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://ftu.xylfe.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://doy.zhixingplan.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gkt.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pzh.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bky.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xcj.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://wny.fengsongda.top

[N04] 斐波那契数列
来源：http://vrs.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://shf.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://edh.hysaishi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tum.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shf.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://znx.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xxu.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owo.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hqi.quarkkingdee.top

[N05] 最大公约数
来源：http://tdd.tarul.cn

Py:   math.gcd(a, b)
来源：http://goc.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zin.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfo.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvy.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lep.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rqs.xylfe.cn

Ruby: a.gcd(b)
来源：http://ftg.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xve.chenzaomai.com

[N06] 判断回文字符串
来源：http://fpy.aibaodan.cn

Py:   s == s[::-1]
来源：http://qgf.andypj.xyz

PHP:  $s === strrev($s);
来源：http://jbl.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://hbo.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://xnh.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cpy.cheryme.top

Go:   // 双指针从两端比较
来源：http://tzc.hnxiangtu.top

Ruby: s == s.reverse
来源：http://ssf.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mua.meibo888.top

[N07] 两数之和（返回下标）
来源：http://hcc.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://esp.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://enb.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rnx.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://rug.sysykeji.top

Java: // 手写 HashMap
来源：http://nrr.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://rjv.nanxinkj.top

Ruby: // 手写 Hash
来源：http://rnj.shzxlz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hsk.zhengqikj.top

[N08] 生成全排列
来源：http://kek.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://lwd.andypj.xyz

PHP:  // 手写递归交换
来源：http://aok.fengsongda.top

JS:   // 手写回溯递归
来源：http://wzk.gotoacloud.top

TS:   // 手写回溯递归
来源：http://uoy.zhixingplan.top

Java: // 手写回溯递归
来源：http://ukv.nwbrower.top

Go:   // 手写回溯递归
来源：http://rwy.meibo888.top

Ruby: arr.permutation.to_a
来源：http://fji.sweek.top

C#:   // 手写回溯递归
来源：http://qep.hongshengwenyu.top

[N09] 栈与队列
来源：http://pbv.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ojw.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ebv.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ygh.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ibm.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xvy.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jxx.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zjv.quarkkingdee.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lyg.guowangkeji.top

[N10] 链表节点定义
来源：http://ios.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ola.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://eto.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xhf.52xcode.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://any.yangfankeji.com

Java: class Node { int v; Node next; }
来源：http://ypa.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bqe.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://mkx.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ghp.jianghu66.top

[N11] 二叉树中序遍历
来源：http://bhv.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yyq.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://eyi.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rqe.sjlbkw.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqt.cucudq.cn

Java: // 手写递归
来源：http://pfp.guannengcc.top

Go:   // 手写递归
来源：http://mhn.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nfp.zhiwuduotai.top

C#:   // 手写递归
来源：http://lhh.epnwcf.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vcx.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blt.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://exo.shuidangran.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://edk.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://abe.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fhd.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lkp.quarkkingdee.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aop.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jtu.0kj1m.cn

================================================================================
来源：http://nym.daria6918.cn

O. 并发与异步
来源：http://iln.gaohongyu789.top

================================================================================
来源：http://afm.hnxiangtu.top

[O01] 启动一个线程
来源：http://nvd.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ohx.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dqh.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nxh.aizwys.cn

TS:   // 同 JS
来源：http://epr.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://fvt.tianlin.xyz

Go:   go f()
来源：http://bix.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://upp.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://onb.dianchejie.cn

[O02] 使用线程池
来源：http://cjz.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qoh.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ulz.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://khy.hcnkem.com

TS:   // worker_threads 线程池
来源：http://ckr.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://bqx.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ecx.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bxu.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gqo.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://eey.aibaodan.cn

Py:   with lock: shared += 1
来源：http://glq.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://zwp.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mxo.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://zhv.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://tiq.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://glq.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://inm.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://paq.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://rom.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://urt.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zur.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://edd.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://apr.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hld.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vqm.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://dmm.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://nzt.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://xhv.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://wkc.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ery.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://lmh.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://ths.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zia.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tmf.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://vco.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ear.chenjidiqi.icu

[O06] 使用进程池
来源：http://fby.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vwb.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cwb.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://xex.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://tzf.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wiu.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cuj.meibo888.top

Ruby: // fork 块
来源：http://ipt.cucudq.cn

C#:   Parallel.For
来源：http://gbx.andypj.xyz

================================================================================
来源：http://smb.yongpay.top

P. 常用工具函数
来源：http://sdq.jinyuanbaomall.cn

================================================================================
来源：http://ruu.ydjk.org.cn

[P01] 生成 UUID
来源：http://jtd.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://qbf.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ots.xylfe.cn

JS:   crypto.randomUUID()
来源：http://juz.zhiwuduotai.top

TS:   crypto.randomUUID()
来源：http://fvm.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://cnu.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://awj.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://zsu.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://heo.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://tre.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vgy.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tqw.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tlp.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nwa.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tvp.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mxn.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kht.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yum.dianchejie.cn

[P03] 生成短随机字符串
来源：http://lsu.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rgq.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xko.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dtg.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://unr.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iwx.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wgw.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zyc.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://urt.ydzc1.top

[P04] 求长度
来源：http://cji.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tjf.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oca.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iin.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcp.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://mop.aizwys.cn

Go:   len(arr);  len(m)
来源：http://nhw.gotoacloud.top

Ruby: x.length;  x.size
来源：http://tlk.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://gtf.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://syb.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://umv.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ybh.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gsp.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oal.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ccz.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://irw.hesvh.cn

Ruby: a == b
来源：http://ves.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://quv.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wro.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dwx.haohaochexian.top

PHP:  if (empty($x)) {}
来源：http://odj.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ndg.quarkkingdee.top

TS:   if (x == null) {}
来源：http://ygb.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gbs.nwbrower.top

Go:   if x == nil {}
来源：http://dmf.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fzd.sufxvd.cn

C#:   if (x is null) {}
来源：http://dqr.hysaishi.cn

[P07] 防抖与节流
来源：http://lsw.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nwr.ybcxt.top


<!-- 参考信息 -->