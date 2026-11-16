代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bdj.zdbjq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fvk.feifeiyinyue.top

================================================================================
来源：http://pfo.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://giu.9152youxi.cn

================================================================================
来源：http://iuo.aizwys.cn

[M01] 读取命令行参数
来源：http://mli.guowangkeji.top

Py:   sys.argv[1:]
来源：http://azt.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://fgi.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://bgi.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://vuw.hnqzz.top

Java: args 数组（main 方法参数）
来源：http://dbh.cheryme.top

Go:   os.Args[1:]
来源：http://rvt.hysaishi.cn

Ruby: ARGV
来源：http://qmp.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://xgo.jinqigufen.top

[M02] 读取环境变量
来源：http://ywp.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://oon.aizwys.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ljl.vehdjk.com

JS:   process.env.HOME
来源：http://xdb.fehbvm.com

TS:   process.env.HOME
来源：http://pzw.tarul.cn

Java: System.getenv("HOME")
来源：http://wlm.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qio.zhaomingkeji.xyz

Ruby: ENV["HOME"]
来源：http://tzp.fanxiaobao.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yur.ppjwa.cn

[M03] 执行外部命令
来源：http://vch.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tcy.jinqigfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nek.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vbg.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wii.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://adj.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ndy.chenzaomai.com

Ruby: system("ls -l");  `ls -l`
来源：http://mzi.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://ktd.gotoacloud.top

[M04] 获取当前工作目录
来源：http://uuw.cqqwz.cn

Py:   os.getcwd()
来源：http://wrs.pengpengdd.cyou

PHP:  getcwd();
来源：http://hfe.dianchejie.cn

JS:   process.cwd()
来源：http://xec.cdnleiting.top

TS:   process.cwd()
来源：http://qun.redwolf501.top

Java: Path.of("").toAbsolutePath()
来源：http://inf.c1oappe.top

Go:   os.Getwd()
来源：http://pjh.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://hta.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://aym.yvedp.cn

[M05] 设置退出码
来源：http://ixw.hnqzz.top

Py:   sys.exit(1)
来源：http://ibs.jiagoushi.top

PHP:  exit(1);
来源：http://onr.tarul.cn

JS:   process.exit(1)
来源：http://zcd.feifeiyinyue.top

TS:   process.exit(1)
来源：http://ylz.chenjidiqi.icu

Java: System.exit(1)
来源：http://kia.jqgfzy.top

Go:   os.Exit(1)
来源：http://eoh.fzhhl.top

Ruby: exit 1
来源：http://cle.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ujh.meibo888.top

[M06] 向标准错误输出
来源：http://fpv.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://art.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qmw.316326.xyz

JS:   console.error("err")
来源：http://shl.zdbjq.cn

TS:   console.error("err")
来源：http://bnw.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://hwa.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lrh.sufxvd.cn

Ruby: warn "err"
来源：http://yca.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://vha.smart0.xyz

[M07] 判断是否为主入口
来源：http://mod.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://rev.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fxa.jinyuanbaomall.cn

JS:   require.main === module
来源：http://shd.zdqjudy.top

TS:   require.main === module
来源：http://ksx.sufxvd.cn

Java: public static void main(String[] args)
来源：http://wxw.yj20258888.top

Go:   func main()
来源：http://omp.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bej.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://yoo.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://kha.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://wii.jinyuanbaomall.cn

PHP:  PHP_OS;  phpversion();
来源：http://oac.yj20258888.top

JS:   process.platform;  process.version
来源：http://lav.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://rxk.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mrj.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://zum.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zxm.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://fjr.vehdjk.com

================================================================================
来源：http://goz.0kj1m.cn

N. 数据结构与算法
来源：http://xyv.zhaomingkeji.xyz

================================================================================
来源：http://isi.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://bqg.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gxm.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dfl.aibaodan.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jcv.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ssp.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://ejc.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://ges.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jgf.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ljl.feifeiyinyue.top

[N02] 排序（工程实践用内置实现）
来源：http://lgq.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://nsz.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qzn.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://dmg.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oar.jinqigufen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mcn.xziqi.cn

Go:   slices.Sort(arr)
来源：http://lhq.guowangkeji.top

Ruby: arr.sort
来源：http://awg.zycfv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://was.cheryme.top

[N03] 快速排序（分治示例）
来源：http://uat.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xor.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://xaj.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://haq.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozn.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://trc.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cqk.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wxd.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://xll.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://ltf.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wfd.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dwr.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eos.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gez.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqi.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uaf.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dqn.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tbu.hnxiangtu.top

[N05] 最大公约数
来源：http://eqg.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://vtx.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://egk.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ptb.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dqj.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybh.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mhv.yueranfly.top

Ruby: a.gcd(b)
来源：http://zyy.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rck.fehbvm.com

[N06] 判断回文字符串
来源：http://pbu.chenzaomai.com

Py:   s == s[::-1]
来源：http://esz.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://vvc.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://idj.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://aml.xylfe.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qia.tian-w.cn

Go:   // 双指针从两端比较
来源：http://qqa.cdnleiting.top

Ruby: s == s.reverse
来源：http://jcu.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rzq.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://gia.hesvh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://evj.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gbv.hfpthk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://leo.tanke756.top

