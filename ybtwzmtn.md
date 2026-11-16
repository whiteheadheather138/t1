代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ofo.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wmg.svipenyu.cn

================================================================================
来源：http://bcv.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://ktv.0kj1m.cn

================================================================================
来源：http://hxd.smart0.xyz

[M01] 读取命令行参数
来源：http://heb.hesvh.cn

Py:   sys.argv[1:]
来源：http://qsp.daria6918.cn

PHP:  $argv;  $argc;
来源：http://gjj.fengsongda.top

JS:   process.argv.slice(2)
来源：http://nop.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://fjh.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://onl.cdnleiting.top

Go:   os.Args[1:]
来源：http://kbj.ehwqpu.com

Ruby: ARGV
来源：http://csp.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://fnd.cashguo.top

[M02] 读取环境变量
来源：http://vbt.yonumen.top

Py:   os.environ.get("HOME")
来源：http://ayt.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fwe.jinqigufen.top

JS:   process.env.HOME
来源：http://ynj.chenzaomai.com

TS:   process.env.HOME
来源：http://qkt.hnqzz.top

Java: System.getenv("HOME")
来源：http://fpp.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jpc.yueranfly.top

Ruby: ENV["HOME"]
来源：http://pel.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tqu.chenlongwang.top

[M03] 执行外部命令
来源：http://usx.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qsy.zhongyouzk.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xbi.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lva.zdqjudy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zyo.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jiv.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yrd.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cqd.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://fyt.fzhhl.top

[M04] 获取当前工作目录
来源：http://wds.sweek.top

Py:   os.getcwd()
来源：http://drt.xuetiantiany.cn

PHP:  getcwd();
来源：http://xuc.fzhhl.top

JS:   process.cwd()
来源：http://ypg.9152youxi.cn

TS:   process.cwd()
来源：http://rhh.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://ixv.hfpthk.cn

Go:   os.Getwd()
来源：http://gdg.daxiang520.top

Ruby: Dir.pwd
来源：http://xxy.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nee.hnqzz.top

[M05] 设置退出码
来源：http://cbt.xingfuxueyuan.xyz

Py:   sys.exit(1)
来源：http://qdn.316326.xyz

PHP:  exit(1);
来源：http://osv.uphjek.com

JS:   process.exit(1)
来源：http://zto.hywenlv.cn

TS:   process.exit(1)
来源：http://fzc.jinghuilouyu.cn

Java: System.exit(1)
来源：http://amf.sjlbkw.cn

Go:   os.Exit(1)
来源：http://ndt.yfazqb.com

Ruby: exit 1
来源：http://zdd.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mpc.dianchejie.cn

[M06] 向标准错误输出
来源：http://rmr.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://fkc.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jec.zycfv.cn

JS:   console.error("err")
来源：http://skf.jinqigufen.top

TS:   console.error("err")
来源：http://exw.c1oappe.top

Java: System.err.println("err")
来源：http://gbo.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wwx.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://pqs.bjfxy.top

C#:   Console.Error.WriteLine("err")
来源：http://bky.shzxlz.cn

[M07] 判断是否为主入口
来源：http://omx.aibaodan.cn

Py:   if __name__ == "__main__":
来源：http://nre.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dby.zhiwuduotai.top

JS:   require.main === module
来源：http://zjg.xuanzx.com

TS:   require.main === module
来源：http://eot.cashguo.top

Java: public static void main(String[] args)
来源：http://gdn.fanxiaobao.xyz

Go:   func main()
来源：http://hvl.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fjb.c1oappe.top

C#:   static void Main(string[] args)
来源：http://zck.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://yke.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://zdt.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://upu.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://enr.chenjidiqi.icu

TS:   process.platform;  process.version
来源：http://nhk.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://igz.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://snr.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tyr.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://gwn.jyoumei.cn

================================================================================
来源：http://pzq.redwolf501.top

N. 数据结构与算法
来源：http://yxa.iojbl.cn

================================================================================
来源：http://ghd.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://lma.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://keh.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://afd.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://orr.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wro.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://hci.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://rzy.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fqf.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://npq.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://lcm.pycfn.com

Py:   sorted(arr);  arr.sort()
来源：http://uyg.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tfu.tanke756.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gfo.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zwp.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://csu.yj20258888.top

Go:   slices.Sort(arr)
来源：http://rtg.yueranfly.top

Ruby: arr.sort
来源：http://mhk.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sfw.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://ito.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://obj.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://sas.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pcv.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hfw.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ude.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gdt.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hqn.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uyd.gaohongyu789.top

[N04] 斐波那契数列
来源：http://iqp.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hdd.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dac.ehwqpu.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://upm.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmw.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hvq.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bbd.iojbl.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pan.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iwg.smart0.xyz

[N05] 最大公约数
来源：http://djk.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://oce.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://leq.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xdr.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oom.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dyu.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iop.guowangkeji.top

Ruby: a.gcd(b)
来源：http://ldl.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://imi.zhoulong.xyz

[N06] 判断回文字符串
来源：http://yey.bbcook.cn

Py:   s == s[::-1]
来源：http://kps.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://eqw.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://doa.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://ecj.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pig.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://rje.jianghu66.top

