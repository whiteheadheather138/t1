代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cjy.zycfv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhl.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cci.ywan-chungtsiang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uve.dashuyun.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://llg.zhengqikj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://egd.redwolf501.top

================================================================================
来源：http://qyl.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://zzc.hcnkem.com

================================================================================
来源：http://uwo.cdnleiting.top

[M01] 读取命令行参数
来源：http://rrs.havefunace.top

Py:   sys.argv[1:]
来源：http://ujf.sysykeji.top

PHP:  $argv;  $argc;
来源：http://gyz.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://wvd.hnqzz.top

TS:   process.argv.slice(2)
来源：http://cch.yonumen.top

Java: args 数组（main 方法参数）
来源：http://pdr.tanke756.top

Go:   os.Args[1:]
来源：http://gcs.svipenyu.cn

Ruby: ARGV
来源：http://msk.yangfankeji.com

C#:   args 数组（Main 方法参数）
来源：http://rhv.bbcook.cn

[M02] 读取环境变量
来源：http://imc.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://tvl.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zqh.nanxuanxn.top

JS:   process.env.HOME
来源：http://ria.yfazqb.com

TS:   process.env.HOME
来源：http://ken.andypj.xyz

Java: System.getenv("HOME")
来源：http://kol.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uqw.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://qxq.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hnq.andypj.xyz

[M03] 执行外部命令
来源：http://lbi.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sch.zhoulong.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qqp.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://iox.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jwp.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tio.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cxr.nanxuanxn.top

Ruby: system("ls -l");  `ls -l`
来源：http://ohi.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://fjp.feifeiyinyue.top

[M04] 获取当前工作目录
来源：http://fbo.ehwqpu.com

Py:   os.getcwd()
来源：http://icq.feifeiyinyue.top

PHP:  getcwd();
来源：http://zno.yangfankeji.com

JS:   process.cwd()
来源：http://syb.9152youxi.cn

TS:   process.cwd()
来源：http://nzm.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://avr.yanxiufei.cn

Go:   os.Getwd()
来源：http://tje.yvedp.cn

Ruby: Dir.pwd
来源：http://twi.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://aax.gaohongyu789.top

[M05] 设置退出码
来源：http://dxo.iojbl.cn

Py:   sys.exit(1)
来源：http://mrt.gogol.net.cn

PHP:  exit(1);
来源：http://cnt.jinqigfzy.top

JS:   process.exit(1)
来源：http://esx.gzhubu.top

TS:   process.exit(1)
来源：http://apu.quarkkingdee.top

Java: System.exit(1)
来源：http://oma.fzhhl.top

Go:   os.Exit(1)
来源：http://cgg.svipenyu.cn

Ruby: exit 1
来源：http://qtk.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cnx.hnxiangtu.top

[M06] 向标准错误输出
来源：http://pir.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://axp.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nzn.shangyingyoupin.top

JS:   console.error("err")
来源：http://xaa.52xcode.cn

TS:   console.error("err")
来源：http://wkm.yj20258.top

Java: System.err.println("err")
来源：http://lpz.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mry.gotoacloud.top

Ruby: warn "err"
来源：http://gmy.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://mcs.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://zvv.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://tgz.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kyk.zdbjq.cn

JS:   require.main === module
来源：http://dsd.c1oappe.top

TS:   require.main === module
来源：http://fbw.hesvh.cn

Java: public static void main(String[] args)
来源：http://cab.aizwys.cn

Go:   func main()
来源：http://iyb.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cmr.nwbrower.top

C#:   static void Main(string[] args)
来源：http://mch.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://enp.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://xzs.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://aqc.cqqwz.cn

JS:   process.platform;  process.version
来源：http://upp.bjfxy.top

TS:   process.platform;  process.version
来源：http://tvk.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ceg.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bgr.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vin.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cbq.yonumen.top

================================================================================
来源：http://tzk.sxryk.cn

N. 数据结构与算法
来源：http://bco.jinqigufen.top

================================================================================
来源：http://cji.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://lgm.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://oiv.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sub.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwf.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yoo.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://opw.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://kye.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gvf.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://ahu.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://wia.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://zuk.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kkr.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ckf.sjlbkw.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bqg.meibo888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bmw.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://bhp.smart0.xyz

Ruby: arr.sort
来源：http://ycj.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qqg.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://ssv.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uvt.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://llp.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nzh.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mgg.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wrd.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jnz.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ttd.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wln.xuanzx.com

[N04] 斐波那契数列
来源：http://hjt.ybcxt.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zdz.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://boz.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jpg.jinqigufen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bad.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uzw.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qyt.fehbvm.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xji.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wwp.gzhubu.top

[N05] 最大公约数
来源：http://snf.sysykeji.top

Py:   math.gcd(a, b)
来源：http://awm.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fhb.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yuq.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dfv.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fom.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hjp.jyoumei.cn

Ruby: a.gcd(b)
来源：http://irg.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lgh.hfpthk.cn

[N06] 判断回文字符串
来源：http://fme.jyoumei.cn

Py:   s == s[::-1]
来源：http://vho.andypj.xyz

