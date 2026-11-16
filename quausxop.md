代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://luy.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yer.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://oud.yuxming.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mcl.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://goh.c1oappe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hwu.ydzc1.top

================================================================================
来源：http://xom.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://czj.gogol.net.cn

================================================================================
来源：http://fai.yanxiufei.cn

[M01] 读取命令行参数
来源：http://poe.bjfxy.top

Py:   sys.argv[1:]
来源：http://auu.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://bnr.tanke756.top

JS:   process.argv.slice(2)
来源：http://wwu.ybcxt.top

TS:   process.argv.slice(2)
来源：http://eiu.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://lfb.gzhubu.top

Go:   os.Args[1:]
来源：http://jft.zycfv.cn

Ruby: ARGV
来源：http://xrs.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://hvq.chenjidiqi.icu

[M02] 读取环境变量
来源：http://jcp.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://ejq.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://otl.tarul.cn

JS:   process.env.HOME
来源：http://smg.xylfe.cn

TS:   process.env.HOME
来源：http://dae.jlsjyb.cn

Java: System.getenv("HOME")
来源：http://jdm.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uxb.iojbl.cn

Ruby: ENV["HOME"]
来源：http://dxw.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jiy.xylfe.cn

[M03] 执行外部命令
来源：http://lnr.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://agn.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://trq.yuxming.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xlo.zhoulong.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xtf.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hqv.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://eoe.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://zvm.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://zkx.xziqi.cn

[M04] 获取当前工作目录
来源：http://vvt.ybcxt.top

Py:   os.getcwd()
来源：http://yiy.zdbjq.cn

PHP:  getcwd();
来源：http://uic.zdqjudy.top

JS:   process.cwd()
来源：http://lta.dianchejie.cn

TS:   process.cwd()
来源：http://klh.quarkkingdee.top

Java: Path.of("").toAbsolutePath()
来源：http://idp.aizwys.cn

Go:   os.Getwd()
来源：http://ast.hywenlv.cn

Ruby: Dir.pwd
来源：http://enq.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://iwr.quarkkingdee.top

[M05] 设置退出码
来源：http://tzg.kuanghao11.cn

Py:   sys.exit(1)
来源：http://qfj.shzxlz.cn

PHP:  exit(1);
来源：http://hwo.uphjek.com

JS:   process.exit(1)
来源：http://uuh.feifeiyinyue.top

TS:   process.exit(1)
来源：http://ghx.ydjk.org.cn

Java: System.exit(1)
来源：http://mpe.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://qrv.xinyue.icu

Ruby: exit 1
来源：http://nxx.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ocj.fengsongda.top

[M06] 向标准错误输出
来源：http://pjh.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://puv.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cca.316326.xyz

JS:   console.error("err")
来源：http://edc.fehbvm.com

TS:   console.error("err")
来源：http://wlx.aizwys.cn

Java: System.err.println("err")
来源：http://ado.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://clk.pengpengdd.cyou

Ruby: warn "err"
来源：http://eow.zhoulong.xyz

C#:   Console.Error.WriteLine("err")
来源：http://gkn.jyoumei.cn

[M07] 判断是否为主入口
来源：http://xvb.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://hdn.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://shz.daria6918.cn

JS:   require.main === module
来源：http://got.jqgufenzy.top

TS:   require.main === module
来源：http://fkt.ehwqpu.com

Java: public static void main(String[] args)
来源：http://bjq.jianghu66.top

Go:   func main()
来源：http://rfn.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kgg.wangdashe.top

C#:   static void Main(string[] args)
来源：http://mju.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://jux.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://pbm.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://yox.tianlin.xyz

JS:   process.platform;  process.version
来源：http://mds.yj20258.top

TS:   process.platform;  process.version
来源：http://drl.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yyq.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uta.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxg.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fcm.daria6918.cn

================================================================================
来源：http://jns.bbcook.cn

N. 数据结构与算法
来源：http://cnr.shuidangran.top

================================================================================
来源：http://otl.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://fed.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ubx.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xql.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nms.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fww.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ivn.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://rbo.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lam.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://ici.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://tft.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://wxv.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mde.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nfo.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://tqh.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hny.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://xzm.jinyuanbaomall.cn

Ruby: arr.sort
来源：http://phb.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gtv.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://twf.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://stc.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://mzh.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ofl.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yuj.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://msi.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xsg.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iaw.xziqi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kgk.jqgfzy.top

[N04] 斐波那契数列
来源：http://xop.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pak.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://knu.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://izv.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qhh.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jda.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pnd.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pru.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zjc.haohaochexian.top

[N05] 最大公约数
来源：http://jzu.iojbl.cn

Py:   math.gcd(a, b)
来源：http://cxo.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jsi.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byo.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vuj.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gia.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zia.cucudq.cn

Ruby: a.gcd(b)
来源：http://jod.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ikv.zhoulong.xyz

[N06] 判断回文字符串
来源：http://ajt.yongpay.top

Py:   s == s[::-1]
来源：http://gyu.sweek.top

