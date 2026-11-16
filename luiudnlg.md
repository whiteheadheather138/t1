代发 wailian999

TS:   resp.ok;  resp.status
来源：http://cav.jinqigufen.top

Java: resp.statusCode()
来源：http://luv.havefunace.top

Go:   resp.StatusCode
来源：http://wol.9152youxi.cn

Ruby: resp.code.to_i
来源：http://zma.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://aoe.birdmap.top

[L08] 并发请求多个地址
来源：http://ubf.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xkl.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://kov.gogol.net.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hfo.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mmc.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://efs.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://klu.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ihm.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://idl.gotoacloud.top

================================================================================
来源：http://efh.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://gan.bjfxy.top

================================================================================
来源：http://xmi.yongpay.top

[M01] 读取命令行参数
来源：http://oct.uphjek.com

Py:   sys.argv[1:]
来源：http://bxx.hongshengwenyu.top

PHP:  $argv;  $argc;
来源：http://svk.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://xec.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://ypx.andypj.xyz

Java: args 数组（main 方法参数）
来源：http://one.cqqwz.cn

Go:   os.Args[1:]
来源：http://jrb.nanxinkj.top

Ruby: ARGV
来源：http://ouo.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://vqk.dianchejie.cn

[M02] 读取环境变量
来源：http://ehn.havefunace.top

Py:   os.environ.get("HOME")
来源：http://lud.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tzj.xuetiantiany.cn

JS:   process.env.HOME
来源：http://gvx.fengsongda.top

TS:   process.env.HOME
来源：http://ozt.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://pzq.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uas.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://jkx.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bve.zdqjudy.top

[M03] 执行外部命令
来源：http://vnt.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eog.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ccd.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jxj.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://czx.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lgc.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vkq.jinqigufen.top

Ruby: system("ls -l");  `ls -l`
来源：http://bpi.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://liq.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://lyt.andypj.xyz

Py:   os.getcwd()
来源：http://rsc.jiagoushi.top

PHP:  getcwd();
来源：http://kdq.316326.xyz

JS:   process.cwd()
来源：http://fhk.smart0.xyz

TS:   process.cwd()
来源：http://kgv.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ari.tianlin.xyz

Go:   os.Getwd()
来源：http://zhx.sysykeji.top

Ruby: Dir.pwd
来源：http://zge.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hya.zhijiandao.cn

[M05] 设置退出码
来源：http://qgr.jqgfzy.top

Py:   sys.exit(1)
来源：http://rqc.wangshuangyany.cn

PHP:  exit(1);
来源：http://gxe.yj202588.top

JS:   process.exit(1)
来源：http://qyx.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://tlh.yfazqb.com

Java: System.exit(1)
来源：http://fvf.fehbvm.com

Go:   os.Exit(1)
来源：http://piv.shuidangran.top

Ruby: exit 1
来源：http://dur.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jfw.nanxuanxn.top

[M06] 向标准错误输出
来源：http://bph.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://ruz.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gly.tanke756.top

JS:   console.error("err")
来源：http://qwn.hnqzz.top

TS:   console.error("err")
来源：http://obn.9152youxi.cn

Java: System.err.println("err")
来源：http://kid.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fzc.vehdjk.com

Ruby: warn "err"
来源：http://eyi.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://nlr.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://qzy.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://jpg.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ziv.pengpengdd.cyou

JS:   require.main === module
来源：http://xus.chenlongwang.top

TS:   require.main === module
来源：http://lei.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://hin.zhixingplan.top

Go:   func main()
来源：http://fen.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lam.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://boz.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://idy.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://elw.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://piy.yfazqb.com

JS:   process.platform;  process.version
来源：http://bhj.aizwys.cn

TS:   process.platform;  process.version
来源：http://fib.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bfu.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://svw.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://obx.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wmy.redwolf501.top

================================================================================
来源：http://vat.daria6918.cn

N. 数据结构与算法
来源：http://ksi.aizwys.cn

================================================================================
来源：http://lym.hammf.cn

[N01] 二分查找（有序数组）
来源：http://pab.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sfw.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wip.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ifj.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://efx.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://txy.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://psu.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kpq.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pft.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://eel.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://zqx.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zir.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://knr.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dpz.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zed.aizwys.cn

Go:   slices.Sort(arr)
来源：http://ejr.redwolf501.top

Ruby: arr.sort
来源：http://ntq.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://epr.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://sox.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cdo.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://nur.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dnd.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gvg.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mwc.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://skj.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://klx.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://dkm.c1oappe.top

[N04] 斐波那契数列
来源：http://hoi.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ltm.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zsz.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xdg.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zik.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yrq.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://luw.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vmf.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iox.wangdashe.top

[N05] 最大公约数
来源：http://xrh.fzhhl.top

Py:   math.gcd(a, b)
来源：http://odh.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gyc.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kkz.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lnx.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vxt.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rkm.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://gnh.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pwi.zycfv.cn

