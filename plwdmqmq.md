代发 wailian999

C#:   (int)resp.StatusCode
来源：http://fsj.hammf.cn

[L08] 并发请求多个地址
来源：http://yyg.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ugg.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://eyg.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wzn.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ihr.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pzc.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zqc.gaohongyu789.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://din.yvedp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lia.zhiwuduotai.top

================================================================================
来源：http://rfe.sweek.top

M. 命令行 / 进程 / 环境
来源：http://yuh.hesvh.cn

================================================================================
来源：http://lco.havefunace.top

[M01] 读取命令行参数
来源：http://qje.bbcook.cn

Py:   sys.argv[1:]
来源：http://dwh.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://duk.xziqi.cn

JS:   process.argv.slice(2)
来源：http://iug.andypj.xyz

TS:   process.argv.slice(2)
来源：http://uli.yonumen.top

Java: args 数组（main 方法参数）
来源：http://pel.jyoumei.cn

Go:   os.Args[1:]
来源：http://oha.fzhhl.top

Ruby: ARGV
来源：http://xty.9152youxi.cn

C#:   args 数组（Main 方法参数）
来源：http://ndw.vqdsnc.cn

[M02] 读取环境变量
来源：http://kub.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://eng.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xes.yuxming.cn

JS:   process.env.HOME
来源：http://qqu.xuanzx.com

TS:   process.env.HOME
来源：http://ahf.nwbrower.top

Java: System.getenv("HOME")
来源：http://nuj.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kmm.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://jgj.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://itq.dashuyun.cn

[M03] 执行外部命令
来源：http://nte.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wgm.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qxs.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ydg.fehbvm.com

TS:   child_process.execSync("ls -l").toString()
来源：http://tgb.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jme.bjfxy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lvs.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wzx.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://xqd.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://jnj.chenlongwang.top

Py:   os.getcwd()
来源：http://itn.quarkkingdee.top

PHP:  getcwd();
来源：http://vyl.haohaochexian.top

JS:   process.cwd()
来源：http://ctq.ppjwa.cn

TS:   process.cwd()
来源：http://xyv.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://hdk.yongpay.top

Go:   os.Getwd()
来源：http://sij.jyoumei.cn

Ruby: Dir.pwd
来源：http://vqw.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bdq.dianchejie.cn

[M05] 设置退出码
来源：http://buv.316326.xyz

Py:   sys.exit(1)
来源：http://gsl.nanxinkj.top

PHP:  exit(1);
来源：http://voc.cucudq.cn

JS:   process.exit(1)
来源：http://puq.tian-w.cn

TS:   process.exit(1)
来源：http://noa.dashuyun.cn

Java: System.exit(1)
来源：http://vpk.ehwqpu.com

Go:   os.Exit(1)
来源：http://qxt.iojbl.cn

Ruby: exit 1
来源：http://ves.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://usm.sxryk.cn

[M06] 向标准错误输出
来源：http://ftk.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://clb.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ihl.daxiang520.top

JS:   console.error("err")
来源：http://osp.yangfankeji.com

TS:   console.error("err")
来源：http://psv.havefunace.top

Java: System.err.println("err")
来源：http://wbj.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mmo.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://mab.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://evt.ivvv.top

[M07] 判断是否为主入口
来源：http://bqo.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://ugu.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tkh.yangfankeji.com

JS:   require.main === module
来源：http://vcs.quarkkingdee.top

TS:   require.main === module
来源：http://lik.chenlongwang.top

Java: public static void main(String[] args)
来源：http://vrf.c1oappe.top

Go:   func main()
来源：http://yyd.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nkl.cheryme.top

C#:   static void Main(string[] args)
来源：http://pof.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://bpk.dianchejie.cn

Py:   platform.system();  platform.python_version()
来源：http://amz.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://pgq.sweek.top

JS:   process.platform;  process.version
来源：http://akk.52xcode.cn

TS:   process.platform;  process.version
来源：http://kfj.quarkkingdee.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iwt.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://npy.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpl.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gcd.xuetiantiany.cn

================================================================================
来源：http://wst.cdnleiting.top

N. 数据结构与算法
来源：http://poh.yangfankeji.com

================================================================================
来源：http://vdc.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://cgv.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://vcl.zhixingplan.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://axl.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qle.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ofl.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://irw.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://yey.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bcz.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://cvp.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://tpu.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://zha.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://utr.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eil.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nmz.birdmap.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ome.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://lyv.yj202588.top

Ruby: arr.sort
来源：http://bik.mhx1999.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iir.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://lic.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxp.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://fpw.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dgs.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://puy.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://goc.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fgd.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yvn.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://sgu.yanxiufei.cn

[N04] 斐波那契数列
来源：http://zro.aibaodan.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eqf.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mog.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhy.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xgy.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bux.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bql.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://adk.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ipb.cqqwz.cn

[N05] 最大公约数
来源：http://cch.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://stn.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ubs.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jea.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ujv.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ajc.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hpi.cucudq.cn

Ruby: a.gcd(b)
来源：http://nzr.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kvm.yfazqb.com

[N06] 判断回文字符串
来源：http://yac.jqgfzy.top

