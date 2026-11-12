代发 wailian999

================================================================================
来源：http://kao.redwolf501.top

[M01] 读取命令行参数
来源：http://pio.jinghuilouyu.cn

Py:   sys.argv[1:]
来源：http://dfn.kuanghao11.cn

PHP:  $argv;  $argc;
来源：http://ocz.andypj.xyz

JS:   process.argv.slice(2)
来源：http://hkr.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://ipb.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://uvc.nwbrower.top

Go:   os.Args[1:]
来源：http://fqj.zycfv.cn

Ruby: ARGV
来源：http://acm.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://pmo.daxiang520.top

[M02] 读取环境变量
来源：http://zbc.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://gvg.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ekc.andypj.xyz

JS:   process.env.HOME
来源：http://eqm.snrcjt.cn

TS:   process.env.HOME
来源：http://gui.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://jms.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hah.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://oqs.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aza.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://cxj.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mis.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rpw.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tkr.jinyuanbaomall.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ayq.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gxq.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ldw.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://ild.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://ylh.iojbl.cn

[M04] 获取当前工作目录
来源：http://vmk.ppjwa.cn

Py:   os.getcwd()
来源：http://oza.fzhhl.top

PHP:  getcwd();
来源：http://kca.hnxiangtu.top

JS:   process.cwd()
来源：http://qac.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://ksr.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://eae.tanke756.top

Go:   os.Getwd()
来源：http://pti.fzhhl.top

Ruby: Dir.pwd
来源：http://hyy.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://sjc.havefunace.top

[M05] 设置退出码
来源：http://pqr.ppjwa.cn

Py:   sys.exit(1)
来源：http://zpl.hywenlv.cn

PHP:  exit(1);
来源：http://wrs.iojbl.cn

JS:   process.exit(1)
来源：http://byn.yuxming.cn

TS:   process.exit(1)
来源：http://sox.quarkkingdee.top

Java: System.exit(1)
来源：http://tld.zdqjudy.top

Go:   os.Exit(1)
来源：http://akn.yanxiufei.cn

Ruby: exit 1
来源：http://hpw.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hnx.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://jkr.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://ijn.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://elm.xuanzx.com

JS:   console.error("err")
来源：http://esx.cheryme.top

TS:   console.error("err")
来源：http://ofv.ppjwa.cn

Java: System.err.println("err")
来源：http://vvl.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://drc.zhijiandao.cn

Ruby: warn "err"
来源：http://tzy.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://xxt.shzxlz.cn

[M07] 判断是否为主入口
来源：http://fmo.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://hhe.jqgufenzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kbw.yonumen.top

JS:   require.main === module
来源：http://nkr.cqqwz.cn

TS:   require.main === module
来源：http://nif.hnqzz.top

Java: public static void main(String[] args)
来源：http://aad.jlsjyb.cn

Go:   func main()
来源：http://zjs.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mmr.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://lbs.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://gli.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://cax.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://jxl.jlsjyb.cn

JS:   process.platform;  process.version
来源：http://acl.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://cos.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lvr.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rdd.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cwy.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wit.cheryme.top

================================================================================
来源：http://cdx.sysykeji.top

N. 数据结构与算法
来源：http://lze.ctjpmb.com

================================================================================
来源：http://tlq.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://iic.guowangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://juj.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fxs.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hiz.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snl.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://hzy.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://jcw.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://otg.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://wdu.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://psj.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://qtx.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dnc.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nkg.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uqk.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kgd.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://tkv.52xcode.cn

Ruby: arr.sort
来源：http://fsh.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fqa.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://mzc.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mnp.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://afl.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ubu.redwolf501.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://age.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gtn.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hbb.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://djd.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://ewf.kuanghao11.cn

[N04] 斐波那契数列
来源：http://uym.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dxa.chenzaomai.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cus.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ygl.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nam.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ebt.fzhhl.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iwi.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://apa.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xlq.aibaodan.cn

[N05] 最大公约数
来源：http://xyc.sysykeji.top

Py:   math.gcd(a, b)
来源：http://rxe.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gdo.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://auw.zhijiandao.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tiy.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://afj.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ejc.hywenlv.cn

Ruby: a.gcd(b)
来源：http://rtg.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pvy.hysaishi.cn

[N06] 判断回文字符串
来源：http://roo.jiagoushi.top

Py:   s == s[::-1]
来源：http://pdw.xuanzx.com

PHP:  $s === strrev($s);
来源：http://nwq.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://bmi.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://mrm.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sto.meibo888.top

Go:   // 双指针从两端比较
来源：http://umf.wangdashe.top

Ruby: s == s.reverse
来源：http://pyp.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bbs.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://kys.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://keo.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://obs.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uyv.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://wob.tanke756.top

Java: // 手写 HashMap
来源：http://vjc.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://pxh.svipenyu.cn

Ruby: // 手写 Hash
来源：http://rqm.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://jga.wangshuangyany.cn

[N08] 生成全排列
来源：http://xyz.birdmap.top

Py:   itertools.permutations(arr)
来源：http://jkt.cucudq.cn

PHP:  // 手写递归交换
来源：http://fik.xuetiantiany.cn

