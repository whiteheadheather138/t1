代发 wailian999

================================================================================
来源：http://vuw.snrcjt.cn

[M01] 读取命令行参数
来源：http://jop.fengsongda.top

Py:   sys.argv[1:]
来源：http://vzi.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://jqi.tarul.cn

JS:   process.argv.slice(2)
来源：http://aum.havefunace.top

TS:   process.argv.slice(2)
来源：http://wxf.jinyuanbaomall.cn

Java: args 数组（main 方法参数）
来源：http://xsq.snrcjt.cn

Go:   os.Args[1:]
来源：http://tos.xuanzx.com

Ruby: ARGV
来源：http://ydv.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://pfc.vqdsnc.cn

[M02] 读取环境变量
来源：http://cai.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://qva.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qgg.shangyingyoupin.top

JS:   process.env.HOME
来源：http://wzk.shanyushiyangkeji.top

TS:   process.env.HOME
来源：http://oxh.svipenyu.cn

Java: System.getenv("HOME")
来源：http://ued.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://skc.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://mql.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kds.ehwqpu.com

[M03] 执行外部命令
来源：http://ofg.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ivn.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qzy.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://xnv.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://koh.yj202588.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://imz.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://neg.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hal.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://tpo.hcnkem.com

[M04] 获取当前工作目录
来源：http://qsi.bbcook.cn

Py:   os.getcwd()
来源：http://qgn.sufxvd.cn

PHP:  getcwd();
来源：http://wfv.ctjpmb.com

JS:   process.cwd()
来源：http://kxm.ctjpmb.com

TS:   process.cwd()
来源：http://ahw.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://zqd.9152youxi.cn

Go:   os.Getwd()
来源：http://ktp.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://msl.jianghu66.top

C#:   Directory.GetCurrentDirectory()
来源：http://mxc.sufxvd.cn

[M05] 设置退出码
来源：http://wsv.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://uqt.xuetiantiany.cn

PHP:  exit(1);
来源：http://mqt.dianchejie.cn

JS:   process.exit(1)
来源：http://vuv.yvedp.cn

TS:   process.exit(1)
来源：http://ilq.xuetiantiany.cn

Java: System.exit(1)
来源：http://hej.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://ime.andypj.xyz

Ruby: exit 1
来源：http://dqi.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mfn.dianchejie.cn

[M06] 向标准错误输出
来源：http://ekc.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://unf.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sda.hnxiangtu.top

JS:   console.error("err")
来源：http://vyy.cashguo.top

TS:   console.error("err")
来源：http://mev.fengsongda.top

Java: System.err.println("err")
来源：http://aqi.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cqg.tianlin.xyz

Ruby: warn "err"
来源：http://myg.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://pzq.snrcjt.cn

[M07] 判断是否为主入口
来源：http://rlx.uphjek.com

Py:   if __name__ == "__main__":
来源：http://mkj.ywan-chungtsiang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wpt.chenjidiqi.icu

JS:   require.main === module
来源：http://wrp.chenzaomai.com

TS:   require.main === module
来源：http://ldc.jqgfzy.top

Java: public static void main(String[] args)
来源：http://fhi.meibo888.top

Go:   func main()
来源：http://snt.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://smk.vehdjk.com

C#:   static void Main(string[] args)
来源：http://sph.yonumen.top

[M08] 获取系统与运行时信息
来源：http://wlw.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://fyn.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://mbt.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://fpy.hammf.cn

TS:   process.platform;  process.version
来源：http://ebw.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bqk.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tdl.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lat.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hnp.cashguo.top

================================================================================
来源：http://ljh.nwbrower.top

N. 数据结构与算法
来源：http://pza.iojbl.cn

================================================================================
来源：http://vic.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://uzi.gotoacloud.top

Py:   bisect.bisect_left(arr, x)
来源：http://mkk.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kcy.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xay.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vhi.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://orh.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://got.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://nfk.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://aih.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://abh.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://nhx.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eui.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://epc.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jxe.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://coj.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://iey.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://gcp.birdmap.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://blg.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://nua.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jfi.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://xkh.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pus.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pkn.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://etz.andypj.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cum.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nks.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://mna.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://sfq.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jqy.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ini.zycfv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhp.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ann.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hkw.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rag.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lpj.haohaochexian.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pqm.sysykeji.top

[N05] 最大公约数
来源：http://jmd.fzhhl.top

Py:   math.gcd(a, b)
来源：http://okv.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ene.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pny.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hhc.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dif.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dsn.hfpthk.cn

Ruby: a.gcd(b)
来源：http://rka.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qpx.hcnkem.com

[N06] 判断回文字符串
来源：http://mxs.zhixingplan.top

Py:   s == s[::-1]
来源：http://xoo.epnwcf.com

PHP:  $s === strrev($s);
来源：http://mzs.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://gxq.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://ing.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hbc.nwbrower.top

Go:   // 双指针从两端比较
来源：http://slu.yongpay.top

Ruby: s == s.reverse
来源：http://tad.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vir.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://eat.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fuq.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://doe.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bbx.zhixingplan.top

TS:   // 手写 Map<string, number>
来源：http://pzy.redwolf501.top

