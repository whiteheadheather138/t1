代发 wailian999

JS:   process.argv.slice(2)
来源：http://ooc.316326.xyz

TS:   process.argv.slice(2)
来源：http://ubt.ivvv.top

Java: args 数组（main 方法参数）
来源：http://mrg.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://lsk.sjlbkw.cn

Ruby: ARGV
来源：http://hgs.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://zfh.nanxuanxn.top

[M02] 读取环境变量
来源：http://ono.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://mif.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qqx.sweek.top

JS:   process.env.HOME
来源：http://ucs.fzhhl.top

TS:   process.env.HOME
来源：http://phc.xylfe.cn

Java: System.getenv("HOME")
来源：http://hsa.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cng.redwolf501.top

Ruby: ENV["HOME"]
来源：http://xxc.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sry.zhijiandao.cn

[M03] 执行外部命令
来源：http://umr.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kkg.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zdl.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://slz.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wrd.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://odx.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zcz.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://vzf.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://mll.tianlin.xyz

[M04] 获取当前工作目录
来源：http://tjy.zhijiandao.cn

Py:   os.getcwd()
来源：http://eaw.yangfankeji.com

PHP:  getcwd();
来源：http://bxj.sweek.top

JS:   process.cwd()
来源：http://hpb.gotoacloud.top

TS:   process.cwd()
来源：http://wsu.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://eih.nwbrower.top

Go:   os.Getwd()
来源：http://gim.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://spk.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://owy.nanxuanxn.top

[M05] 设置退出码
来源：http://qyb.xziqi.cn

Py:   sys.exit(1)
来源：http://smj.zycfv.cn

PHP:  exit(1);
来源：http://wvh.jiagoushi.top

JS:   process.exit(1)
来源：http://fdx.vqdsnc.cn

TS:   process.exit(1)
来源：http://caa.xziqi.cn

Java: System.exit(1)
来源：http://vdl.nwbrower.top

Go:   os.Exit(1)
来源：http://rut.ybcxt.top

Ruby: exit 1
来源：http://mqt.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://loo.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://cve.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://qtd.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gol.feifeiyinyue.top

JS:   console.error("err")
来源：http://atk.nanxuanxn.top

TS:   console.error("err")
来源：http://wga.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://oca.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ntg.hongshengwenyu.top

Ruby: warn "err"
来源：http://nue.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://alu.bjfxy.top

[M07] 判断是否为主入口
来源：http://iao.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://mbw.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bmq.shangyingyoupin.top

JS:   require.main === module
来源：http://jdn.hnxiangtu.top

TS:   require.main === module
来源：http://kti.jyoumei.cn

Java: public static void main(String[] args)
来源：http://epo.sjlbkw.cn

Go:   func main()
来源：http://nhb.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bni.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://asu.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://iyc.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://jeg.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://alx.ehwqpu.com

JS:   process.platform;  process.version
来源：http://owh.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://pbm.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lsb.havefunace.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://njg.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wbg.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fgx.cqqwz.cn

================================================================================
来源：http://obs.sufxvd.cn

N. 数据结构与算法
来源：http://nfq.shanyushiyangtech.top

================================================================================
来源：http://vei.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://awe.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://ifq.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dqi.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwo.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ivr.jianghu66.top

Java: Arrays.binarySearch(arr, x)
来源：http://xsh.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://nyd.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ccb.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lvy.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://dyf.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://cwm.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://txw.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://cpg.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bbi.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://six.hammf.cn

Go:   slices.Sort(arr)
来源：http://nno.tian-w.cn

Ruby: arr.sort
来源：http://kzp.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tim.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://cdo.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lom.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://owi.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://czq.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://peg.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ick.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fjf.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yoj.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wyi.hcnkem.com

[N04] 斐波那契数列
来源：http://bdh.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nsg.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xrv.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rhs.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jhs.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dul.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xxt.smart0.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://opv.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fpn.jyoumei.cn

[N05] 最大公约数
来源：http://mtn.shanyushiyangkeji.top

Py:   math.gcd(a, b)
来源：http://doq.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fhm.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zjz.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ync.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wkt.yuxming.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jtm.9152youxi.cn

Ruby: a.gcd(b)
来源：http://pgx.gaohongyu789.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rft.ybcxt.top

[N06] 判断回文字符串
来源：http://njm.fzhhl.top

Py:   s == s[::-1]
来源：http://khi.cashguo.top

PHP:  $s === strrev($s);
来源：http://zfe.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://vud.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://lxu.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xtq.smart0.xyz

Go:   // 双指针从两端比较
来源：http://ofj.yj20258888.top

Ruby: s == s.reverse
来源：http://yfa.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zny.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://aln.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://poo.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tve.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://fzs.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://tft.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://zea.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://gft.tarul.cn

Ruby: // 手写 Hash
来源：http://der.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://fzn.quarkkingdee.top

[N08] 生成全排列
来源：http://uyn.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://ljl.tianlin.xyz

