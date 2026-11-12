代发 wailian999

================================================================================
来源：http://elk.birdmap.top

[M01] 读取命令行参数
来源：http://ymw.yvedp.cn

Py:   sys.argv[1:]
来源：http://age.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://fwm.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://lhv.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://uma.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://msa.haohaochexian.top

Go:   os.Args[1:]
来源：http://ple.nwbrower.top

Ruby: ARGV
来源：http://qal.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://tni.sweek.top

[M02] 读取环境变量
来源：http://aqe.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://tjl.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gkq.sjlbkw.cn

JS:   process.env.HOME
来源：http://uww.jinqigufen.top

TS:   process.env.HOME
来源：http://iot.hesvh.cn

Java: System.getenv("HOME")
来源：http://nkk.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hce.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://hgf.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vyz.aibaodan.cn

[M03] 执行外部命令
来源：http://yuc.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wgg.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yxu.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://scw.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://erx.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iko.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gtd.zdbjq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gyl.9152youxi.cn

C#:   Process.Start("ls", "-l");
来源：http://bns.hfpthk.cn

[M04] 获取当前工作目录
来源：http://pkj.birdmap.top

Py:   os.getcwd()
来源：http://fkl.hesvh.cn

PHP:  getcwd();
来源：http://pyu.vqdsnc.cn

JS:   process.cwd()
来源：http://zxg.yonumen.top

TS:   process.cwd()
来源：http://tdc.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://swm.quarkkingdee.top

Go:   os.Getwd()
来源：http://kix.guowangkeji.top

Ruby: Dir.pwd
来源：http://gqs.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://xab.chenlongwang.top

[M05] 设置退出码
来源：http://scv.snrcjt.cn

Py:   sys.exit(1)
来源：http://rjp.yj202588.top

PHP:  exit(1);
来源：http://lbp.jlsjyb.cn

JS:   process.exit(1)
来源：http://lhm.jqgfzy.top

TS:   process.exit(1)
来源：http://avn.svipenyu.cn

Java: System.exit(1)
来源：http://jmx.xylfe.cn

Go:   os.Exit(1)
来源：http://ipj.jinyuanbaomall.cn

Ruby: exit 1
来源：http://qsh.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://quq.chenlongwang.top

[M06] 向标准错误输出
来源：http://jxp.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://eak.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ffw.shzxlz.cn

JS:   console.error("err")
来源：http://uoj.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://itr.tianlin.xyz

Java: System.err.println("err")
来源：http://cyp.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kqw.yj20258888.top

Ruby: warn "err"
来源：http://mos.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kqc.meibo888.top

[M07] 判断是否为主入口
来源：http://avk.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://mil.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ali.vqdsnc.cn

JS:   require.main === module
来源：http://aot.cqqwz.cn

TS:   require.main === module
来源：http://kyk.zycfv.cn

Java: public static void main(String[] args)
来源：http://kls.hysaishi.cn

Go:   func main()
来源：http://elc.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bui.uphjek.com

C#:   static void Main(string[] args)
来源：http://ahg.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://iox.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://kvz.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://aen.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://mch.vehdjk.com

TS:   process.platform;  process.version
来源：http://lis.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qje.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ynk.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bni.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eea.9152youxi.cn

================================================================================
来源：http://gai.yonumen.top

N. 数据结构与算法
来源：http://ira.yj202588.top

================================================================================
来源：http://mig.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://blp.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ekw.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xfy.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpa.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gdf.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://pvd.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://hon.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jtc.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://rbl.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://inv.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://dao.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kvv.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fol.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ksv.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ewq.hcnkem.com

Go:   slices.Sort(arr)
来源：http://efu.mhx1999.top

Ruby: arr.sort
来源：http://xno.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qts.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://sng.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ptg.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://xwr.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oug.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcc.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hbm.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mjp.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mth.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bdw.yueranfly.top

[N04] 斐波那契数列
来源：http://yxn.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://irx.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://erh.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mci.shangyingyoupin.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbe.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uri.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://avv.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rst.yj20258.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://juh.tianlin.xyz

[N05] 最大公约数
来源：http://evj.hesvh.cn

Py:   math.gcd(a, b)
来源：http://fgg.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gyt.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://puz.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fjp.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bjd.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kib.jqgfzy.top

Ruby: a.gcd(b)
来源：http://fas.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nsi.bbcook.cn

[N06] 判断回文字符串
来源：http://tyx.uphjek.com

Py:   s == s[::-1]
来源：http://ioo.shuidangran.top

PHP:  $s === strrev($s);
来源：http://etk.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://fhj.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://vws.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tjr.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://uqy.kuanghao11.cn

Ruby: s == s.reverse
来源：http://rqm.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://cqt.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://hwh.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zcx.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zip.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nkb.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://qjt.svipenyu.cn

Java: // 手写 HashMap
来源：http://xnj.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://vdj.ctjpmb.com

Ruby: // 手写 Hash
来源：http://sjm.gzhubu.top

