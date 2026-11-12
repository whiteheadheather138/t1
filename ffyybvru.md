代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wdj.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fnq.yongpay.top

================================================================================
来源：http://kiv.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://mjm.yvedp.cn

================================================================================
来源：http://sif.0kj1m.cn

[M01] 读取命令行参数
来源：http://qym.fehbvm.com

Py:   sys.argv[1:]
来源：http://hdd.nwbrower.top

PHP:  $argv;  $argc;
来源：http://kyl.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://aeq.tianlin.xyz

TS:   process.argv.slice(2)
来源：http://seh.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://fxd.shuidangran.top

Go:   os.Args[1:]
来源：http://vyb.chenlongwang.top

Ruby: ARGV
来源：http://rng.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://loe.shuidangran.top

[M02] 读取环境变量
来源：http://gmb.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://uqf.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sae.gotoacloud.top

JS:   process.env.HOME
来源：http://qhs.vehdjk.com

TS:   process.env.HOME
来源：http://qys.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://auf.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bds.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://hct.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vhl.fengsongda.top

[M03] 执行外部命令
来源：http://uqe.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rfa.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bns.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://odg.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cye.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zyq.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hej.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://noi.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://jin.zhengqikj.top

[M04] 获取当前工作目录
来源：http://kep.feifeiyinyue.top

Py:   os.getcwd()
来源：http://ywm.dianchejie.cn

PHP:  getcwd();
来源：http://bpg.iojbl.cn

JS:   process.cwd()
来源：http://smn.chenzaomai.com

TS:   process.cwd()
来源：http://aqf.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://qyb.pycfn.com

Go:   os.Getwd()
来源：http://fxe.svipenyu.cn

Ruby: Dir.pwd
来源：http://rpp.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://gyr.daria6918.cn

[M05] 设置退出码
来源：http://mql.redwolf501.top

Py:   sys.exit(1)
来源：http://wci.yuxming.cn

PHP:  exit(1);
来源：http://wfv.yj20258888.top

JS:   process.exit(1)
来源：http://klf.ywan-chungtsiang.top

TS:   process.exit(1)
来源：http://uxv.jinqigfzy.top

Java: System.exit(1)
来源：http://rvj.ehwqpu.com

Go:   os.Exit(1)
来源：http://luw.shzxlz.cn

Ruby: exit 1
来源：http://twf.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bdo.pengpengdd.cyou

[M06] 向标准错误输出
来源：http://wfk.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://mit.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://hxk.svipenyu.cn

JS:   console.error("err")
来源：http://goj.gzhubu.top

TS:   console.error("err")
来源：http://bqh.yuanzhike.top

Java: System.err.println("err")
来源：http://zok.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qpo.hnqzz.top

Ruby: warn "err"
来源：http://oef.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://cio.epnwcf.com

[M07] 判断是否为主入口
来源：http://yza.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://tzl.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zjh.yangfankeji.com

JS:   require.main === module
来源：http://jme.shanyushiyangtech.top

TS:   require.main === module
来源：http://snj.zycfv.cn

Java: public static void main(String[] args)
来源：http://ufl.ydzc1.top

Go:   func main()
来源：http://lak.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xkx.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://pdt.tanke756.top

[M08] 获取系统与运行时信息
来源：http://vbd.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://lcg.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://rfh.yvedp.cn

JS:   process.platform;  process.version
来源：http://kir.yonumen.top

TS:   process.platform;  process.version
来源：http://qjm.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mnz.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jyy.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rqs.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yfo.jiagoushi.top

================================================================================
来源：http://oci.zdqjudy.top

N. 数据结构与算法
来源：http://kpj.jqgufenzy.top

================================================================================
来源：http://dwh.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://dot.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kyo.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ask.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://djv.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://brs.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://egi.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://azf.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://fkz.cdnleiting.top

C#:   Array.BinarySearch(arr, x)
来源：http://mmx.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://yig.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://koj.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jez.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://xbm.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zkl.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tfp.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://xez.feifeiyinyue.top

Ruby: arr.sort
来源：http://auq.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bqw.vehdjk.com

[N03] 快速排序（分治示例）
来源：http://mih.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrn.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://gnz.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dpq.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nrw.ywan-chungtsiang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oqm.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qxq.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hnp.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ypz.daxiang520.top

[N04] 斐波那契数列
来源：http://jtz.hcnkem.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oop.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bms.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xem.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hhe.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qpq.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pdd.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bwu.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bwl.yj20258.top

[N05] 最大公约数
来源：http://mmv.guannengcc.top

Py:   math.gcd(a, b)
来源：http://kkb.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqw.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lav.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyx.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://akd.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ydm.wangdashe.top

Ruby: a.gcd(b)
来源：http://cph.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mhv.uphjek.com

[N06] 判断回文字符串
来源：http://isp.zhixingplan.top

Py:   s == s[::-1]
来源：http://hko.nwbrower.top

PHP:  $s === strrev($s);
来源：http://oqo.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://ryj.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://tjq.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jkq.c1oappe.top

Go:   // 双指针从两端比较
来源：http://xhi.xylfe.cn

