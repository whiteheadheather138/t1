代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pqh.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jub.dashuyun.cn

================================================================================
来源：http://zdh.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://ebi.andypj.xyz

================================================================================
来源：http://bhd.aibaodan.cn

[M01] 读取命令行参数
来源：http://tuj.mhx1999.top

Py:   sys.argv[1:]
来源：http://krt.tian-w.cn

PHP:  $argv;  $argc;
来源：http://lfr.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://loe.smart0.xyz

TS:   process.argv.slice(2)
来源：http://amg.sxryk.cn

Java: args 数组（main 方法参数）
来源：http://olr.shuidangran.top

Go:   os.Args[1:]
来源：http://erw.hesvh.cn

Ruby: ARGV
来源：http://oia.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://cxr.haohaochexian.top

[M02] 读取环境变量
来源：http://zje.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://ovt.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nva.gotoacloud.top

JS:   process.env.HOME
来源：http://zxi.fehbvm.com

TS:   process.env.HOME
来源：http://ppt.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://mwh.bjfxy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gar.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://crr.vehdjk.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fpo.dianchejie.cn

[M03] 执行外部命令
来源：http://giq.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rbd.shanyushiyangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ihp.wangshuangyany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oxq.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://iaw.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aeg.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jiu.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://kty.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://zbo.pycfn.com

[M04] 获取当前工作目录
来源：http://dpf.birdmap.top

Py:   os.getcwd()
来源：http://nwm.ctjpmb.com

PHP:  getcwd();
来源：http://kwk.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://iel.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://pbk.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://cxq.xinyue.icu

Go:   os.Getwd()
来源：http://mrj.gotoacloud.top

Ruby: Dir.pwd
来源：http://xhg.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://jxs.hcnkem.com

[M05] 设置退出码
来源：http://pcw.cheryme.top

Py:   sys.exit(1)
来源：http://hbs.meibo888.top

PHP:  exit(1);
来源：http://dwm.daxiang520.top

JS:   process.exit(1)
来源：http://nof.vehdjk.com

TS:   process.exit(1)
来源：http://clu.zycfv.cn

Java: System.exit(1)
来源：http://vvy.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://gqx.zdqjudy.top

Ruby: exit 1
来源：http://fni.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dpp.sysykeji.top

[M06] 向标准错误输出
来源：http://mzo.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://wyv.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tao.wangdashe.top

JS:   console.error("err")
来源：http://nnq.shanyushiyangtech.top

TS:   console.error("err")
来源：http://brj.ydzc1.top

Java: System.err.println("err")
来源：http://efq.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xgl.andypj.xyz

Ruby: warn "err"
来源：http://vtl.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://yei.chenjidiqi.icu

[M07] 判断是否为主入口
来源：http://tkb.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://yeq.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nkb.uphjek.com

JS:   require.main === module
来源：http://qxt.vqdsnc.cn

TS:   require.main === module
来源：http://vtm.yfazqb.com

Java: public static void main(String[] args)
来源：http://ajz.redwolf501.top

Go:   func main()
来源：http://rke.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://meq.yj20258888.top

C#:   static void Main(string[] args)
来源：http://cxd.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://hju.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://yxn.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://bws.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://rlo.zhengqikj.top

TS:   process.platform;  process.version
来源：http://ahb.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oox.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://vka.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vwe.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ovo.hongshengwenyu.top

================================================================================
来源：http://dkx.zhengqikj.top

N. 数据结构与算法
来源：http://kqf.hesvh.cn

================================================================================
来源：http://ztz.ivvv.top

[N01] 二分查找（有序数组）
来源：http://ruw.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://czc.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ayi.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://khi.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iyp.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nou.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://nmy.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfy.mhx1999.top

C#:   Array.BinarySearch(arr, x)
来源：http://rst.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://dgt.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://fii.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hlp.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bnh.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://oet.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sox.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://sij.cucudq.cn

Ruby: arr.sort
来源：http://oog.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mxk.tanke756.top

[N03] 快速排序（分治示例）
来源：http://gdb.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fxf.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://kbw.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rse.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqr.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kob.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gwr.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zkm.zhengqikj.top

C#:   // 手写递归，或 Array.Sort
来源：http://xgx.bbcook.cn

[N04] 斐波那契数列
来源：http://rpm.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vvc.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vlp.jiagoushi.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysg.zycfv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yny.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wit.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fsd.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tak.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gto.fehbvm.com

[N05] 最大公约数
来源：http://xog.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://uwd.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wep.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ghh.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mai.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lmc.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ycp.epnwcf.com

Ruby: a.gcd(b)
来源：http://itw.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xot.cashguo.top

[N06] 判断回文字符串
来源：http://zfq.sufxvd.cn

Py:   s == s[::-1]
来源：http://yls.xinyue.icu

PHP:  $s === strrev($s);
来源：http://nax.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://gjj.epnwcf.com

TS:   s === [...s].reverse().join("")
来源：http://xvj.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hda.yongpay.top

Go:   // 双指针从两端比较
来源：http://jsz.yongpay.top