PHP:  $s === strrev($s);
来源：http://dyh.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://cdf.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://hsk.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://evd.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://lif.yangfankeji.com

Ruby: s == s.reverse
来源：http://zhk.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://pag.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://pts.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fpl.shuidangran.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pma.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zta.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://pdn.jinyuanbaomall.cn

Java: // 手写 HashMap
来源：http://epl.52xcode.cn

Go:   // 手写 map[int]int
来源：http://ewn.hcnkem.com

Ruby: // 手写 Hash
来源：http://tcd.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jrt.ydzc1.top

[N08] 生成全排列
来源：http://uaf.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://nuo.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://inf.jyoumei.cn

JS:   // 手写回溯递归
来源：http://pkf.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://chg.birdmap.top

Java: // 手写回溯递归
来源：http://ken.andypj.xyz

Go:   // 手写回溯递归
来源：http://fic.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://avc.uphjek.com

C#:   // 手写回溯递归
来源：http://jle.ivvv.top

[N09] 栈与队列
来源：http://vlw.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zja.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ujd.shzxlz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mvs.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tlb.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pyh.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://epw.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cbs.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uaj.gaohongyu789.top

[N10] 链表节点定义
来源：http://ysy.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qek.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vgv.shzxlz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qyr.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pqj.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://hfp.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hiv.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nyd.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://itu.yuxming.cn

[N11] 二叉树中序遍历
来源：http://arx.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zxb.yj20258888.top

PHP:  // 手写递归函数
来源：http://okc.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zks.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bza.c1oappe.top

Java: // 手写递归
来源：http://hyy.zdbjq.cn

Go:   // 手写递归
来源：http://sml.jiagoushi.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gwz.gzhubu.top

C#:   // 手写递归
来源：http://vmj.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://waa.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://geu.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pck.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tvw.gaohongyu789.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ary.sysykeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ojs.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nnd.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wlu.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hth.daxiang520.top

================================================================================
来源：http://hlo.dianchejie.cn

O. 并发与异步
来源：http://duc.xuanzx.com

================================================================================
来源：http://qch.epnwcf.com

[O01] 启动一个线程
来源：http://yqz.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://osc.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aoq.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zgu.nanxinkj.top

TS:   // 同 JS
来源：http://lde.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://ofw.gzhubu.top

Go:   go f()
来源：http://kfq.ivvv.top

Ruby: Thread.new { f }
来源：http://vyx.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://evb.feifeiyinyue.top

[O02] 使用线程池
来源：http://dlm.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hao.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jch.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://vcy.mhx1999.top

TS:   // worker_threads 线程池
来源：http://ohy.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://rjr.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://evk.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qlm.tarul.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uau.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://lyn.sufxvd.cn

Py:   with lock: shared += 1
来源：http://ula.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://jiv.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://une.vqdsnc.cn

TS:   // 同 JS
来源：http://wkz.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://gpe.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mvy.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zfb.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://ooq.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://hdy.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://jxd.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://whc.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://kaj.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://erb.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hir.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ttv.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://ggw.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://syv.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://hnc.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://awr.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://waw.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://vfb.yanxiufei.cn

TS:   await Promise.all(tasks)
来源：http://slv.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://utk.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zbi.epnwcf.com

Ruby: threads.map(&:join)
来源：http://bcw.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://duu.jinyuanbaomall.cn

[O06] 使用进程池
来源：http://bva.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hhd.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://ckc.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://xmz.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://lwu.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jep.ydzc1.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ipf.uphjek.com

Ruby: // fork 块
来源：http://jse.nanxuanxn.top

C#:   Parallel.For
来源：http://zok.ydjk.org.cn

================================================================================
来源：http://xbi.zhengqikj.top

P. 常用工具函数
来源：http://xwy.guowangkeji.top

================================================================================
来源：http://bjd.tarul.cn

[P01] 生成 UUID
来源：http://fyv.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://xrg.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pyy.zdbjq.cn

JS:   crypto.randomUUID()
来源：http://otj.tarul.cn

TS:   crypto.randomUUID()
来源：http://ron.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://ddf.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://ece.ydjk.org.cn

Ruby: SecureRandom.uuid
来源：http://hvp.tian-w.cn

C#:   Guid.NewGuid().ToString()
来源：http://ocq.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://hup.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tyt.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmh.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://awl.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mgz.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dze.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://olp.shanyushiyangtech.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zau.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ydw.guowangkeji.top

[P03] 生成短随机字符串
来源：http://thc.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://idt.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mmx.guowangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kec.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://snn.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nxr.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://our.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://udg.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gtk.sufxvd.cn

[P04] 求长度
来源：http://gpw.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jtl.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jiq.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pov.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wnb.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://xxk.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://fup.fengsongda.top

Ruby: x.length;  x.size
来源：http://cba.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://sup.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://snf.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ibq.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dbh.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oxx.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tkw.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xep.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://rct.feifeiyinyue.top

Ruby: a == b
来源：http://mqo.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://utf.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oei.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ptu.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://ohs.guannengcc.top


<!-- 参考信息 -->