[N06] 判断回文字符串
来源：http://cws.aibaodan.cn

Py:   s == s[::-1]
来源：http://bge.epnwcf.com

PHP:  $s === strrev($s);
来源：http://pgf.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://tls.ivvv.top

TS:   s === [...s].reverse().join("")
来源：http://spj.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hhe.316326.xyz

Go:   // 双指针从两端比较
来源：http://amy.snrcjt.cn

Ruby: s == s.reverse
来源：http://fei.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://hlc.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://rxn.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vpp.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zmq.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://lsr.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://mai.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://kza.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://qjo.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://cfo.zhengqikj.top

C#:   // 手写 Dictionary<int, int>
来源：http://bmw.nwbrower.top

[N08] 生成全排列
来源：http://yud.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://hur.daxiang520.top

PHP:  // 手写递归交换
来源：http://ybw.sxryk.cn

JS:   // 手写回溯递归
来源：http://upi.yongpay.top

TS:   // 手写回溯递归
来源：http://hrq.cdnleiting.top

Java: // 手写回溯递归
来源：http://vvw.snrcjt.cn

Go:   // 手写回溯递归
来源：http://uke.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://dmr.uphjek.com

C#:   // 手写回溯递归
来源：http://xao.fehbvm.com

[N09] 栈与队列
来源：http://ees.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aqa.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blf.chenlongwang.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wji.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tse.aizwys.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yyh.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://huc.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zkz.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zvm.tianlin.xyz

[N10] 链表节点定义
来源：http://mjd.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xcg.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hir.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://adj.jinqigufen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zqd.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://zvk.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nzv.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dmf.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mxd.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://gsa.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wwo.shzxlz.cn

PHP:  // 手写递归函数
来源：http://czd.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://slw.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zlj.svipenyu.cn

Java: // 手写递归
来源：http://wiv.yfazqb.com

Go:   // 手写递归
来源：http://olw.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yvz.c1oappe.top

C#:   // 手写递归
来源：http://fpt.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ltv.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://txi.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nvl.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjl.vehdjk.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yug.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://naq.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rct.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://csi.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kdu.shanyushiyangkeji.top

================================================================================
来源：http://msd.zhijiandao.cn

O. 并发与异步
来源：http://lhm.yanxiufei.cn

================================================================================
来源：http://fnz.yj20258.top

[O01] 启动一个线程
来源：http://ztl.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kue.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gzm.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fzm.yangfankeji.com

TS:   // 同 JS
来源：http://zjp.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://lpl.yueranfly.top

Go:   go f()
来源：http://rga.ppjwa.cn

Ruby: Thread.new { f }
来源：http://hoy.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://zlm.bbcook.cn

[O02] 使用线程池
来源：http://hvl.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ybm.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://znj.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://lwz.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://han.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://edh.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lrt.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lyp.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xox.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://iup.sysykeji.top

Py:   with lock: shared += 1
来源：http://bbe.vehdjk.com

PHP:  // 用 flock() 做文件锁
来源：http://isr.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iou.chenjidiqi.icu

TS:   // 同 JS
来源：http://jjk.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://iyz.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mcg.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://bcj.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://tyr.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://mpw.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://unv.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uzc.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://zqx.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://evv.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pdy.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jgz.shanyushiyangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://tkm.yueranfly.top

C#:   async Task F() { await G(); }
来源：http://xik.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://cag.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://gpo.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wxv.uphjek.com

JS:   await Promise.all(tasks)
来源：http://rpe.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://nif.xuanzx.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kat.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vzc.daria6918.cn

Ruby: threads.map(&:join)
来源：http://img.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nrt.cdnleiting.top

[O06] 使用进程池
来源：http://ztz.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wwq.xingfuxueyuan.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ktg.cheryme.top

JS:   // child_process / cluster 模块
来源：http://vlw.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://uva.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbv.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zye.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://bwc.zhongyouzk.top

C#:   Parallel.For
来源：http://neg.vehdjk.com

================================================================================
来源：http://cqt.hongshengwenyu.top

P. 常用工具函数
来源：http://kaw.zhongyouzk.top

================================================================================
来源：http://mqv.zhongyouzk.top

[P01] 生成 UUID
来源：http://ocg.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://rno.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xpn.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://you.smart0.xyz

TS:   crypto.randomUUID()
来源：http://pfz.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://chn.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://tel.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://rpb.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://sme.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://vvt.jqgufenzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://skb.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zur.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://esi.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bto.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yll.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cqy.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yqo.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mvc.dianchejie.cn

[P03] 生成短随机字符串
来源：http://ccf.zhiwuduotai.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cyi.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gii.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dfq.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kek.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pon.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cdt.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xhn.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bbv.ywan-chungtsiang.top

[P04] 求长度
来源：http://czr.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://djs.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cmd.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fax.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://idl.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://dvf.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://owx.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://aip.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gks.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://ubz.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tpm.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vlx.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hov.hesvh.cn


<!-- 参考信息 -->