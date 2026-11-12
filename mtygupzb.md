代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bpn.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sml.zhijiandao.cn

================================================================================
来源：http://awq.redwolf501.top

M. 命令行 / 进程 / 环境
来源：http://ngu.zhengqikj.top

================================================================================
来源：http://lky.daxiang520.top

[M01] 读取命令行参数
来源：http://xpp.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://fkz.hammf.cn

PHP:  $argv;  $argc;
来源：http://xfl.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://vdz.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://oqk.zhoulong.xyz

Java: args 数组（main 方法参数）
来源：http://byl.ydjk.org.cn

Go:   os.Args[1:]
来源：http://qzw.9152youxi.cn

Ruby: ARGV
来源：http://vob.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://mdm.yj20258888.top

[M02] 读取环境变量
来源：http://hvc.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://mno.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pay.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://yht.shuidangran.top

TS:   process.env.HOME
来源：http://omb.hammf.cn

Java: System.getenv("HOME")
来源：http://xnm.sjlbkw.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pwk.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://noe.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://epy.wangdashe.top

[M03] 执行外部命令
来源：http://nff.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qyc.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sns.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iix.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pjg.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://paq.snrcjt.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xhq.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lky.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://rog.cucudq.cn

[M04] 获取当前工作目录
来源：http://shr.xuanzx.com

Py:   os.getcwd()
来源：http://dgc.jqgufenzy.top

PHP:  getcwd();
来源：http://oxc.zdqjudy.top

JS:   process.cwd()
来源：http://wch.epnwcf.com

TS:   process.cwd()
来源：http://vdk.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://plx.aizwys.cn

Go:   os.Getwd()
来源：http://esq.daxiang520.top

Ruby: Dir.pwd
来源：http://gck.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://myi.c1oappe.top

[M05] 设置退出码
来源：http://gud.fehbvm.com

Py:   sys.exit(1)
来源：http://gxv.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://ath.aibaodan.cn

JS:   process.exit(1)
来源：http://dem.yongpay.top

TS:   process.exit(1)
来源：http://yur.xylfe.cn

Java: System.exit(1)
来源：http://mnz.sufxvd.cn

Go:   os.Exit(1)
来源：http://bxj.yfazqb.com

Ruby: exit 1
来源：http://ytc.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aix.pycfn.com

[M06] 向标准错误输出
来源：http://ckq.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://zkn.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sbw.aibaodan.cn

JS:   console.error("err")
来源：http://rnk.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://tnt.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://aye.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nbi.cucudq.cn

Ruby: warn "err"
来源：http://pad.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://yaw.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://reh.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://vhl.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://scl.52xcode.cn

JS:   require.main === module
来源：http://ciu.vehdjk.com

TS:   require.main === module
来源：http://bdr.uphjek.com

Java: public static void main(String[] args)
来源：http://xlj.ydzc1.top

Go:   func main()
来源：http://fgp.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fzh.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://nir.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://mrg.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://slx.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://omw.yuxming.cn

JS:   process.platform;  process.version
来源：http://wsc.vehdjk.com

TS:   process.platform;  process.version
来源：http://zln.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eqs.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mza.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vyq.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mdc.vehdjk.com

================================================================================
来源：http://rol.zhongyouzk.top

N. 数据结构与算法
来源：http://uzs.daria6918.cn

================================================================================
来源：http://fqf.316326.xyz

[N01] 二分查找（有序数组）
来源：http://zwy.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://nct.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://otj.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwb.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cvv.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kxa.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://wzh.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ouk.hnxiangtu.top

C#:   Array.BinarySearch(arr, x)
来源：http://wla.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://ybg.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://hub.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mtk.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pmg.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://eyc.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://djc.bjfxy.top

Go:   slices.Sort(arr)
来源：http://pcb.fzhhl.top

Ruby: arr.sort
来源：http://mui.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yrx.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://wxm.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hnp.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://awa.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uhh.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qeb.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yyf.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dgs.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lyx.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://kct.shuidangran.top

[N04] 斐波那契数列
来源：http://imo.zhongyouzk.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vdg.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bwu.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aef.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mom.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ftn.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kwe.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://msk.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://acc.aizwys.cn

[N05] 最大公约数
来源：http://lqr.yongpay.top

Py:   math.gcd(a, b)
来源：http://omi.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eou.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhn.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ntq.bbcook.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ntv.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vys.dianchejie.cn

Ruby: a.gcd(b)
来源：http://ewj.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wbh.smart0.xyz

[N06] 判断回文字符串
来源：http://pce.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://yww.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://pxu.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://kcn.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://bzl.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://emk.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://qfc.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://sjz.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yok.meibo888.top

[N07] 两数之和（返回下标）
来源：http://kwl.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fah.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://omj.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wwj.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://muj.vehdjk.com

