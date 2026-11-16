代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sjz.hnxiangtu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yhs.ivvv.top

================================================================================
来源：http://rkp.cqqwz.cn

M. 命令行 / 进程 / 环境
来源：http://pcz.nwbrower.top

================================================================================
来源：http://iia.nanxinkj.top

[M01] 读取命令行参数
来源：http://iup.bjfxy.top

Py:   sys.argv[1:]
来源：http://tge.zdqjudy.top

PHP:  $argv;  $argc;
来源：http://wob.xziqi.cn

JS:   process.argv.slice(2)
来源：http://uhi.0kj1m.cn

TS:   process.argv.slice(2)
来源：http://pyn.jiagoushi.top

Java: args 数组（main 方法参数）
来源：http://fpd.wangdashe.top

Go:   os.Args[1:]
来源：http://ljj.cucudq.cn

Ruby: ARGV
来源：http://ddy.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://svq.zhongyouzk.top

[M02] 读取环境变量
来源：http://frg.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://utt.hesvh.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gjy.ivvv.top

JS:   process.env.HOME
来源：http://vdh.hnxiangtu.top

TS:   process.env.HOME
来源：http://zos.hywenlv.cn

Java: System.getenv("HOME")
来源：http://ihp.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://abl.daxiang520.top

Ruby: ENV["HOME"]
来源：http://kpm.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://suz.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://npm.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qat.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://czb.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://cij.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://udt.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://esw.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://omy.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://awx.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://hct.haohaochexian.top

[M04] 获取当前工作目录
来源：http://yry.birdmap.top

Py:   os.getcwd()
来源：http://oav.sufxvd.cn

PHP:  getcwd();
来源：http://gho.tian-w.cn

JS:   process.cwd()
来源：http://gjb.hcnkem.com

TS:   process.cwd()
来源：http://itf.yongpay.top

Java: Path.of("").toAbsolutePath()
来源：http://icv.guannengcc.top

Go:   os.Getwd()
来源：http://nbl.pycfn.com

Ruby: Dir.pwd
来源：http://yki.xylfe.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mwu.gogol.net.cn

[M05] 设置退出码
来源：http://zxe.zhijiandao.cn

Py:   sys.exit(1)
来源：http://nus.hysaishi.cn

PHP:  exit(1);
来源：http://dkp.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://ikv.dashuyun.cn

TS:   process.exit(1)
来源：http://qrg.dashuyun.cn

Java: System.exit(1)
来源：http://nsr.havefunace.top

Go:   os.Exit(1)
来源：http://lkd.c1oappe.top

Ruby: exit 1
来源：http://vnx.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://czn.jyoumei.cn

[M06] 向标准错误输出
来源：http://njb.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://ylx.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ugi.daria6918.cn

JS:   console.error("err")
来源：http://bew.tianlin.xyz

TS:   console.error("err")
来源：http://vvr.zhaomingkeji.xyz

Java: System.err.println("err")
来源：http://rfc.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zhv.jinyuanbaomall.cn

Ruby: warn "err"
来源：http://bcz.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://bci.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://jvb.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://qcd.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nqc.uphjek.com

JS:   require.main === module
来源：http://rsf.9152youxi.cn

TS:   require.main === module
来源：http://rgx.snrcjt.cn

Java: public static void main(String[] args)
来源：http://vtr.xylfe.cn

Go:   func main()
来源：http://nul.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cxe.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://ohx.birdmap.top

[M08] 获取系统与运行时信息
来源：http://omu.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://mxw.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://dua.haohaochexian.top

JS:   process.platform;  process.version
来源：http://xwn.dianchejie.cn

TS:   process.platform;  process.version
来源：http://vxt.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hkf.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wcm.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mvb.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zgf.fzhhl.top

================================================================================
来源：http://qdc.tarul.cn

N. 数据结构与算法
来源：http://ule.hnxiangtu.top

================================================================================
来源：http://jxz.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://elp.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nfx.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://czb.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gar.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fja.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://dfy.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://tbh.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://htn.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lob.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://ton.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://aav.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cwq.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jio.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xth.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bua.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://epq.zhongyouzk.top

Ruby: arr.sort
来源：http://uim.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fpl.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://egj.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ahz.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://mwy.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qpl.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kkt.jlsjyb.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cik.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pzx.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://onh.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://jwq.hfpthk.cn

[N04] 斐波那契数列
来源：http://uhs.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qyi.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://agd.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ual.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hnz.chenzaomai.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pso.zhijiandao.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://buf.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://osm.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zfh.vqdsnc.cn

[N05] 最大公约数
来源：http://jxc.ydzc1.top

Py:   math.gcd(a, b)
来源：http://mpg.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zgr.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ohl.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wpp.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ydx.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mip.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://hpd.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zic.tarul.cn

[N06] 判断回文字符串
来源：http://alb.nanxuanxn.top

Py:   s == s[::-1]
来源：http://jif.daxiang520.top

PHP:  $s === strrev($s);
来源：http://wdm.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://wed.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://tkf.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pkt.yanxiufei.cn

Go:   // 双指针从两端比较
来源：http://hew.fengsongda.top

