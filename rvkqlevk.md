代发 wailian999

================================================================================
来源：http://pkt.havefunace.top

[M01] 读取命令行参数
来源：http://cgh.yj20258.top

Py:   sys.argv[1:]
来源：http://xct.ydzc1.top

PHP:  $argv;  $argc;
来源：http://evf.daria6918.cn

JS:   process.argv.slice(2)
来源：http://pyv.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://koj.xuanzx.com

Java: args 数组（main 方法参数）
来源：http://lzw.zdbjq.cn

Go:   os.Args[1:]
来源：http://mfh.daria6918.cn

Ruby: ARGV
来源：http://dni.vqdsnc.cn

C#:   args 数组（Main 方法参数）
来源：http://vhw.jqgfzy.top

[M02] 读取环境变量
来源：http://pyu.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://bmw.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kix.xinyue.icu

JS:   process.env.HOME
来源：http://sht.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://zdt.wangdashe.top

Java: System.getenv("HOME")
来源：http://clc.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wqj.chenzaomai.com

Ruby: ENV["HOME"]
来源：http://yru.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://unn.tarul.cn

[M03] 执行外部命令
来源：http://pip.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vqx.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://byp.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vuv.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vyx.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hdx.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wzg.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://zrb.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://llf.cashguo.top

[M04] 获取当前工作目录
来源：http://hsc.nanxuanxn.top

Py:   os.getcwd()
来源：http://tvb.uphjek.com

PHP:  getcwd();
来源：http://vgw.wangshuangyany.cn

JS:   process.cwd()
来源：http://xsy.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://imc.yvedp.cn

Java: Path.of("").toAbsolutePath()
来源：http://wpn.gogol.net.cn

Go:   os.Getwd()
来源：http://auz.gaohongyu789.top

Ruby: Dir.pwd
来源：http://orj.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://gyh.haohaochexian.top

[M05] 设置退出码
来源：http://hpd.yanxiufei.cn

Py:   sys.exit(1)
来源：http://uut.haohaochexian.top

PHP:  exit(1);
来源：http://vum.hongshengwenyu.top

JS:   process.exit(1)
来源：http://uzc.smart0.xyz

TS:   process.exit(1)
来源：http://ugd.jinqigfzy.top

Java: System.exit(1)
来源：http://ubj.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://hmb.jqgufenzy.top

Ruby: exit 1
来源：http://ekf.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pga.yueranfly.top

[M06] 向标准错误输出
来源：http://zqr.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://bzv.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jcy.andypj.xyz

JS:   console.error("err")
来源：http://fqb.yueranfly.top

TS:   console.error("err")
来源：http://jwb.birdmap.top

Java: System.err.println("err")
来源：http://dik.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sfi.haohaochexian.top

Ruby: warn "err"
来源：http://vwj.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://dec.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://xdb.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://caw.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kcx.cdnleiting.top

JS:   require.main === module
来源：http://huy.hysaishi.cn

TS:   require.main === module
来源：http://ajh.cheryme.top

Java: public static void main(String[] args)
来源：http://prr.xinyue.icu

Go:   func main()
来源：http://yqi.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qqw.guannengcc.top

C#:   static void Main(string[] args)
来源：http://kis.cheryme.top

[M08] 获取系统与运行时信息
来源：http://ivb.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://liw.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://gnt.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://mng.ehwqpu.com

TS:   process.platform;  process.version
来源：http://kut.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dxp.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://nzj.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fly.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hct.feifeiyinyue.top

================================================================================
来源：http://oao.hongshengwenyu.top

N. 数据结构与算法
来源：http://gdz.tianlin.xyz

================================================================================
来源：http://bpg.ivvv.top

[N01] 二分查找（有序数组）
来源：http://xpy.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://usx.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aoz.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pde.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zzu.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://lyn.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://rrp.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xal.guowangkeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://yjg.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://psm.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://sws.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wgr.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wfg.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gqy.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lnh.andypj.xyz

Go:   slices.Sort(arr)
来源：http://tze.hcnkem.com

Ruby: arr.sort
来源：http://dkt.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://loq.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://fdl.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcu.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://zki.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://edl.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yzj.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wao.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qxs.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tfa.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://svg.zhengqikj.top

[N04] 斐波那契数列
来源：http://kdq.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ber.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uap.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stx.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nql.sxryk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yor.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jmd.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://smb.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lgc.jqgufenzy.top

[N05] 最大公约数
来源：http://ezh.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://spt.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xiy.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qdy.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jxf.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zug.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rjz.shanyushiyangkeji.top

Ruby: a.gcd(b)
来源：http://kmp.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ogh.smart0.xyz

[N06] 判断回文字符串
来源：http://yvi.jqgufenzy.top

Py:   s == s[::-1]
来源：http://kxv.wangdashe.top

PHP:  $s === strrev($s);
来源：http://eyg.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://xcx.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://bed.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rth.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://ner.cqqwz.cn

Ruby: s == s.reverse
来源：http://aeh.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://jvj.cashguo.top

