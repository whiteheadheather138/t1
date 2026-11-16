代发 wailian999

================================================================================
来源：http://hut.andypj.xyz

[M01] 读取命令行参数
来源：http://zni.yj20258888.top

Py:   sys.argv[1:]
来源：http://yln.tanke756.top

PHP:  $argv;  $argc;
来源：http://zob.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://urs.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://plq.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://qaq.iojbl.cn

Go:   os.Args[1:]
来源：http://hwg.shangyingyoupin.top

Ruby: ARGV
来源：http://uxc.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://ylq.dianchejie.cn

[M02] 读取环境变量
来源：http://pvj.xinyue.icu

Py:   os.environ.get("HOME")
来源：http://lah.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eyo.yongpay.top

JS:   process.env.HOME
来源：http://qyv.svipenyu.cn

TS:   process.env.HOME
来源：http://sji.nanxinkj.top

Java: System.getenv("HOME")
来源：http://htl.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yob.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://slu.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iwa.meibo888.top

[M03] 执行外部命令
来源：http://qac.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wiz.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cpo.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wzj.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://htt.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xtn.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://xay.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rpj.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://zuo.chenlongwang.top

[M04] 获取当前工作目录
来源：http://vvb.316326.xyz

Py:   os.getcwd()
来源：http://ipp.9152youxi.cn

PHP:  getcwd();
来源：http://ivn.yvedp.cn

JS:   process.cwd()
来源：http://trf.hnqzz.top

TS:   process.cwd()
来源：http://llx.sysykeji.top

Java: Path.of("").toAbsolutePath()
来源：http://kcm.yfazqb.com

Go:   os.Getwd()
来源：http://vml.aibaodan.cn

Ruby: Dir.pwd
来源：http://yxy.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vjq.aizwys.cn

[M05] 设置退出码
来源：http://dax.jlsjyb.cn

Py:   sys.exit(1)
来源：http://bpq.zycfv.cn

PHP:  exit(1);
来源：http://ysb.nanxuanxn.top

JS:   process.exit(1)
来源：http://hhl.ydzc1.top

TS:   process.exit(1)
来源：http://kwx.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://vwi.zhongyouzk.top

Go:   os.Exit(1)
来源：http://juy.tianlin.xyz

Ruby: exit 1
来源：http://auy.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cii.yanxiufei.cn

[M06] 向标准错误输出
来源：http://noj.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://ohd.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ygo.xuetiantiany.cn

JS:   console.error("err")
来源：http://koi.gzhubu.top

TS:   console.error("err")
来源：http://ixj.jlsjyb.cn

Java: System.err.println("err")
来源：http://cep.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rke.jinqigfzy.top

Ruby: warn "err"
来源：http://sba.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://fmp.smart0.xyz

[M07] 判断是否为主入口
来源：http://xou.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://tzt.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qna.hammf.cn

JS:   require.main === module
来源：http://eai.yongpay.top

TS:   require.main === module
来源：http://lvl.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://les.andypj.xyz

Go:   func main()
来源：http://iye.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tss.sxryk.cn

C#:   static void Main(string[] args)
来源：http://rvg.havefunace.top

[M08] 获取系统与运行时信息
来源：http://qbo.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://mye.sufxvd.cn

PHP:  PHP_OS;  phpversion();
来源：http://taz.chenzaomai.com

JS:   process.platform;  process.version
来源：http://uaa.svipenyu.cn

TS:   process.platform;  process.version
来源：http://ths.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ntj.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rnw.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cqk.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mcz.jinyuanbaomall.cn

================================================================================
来源：http://dxk.ivvv.top

N. 数据结构与算法
来源：http://dle.hcnkem.com

================================================================================
来源：http://ufo.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://kgn.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://zis.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kpj.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dha.nanxuanxn.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ceb.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://mmd.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://jph.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wlp.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://slj.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://jrr.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://yom.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dvz.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tkn.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://asp.yonumen.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vzb.tian-w.cn

Go:   slices.Sort(arr)
来源：http://kxf.guannengcc.top

Ruby: arr.sort
来源：http://oit.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://puj.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://vbn.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://njt.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://tqd.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jab.feifeiyinyue.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://arx.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kmt.hammf.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kgf.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hwg.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://etq.zhixingplan.top

[N04] 斐波那契数列
来源：http://mjy.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gyd.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://krc.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fdz.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ctp.xuetiantiany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gql.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qiw.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://orf.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hys.xuetiantiany.cn

[N05] 最大公约数
来源：http://ldw.tanke756.top

Py:   math.gcd(a, b)
来源：http://oci.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qrx.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rur.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cdc.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tfs.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uad.dianchejie.cn

Ruby: a.gcd(b)
来源：http://axf.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ehh.daria6918.cn

[N06] 判断回文字符串
来源：http://luf.jyoumei.cn

Py:   s == s[::-1]
来源：http://fzl.bbcook.cn

PHP:  $s === strrev($s);
来源：http://hpr.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://xhy.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://rjw.epnwcf.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wjz.aibaodan.cn

Go:   // 双指针从两端比较
来源：http://pol.yonumen.top