PHP:  $s === strrev($s);
来源：http://tjb.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://nfs.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://jky.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lxx.yongpay.top

Go:   // 双指针从两端比较
来源：http://vwg.tarul.cn

Ruby: s == s.reverse
来源：http://wmd.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xjr.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://jyl.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cmt.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://klq.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qfn.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://bmv.smart0.xyz

Java: // 手写 HashMap
来源：http://aca.iojbl.cn

Go:   // 手写 map[int]int
来源：http://gca.hesvh.cn

Ruby: // 手写 Hash
来源：http://zdt.birdmap.top

C#:   // 手写 Dictionary<int, int>
来源：http://cfo.0kj1m.cn

[N08] 生成全排列
来源：http://vro.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://uxv.haohaochexian.top

PHP:  // 手写递归交换
来源：http://bmn.316326.xyz

JS:   // 手写回溯递归
来源：http://tvm.birdmap.top

TS:   // 手写回溯递归
来源：http://vsj.ybcxt.top

Java: // 手写回溯递归
来源：http://obt.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://kdz.tanke756.top

Ruby: arr.permutation.to_a
来源：http://atk.xziqi.cn

C#:   // 手写回溯递归
来源：http://gyg.chenlongwang.top

[N09] 栈与队列
来源：http://nib.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vth.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ufm.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://awa.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hej.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://skh.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hql.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qml.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://djv.ydjk.org.cn

[N10] 链表节点定义
来源：http://iji.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ihg.cucudq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sth.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bse.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nkv.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://lqy.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://qyy.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dja.iojbl.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://lae.yj20258.top

[N11] 二叉树中序遍历
来源：http://qyv.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wol.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://fpz.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wbm.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rfp.birdmap.top

Java: // 手写递归
来源：http://bvk.hesvh.cn

Go:   // 手写递归
来源：http://zrs.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mtu.jqgufenzy.top

C#:   // 手写递归
来源：http://uwy.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dsc.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rry.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jrg.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dfw.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://req.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://scn.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tib.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ngh.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xlm.pycfn.com

================================================================================
来源：http://cbo.yangfankeji.com

O. 并发与异步
来源：http://awu.zdbjq.cn

================================================================================
来源：http://veu.yj20258.top

[O01] 启动一个线程
来源：http://kwn.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jnd.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jwd.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bdy.ybcxt.top

TS:   // 同 JS
来源：http://mhh.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://dzo.shzxlz.cn

Go:   go f()
来源：http://krx.svipenyu.cn

Ruby: Thread.new { f }
来源：http://qyq.daxiang520.top

C#:   Task.Run(() => F());
来源：http://afr.hcnkem.com

[O02] 使用线程池
来源：http://dpw.jiagoushi.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qmh.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pjg.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://tkc.hesvh.cn

TS:   // worker_threads 线程池
来源：http://gix.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://sdk.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dyi.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://auq.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zly.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://lqw.ydzc1.top

Py:   with lock: shared += 1
来源：http://pnc.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://muz.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gga.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://duu.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://klk.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://imh.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cau.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://uub.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://crj.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://eba.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://btg.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://onw.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://olp.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://abq.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ccz.havefunace.top

Ruby: # 用 Fiber 或 async gem
来源：http://xwc.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://pnn.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://gud.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://wga.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dmw.cashguo.top

JS:   await Promise.all(tasks)
来源：http://xis.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://dcq.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://phx.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zbw.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://vvr.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://axz.gzhubu.top

[O06] 使用进程池
来源：http://wrp.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ixo.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://maw.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://gkb.yonumen.top

TS:   // child_process / cluster 模块
来源：http://fiy.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mcb.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ozz.pengpengdd.cyou

Ruby: // fork 块
来源：http://tts.guannengcc.top

C#:   Parallel.For
来源：http://oux.yvedp.cn

================================================================================
来源：http://hbr.jyoumei.cn

P. 常用工具函数
来源：http://pnw.cucudq.cn

================================================================================
来源：http://gjr.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://gcw.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://akz.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zlg.xziqi.cn

JS:   crypto.randomUUID()
来源：http://yrl.fzhhl.top

TS:   crypto.randomUUID()
来源：http://mli.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://pof.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://ijz.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://itj.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://nbj.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://dbd.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://azt.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ham.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uhb.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bwi.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jpc.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rys.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vxt.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://icu.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://dwa.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hjq.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kwr.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://euf.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tfs.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oni.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tsx.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fyj.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rew.chenjidiqi.icu

[P04] 求长度
来源：http://vnq.9152youxi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vea.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ajm.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tpy.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mpr.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://buq.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://drk.xingfuxueyuan.xyz

Ruby: x.length;  x.size
来源：http://yux.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xpf.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://ifb.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xwq.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://upd.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qbl.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wey.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bas.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://irg.birdmap.top

Ruby: a == b
来源：http://mgw.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lph.wangshuangyany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dzp.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dkh.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://grf.gaohongyu789.top


<!-- 参考信息 -->