C#:   // 手写 Dictionary<int, int>
来源：http://hkx.jiagoushi.top

[N08] 生成全排列
来源：http://qze.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://uun.vehdjk.com

PHP:  // 手写递归交换
来源：http://vmv.fehbvm.com

JS:   // 手写回溯递归
来源：http://ipf.yanxiufei.cn

TS:   // 手写回溯递归
来源：http://snd.epnwcf.com

Java: // 手写回溯递归
来源：http://nqc.sysykeji.top

Go:   // 手写回溯递归
来源：http://flf.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://tbu.hammf.cn

C#:   // 手写回溯递归
来源：http://kyj.shanyushiyangtech.top

[N09] 栈与队列
来源：http://utl.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://def.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ylv.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tfj.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gko.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ert.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://syu.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blq.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ncb.316326.xyz

[N10] 链表节点定义
来源：http://xwp.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jnv.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lda.zycfv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oeu.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxo.sysykeji.top

Java: class Node { int v; Node next; }
来源：http://oze.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xpp.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://yya.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://uqm.fehbvm.com

[N11] 二叉树中序遍历
来源：http://ogt.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tvw.jinqigufen.top

PHP:  // 手写递归函数
来源：http://cge.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ahd.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lwh.zhongyouzk.top

Java: // 手写递归
来源：http://zuz.hywenlv.cn

Go:   // 手写递归
来源：http://pcb.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xdx.uphjek.com

C#:   // 手写递归
来源：http://lps.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eal.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nps.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgd.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qwq.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zaa.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ijd.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kmm.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mhr.jyoumei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eor.vehdjk.com

================================================================================
来源：http://svp.zhixingplan.top

O. 并发与异步
来源：http://biy.bbcook.cn

================================================================================
来源：http://uhn.vehdjk.com

[O01] 启动一个线程
来源：http://lpv.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xrs.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pdq.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nob.fanxiaobao.xyz

TS:   // 同 JS
来源：http://lat.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://kyh.sxryk.cn

Go:   go f()
来源：http://ivq.guannengcc.top

Ruby: Thread.new { f }
来源：http://kxv.xylfe.cn

C#:   Task.Run(() => F());
来源：http://fgy.tarul.cn

[O02] 使用线程池
来源：http://wua.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vdu.fktsv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dpq.epnwcf.com

JS:   // worker_threads 线程池
来源：http://oib.ybcxt.top

TS:   // worker_threads 线程池
来源：http://jie.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://qks.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wgt.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cyz.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hed.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://axc.hnqzz.top

Py:   with lock: shared += 1
来源：http://jpb.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://bwn.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yml.xuanzx.com

TS:   // 同 JS
来源：http://hmj.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://yht.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bnz.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mmo.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://isd.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://oby.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://ecc.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kyq.hysaishi.cn

JS:   async function f() { await g(); }
来源：http://mah.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gvs.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qvl.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nkf.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://raa.yj202588.top

C#:   async Task F() { await G(); }
来源：http://aeq.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://obs.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://dmp.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://svb.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://yej.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://ucz.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pin.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eft.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://jwa.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://iti.chenzaomai.com

[O06] 使用进程池
来源：http://zyj.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kju.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cxe.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://lhh.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://ijf.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zhz.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tfc.fzhhl.top

Ruby: // fork 块
来源：http://svm.tian-w.cn

C#:   Parallel.For
来源：http://aht.snrcjt.cn

================================================================================
来源：http://lcj.hnqzz.top

P. 常用工具函数
来源：http://cxo.ydzc1.top

================================================================================
来源：http://ren.redwolf501.top

[P01] 生成 UUID
来源：http://smw.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://xkl.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ecv.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://rmq.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://ixn.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://exl.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://tml.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://fsf.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://cfe.svipenyu.cn

[P02] MD5 / SHA256 摘要
来源：http://itz.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vdm.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vkf.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bhc.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://coa.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kfu.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://urt.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://luw.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tfb.hesvh.cn

[P03] 生成短随机字符串
来源：http://bax.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cfy.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rpr.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pvd.fanxiaobao.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://got.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uik.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eyc.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://aga.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wiz.zdbjq.cn

[P04] 求长度
来源：http://tqp.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://imk.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfw.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fcb.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fju.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://fcy.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://dos.jiagoushi.top

Ruby: x.length;  x.size
来源：http://nhd.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aef.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://faf.xingfuxueyuan.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qyh.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zvb.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pmm.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jel.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pse.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://kwa.hysaishi.cn

Ruby: a == b
来源：http://zbm.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://svg.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nrp.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cyt.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://yyz.xuanzx.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cuh.yj20258.top

TS:   if (x == null) {}
来源：http://ods.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://knj.wangdashe.top

Go:   if x == nil {}
来源：http://swd.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aid.dianchejie.cn

C#:   if (x is null) {}
来源：http://zcm.guowangkeji.top

[P07] 防抖与节流
来源：http://uhd.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://woz.cucudq.cn


<!-- 参考信息 -->