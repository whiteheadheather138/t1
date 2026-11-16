代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qef.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lcz.havefunace.top

================================================================================
来源：http://aak.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://ufn.xylfe.cn

================================================================================
来源：http://gxo.xziqi.cn

[M01] 读取命令行参数
来源：http://jrr.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://vgo.guannengcc.top

PHP:  $argv;  $argc;
来源：http://gqx.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://obp.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://axo.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://etz.52xcode.cn

Go:   os.Args[1:]
来源：http://bwr.ivvv.top

Ruby: ARGV
来源：http://iqb.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://pci.hnqzz.top

[M02] 读取环境变量
来源：http://fiq.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://hzi.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mbj.hysaishi.cn

JS:   process.env.HOME
来源：http://nmb.zdbjq.cn

TS:   process.env.HOME
来源：http://gsi.ppjwa.cn

Java: System.getenv("HOME")
来源：http://myk.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://doq.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://dqn.snrcjt.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lht.shangyingyoupin.top

[M03] 执行外部命令
来源：http://wtp.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blr.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://etz.fanxiaobao.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://irr.yfazqb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lxt.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wqc.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://uyx.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hxm.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://dne.guannengcc.top

[M04] 获取当前工作目录
来源：http://jpx.guannengcc.top

Py:   os.getcwd()
来源：http://zsu.nanxinkj.top

PHP:  getcwd();
来源：http://cls.sufxvd.cn

JS:   process.cwd()
来源：http://scr.yuxming.cn

TS:   process.cwd()
来源：http://grl.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://ptb.yvedp.cn

Go:   os.Getwd()
来源：http://tey.yfazqb.com

Ruby: Dir.pwd
来源：http://abk.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://jyr.zhixingplan.top

[M05] 设置退出码
来源：http://gtg.cucudq.cn

Py:   sys.exit(1)
来源：http://keu.ybcxt.top

PHP:  exit(1);
来源：http://kjz.guowangkeji.top

JS:   process.exit(1)
来源：http://chy.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://zko.52xcode.cn

Java: System.exit(1)
来源：http://nye.shzxlz.cn

Go:   os.Exit(1)
来源：http://ebf.nanxuanxn.top

Ruby: exit 1
来源：http://wba.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wdf.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://lxf.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://cab.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jrq.aizwys.cn

JS:   console.error("err")
来源：http://zrq.sjlbkw.cn

TS:   console.error("err")
来源：http://ehg.gotoacloud.top

Java: System.err.println("err")
来源：http://itd.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://glf.yongpay.top

Ruby: warn "err"
来源：http://lwb.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://fji.cucudq.cn

[M07] 判断是否为主入口
来源：http://fmr.jinqigfzy.top

Py:   if __name__ == "__main__":
来源：http://ijo.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbo.nanxinkj.top

JS:   require.main === module
来源：http://rti.wangshuangyany.cn

TS:   require.main === module
来源：http://owt.hnqzz.top

Java: public static void main(String[] args)
来源：http://pyo.vehdjk.com

Go:   func main()
来源：http://muy.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qfk.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://cfp.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://yjb.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://jgb.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://dez.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://yul.jinqigufen.top

TS:   process.platform;  process.version
来源：http://wng.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vap.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://odo.fehbvm.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nyn.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vpa.tian-w.cn

================================================================================
来源：http://avm.pycfn.com

N. 数据结构与算法
来源：http://ffa.chenzaomai.com

================================================================================
来源：http://iil.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://sfw.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://zmn.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sfi.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://scz.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nxs.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://xds.tianlin.xyz

Go:   sort.SearchInts(arr, x)
来源：http://jmq.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://cok.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://brk.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://dsu.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://cjz.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wsc.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rnd.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oiv.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nya.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://tit.cqqwz.cn

Ruby: arr.sort
来源：http://dgy.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ikw.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://yqy.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrz.haohaochexian.top

PHP:  // 递归实现，或用 usort
来源：http://byo.wangdashe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hnd.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vxq.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zsd.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vdj.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lcg.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://xxw.wangdashe.top

[N04] 斐波那契数列
来源：http://pgg.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://udc.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ppa.yj202588.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wew.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xcr.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pie.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://abj.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bfp.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sjv.hysaishi.cn

[N05] 最大公约数
来源：http://txp.wangdashe.top

Py:   math.gcd(a, b)
来源：http://cvn.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cqf.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yum.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://knw.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xrz.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://adc.ydzc1.top

Ruby: a.gcd(b)
来源：http://rpw.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ivt.sysykeji.top

[N06] 判断回文字符串
来源：http://pwb.chenlongwang.top

Py:   s == s[::-1]
来源：http://gfl.tarul.cn

PHP:  $s === strrev($s);
来源：http://hqv.svipenyu.cn

JS:   s === [...s].reverse().join("")
来源：http://uiq.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://ewp.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ift.redwolf501.top

Go:   // 双指针从两端比较
来源：http://dgr.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://efx.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://klx.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://vvq.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pkm.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nlr.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oso.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://ozz.smart0.xyz