Java: // 手写 HashMap
来源：http://jdp.yj202588.top

Go:   // 手写 map[int]int
来源：http://rdd.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://dxb.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://dem.gzhubu.top

[N08] 生成全排列
来源：http://uuv.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://iru.haohaochexian.top

PHP:  // 手写递归交换
来源：http://teq.316326.xyz

JS:   // 手写回溯递归
来源：http://spn.daria6918.cn

TS:   // 手写回溯递归
来源：http://aue.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://qfh.yuxming.cn

Go:   // 手写回溯递归
来源：http://mrw.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://hdt.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://amz.cdnleiting.top

[N09] 栈与队列
来源：http://ypf.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zqo.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ftw.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ugw.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yyn.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jcr.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hqr.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zvy.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rvu.haohaochexian.top

[N10] 链表节点定义
来源：http://zur.haohaochexian.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ebb.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ped.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kks.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lkr.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://blo.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://akf.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tck.yuxming.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rhc.ydzc1.top

[N11] 二叉树中序遍历
来源：http://gdn.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gab.fengsongda.top

PHP:  // 手写递归函数
来源：http://mhj.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rkx.yvedp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iky.xziqi.cn

Java: // 手写递归
来源：http://dxv.guowangkeji.top

Go:   // 手写递归
来源：http://ppw.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gnm.ydzc1.top

C#:   // 手写递归
来源：http://fae.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bzt.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oaa.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ikr.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://efx.fengsongda.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yqs.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uiu.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ylw.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tvg.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kwh.dashuyun.cn

================================================================================
来源：http://rcc.chenzaomai.com

O. 并发与异步
来源：http://gzj.sufxvd.cn

================================================================================
来源：http://uva.jqgfzy.top

[O01] 启动一个线程
来源：http://jnv.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://adf.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bpl.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qms.ehwqpu.com

TS:   // 同 JS
来源：http://zim.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://dvd.xuanzx.com

Go:   go f()
来源：http://omt.sysykeji.top

Ruby: Thread.new { f }
来源：http://jgx.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://gsz.hywenlv.cn

[O02] 使用线程池
来源：http://els.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fnf.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://inh.xinyue.icu

JS:   // worker_threads 线程池
来源：http://fhe.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://ceg.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rri.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wpz.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kdu.sjlbkw.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gsz.yuxming.cn

[O03] 加锁保护共享数据
来源：http://nxu.fzhhl.top

Py:   with lock: shared += 1
来源：http://wnk.haohaochexian.top

PHP:  // 用 flock() 做文件锁
来源：http://ngm.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ula.epnwcf.com

TS:   // 同 JS
来源：http://why.xingfuxueyuan.xyz

Java: synchronized (this) { shared++; }
来源：http://bwv.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xes.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aax.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://ijt.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://aii.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://ufk.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nhc.cheryme.top

JS:   async function f() { await g(); }
来源：http://mvo.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fzo.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mzk.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://acu.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ptr.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://owi.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://ejn.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://gtb.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kpl.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://tih.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://odr.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vtd.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lao.daria6918.cn

Ruby: threads.map(&:join)
来源：http://uto.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xcf.jinqigufen.top

[O06] 使用进程池
来源：http://byn.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xfx.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bse.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://ijp.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://unz.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mgs.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ild.zhongyouzk.top

Ruby: // fork 块
来源：http://kfg.jqgfzy.top

C#:   Parallel.For
来源：http://ays.zdqjudy.top

================================================================================
来源：http://fac.pengpengdd.cyou

P. 常用工具函数
来源：http://fuv.hywenlv.cn

================================================================================
来源：http://azi.birdmap.top

[P01] 生成 UUID
来源：http://kuy.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://lrm.aibaodan.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xcn.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://gpc.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://ady.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://wee.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://kwn.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://sqd.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://xog.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://yxl.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pdl.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yvx.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kds.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vyt.0kj1m.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ppy.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dvt.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ydo.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asz.fengsongda.top

[P03] 生成短随机字符串
来源：http://dss.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xmp.cheryme.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jmg.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ckp.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grl.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zdy.c1oappe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tar.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://fhy.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zdr.cashguo.top

[P04] 求长度
来源：http://cbg.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kck.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tid.gzhubu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryt.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezt.gotoacloud.top

Java: list.size();  map.size();  s.length()
来源：http://web.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://bbv.tianlin.xyz

Ruby: x.length;  x.size
来源：http://pmx.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://vho.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://ptw.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://aqk.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sjj.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fak.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hxz.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zcz.shzxlz.cn

Go:   reflect.DeepEqual(a, b)
来源：http://oaz.fengsongda.top

Ruby: a == b
来源：http://rll.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://axh.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://car.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rts.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://cqo.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yhk.hcnkem.com

TS:   if (x == null) {}
来源：http://zbu.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fis.0kj1m.cn

Go:   if x == nil {}
来源：http://bmh.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bob.9152youxi.cn

C#:   if (x is null) {}
来源：http://ils.snrcjt.cn

[P07] 防抖与节流
来源：http://nzo.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://khl.cdnleiting.top


<!-- 参考信息 -->