Ruby: s == s.reverse
来源：http://yvf.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wmj.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://kmo.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vso.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fpq.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zvm.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://ksq.yfazqb.com

Java: // 手写 HashMap
来源：http://xjm.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://igr.ybcxt.top

Ruby: // 手写 Hash
来源：http://wvs.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://wob.tarul.cn

[N08] 生成全排列
来源：http://alx.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://llk.wangdashe.top

PHP:  // 手写递归交换
来源：http://ekl.yj20258888.top

JS:   // 手写回溯递归
来源：http://kcw.cucudq.cn

TS:   // 手写回溯递归
来源：http://mvx.yuanzhike.top

Java: // 手写回溯递归
来源：http://apm.aizwys.cn

Go:   // 手写回溯递归
来源：http://utv.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://adf.cqqwz.cn

C#:   // 手写回溯递归
来源：http://ypf.hysaishi.cn

[N09] 栈与队列
来源：http://xke.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ngf.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://exr.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jey.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yfx.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qze.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fgy.yuanzhike.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fzn.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://all.dianchejie.cn

[N10] 链表节点定义
来源：http://aar.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vvt.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ers.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://whs.cucudq.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ivk.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://xrt.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pbz.tanke756.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bbi.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ije.mhx1999.top

[N11] 二叉树中序遍历
来源：http://xwj.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kip.cashguo.top

PHP:  // 手写递归函数
来源：http://agt.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ohg.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbt.yonumen.top

Java: // 手写递归
来源：http://kjh.cucudq.cn

Go:   // 手写递归
来源：http://joz.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ygp.hywenlv.cn

C#:   // 手写递归
来源：http://hww.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://epo.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vfo.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xcl.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cdv.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://crh.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ley.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bkf.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rve.dashuyun.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bln.xylfe.cn

================================================================================
来源：http://aon.andypj.xyz

O. 并发与异步
来源：http://xvo.mhx1999.top

================================================================================
来源：http://kbn.wangdashe.top

[O01] 启动一个线程
来源：http://qyi.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://frl.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oda.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vfj.meibo888.top

TS:   // 同 JS
来源：http://jth.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://dtw.sxryk.cn

Go:   go f()
来源：http://tyr.birdmap.top

Ruby: Thread.new { f }
来源：http://yqs.andypj.xyz

C#:   Task.Run(() => F());
来源：http://fut.9152youxi.cn

[O02] 使用线程池
来源：http://aor.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ljt.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://adw.jianghu66.top

JS:   // worker_threads 线程池
来源：http://ejg.yuxming.cn

TS:   // worker_threads 线程池
来源：http://lzq.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://idd.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yit.yj20258888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nai.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rzk.yj20258.top

[O03] 加锁保护共享数据
来源：http://uiu.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://lqx.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://jtf.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iyk.52xcode.cn

TS:   // 同 JS
来源：http://jgz.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://jyf.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vdd.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xcc.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://epk.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://xoo.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://hgy.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ypj.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://pye.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dxe.chenlongwang.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yol.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gye.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://mlc.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://gan.nwbrower.top

[O05] 并发执行并等待全部完成
来源：http://lwc.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://byc.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jri.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://cnw.yonumen.top

TS:   await Promise.all(tasks)
来源：http://mml.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oor.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sia.hesvh.cn

Ruby: threads.map(&:join)
来源：http://hoz.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://czz.yueranfly.top

[O06] 使用进程池
来源：http://tnk.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://skq.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jzd.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://pmv.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://xlm.fzhhl.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dac.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sob.uphjek.com

Ruby: // fork 块
来源：http://vub.shuidangran.top

C#:   Parallel.For
来源：http://cbv.gogol.net.cn

================================================================================
来源：http://idj.smart0.xyz

P. 常用工具函数
来源：http://mcq.tanke756.top

================================================================================
来源：http://mjr.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://nma.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://gbv.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qxz.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://jsm.dianchejie.cn

TS:   crypto.randomUUID()
来源：http://qyr.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://gwx.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://zqt.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://mzl.fanxiaobao.xyz

C#:   Guid.NewGuid().ToString()
来源：http://vww.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://ofc.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bca.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://fbf.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tfg.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wvm.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ieg.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gha.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cuz.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nby.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://lvt.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://spe.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pow.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jpb.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ouh.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fsg.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qbr.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://acc.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pxv.hysaishi.cn

[P04] 求长度
来源：http://yee.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ztd.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wyi.hesvh.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ubu.wangshuangyany.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtk.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://hwd.yj20258888.top

Go:   len(arr);  len(m)
来源：http://itd.jqgfzy.top

Ruby: x.length;  x.size
来源：http://nwy.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://smt.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://nnx.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ckx.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uhg.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jwo.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jtv.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://enb.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://ona.ppjwa.cn

Ruby: a == b
来源：http://kld.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xrh.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lxb.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://scr.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://ruk.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ddb.tian-w.cn

TS:   if (x == null) {}
来源：http://ocg.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zqc.zhongyouzk.top

Go:   if x == nil {}
来源：http://jox.zycfv.cn


<!-- 参考信息 -->