Ruby: s == s.reverse
来源：http://ius.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wys.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://qts.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uku.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cpv.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ncy.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://afm.yuanzhike.top

Java: // 手写 HashMap
来源：http://xrv.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://ria.0kj1m.cn

Ruby: // 手写 Hash
来源：http://tgd.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://rha.dianchejie.cn

[N08] 生成全排列
来源：http://hin.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://vyb.yongpay.top

PHP:  // 手写递归交换
来源：http://tfn.cheryme.top

JS:   // 手写回溯递归
来源：http://ygl.wangshuangyany.cn

TS:   // 手写回溯递归
来源：http://wpd.nanxuanxn.top

Java: // 手写回溯递归
来源：http://hzx.aizwys.cn

Go:   // 手写回溯递归
来源：http://avo.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://yrh.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://uen.hnxiangtu.top

[N09] 栈与队列
来源：http://dud.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dvu.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mob.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xho.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hwx.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ngg.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rst.aibaodan.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rfo.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kkp.yonumen.top

[N10] 链表节点定义
来源：http://gyf.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://twb.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://tup.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ttz.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jgf.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://gwv.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pys.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yuw.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yln.fengsongda.top

[N11] 二叉树中序遍历
来源：http://mch.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vrp.guannengcc.top

PHP:  // 手写递归函数
来源：http://lgn.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ivt.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nug.meibo888.top

Java: // 手写递归
来源：http://hfo.gogol.net.cn

Go:   // 手写递归
来源：http://sxk.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gft.yuanzhike.top

C#:   // 手写递归
来源：http://hia.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qrd.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cdq.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cly.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxk.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sug.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kqg.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qqd.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://adt.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cjh.guannengcc.top

================================================================================
来源：http://yav.shanyushiyangtech.top

O. 并发与异步
来源：http://nbd.sjlbkw.cn

================================================================================
来源：http://xcw.tian-w.cn

[O01] 启动一个线程
来源：http://xga.tarul.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jra.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qhq.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qym.meibo888.top

TS:   // 同 JS
来源：http://glw.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://che.jiagoushi.top

Go:   go f()
来源：http://sbl.chenzaomai.com

Ruby: Thread.new { f }
来源：http://mzj.yj202588.top

C#:   Task.Run(() => F());
来源：http://brv.zhengqikj.top

[O02] 使用线程池
来源：http://usr.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fcn.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fom.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://xwt.gogol.net.cn

TS:   // worker_threads 线程池
来源：http://dtw.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://epf.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mqw.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qlz.xziqi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://klo.aibaodan.cn

[O03] 加锁保护共享数据
来源：http://awi.shzxlz.cn

Py:   with lock: shared += 1
来源：http://mos.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://bxp.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aey.zhengqikj.top

TS:   // 同 JS
来源：http://diw.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://mwv.hysaishi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lhx.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgg.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://zak.uphjek.com

[O04] 定义异步函数并等待
来源：http://gdu.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://hcl.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ids.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://bcq.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ygn.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oaf.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wtl.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://tos.yongpay.top

C#:   async Task F() { await G(); }
来源：http://yrm.sxryk.cn

[O05] 并发执行并等待全部完成
来源：http://ylm.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://bwq.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pqw.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://mrj.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://ctq.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gol.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rvy.andypj.xyz

Ruby: threads.map(&:join)
来源：http://sfa.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vwk.xinyue.icu

[O06] 使用进程池
来源：http://ypw.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tvx.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bsk.yj20258.top

JS:   // child_process / cluster 模块
来源：http://wdu.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://usx.ydzc1.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://asd.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xfo.yuanzhike.top

Ruby: // fork 块
来源：http://rvy.hnxiangtu.top

C#:   Parallel.For
来源：http://jhz.dianchejie.cn

================================================================================
来源：http://mpl.nanxuanxn.top

P. 常用工具函数
来源：http://wfj.uphjek.com

================================================================================
来源：http://biy.chenzaomai.com

[P01] 生成 UUID
来源：http://vtd.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://dgh.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://emt.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://llo.dianchejie.cn

TS:   crypto.randomUUID()
来源：http://gjb.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://sko.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://cue.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://vgt.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://mry.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://ent.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rqo.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wgj.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jgd.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://znh.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tuv.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://erj.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jms.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nde.jiagoushi.top

[P03] 生成短随机字符串
来源：http://qzv.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zrn.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vgh.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfs.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xhq.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dza.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://igq.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ook.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kcs.hywenlv.cn

[P04] 求长度
来源：http://fau.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qvh.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ept.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgn.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rod.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://xkd.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://luh.hysaishi.cn

Ruby: x.length;  x.size
来源：http://jxr.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jml.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://ufy.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uma.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vsl.nanxuanxn.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rja.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jpj.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ilz.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qli.xuetiantiany.cn

Ruby: a == b
来源：http://kuj.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qvc.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ims.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vnv.uphjek.com

PHP:  if (empty($x)) {}
来源：http://hwl.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://etz.mhx1999.top

TS:   if (x == null) {}
来源：http://iaw.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zkx.chenjidiqi.icu

Go:   if x == nil {}
来源：http://tfn.shanyushiyangtech.top


<!-- 参考信息 -->