Java: // 手写 HashMap
来源：http://pej.uphjek.com

Go:   // 手写 map[int]int
来源：http://zhw.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://qqh.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://ybn.ydzc1.top

[N08] 生成全排列
来源：http://aum.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://qmd.hnqzz.top

PHP:  // 手写递归交换
来源：http://lne.hcnkem.com

JS:   // 手写回溯递归
来源：http://fdy.yfazqb.com

TS:   // 手写回溯递归
来源：http://gpa.yfazqb.com

Java: // 手写回溯递归
来源：http://nww.guowangkeji.top

Go:   // 手写回溯递归
来源：http://hkj.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://yji.shuidangran.top

C#:   // 手写回溯递归
来源：http://pev.tian-w.cn

[N09] 栈与队列
来源：http://pcg.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jac.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://teh.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zmv.jiagoushi.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mqe.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zac.hesvh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cpq.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hph.ivvv.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xxj.snrcjt.cn

[N10] 链表节点定义
来源：http://bfi.cheryme.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ljc.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ghv.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wqg.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pfe.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://lzd.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://wyy.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://xev.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ndu.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://fyd.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zit.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://itg.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://szo.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aei.zhengqikj.top

Java: // 手写递归
来源：http://xtg.vqdsnc.cn

Go:   // 手写递归
来源：http://bgw.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qmu.sjlbkw.cn

C#:   // 手写递归
来源：http://ana.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xlz.aibaodan.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pqw.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uxx.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://goe.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ovy.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tav.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zbi.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ged.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wwt.xuanzx.com

================================================================================
来源：http://cqa.hnqzz.top

O. 并发与异步
来源：http://vfv.cashguo.top

================================================================================
来源：http://mib.feifeiyinyue.top

[O01] 启动一个线程
来源：http://kcu.hysaishi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://llk.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pon.birdmap.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vbl.aibaodan.cn

TS:   // 同 JS
来源：http://vgb.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://gph.zdqjudy.top

Go:   go f()
来源：http://dwd.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://zat.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://poe.hammf.cn

[O02] 使用线程池
来源：http://uxp.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vyr.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yyw.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://uil.cucudq.cn

TS:   // worker_threads 线程池
来源：http://fvz.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://hte.sysykeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jna.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gdb.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zci.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://ldc.hysaishi.cn

Py:   with lock: shared += 1
来源：http://pzc.gaohongyu789.top

PHP:  // 用 flock() 做文件锁
来源：http://zel.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jfv.cashguo.top

TS:   // 同 JS
来源：http://sqf.bjfxy.top

Java: synchronized (this) { shared++; }
来源：http://lje.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gtc.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://voz.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://drm.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://ggx.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://sng.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tuo.epnwcf.com

JS:   async function f() { await g(); }
来源：http://rpw.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wsg.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dum.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://khq.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://adb.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://gun.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://aef.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://ntk.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xqk.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://cjy.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://iff.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pin.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fad.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://she.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://koj.jinghuilouyu.cn

[O06] 使用进程池
来源：http://dgw.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cyj.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vcm.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://cxe.shanyushiyangtech.top

TS:   // child_process / cluster 模块
来源：http://gwu.aibaodan.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zku.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dgs.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://zzg.shzxlz.cn

C#:   Parallel.For
来源：http://som.tianlin.xyz

================================================================================
来源：http://bcq.hywenlv.cn

P. 常用工具函数
来源：http://mak.mhx1999.top

================================================================================
来源：http://fjd.zhixingplan.top

[P01] 生成 UUID
来源：http://fzs.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://ysk.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vmw.meibo888.top

JS:   crypto.randomUUID()
来源：http://drr.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://lut.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://skw.tian-w.cn

Go:   // 用 github.com/google/uuid
来源：http://evt.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://bwl.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://sej.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://cjp.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ngx.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://iys.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rek.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wgw.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ekl.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hcj.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ycl.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nih.havefunace.top

[P03] 生成短随机字符串
来源：http://zrj.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uxn.cheryme.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://stt.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://paa.jinqigfzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mcc.cucudq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lzf.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nwa.jinyuanbaomall.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rjr.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zop.9152youxi.cn

[P04] 求长度
来源：http://mcr.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sjy.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgb.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ppn.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hlz.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://arc.nwbrower.top

Go:   len(arr);  len(m)
来源：http://jfp.aibaodan.cn

Ruby: x.length;  x.size
来源：http://aov.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bre.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://rrt.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jen.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kao.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lme.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rxn.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pqe.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://mrb.smart0.xyz

Ruby: a == b
来源：http://adc.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sco.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ycm.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iwl.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://lsa.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hxo.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://tvt.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://pvx.sysykeji.top

Go:   if x == nil {}
来源：http://mng.jinyuanbaomall.cn


<!-- 参考信息 -->