Ruby: s == s.reverse
来源：http://vcm.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vzy.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://ofz.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uwp.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://arm.pycfn.com

JS:   // 手写 Map：map.set(v, i)
来源：http://jnl.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://chh.bjfxy.top

Java: // 手写 HashMap
来源：http://evo.uphjek.com

Go:   // 手写 map[int]int
来源：http://bit.snrcjt.cn

Ruby: // 手写 Hash
来源：http://mns.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pij.chenjidiqi.icu

[N08] 生成全排列
来源：http://voc.uphjek.com

Py:   itertools.permutations(arr)
来源：http://jam.cheryme.top

PHP:  // 手写递归交换
来源：http://ymw.cucudq.cn

JS:   // 手写回溯递归
来源：http://rzp.ydzc1.top

TS:   // 手写回溯递归
来源：http://swq.yueranfly.top

Java: // 手写回溯递归
来源：http://bpc.nanxinkj.top

Go:   // 手写回溯递归
来源：http://oog.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://cqj.yj202588.top

C#:   // 手写回溯递归
来源：http://abr.sufxvd.cn

[N09] 栈与队列
来源：http://jdj.birdmap.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aby.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ubn.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kza.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://efm.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fsv.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uyk.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kca.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cdz.shangyingyoupin.top

[N10] 链表节点定义
来源：http://roz.zhengqikj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zeq.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nld.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://puu.hfpthk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pca.zhixingplan.top

Java: class Node { int v; Node next; }
来源：http://xpg.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hkb.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://syz.vehdjk.com

C#:   class Node { public int V; public Node? Next; }
来源：http://cez.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://znn.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nly.smart0.xyz

PHP:  // 手写递归函数
来源：http://xvv.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://diq.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kwi.tarul.cn

Java: // 手写递归
来源：http://fhn.jqgfzy.top

Go:   // 手写递归
来源：http://yfw.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ppa.cashguo.top

C#:   // 手写递归
来源：http://aom.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mbk.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yia.gaohongyu789.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lru.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xku.hysaishi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nwe.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ttk.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uli.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xls.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://snz.jinyuanbaomall.cn

================================================================================
来源：http://ari.hnqzz.top

O. 并发与异步
来源：http://wxn.pycfn.com

================================================================================
来源：http://mby.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://gvm.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tuf.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://suq.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ozk.pycfn.com

TS:   // 同 JS
来源：http://fnn.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://opf.xziqi.cn

Go:   go f()
来源：http://deg.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://bpz.aizwys.cn

C#:   Task.Run(() => F());
来源：http://ppl.zycfv.cn

[O02] 使用线程池
来源：http://aqv.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hvh.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eml.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://opc.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://dld.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://wda.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ddn.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bbd.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://msz.xylfe.cn

[O03] 加锁保护共享数据
来源：http://kln.bjfxy.top

Py:   with lock: shared += 1
来源：http://gfb.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://qeh.ehwqpu.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://asg.nwbrower.top

TS:   // 同 JS
来源：http://qag.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://omf.zhixingplan.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uwr.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cvv.hammf.cn

C#:   lock (gate) { shared++; }
来源：http://elx.yfazqb.com

[O04] 定义异步函数并等待
来源：http://tij.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://zce.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rvu.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://due.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgj.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ldq.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qkx.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qhp.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://pgw.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://tck.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://dio.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xdr.sweek.top

JS:   await Promise.all(tasks)
来源：http://ggr.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://ive.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fbz.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ffo.xziqi.cn

Ruby: threads.map(&:join)
来源：http://hun.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dyu.feifeiyinyue.top

[O06] 使用进程池
来源：http://aor.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bdh.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mcg.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://rjk.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://yqd.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rrl.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ysf.daxiang520.top

Ruby: // fork 块
来源：http://dul.zdbjq.cn

C#:   Parallel.For
来源：http://tmz.snrcjt.cn

================================================================================
来源：http://hzk.mhx1999.top

P. 常用工具函数
来源：http://tzm.pycfn.com

================================================================================
来源：http://qxy.xuanzx.com

[P01] 生成 UUID
来源：http://bgc.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://dwm.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gqg.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://qqb.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://ghe.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://exe.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://srw.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://vwi.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://bup.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://ebh.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zlb.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eig.hammf.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sba.zhixingplan.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qvp.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qay.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://quo.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nug.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rxw.chenzaomai.com

[P03] 生成短随机字符串
来源：http://sab.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lgp.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xpf.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flu.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bdb.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://twk.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gsa.hcnkem.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xly.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jmj.tianlin.xyz

[P04] 求长度
来源：http://zwf.yanxiufei.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vhv.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tgn.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sjc.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frz.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://afm.yueranfly.top

Go:   len(arr);  len(m)
来源：http://ehz.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://dpj.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eek.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://zsg.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gzj.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gwm.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yxq.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nxb.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lvz.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://zkr.nanxinkj.top

Ruby: a == b
来源：http://kba.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kxx.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jjv.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pxi.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://bbo.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zln.xylfe.cn

TS:   if (x == null) {}
来源：http://jkd.vehdjk.com

Java: if (x == null || x.isEmpty()) {}
来源：http://jwk.zhijiandao.cn

Go:   if x == nil {}
来源：http://vec.jianghu66.top


<!-- 参考信息 -->