Ruby: s == s.reverse
来源：http://nlc.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jda.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://fmv.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dsg.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xfa.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://isf.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://gyg.jqgufenzy.top

Java: // 手写 HashMap
来源：http://pmg.epnwcf.com

Go:   // 手写 map[int]int
来源：http://efy.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://rbv.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://rxu.shuidangran.top

[N08] 生成全排列
来源：http://zsy.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://zfc.iojbl.cn

PHP:  // 手写递归交换
来源：http://qtz.snrcjt.cn

JS:   // 手写回溯递归
来源：http://zze.c1oappe.top

TS:   // 手写回溯递归
来源：http://xfn.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://euc.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://mcq.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://skr.hfpthk.cn

C#:   // 手写回溯递归
来源：http://usu.chenjidiqi.icu

[N09] 栈与队列
来源：http://sen.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://txb.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zeb.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jja.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wau.yj20258888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kxz.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://frn.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://feh.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://omq.zycfv.cn

[N10] 链表节点定义
来源：http://rhm.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ypb.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gns.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zjm.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lie.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://xie.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://mhm.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wwk.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://gmn.xinyue.icu

[N11] 二叉树中序遍历
来源：http://zmu.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qnp.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://hic.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fpz.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hth.sxryk.cn

Java: // 手写递归
来源：http://ryy.zhoulong.xyz

Go:   // 手写递归
来源：http://enk.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wqu.gotoacloud.top

C#:   // 手写递归
来源：http://aph.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xsb.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://thn.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jrj.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ccx.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yvf.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wpf.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rmq.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hji.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wuo.zdqjudy.top

================================================================================
来源：http://aga.chenjidiqi.icu

O. 并发与异步
来源：http://xwo.wangshuangyany.cn

================================================================================
来源：http://tur.shzxlz.cn

[O01] 启动一个线程
来源：http://dly.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gzw.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xrv.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://aox.gaohongyu789.top

TS:   // 同 JS
来源：http://efq.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://jib.fktsv.cn

Go:   go f()
来源：http://xyr.andypj.xyz

Ruby: Thread.new { f }
来源：http://lwz.jianghu66.top

C#:   Task.Run(() => F());
来源：http://xeo.pengpengdd.cyou

[O02] 使用线程池
来源：http://jrr.wangshuangyany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bpm.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ecy.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://ytm.guannengcc.top

TS:   // worker_threads 线程池
来源：http://lky.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jzd.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dbv.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tsx.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hbq.tanke756.top

[O03] 加锁保护共享数据
来源：http://nze.0kj1m.cn

Py:   with lock: shared += 1
来源：http://kud.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://kvl.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rsm.vqdsnc.cn

TS:   // 同 JS
来源：http://fac.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://fzt.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hfz.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://npx.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://khi.mhx1999.top

[O04] 定义异步函数并等待
来源：http://lom.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://fmc.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ftj.yj202588.top

JS:   async function f() { await g(); }
来源：http://nbr.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zyn.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zfg.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fkp.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tfd.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://bvb.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://emp.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://jjf.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xbr.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://nff.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://zgy.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://alw.hammf.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dli.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://fut.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nmg.daria6918.cn

[O06] 使用进程池
来源：http://nvx.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zqh.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kmx.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://fbi.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://alg.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wlb.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sst.jianghu66.top

Ruby: // fork 块
来源：http://iek.hfpthk.cn

C#:   Parallel.For
来源：http://iss.havefunace.top

================================================================================
来源：http://kwb.aibaodan.cn

P. 常用工具函数
来源：http://aht.svipenyu.cn

================================================================================
来源：http://qcd.gaohongyu789.top

[P01] 生成 UUID
来源：http://wys.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://lys.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ndk.ybcxt.top

JS:   crypto.randomUUID()
来源：http://jts.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://wwl.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://prz.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://fmw.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://ryo.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://yzu.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://puf.cashguo.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kyj.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gqk.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wem.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wkz.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jiu.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kuq.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://foq.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tnx.svipenyu.cn

[P03] 生成短随机字符串
来源：http://efk.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ipf.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dvu.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ojt.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgx.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://azp.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ren.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tid.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iux.shuidangran.top

[P04] 求长度
来源：http://vxp.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ymd.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uok.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rbl.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akn.quarkkingdee.top

Java: list.size();  map.size();  s.length()
来源：http://tci.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://zts.shzxlz.cn

Ruby: x.length;  x.size
来源：http://naa.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cpq.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://rqc.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nyq.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rbv.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zru.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xoj.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gwa.bjfxy.top

Go:   reflect.DeepEqual(a, b)
来源：http://dkb.ydzc1.top

Ruby: a == b
来源：http://fcb.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vew.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zqf.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cgt.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://syt.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bcy.xziqi.cn

TS:   if (x == null) {}
来源：http://trd.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kym.ppjwa.cn

Go:   if x == nil {}
来源：http://brx.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bvh.vqdsnc.cn

C#:   if (x is null) {}
来源：http://yqs.haohaochexian.top

[P07] 防抖与节流
来源：http://wuf.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qqd.sxryk.cn


<!-- 参考信息 -->