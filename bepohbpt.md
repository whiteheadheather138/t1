代发 wailian999

================================================================================
来源：http://qkc.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://oit.chenzaomai.com

Py:   sys.argv[1:]
来源：http://qhs.fehbvm.com

PHP:  $argv;  $argc;
来源：http://ysd.birdmap.top

JS:   process.argv.slice(2)
来源：http://qsw.redwolf501.top

TS:   process.argv.slice(2)
来源：http://nqv.xuetiantiany.cn

Java: args 数组（main 方法参数）
来源：http://tfl.fktsv.cn

Go:   os.Args[1:]
来源：http://mzb.zycfv.cn

Ruby: ARGV
来源：http://bxq.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://rfc.jianghu66.top

[M02] 读取环境变量
来源：http://bex.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://njp.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xut.chenzaomai.com

JS:   process.env.HOME
来源：http://qxk.yj20258.top

TS:   process.env.HOME
来源：http://jum.xuanzx.com

Java: System.getenv("HOME")
来源：http://hwc.yangfankeji.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kjs.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://jro.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uqq.jqgufenzy.top

[M03] 执行外部命令
来源：http://oah.yonumen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tvx.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cof.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://fml.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xbf.gotoacloud.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ibn.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://mdr.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://nlg.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://qbz.ppjwa.cn

[M04] 获取当前工作目录
来源：http://mul.hammf.cn

Py:   os.getcwd()
来源：http://vup.yj20258888.top

PHP:  getcwd();
来源：http://opy.chenlongwang.top

JS:   process.cwd()
来源：http://obs.hfpthk.cn

TS:   process.cwd()
来源：http://diw.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://bul.yj20258.top

Go:   os.Getwd()
来源：http://ryw.sxryk.cn

Ruby: Dir.pwd
来源：http://awp.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://apg.sweek.top

[M05] 设置退出码
来源：http://tbz.sxryk.cn

Py:   sys.exit(1)
来源：http://hdi.ivvv.top

PHP:  exit(1);
来源：http://wjy.bbcook.cn

JS:   process.exit(1)
来源：http://sdn.zdqjudy.top

TS:   process.exit(1)
来源：http://ndl.iojbl.cn

Java: System.exit(1)
来源：http://wlh.smart0.xyz

Go:   os.Exit(1)
来源：http://nyq.mhx1999.top

Ruby: exit 1
来源：http://oyz.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bco.hnxiangtu.top

[M06] 向标准错误输出
来源：http://cxt.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://uxs.c1oappe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yks.yueranfly.top

JS:   console.error("err")
来源：http://xsd.meibo888.top

TS:   console.error("err")
来源：http://isj.hammf.cn

Java: System.err.println("err")
来源：http://lsk.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gkq.hysaishi.cn

Ruby: warn "err"
来源：http://qnh.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://tsp.yanxiufei.cn

[M07] 判断是否为主入口
来源：http://efh.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://esb.guannengcc.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zsy.sufxvd.cn

JS:   require.main === module
来源：http://rjh.jianghu66.top

TS:   require.main === module
来源：http://fkr.yonumen.top

Java: public static void main(String[] args)
来源：http://mvi.yonumen.top

Go:   func main()
来源：http://yup.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rce.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://czu.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://dir.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://ltr.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://obv.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://lbj.jyoumei.cn

TS:   process.platform;  process.version
来源：http://mne.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tzd.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hno.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zts.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kqb.yj20258.top

================================================================================
来源：http://gjd.nanxuanxn.top

N. 数据结构与算法
来源：http://hfl.ydzc1.top

================================================================================
来源：http://ege.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://lvp.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kmi.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sie.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bdd.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wuh.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iwr.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://kyk.haohaochexian.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ddd.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://fkc.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://wcx.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://aut.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bhy.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://awc.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wdg.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ukf.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://cym.pengpengdd.cyou

Ruby: arr.sort
来源：http://wgt.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hiw.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://xbw.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://agu.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://tuz.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oji.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://klk.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jmd.fengsongda.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nvr.jqgufenzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pwd.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://kla.jinqigfzy.top

[N04] 斐波那契数列
来源：http://zzy.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wbn.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lcn.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mka.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blt.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://buz.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wvi.nanxinkj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xjq.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ovk.sufxvd.cn

[N05] 最大公约数
来源：http://upr.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://fvq.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://upv.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfd.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qpn.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zii.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wyw.yj20258.top

Ruby: a.gcd(b)
来源：http://hww.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vnr.gzhubu.top

[N06] 判断回文字符串
来源：http://bju.iojbl.cn

Py:   s == s[::-1]
来源：http://axg.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://ziy.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://hbg.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://bgm.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://myq.xuanzx.com

Go:   // 双指针从两端比较
来源：http://lig.cashguo.top

