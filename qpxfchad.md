代发 wailian999

================================================================================
来源：http://rrg.ybcxt.top

[M01] 读取命令行参数
来源：http://dhv.9152youxi.cn

Py:   sys.argv[1:]
来源：http://xrw.mhx1999.top

PHP:  $argv;  $argc;
来源：http://sti.tanke756.top

JS:   process.argv.slice(2)
来源：http://iqs.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://iaj.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://tth.hfpthk.cn

Go:   os.Args[1:]
来源：http://cku.c1oappe.top

Ruby: ARGV
来源：http://sos.xuetiantiany.cn

C#:   args 数组（Main 方法参数）
来源：http://zoe.dianchejie.cn

[M02] 读取环境变量
来源：http://kzi.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://hqy.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://knx.hammf.cn

JS:   process.env.HOME
来源：http://pth.cheryme.top

TS:   process.env.HOME
来源：http://otk.tarul.cn

Java: System.getenv("HOME")
来源：http://tpf.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ksy.xylfe.cn

Ruby: ENV["HOME"]
来源：http://qdn.316326.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://acx.uphjek.com

[M03] 执行外部命令
来源：http://aqq.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ogq.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gxn.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://krl.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://lfz.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rbb.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kqp.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://cyn.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://gzp.nwbrower.top

[M04] 获取当前工作目录
来源：http://kky.yangfankeji.com

Py:   os.getcwd()
来源：http://iwd.jinqigfzy.top

PHP:  getcwd();
来源：http://nmy.pengpengdd.cyou

JS:   process.cwd()
来源：http://jbh.cashguo.top

TS:   process.cwd()
来源：http://kyo.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://fxg.cheryme.top

Go:   os.Getwd()
来源：http://dko.vqdsnc.cn

Ruby: Dir.pwd
来源：http://hbj.yangfankeji.com

C#:   Directory.GetCurrentDirectory()
来源：http://wyz.gzhubu.top

[M05] 设置退出码
来源：http://gph.jiagoushi.top

Py:   sys.exit(1)
来源：http://zna.cdnleiting.top

PHP:  exit(1);
来源：http://ywk.jiagoushi.top

JS:   process.exit(1)
来源：http://ntz.yj20258.top

TS:   process.exit(1)
来源：http://izx.jinqigfzy.top

Java: System.exit(1)
来源：http://ics.xziqi.cn

Go:   os.Exit(1)
来源：http://abw.zhaomingkeji.xyz

Ruby: exit 1
来源：http://pze.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xlr.sjlbkw.cn

[M06] 向标准错误输出
来源：http://hsl.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://vqu.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://imb.meibo888.top

JS:   console.error("err")
来源：http://mep.vqdsnc.cn

TS:   console.error("err")
来源：http://zoc.jianghu66.top

Java: System.err.println("err")
来源：http://zmu.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lrw.pengpengdd.cyou

Ruby: warn "err"
来源：http://cgh.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://wci.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://pal.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://ohc.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hkz.jlsjyb.cn

JS:   require.main === module
来源：http://gte.wangshuangyany.cn

TS:   require.main === module
来源：http://tls.hfpthk.cn

Java: public static void main(String[] args)
来源：http://ihg.316326.xyz

Go:   func main()
来源：http://xdl.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hbh.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://gte.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://nsm.chenlongwang.top

Py:   platform.system();  platform.python_version()
来源：http://xvq.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://hgd.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://ntd.tanke756.top

TS:   process.platform;  process.version
来源：http://qzw.feifeiyinyue.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hqu.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vzl.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://emk.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oyb.aizwys.cn

================================================================================
来源：http://jyc.jyoumei.cn

N. 数据结构与算法
来源：http://drs.hnxiangtu.top

================================================================================
来源：http://mer.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://bmo.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://dni.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rvx.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vvx.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mxz.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://nnu.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://sqr.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zwo.c1oappe.top

C#:   Array.BinarySearch(arr, x)
来源：http://mnk.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://kls.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://iub.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uvs.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ifn.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jlr.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cgf.xylfe.cn

Go:   slices.Sort(arr)
来源：http://iek.dianchejie.cn

Ruby: arr.sort
来源：http://hhn.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://oiv.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://aks.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rns.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://szl.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fra.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://twy.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ikp.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ypn.xinyue.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gav.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://ech.vehdjk.com

[N04] 斐波那契数列
来源：http://for.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zor.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://chb.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tzb.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lcw.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gej.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yfy.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wtp.chenjidiqi.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xwl.ydzc1.top

[N05] 最大公约数
来源：http://spq.tian-w.cn

Py:   math.gcd(a, b)
来源：http://lwk.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghk.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gen.yueranfly.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgh.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://txf.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ifh.zdqjudy.top

Ruby: a.gcd(b)
来源：http://tzd.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tvn.bjfxy.top

[N06] 判断回文字符串
来源：http://vvq.ivvv.top

Py:   s == s[::-1]
来源：http://jwg.cheryme.top

PHP:  $s === strrev($s);
来源：http://vjg.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://khu.dashuyun.cn