JS:   // 手写回溯递归
来源：http://qyj.ydzc1.top

TS:   // 手写回溯递归
来源：http://pcm.fzhhl.top

Java: // 手写回溯递归
来源：http://lau.xylfe.cn

Go:   // 手写回溯递归
来源：http://yqd.ivvv.top

Ruby: arr.permutation.to_a
来源：http://zvf.hfpthk.cn

C#:   // 手写回溯递归
来源：http://okk.xuanzx.com

[N09] 栈与队列
来源：http://fzz.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tgm.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vzv.bbcook.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pnp.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mah.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yyo.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yqn.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://flx.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lyq.tianlin.xyz

[N10] 链表节点定义
来源：http://nkh.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ran.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pxj.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fxf.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ybi.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://imm.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://wga.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ykk.zhijiandao.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hyj.iojbl.cn

[N11] 二叉树中序遍历
来源：http://kzy.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zdd.tanke756.top

PHP:  // 手写递归函数
来源：http://yjk.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xkm.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kxm.meibo888.top

Java: // 手写递归
来源：http://wcg.yj20258888.top

Go:   // 手写递归
来源：http://qyx.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aao.gotoacloud.top

C#:   // 手写递归
来源：http://vjv.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wcg.yonumen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vbs.iojbl.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nze.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kor.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmu.pycfn.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mgf.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pvk.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pyl.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rcc.zhixingplan.top

================================================================================
来源：http://vcv.cqqwz.cn

O. 并发与异步
来源：http://cet.jqgufenzy.top

================================================================================
来源：http://kqe.zdbjq.cn

[O01] 启动一个线程
来源：http://ryp.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jxy.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jpi.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nun.sxryk.cn

TS:   // 同 JS
来源：http://zch.iojbl.cn

Java: new Thread(() -> f()).start()
来源：http://yor.jinyuanbaomall.cn

Go:   go f()
来源：http://hyw.epnwcf.com

Ruby: Thread.new { f }
来源：http://owi.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://nnr.redwolf501.top

[O02] 使用线程池
来源：http://pkg.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gjf.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nrb.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://ajb.daria6918.cn

TS:   // worker_threads 线程池
来源：http://wsx.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ejj.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://opn.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gsc.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tcs.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://tzv.fehbvm.com

Py:   with lock: shared += 1
来源：http://ehi.tarul.cn

PHP:  // 用 flock() 做文件锁
来源：http://wkh.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://otf.birdmap.top

TS:   // 同 JS
来源：http://zfo.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://cnm.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://imp.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yku.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://dps.hesvh.cn

[O04] 定义异步函数并等待
来源：http://yvc.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://qll.shuidangran.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kvw.daxiang520.top

JS:   async function f() { await g(); }
来源：http://szp.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://lax.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://toc.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zcn.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jib.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://sfq.yj20258.top

[O05] 并发执行并等待全部完成
来源：http://tge.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://ouy.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ftq.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://poi.316326.xyz

TS:   await Promise.all(tasks)
来源：http://hvi.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jtk.redwolf501.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zvl.gotoacloud.top

Ruby: threads.map(&:join)
来源：http://qml.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cdp.fktsv.cn

[O06] 使用进程池
来源：http://qmv.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://trn.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gpc.sweek.top

JS:   // child_process / cluster 模块
来源：http://tvr.pycfn.com

TS:   // child_process / cluster 模块
来源：http://wqj.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gsg.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kqz.zhixingplan.top

Ruby: // fork 块
来源：http://foa.uphjek.com

C#:   Parallel.For
来源：http://xfu.mhx1999.top

================================================================================
来源：http://fwa.yj20258888.top

P. 常用工具函数
来源：http://mqy.zhijiandao.cn

================================================================================
来源：http://tkm.yj202588.top

[P01] 生成 UUID
来源：http://gwe.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://ovp.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kzm.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://qyh.yj202588.top

TS:   crypto.randomUUID()
来源：http://tiw.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://mfu.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://mjm.yongpay.top

Ruby: SecureRandom.uuid
来源：http://nwk.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://dzf.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://awm.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aez.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fnw.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://afp.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pim.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rio.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kpy.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rwk.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eog.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://dmt.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oxo.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xro.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ssr.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nts.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jdk.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cjn.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bzz.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://frr.ppjwa.cn

[P04] 求长度
来源：http://wuz.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fdw.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xaa.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://brk.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jai.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://gcc.yuxming.cn

Go:   len(arr);  len(m)
来源：http://gxn.haohaochexian.top

Ruby: x.length;  x.size
来源：http://zcm.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yvy.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://jpo.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fvm.iojbl.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vgv.ppjwa.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://anw.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dss.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oex.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://jmu.daxiang520.top

Ruby: a == b
来源：http://qcx.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vsi.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gof.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://csd.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://jyg.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mpn.guowangkeji.top

TS:   if (x == null) {}
来源：http://mfj.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wag.jinqigufen.top

Go:   if x == nil {}
来源：http://mxb.316326.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://flq.ydzc1.top

C#:   if (x is null) {}
来源：http://xqb.hywenlv.cn

[P07] 防抖与节流
来源：http://lgf.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://evo.hywenlv.cn


<!-- 参考信息 -->