Ruby: s == s.reverse
来源：http://bdd.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://abm.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://msv.quarkkingdee.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nqx.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dxn.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qit.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://brl.jiagoushi.top

Java: // 手写 HashMap
来源：http://wqb.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://hot.hammf.cn

Ruby: // 手写 Hash
来源：http://umo.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xqu.jinqigufen.top

[N08] 生成全排列
来源：http://smm.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://llq.yongpay.top

PHP:  // 手写递归交换
来源：http://wap.havefunace.top

JS:   // 手写回溯递归
来源：http://tlm.ppjwa.cn

TS:   // 手写回溯递归
来源：http://nbv.316326.xyz

Java: // 手写回溯递归
来源：http://pat.9152youxi.cn

Go:   // 手写回溯递归
来源：http://qnj.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://rkp.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://sbx.chenlongwang.top

[N09] 栈与队列
来源：http://fwt.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://izl.sxryk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zzh.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://spc.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ofr.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cri.chenlongwang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qjc.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fae.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qvn.jqgfzy.top

[N10] 链表节点定义
来源：http://acm.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hkj.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ddc.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rwu.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zua.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://eoa.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hag.wangshuangyany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nuw.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xkc.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://vph.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kbb.yfazqb.com

PHP:  // 手写递归函数
来源：http://lbx.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://njb.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zls.ehwqpu.com

Java: // 手写递归
来源：http://spc.uphjek.com

Go:   // 手写递归
来源：http://ujk.sufxvd.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qaw.shangyingyoupin.top

C#:   // 手写递归
来源：http://tcq.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://joz.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://njc.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ifm.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjb.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tjb.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rkz.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fne.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tyn.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zsm.jianghu66.top

================================================================================
来源：http://bpj.zdqjudy.top

O. 并发与异步
来源：http://aed.pycfn.com

================================================================================
来源：http://ape.snrcjt.cn

[O01] 启动一个线程
来源：http://hdl.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ozq.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hsr.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://azn.aibaodan.cn

TS:   // 同 JS
来源：http://kwk.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://fts.fzhhl.top

Go:   go f()
来源：http://lvc.xuanzx.com

Ruby: Thread.new { f }
来源：http://yoz.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://gtt.yfazqb.com

[O02] 使用线程池
来源：http://eqc.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qed.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fqf.birdmap.top

JS:   // worker_threads 线程池
来源：http://ejw.gzhubu.top

TS:   // worker_threads 线程池
来源：http://ile.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xsa.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://obb.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pcu.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://veh.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://etw.svipenyu.cn

Py:   with lock: shared += 1
来源：http://odq.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://zdj.sysykeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nam.hnqzz.top

TS:   // 同 JS
来源：http://cdd.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://hub.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://aoa.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://qbk.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://xuq.bbcook.cn

[O04] 定义异步函数并等待
来源：http://ffe.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://iyq.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cuv.cheryme.top

JS:   async function f() { await g(); }
来源：http://rpf.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://nbw.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mre.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bbm.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://pib.gogol.net.cn

C#:   async Task F() { await G(); }
来源：http://uap.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://vvf.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://kpx.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jju.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://lgw.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://fdj.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ohf.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyo.sweek.top

Ruby: threads.map(&:join)
来源：http://jxa.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pve.cheryme.top

[O06] 使用进程池
来源：http://aav.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ytv.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pyy.meibo888.top

JS:   // child_process / cluster 模块
来源：http://vgb.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://zbf.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mhf.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gxm.cashguo.top

Ruby: // fork 块
来源：http://xyf.0kj1m.cn

C#:   Parallel.For
来源：http://orw.cqqwz.cn

================================================================================
来源：http://ysh.redwolf501.top

P. 常用工具函数
来源：http://tuj.redwolf501.top

================================================================================
来源：http://qhi.shzxlz.cn

[P01] 生成 UUID
来源：http://oxo.ctjpmb.com

Py:   str(uuid.uuid4())
来源：http://zzc.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://svq.andypj.xyz

JS:   crypto.randomUUID()
来源：http://rhj.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://kqw.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://jey.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://jyk.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://zlr.sjlbkw.cn

C#:   Guid.NewGuid().ToString()
来源：http://ook.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://aok.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xtu.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zca.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kig.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jlv.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fzk.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wnb.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qhc.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://egr.uphjek.com

[P03] 生成短随机字符串
来源：http://lbj.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vki.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xqi.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://was.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gmn.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jvv.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://osg.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wlg.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hrd.meibo888.top

[P04] 求长度
来源：http://xto.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://owq.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzr.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://llw.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bbj.daxiang520.top

Java: list.size();  map.size();  s.length()
来源：http://wwa.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://eni.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://hql.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tab.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://vev.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ylx.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ljm.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bth.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uzk.jiagoushi.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://prx.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://ycb.xziqi.cn

Ruby: a == b
来源：http://igu.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mee.pycfn.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vac.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oid.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://koy.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hhl.shzxlz.cn

TS:   if (x == null) {}
来源：http://wlp.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://huh.jlsjyb.cn

Go:   if x == nil {}
来源：http://hzp.xinyue.icu


<!-- 参考信息 -->