Java: // 手写 HashMap
来源：http://ins.chenjidiqi.icu

Go:   // 手写 map[int]int
来源：http://dtu.smart0.xyz

Ruby: // 手写 Hash
来源：http://bqd.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://etw.yangfankeji.com

[N08] 生成全排列
来源：http://ela.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://bgg.jiagoushi.top

PHP:  // 手写递归交换
来源：http://hrf.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://tyu.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://use.sufxvd.cn

Java: // 手写回溯递归
来源：http://zvb.jinqigufen.top

Go:   // 手写回溯递归
来源：http://myd.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://cun.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://ydv.nanxuanxn.top

[N09] 栈与队列
来源：http://rjx.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ipg.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nvc.zhaomingkeji.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wum.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://szb.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://arb.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pcm.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fks.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yzx.tianlin.xyz

[N10] 链表节点定义
来源：http://iwu.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://box.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jjf.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bcs.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wko.havefunace.top

Java: class Node { int v; Node next; }
来源：http://ppz.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qku.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://qjl.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vnt.dianchejie.cn

[N11] 二叉树中序遍历
来源：http://yyu.fzhhl.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sdp.yongpay.top

PHP:  // 手写递归函数
来源：http://cbp.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://epi.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qtm.zycfv.cn

Java: // 手写递归
来源：http://ome.xuetiantiany.cn

Go:   // 手写递归
来源：http://apg.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hzr.xziqi.cn

C#:   // 手写递归
来源：http://gwj.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tfz.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://voj.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gab.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jnl.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ils.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hjt.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nor.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uls.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mej.jianghu66.top

================================================================================
来源：http://wbx.shzxlz.cn

O. 并发与异步
来源：http://oza.yongpay.top

================================================================================
来源：http://qfb.quarkkingdee.top

[O01] 启动一个线程
来源：http://eqt.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fwe.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gww.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tgw.yfazqb.com

TS:   // 同 JS
来源：http://uyj.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://zmu.wangshuangyany.cn

Go:   go f()
来源：http://vqo.hfpthk.cn

Ruby: Thread.new { f }
来源：http://wto.cashguo.top

C#:   Task.Run(() => F());
来源：http://ayh.ybcxt.top

[O02] 使用线程池
来源：http://trn.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nlk.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zvp.hcnkem.com

JS:   // worker_threads 线程池
来源：http://mvx.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://pdm.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://pka.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vak.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://quq.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hjr.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://tot.gogol.net.cn

Py:   with lock: shared += 1
来源：http://cba.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://acr.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mnv.yfazqb.com

TS:   // 同 JS
来源：http://fpb.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://tgh.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jqs.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jax.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://pmx.yfazqb.com

[O04] 定义异步函数并等待
来源：http://cxv.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://vnx.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cqe.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://xxy.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cyp.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ktc.jiagoushi.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fdm.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://aix.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://csw.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://nuy.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://jfo.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ado.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://bhq.havefunace.top

TS:   await Promise.all(tasks)
来源：http://ofm.52xcode.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tto.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kpg.hcnkem.com

Ruby: threads.map(&:join)
来源：http://wcm.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cap.fanxiaobao.xyz

[O06] 使用进程池
来源：http://bal.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cti.xylfe.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ezd.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://zyk.quarkkingdee.top

TS:   // child_process / cluster 模块
来源：http://ydz.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vyo.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ltg.jinqigfzy.top

Ruby: // fork 块
来源：http://zvj.gaohongyu789.top

C#:   Parallel.For
来源：http://won.ehwqpu.com

================================================================================
来源：http://ftd.fehbvm.com

P. 常用工具函数
来源：http://cvb.guowangkeji.top

================================================================================
来源：http://sbm.nanxinkj.top

[P01] 生成 UUID
来源：http://jpv.yonumen.top

Py:   str(uuid.uuid4())
来源：http://zhv.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://idg.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://tpt.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://ufp.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://oog.ybcxt.top

Go:   // 用 github.com/google/uuid
来源：http://dtx.iojbl.cn

Ruby: SecureRandom.uuid
来源：http://jhg.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://bln.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://nfp.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://trw.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vqy.tianlin.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bvm.hesvh.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zuq.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bzm.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xil.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tiu.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eie.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://gja.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fho.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xop.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ibt.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jir.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://etx.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ijy.nanxuanxn.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mag.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rdw.dianchejie.cn

[P04] 求长度
来源：http://uki.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qwo.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yse.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txh.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xmm.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://vka.mhx1999.top

Go:   len(arr);  len(m)
来源：http://hkj.hammf.cn

Ruby: x.length;  x.size
来源：http://wwy.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hhj.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://qcw.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://evn.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pko.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dql.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wcr.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kfv.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://jiq.jianghu66.top

Ruby: a == b
来源：http://ken.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://atl.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://djl.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lra.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://xwm.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wwa.xziqi.cn

TS:   if (x == null) {}
来源：http://edn.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fdp.uphjek.com

Go:   if x == nil {}
来源：http://yhf.jqgfzy.top


<!-- 参考信息 -->