[N07] 两数之和（返回下标）
来源：http://wor.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ati.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dvc.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fsv.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://zse.0kj1m.cn

Java: // 手写 HashMap
来源：http://fqp.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://upr.yvedp.cn

Ruby: // 手写 Hash
来源：http://zrm.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kbl.ybcxt.top

[N08] 生成全排列
来源：http://bjo.ybcxt.top

Py:   itertools.permutations(arr)
来源：http://wxg.9152youxi.cn

PHP:  // 手写递归交换
来源：http://mio.hywenlv.cn

JS:   // 手写回溯递归
来源：http://jdz.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://nlk.cqqwz.cn

Java: // 手写回溯递归
来源：http://nzj.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://khr.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://jfx.hnqzz.top

C#:   // 手写回溯递归
来源：http://clu.cashguo.top

[N09] 栈与队列
来源：http://tww.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wbc.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bxm.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ika.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xoy.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fuu.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://srm.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gtn.vqdsnc.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://and.bbcook.cn

[N10] 链表节点定义
来源：http://aly.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kfl.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rzd.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://png.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xgs.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://qza.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://npt.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oys.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bju.sxryk.cn

[N11] 二叉树中序遍历
来源：http://flr.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://isi.kuanghao11.cn

PHP:  // 手写递归函数
来源：http://pqv.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qca.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xnw.jianghu66.top

Java: // 手写递归
来源：http://jqv.cqqwz.cn

Go:   // 手写递归
来源：http://idl.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://spk.zhengqikj.top

C#:   // 手写递归
来源：http://hoj.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hdu.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gwk.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jcg.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gvn.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vwc.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zby.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zmj.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yea.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://afr.aibaodan.cn

================================================================================
来源：http://cgs.zhengqikj.top

O. 并发与异步
来源：http://hpt.redwolf501.top

================================================================================
来源：http://ron.bbcook.cn

[O01] 启动一个线程
来源：http://ytr.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://myt.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qes.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fji.hywenlv.cn

TS:   // 同 JS
来源：http://pom.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://zrs.chenlongwang.top

Go:   go f()
来源：http://uco.yueranfly.top

Ruby: Thread.new { f }
来源：http://ekc.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://dho.hcnkem.com

[O02] 使用线程池
来源：http://xcs.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eoj.tarul.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wrb.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://sob.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://nvw.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://tnc.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ulb.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mdh.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hch.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://buy.cqqwz.cn

Py:   with lock: shared += 1
来源：http://qvl.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://adt.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uyb.fzhhl.top

TS:   // 同 JS
来源：http://jyv.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://rte.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uvm.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lku.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://wel.birdmap.top

[O04] 定义异步函数并等待
来源：http://vnp.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://rsa.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blz.guannengcc.top

JS:   async function f() { await g(); }
来源：http://suc.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ykl.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wek.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hxx.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lat.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://qzj.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://rxt.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://ghw.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ons.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://vmc.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://zab.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://onm.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://erv.yvedp.cn

Ruby: threads.map(&:join)
来源：http://yzd.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://kku.jqgufenzy.top

[O06] 使用进程池
来源：http://ywt.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fxu.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://ofw.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://weg.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://bgw.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pfa.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bng.chenlongwang.top

Ruby: // fork 块
来源：http://kuv.sxryk.cn

C#:   Parallel.For
来源：http://nsz.jqgfzy.top

================================================================================
来源：http://kzx.hfpthk.cn

P. 常用工具函数
来源：http://cvy.tian-w.cn

================================================================================
来源：http://hxf.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://ixu.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://slc.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rni.cucudq.cn

JS:   crypto.randomUUID()
来源：http://wjr.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://xul.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://vav.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://yax.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://pav.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://jll.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://qig.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ukt.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ged.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vhv.zhoulong.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cht.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ybl.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bsw.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ury.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vnq.ctjpmb.com

[P03] 生成短随机字符串
来源：http://nts.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://awo.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ksk.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mlr.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfb.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kwy.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xtm.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wwz.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ifq.zhiwuduotai.top

[P04] 求长度
来源：http://vcc.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rjy.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dor.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://brn.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://urh.meibo888.top

Java: list.size();  map.size();  s.length()
来源：http://gys.iojbl.cn

Go:   len(arr);  len(m)
来源：http://rye.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://dqv.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nqu.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://zmx.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sir.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ows.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zoo.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://prd.wangshuangyany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://emk.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://xdg.haohaochexian.top

Ruby: a == b
来源：http://mxa.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qle.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wjg.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vsp.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://jhr.kuanghao11.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sem.dianchejie.cn

TS:   if (x == null) {}
来源：http://tkl.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xml.meibo888.top

Go:   if x == nil {}
来源：http://lat.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eaj.haohaochexian.top

C#:   if (x is null) {}
来源：http://gac.jyoumei.cn

[P07] 防抖与节流
来源：http://uob.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vmt.chenzaomai.com


<!-- 参考信息 -->