TS:   s === [...s].reverse().join("")
来源：http://qij.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zun.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://hbc.jyoumei.cn

Ruby: s == s.reverse
来源：http://fxq.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ahh.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://gla.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rtu.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://caz.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vnq.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://xtz.snrcjt.cn

Java: // 手写 HashMap
来源：http://dzs.ybcxt.top

Go:   // 手写 map[int]int
来源：http://omw.wangdashe.top

Ruby: // 手写 Hash
来源：http://uhv.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://let.cheryme.top

[N08] 生成全排列
来源：http://dhh.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://rft.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://nha.snrcjt.cn

JS:   // 手写回溯递归
来源：http://luf.sufxvd.cn

TS:   // 手写回溯递归
来源：http://zqk.yuxming.cn

Java: // 手写回溯递归
来源：http://hus.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://hfw.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://spq.aibaodan.cn

C#:   // 手写回溯递归
来源：http://rft.jinqigfzy.top

[N09] 栈与队列
来源：http://vfz.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qpd.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sqa.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ody.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://snk.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://byf.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rqv.jiagoushi.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zyw.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qzf.xuetiantiany.cn

[N10] 链表节点定义
来源：http://oyp.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ojm.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cfm.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fys.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zqe.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://hfo.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://eni.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://sex.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gnv.hesvh.cn

[N11] 二叉树中序遍历
来源：http://xwc.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gbo.nwbrower.top

PHP:  // 手写递归函数
来源：http://oyc.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xag.jqgufenzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hdn.52xcode.cn

Java: // 手写递归
来源：http://tlw.sweek.top

Go:   // 手写递归
来源：http://dbl.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mjc.kuanghao11.cn

C#:   // 手写递归
来源：http://yqk.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zcr.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mbs.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dku.shangyingyoupin.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://trc.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vuz.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yrj.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kzv.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://enj.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://skv.c1oappe.top

================================================================================
来源：http://mth.quarkkingdee.top

O. 并发与异步
来源：http://sic.hammf.cn

================================================================================
来源：http://jzh.jyoumei.cn

[O01] 启动一个线程
来源：http://cbf.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kdz.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qsg.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pfu.gogol.net.cn

TS:   // 同 JS
来源：http://pkn.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://yrs.dashuyun.cn

Go:   go f()
来源：http://sqq.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://bry.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://hdl.hfpthk.cn

[O02] 使用线程池
来源：http://hpn.fengsongda.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mgn.fehbvm.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hqi.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://pqn.cheryme.top

TS:   // worker_threads 线程池
来源：http://xxs.havefunace.top

Java: Executors.newFixedThreadPool(4)
来源：http://iod.ydjk.org.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://usj.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sqj.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://urg.yonumen.top

[O03] 加锁保护共享数据
来源：http://nck.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://ntn.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://lym.9152youxi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jdd.quarkkingdee.top

TS:   // 同 JS
来源：http://rws.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://fdm.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://njh.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqf.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://fwc.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://qny.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://xkr.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tst.tanke756.top

JS:   async function f() { await g(); }
来源：http://fnk.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://upg.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kce.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yma.yj20258.top

Ruby: # 用 Fiber 或 async gem
来源：http://yug.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://pge.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://oda.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://tro.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ord.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://wnz.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://iii.xylfe.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pjx.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://puz.shuidangran.top

Ruby: threads.map(&:join)
来源：http://uqc.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aiy.cheryme.top

[O06] 使用进程池
来源：http://plx.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fqr.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ddm.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://mwi.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://xyp.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cja.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ora.fktsv.cn

Ruby: // fork 块
来源：http://ojb.jqgfzy.top

C#:   Parallel.For
来源：http://jwe.quarkkingdee.top

================================================================================
来源：http://hgl.tarul.cn

P. 常用工具函数
来源：http://yrx.ctjpmb.com

================================================================================
来源：http://vog.cdnleiting.top

[P01] 生成 UUID
来源：http://orc.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://oet.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://epb.nwbrower.top

JS:   crypto.randomUUID()
来源：http://bqz.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://rtm.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://jbt.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://law.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://fuj.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://evx.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://lsf.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vsz.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rvg.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lga.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://okm.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zvz.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ebq.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vec.jiagoushi.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://shp.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://swm.nanxuanxn.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://chu.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rel.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ubq.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bni.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://evn.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lqn.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ukh.cheryme.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qpd.c1oappe.top

[P04] 求长度
来源：http://wsc.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mjg.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wzi.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyp.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ttn.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://nxu.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://ipc.sufxvd.cn

Ruby: x.length;  x.size
来源：http://xvi.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dlp.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://zkx.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kbf.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://opf.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uos.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ihn.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://msb.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://zyk.yj20258.top

Ruby: a == b
来源：http://swh.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hsw.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fhl.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kvq.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://prz.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xmn.chenlongwang.top

TS:   if (x == null) {}
来源：http://lar.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pnk.hfpthk.cn

Go:   if x == nil {}
来源：http://ibk.wangshuangyany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ppd.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://shf.quarkkingdee.top

[P07] 防抖与节流
来源：http://qmw.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xlc.yj20258888.top


<!-- 参考信息 -->