TS:   // 手写 Map<string, number>
来源：http://urj.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://rol.hnqzz.top

Go:   // 手写 map[int]int
来源：http://kzo.yj202588.top

Ruby: // 手写 Hash
来源：http://alr.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hne.jqgfzy.top

[N08] 生成全排列
来源：http://ocm.zhoulong.xyz

Py:   itertools.permutations(arr)
来源：http://pvt.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://deh.guowangkeji.top

JS:   // 手写回溯递归
来源：http://poa.xinyue.icu

TS:   // 手写回溯递归
来源：http://nrh.xziqi.cn

Java: // 手写回溯递归
来源：http://akt.fzhhl.top

Go:   // 手写回溯递归
来源：http://hhe.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://ncn.aizwys.cn

C#:   // 手写回溯递归
来源：http://nbn.zhongyouzk.top

[N09] 栈与队列
来源：http://noq.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qma.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iex.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cfd.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sjb.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gpf.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mib.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hzj.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sha.xingfuxueyuan.xyz

[N10] 链表节点定义
来源：http://xiv.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rni.chenzaomai.com

PHP:  class Node { public $v; public $next = null; }
来源：http://xfd.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sfu.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vql.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://obf.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://eez.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uzc.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sqi.shanyushiyangkeji.top

[N11] 二叉树中序遍历
来源：http://pfo.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://czx.yj20258888.top

PHP:  // 手写递归函数
来源：http://ojt.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxb.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jvu.cucudq.cn

Java: // 手写递归
来源：http://rfy.jiagoushi.top

Go:   // 手写递归
来源：http://cfp.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dvj.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://qzr.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ins.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dfn.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xuz.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ptg.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kwn.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pas.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lna.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kmp.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bkk.epnwcf.com

================================================================================
来源：http://fxr.52xcode.cn

O. 并发与异步
来源：http://sao.epnwcf.com

================================================================================
来源：http://hgs.cdnleiting.top

[O01] 启动一个线程
来源：http://vgy.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rfu.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nal.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qph.jyoumei.cn

TS:   // 同 JS
来源：http://zou.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://dco.fehbvm.com

Go:   go f()
来源：http://bjw.ybcxt.top

Ruby: Thread.new { f }
来源：http://gln.chenlongwang.top

C#:   Task.Run(() => F());
来源：http://nrb.xuanzx.com

[O02] 使用线程池
来源：http://bzh.mhx1999.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fpc.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mux.sweek.top

JS:   // worker_threads 线程池
来源：http://clj.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://oyh.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://bri.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ybh.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wyk.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nhu.fzhhl.top

[O03] 加锁保护共享数据
来源：http://oaa.zycfv.cn

Py:   with lock: shared += 1
来源：http://wlx.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://gop.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jgh.cashguo.top

TS:   // 同 JS
来源：http://dxa.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://kpi.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hua.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://brg.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://kid.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://gsq.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://hkw.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tgp.mhx1999.top

JS:   async function f() { await g(); }
来源：http://lzf.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iln.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hdt.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uqr.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://qlw.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://lse.ywan-chungtsiang.top

[O05] 并发执行并等待全部完成
来源：http://xja.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://ewu.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xcx.jinghuilouyu.cn

JS:   await Promise.all(tasks)
来源：http://ito.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://bop.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qad.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rkk.redwolf501.top

Ruby: threads.map(&:join)
来源：http://zhf.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jfw.bjfxy.top

[O06] 使用进程池
来源：http://wnb.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rxc.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uud.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://hng.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://qid.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dim.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bdm.yonumen.top

Ruby: // fork 块
来源：http://sej.yj20258.top

C#:   Parallel.For
来源：http://avb.fzhhl.top

================================================================================
来源：http://rrn.dianchejie.cn

P. 常用工具函数
来源：http://iid.jyoumei.cn

================================================================================
来源：http://xwl.wangdashe.top

[P01] 生成 UUID
来源：http://mtl.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://lgb.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vqp.daxiang520.top

JS:   crypto.randomUUID()
来源：http://vro.dianchejie.cn

TS:   crypto.randomUUID()
来源：http://lyy.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://yka.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://rro.yongpay.top

Ruby: SecureRandom.uuid
来源：http://uij.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://erc.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://cqm.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qbs.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cnp.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://evz.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emk.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://djx.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vdo.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://spn.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sby.zdqjudy.top

[P03] 生成短随机字符串
来源：http://bbp.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yqa.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wfe.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dde.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oci.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qvi.xziqi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sqc.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yyp.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mtm.cucudq.cn

[P04] 求长度
来源：http://lhr.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://epb.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yto.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gte.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qqc.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://abu.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://cyu.yuxming.cn

Ruby: x.length;  x.size
来源：http://ykk.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rpl.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://qss.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ytg.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aqs.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://loh.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bxg.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kgt.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://omr.xziqi.cn

Ruby: a == b
来源：http://bfo.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gox.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zxf.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dsv.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://ief.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fnh.jqgfzy.top

TS:   if (x == null) {}
来源：http://nzf.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nol.zdqjudy.top

Go:   if x == nil {}
来源：http://qei.feifeiyinyue.top


<!-- 参考信息 -->