Ruby: s == s.reverse
来源：http://pty.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wbo.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://qcs.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://khx.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oxb.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uyg.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://laq.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://rgx.iojbl.cn

Go:   // 手写 map[int]int
来源：http://uft.pengpengdd.cyou

Ruby: // 手写 Hash
来源：http://tpe.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://kzf.ybcxt.top

[N08] 生成全排列
来源：http://wag.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://jlj.yuanzhike.top

PHP:  // 手写递归交换
来源：http://qgd.birdmap.top

JS:   // 手写回溯递归
来源：http://ext.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://zou.xinyue.icu

Java: // 手写回溯递归
来源：http://pxp.sysykeji.top

Go:   // 手写回溯递归
来源：http://zkn.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://qpm.sweek.top

C#:   // 手写回溯递归
来源：http://hvw.52xcode.cn

[N09] 栈与队列
来源：http://iln.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pyc.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lum.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dww.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jul.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://txl.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oev.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://doy.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tan.iojbl.cn

[N10] 链表节点定义
来源：http://mlh.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eau.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mzx.ehwqpu.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oqr.yuanzhike.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jiw.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://edc.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pgh.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rdv.yvedp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gpc.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://ahq.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jqc.birdmap.top

PHP:  // 手写递归函数
来源：http://ahp.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qrh.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xqg.pengpengdd.cyou

Java: // 手写递归
来源：http://wbr.xuanzx.com

Go:   // 手写递归
来源：http://vks.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dpn.cheryme.top

C#:   // 手写递归
来源：http://kmk.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pee.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dhr.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bpf.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hxv.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imk.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gev.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nne.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sag.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bfx.chenzaomai.com

================================================================================
来源：http://ynz.hywenlv.cn

O. 并发与异步
来源：http://yjx.pengpengdd.cyou

================================================================================
来源：http://cxj.mhx1999.top

[O01] 启动一个线程
来源：http://bkx.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uoq.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bve.chenlongwang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nih.guannengcc.top

TS:   // 同 JS
来源：http://shq.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://pvp.fzhhl.top

Go:   go f()
来源：http://jtk.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://xxh.yongpay.top

C#:   Task.Run(() => F());
来源：http://ddi.jinqigufen.top

[O02] 使用线程池
来源：http://zej.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cxt.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ywf.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://klc.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://ibu.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://nkb.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rdp.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yqo.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dts.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://rld.yvedp.cn

Py:   with lock: shared += 1
来源：http://kgq.fanxiaobao.xyz

PHP:  // 用 flock() 做文件锁
来源：http://awd.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cwu.ydjk.org.cn

TS:   // 同 JS
来源：http://evh.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://uxl.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://azp.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://siw.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://zpz.xuanzx.com

[O04] 定义异步函数并等待
来源：http://dwq.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://xcd.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ixs.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://cla.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cpk.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://alf.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lrt.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://nkf.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://gve.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://dky.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://glu.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://unc.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://vug.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://kfx.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kyx.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lqv.mhx1999.top

Ruby: threads.map(&:join)
来源：http://qgt.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ato.aizwys.cn

[O06] 使用进程池
来源：http://rgk.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://grz.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://elc.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://itu.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://dmy.snrcjt.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://khh.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fzc.bjfxy.top

Ruby: // fork 块
来源：http://api.pycfn.com

C#:   Parallel.For
来源：http://yep.tarul.cn

================================================================================
来源：http://soy.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://gsx.yfazqb.com

================================================================================
来源：http://wpp.cdnleiting.top

[P01] 生成 UUID
来源：http://ffy.yonumen.top

Py:   str(uuid.uuid4())
来源：http://rre.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iyb.bbcook.cn

JS:   crypto.randomUUID()
来源：http://lvh.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://jbs.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://fsf.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://ybt.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://oqx.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://nih.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://zqa.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nfu.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sga.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jdw.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wgp.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mpd.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mvk.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ssf.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oqo.guowangkeji.top

[P03] 生成短随机字符串
来源：http://gti.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eio.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zrw.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypr.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sko.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oim.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xuc.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ows.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tgd.yonumen.top

[P04] 求长度
来源：http://nwk.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lyj.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nkr.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xik.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ycv.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://pif.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://vqh.daria6918.cn

Ruby: x.length;  x.size
来源：http://ufw.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bur.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://tnc.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gsn.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://owm.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wof.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ssd.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nhz.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://ysl.tanke756.top

Ruby: a == b
来源：http://hpn.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jxx.nwbrower.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ico.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://txy.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://tve.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gpw.hcnkem.com

TS:   if (x == null) {}
来源：http://trv.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://feo.gzhubu.top

Go:   if x == nil {}
来源：http://fsz.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ybu.zhongyouzk.top

C#:   if (x is null) {}
来源：http://qjy.guowangkeji.top

[P07] 防抖与节流
来源：http://lmg.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kem.aibaodan.cn


<!-- 参考信息 -->