PHP:  // 手写递归交换
来源：http://nxx.aizwys.cn

JS:   // 手写回溯递归
来源：http://bgz.uphjek.com

TS:   // 手写回溯递归
来源：http://yat.ppjwa.cn

Java: // 手写回溯递归
来源：http://yxj.chenlongwang.top

Go:   // 手写回溯递归
来源：http://dkj.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://vap.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://tlf.ctjpmb.com

[N09] 栈与队列
来源：http://neh.xingfuxueyuan.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ajw.jinghuilouyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bjl.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ssc.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pvm.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://leh.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kvv.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jek.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mhv.sxryk.cn

[N10] 链表节点定义
来源：http://vth.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jsy.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://goq.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ovc.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gpm.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://oeh.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://czu.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://flx.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xuq.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://qko.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wcb.bbcook.cn

PHP:  // 手写递归函数
来源：http://erj.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xut.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqk.yueranfly.top

Java: // 手写递归
来源：http://cld.fehbvm.com

Go:   // 手写递归
来源：http://ipq.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://agw.svipenyu.cn

C#:   // 手写递归
来源：http://kye.tanke756.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://sbq.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://luy.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://emq.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmj.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://umg.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eqf.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oxe.yanxiufei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjc.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gnw.epnwcf.com

================================================================================
来源：http://nnc.yonumen.top

O. 并发与异步
来源：http://gfr.0kj1m.cn

================================================================================
来源：http://ylj.yuanzhike.top

[O01] 启动一个线程
来源：http://ffu.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cca.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ltj.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tci.xuetiantiany.cn

TS:   // 同 JS
来源：http://ujc.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://wlj.epnwcf.com

Go:   go f()
来源：http://dnk.vehdjk.com

Ruby: Thread.new { f }
来源：http://ufj.havefunace.top

C#:   Task.Run(() => F());
来源：http://jyc.quarkkingdee.top

[O02] 使用线程池
来源：http://ypu.ydjk.org.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ivc.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://miy.sxryk.cn

JS:   // worker_threads 线程池
来源：http://jhx.yvedp.cn

TS:   // worker_threads 线程池
来源：http://uxy.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://kdu.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iiq.tanke756.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bku.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zfo.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://igl.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://wdp.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://lvy.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nij.gotoacloud.top

TS:   // 同 JS
来源：http://gec.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://hui.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bem.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hfd.c1oappe.top

C#:   lock (gate) { shared++; }
来源：http://plx.fktsv.cn

[O04] 定义异步函数并等待
来源：http://vvz.cashguo.top

Py:   async def f():⏎    await g()
来源：http://pbl.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ifb.xinyue.icu

JS:   async function f() { await g(); }
来源：http://ors.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://obe.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rko.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://car.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://zmy.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://wok.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://bvf.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://yia.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xfb.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://nlx.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://adu.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dxd.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uiu.daxiang520.top

Ruby: threads.map(&:join)
来源：http://gpb.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bin.zhijiandao.cn

[O06] 使用进程池
来源：http://zru.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vyd.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://txa.uphjek.com

JS:   // child_process / cluster 模块
来源：http://vga.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://wrm.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tuo.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xlg.gaohongyu789.top

Ruby: // fork 块
来源：http://swd.yangfankeji.com

C#:   Parallel.For
来源：http://qnx.nanxinkj.top

================================================================================
来源：http://ujw.chenlongwang.top

P. 常用工具函数
来源：http://rfa.ppjwa.cn

================================================================================
来源：http://wsu.nwbrower.top

[P01] 生成 UUID
来源：http://vco.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://jdw.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wpw.cucudq.cn

JS:   crypto.randomUUID()
来源：http://deq.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://rsf.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://gtm.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://hir.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://iws.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://ovw.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://irx.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lsy.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vgx.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sny.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://arz.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://okf.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vsg.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gkz.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://egv.svipenyu.cn

[P03] 生成短随机字符串
来源：http://uzh.cheryme.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://idt.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oiy.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cte.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xqw.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aiv.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yta.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bbe.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://imc.jiagoushi.top

[P04] 求长度
来源：http://bpb.cucudq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zby.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rjf.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xaw.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nry.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://coo.mhx1999.top

Go:   len(arr);  len(m)
来源：http://ubr.guowangkeji.top

Ruby: x.length;  x.size
来源：http://isu.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://guf.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://ldm.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lfx.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lnb.cdnleiting.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://adl.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nub.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bef.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ror.316326.xyz

Ruby: a == b
来源：http://cut.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lik.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vta.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jqp.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://dqc.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://svt.hesvh.cn

TS:   if (x == null) {}
来源：http://xbx.cashguo.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hqy.bbcook.cn

Go:   if x == nil {}
来源：http://ajs.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jgs.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://yjm.316326.xyz

[P07] 防抖与节流
来源：http://hhw.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://apk.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://msw.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svb.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://noj.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jej.hesvh.cn


<!-- 参考信息 -->