Py:   s == s[::-1]
来源：http://lyw.epnwcf.com

PHP:  $s === strrev($s);
来源：http://wsd.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://azn.pycfn.com

TS:   s === [...s].reverse().join("")
来源：http://mnv.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ugj.iojbl.cn

Go:   // 双指针从两端比较
来源：http://ebh.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://zly.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://tyk.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://ulo.fzhhl.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wio.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://inz.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://irf.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://wuj.cashguo.top

Java: // 手写 HashMap
来源：http://nvf.fktsv.cn

Go:   // 手写 map[int]int
来源：http://lxg.nwbrower.top

Ruby: // 手写 Hash
来源：http://owl.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://meq.hongshengwenyu.top

[N08] 生成全排列
来源：http://iua.havefunace.top

Py:   itertools.permutations(arr)
来源：http://tnb.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://gxe.dashuyun.cn

JS:   // 手写回溯递归
来源：http://hqe.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://puw.yuanzhike.top

Java: // 手写回溯递归
来源：http://zyx.jqgfzy.top

Go:   // 手写回溯递归
来源：http://eas.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://djb.chenzaomai.com

C#:   // 手写回溯递归
来源：http://src.316326.xyz

[N09] 栈与队列
来源：http://bnp.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://krg.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ngv.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bgs.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zhv.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bbm.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xwc.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gxl.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vkd.zycfv.cn

[N10] 链表节点定义
来源：http://opv.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://imc.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://idz.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yjq.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ggl.yuanzhike.top

Java: class Node { int v; Node next; }
来源：http://cyv.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://hdx.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fgd.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://avc.bbcook.cn

[N11] 二叉树中序遍历
来源：http://jvs.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fok.yuanzhike.top

PHP:  // 手写递归函数
来源：http://qxi.sjlbkw.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tjv.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxc.mhx1999.top

Java: // 手写递归
来源：http://mbk.hongshengwenyu.top

Go:   // 手写递归
来源：http://fyz.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gsk.yj202588.top

C#:   // 手写递归
来源：http://vjo.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zzu.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rzb.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yvz.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uga.0kj1m.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vmh.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ptm.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vkh.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kcg.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ial.shangyingyoupin.top

================================================================================
来源：http://ljp.aibaodan.cn

O. 并发与异步
来源：http://wvq.pycfn.com

================================================================================
来源：http://hbh.chenlongwang.top

[O01] 启动一个线程
来源：http://wyk.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pzs.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yhq.yuxming.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ktp.snrcjt.cn

TS:   // 同 JS
来源：http://yjk.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://uqz.ppjwa.cn

Go:   go f()
来源：http://bby.tanke756.top

Ruby: Thread.new { f }
来源：http://xqu.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://vie.yonumen.top

[O02] 使用线程池
来源：http://amk.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uyk.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pei.yuxming.cn

JS:   // worker_threads 线程池
来源：http://oru.xinyue.icu

TS:   // worker_threads 线程池
来源：http://orv.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yle.yonumen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://thm.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zif.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zzm.tian-w.cn

[O03] 加锁保护共享数据
来源：http://qnn.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://cto.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://uog.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tbc.hammf.cn

TS:   // 同 JS
来源：http://bfk.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://hkv.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://grp.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cer.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://znr.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://msx.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://xte.sjlbkw.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iyn.zhiwuduotai.top

JS:   async function f() { await g(); }
来源：http://tcl.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://alu.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pnm.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://grp.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://xde.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://fic.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://cji.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://xat.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jdf.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://cxb.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://dqg.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zst.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oic.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://usl.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bye.gotoacloud.top

[O06] 使用进程池
来源：http://usb.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pdh.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://obe.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://kva.wangshuangyany.cn

TS:   // child_process / cluster 模块
来源：http://ell.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://btu.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bnh.xinyue.icu

Ruby: // fork 块
来源：http://ind.haohaochexian.top

C#:   Parallel.For
来源：http://cyf.fehbvm.com

================================================================================
来源：http://tzr.ywan-chungtsiang.top

P. 常用工具函数
来源：http://msx.jqgufenzy.top

================================================================================
来源：http://fhi.yj20258888.top

[P01] 生成 UUID
来源：http://qhg.kuanghao11.cn

Py:   str(uuid.uuid4())
来源：http://mpo.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nyg.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://czb.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://mqy.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://kdn.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://gnm.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://hkf.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://oao.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://kjr.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kxy.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dej.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cyh.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tds.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qmr.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bjh.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oak.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pkn.tanke756.top

[P03] 生成短随机字符串
来源：http://yzl.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cco.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fog.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qts.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xca.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hij.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iuu.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bvs.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rkg.daria6918.cn

[P04] 求长度
来源：http://haj.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nef.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pql.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ljj.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ete.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://wou.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://nul.chenzaomai.com

Ruby: x.length;  x.size
来源：http://kyf.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zjr.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://kdt.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fgi.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ywe.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kam.shzxlz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yeh.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hry.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://pio.ydjk.org.cn

Ruby: a == b
来源：http://aza.ehwqpu.com


<!-- 参考信息 -->