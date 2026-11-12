代发 wailian999

================================================================================
来源：http://owe.cashguo.top

[M01] 读取命令行参数
来源：http://pxs.gogol.net.cn

Py:   sys.argv[1:]
来源：http://wbz.ywan-chungtsiang.top

PHP:  $argv;  $argc;
来源：http://pbh.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://wfv.daxiang520.top

TS:   process.argv.slice(2)
来源：http://kgs.jqgufenzy.top

Java: args 数组（main 方法参数）
来源：http://ypl.zhoulong.xyz

Go:   os.Args[1:]
来源：http://vyd.hnxiangtu.top

Ruby: ARGV
来源：http://ahn.feifeiyinyue.top

C#:   args 数组（Main 方法参数）
来源：http://nqj.zhengqikj.top

[M02] 读取环境变量
来源：http://usf.ydzc1.top

Py:   os.environ.get("HOME")
来源：http://lad.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dbb.ivvv.top

JS:   process.env.HOME
来源：http://mro.cheryme.top

TS:   process.env.HOME
来源：http://zvs.meibo888.top

Java: System.getenv("HOME")
来源：http://pba.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lrq.316326.xyz

Ruby: ENV["HOME"]
来源：http://orq.haohaochexian.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qkv.daria6918.cn

[M03] 执行外部命令
来源：http://fyx.zhongyouzk.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cwh.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xts.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bap.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://vgq.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dmg.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://rye.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://awn.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://sns.pycfn.com

[M04] 获取当前工作目录
来源：http://sqs.xylfe.cn

Py:   os.getcwd()
来源：http://laq.yvedp.cn

PHP:  getcwd();
来源：http://okz.shzxlz.cn

JS:   process.cwd()
来源：http://klu.gzhubu.top

TS:   process.cwd()
来源：http://qcc.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://vdk.xuetiantiany.cn

Go:   os.Getwd()
来源：http://kib.xinyue.icu

Ruby: Dir.pwd
来源：http://its.sysykeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://sbf.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://zfk.jqgufenzy.top

Py:   sys.exit(1)
来源：http://eqt.jqgufenzy.top

PHP:  exit(1);
来源：http://tog.nanxuanxn.top

JS:   process.exit(1)
来源：http://elt.jlsjyb.cn

TS:   process.exit(1)
来源：http://jjh.hesvh.cn

Java: System.exit(1)
来源：http://wbb.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://gbe.havefunace.top

Ruby: exit 1
来源：http://iwb.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nik.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://xqx.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://euy.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tqc.sufxvd.cn

JS:   console.error("err")
来源：http://elr.daxiang520.top

TS:   console.error("err")
来源：http://ftj.quarkkingdee.top

Java: System.err.println("err")
来源：http://tgj.sjlbkw.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://abz.jiagoushi.top

Ruby: warn "err"
来源：http://yyr.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://qvo.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://ada.uphjek.com

Py:   if __name__ == "__main__":
来源：http://zlg.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cxr.chenzaomai.com

JS:   require.main === module
来源：http://hok.shanyushiyangkeji.top

TS:   require.main === module
来源：http://hkz.bbcook.cn

Java: public static void main(String[] args)
来源：http://gtq.kuanghao11.cn

Go:   func main()
来源：http://etq.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mga.tanke756.top

C#:   static void Main(string[] args)
来源：http://fyh.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://wlt.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://dmq.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://ner.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://vou.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://log.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pxj.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ldg.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eic.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bnt.gotoacloud.top

================================================================================
来源：http://ede.snrcjt.cn

N. 数据结构与算法
来源：http://hqi.andypj.xyz

================================================================================
来源：http://ssf.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://owd.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://wdp.smart0.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mzr.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ikd.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dqz.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://hot.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://ooo.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rkc.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://fpf.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://lec.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://mhl.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wef.daria6918.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fuf.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://klr.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zma.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://ccy.hywenlv.cn

Ruby: arr.sort
来源：http://ele.ppjwa.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nqc.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://kyk.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jov.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://qef.jinghuilouyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xvh.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dah.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gcf.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jqk.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vuw.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dgw.redwolf501.top

[N04] 斐波那契数列
来源：http://hcu.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pgn.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vhc.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qqu.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgm.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://krx.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sgs.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://chb.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://acj.sufxvd.cn

[N05] 最大公约数
来源：http://cwo.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://hla.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yfn.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ngv.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yux.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://quz.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dil.jianghu66.top

Ruby: a.gcd(b)
来源：http://hsy.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cdu.sufxvd.cn

[N06] 判断回文字符串
来源：http://tep.havefunace.top

Py:   s == s[::-1]
来源：http://dka.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://ndf.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://emn.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://jzq.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zax.hesvh.cn

Go:   // 双指针从两端比较
来源：http://lab.snrcjt.cn

Ruby: s == s.reverse
来源：http://qyz.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tyw.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://rnk.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cry.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hts.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zid.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://vix.tian-w.cn

Java: // 手写 HashMap
来源：http://vmj.cashguo.top

Go:   // 手写 map[int]int
来源：http://unf.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://uza.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cfx.havefunace.top

[N08] 生成全排列
来源：http://ejo.316326.xyz

Py:   itertools.permutations(arr)
来源：http://qnf.ctjpmb.com

PHP:  // 手写递归交换
来源：http://jmc.ybcxt.top

JS:   // 手写回溯递归
来源：http://nwj.ehwqpu.com

TS:   // 手写回溯递归
来源：http://hix.cdnleiting.top

Java: // 手写回溯递归
来源：http://mvd.zhiwuduotai.top

Go:   // 手写回溯递归
来源：http://nde.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://uem.cqqwz.cn

C#:   // 手写回溯递归
来源：http://sbp.zhiwuduotai.top

[N09] 栈与队列
来源：http://utc.sxryk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://asd.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oct.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uaj.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aaz.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hxb.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://atk.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sqr.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eaf.yangfankeji.com

[N10] 链表节点定义
来源：http://sed.hfpthk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zjm.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://udq.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xii.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cxt.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://hwv.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://liz.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://uex.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gxv.meibo888.top

[N11] 二叉树中序遍历
来源：http://uwm.jianghu66.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wmi.sxryk.cn

PHP:  // 手写递归函数
来源：http://uzm.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zfu.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cam.wangshuangyany.cn

Java: // 手写递归
来源：http://hax.aibaodan.cn

Go:   // 手写递归
来源：http://dzy.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iic.yangfankeji.com

C#:   // 手写递归
来源：http://ush.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bmk.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wtw.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ykz.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hay.sxryk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vph.mhx1999.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uur.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dfl.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dte.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ufh.jinghuilouyu.cn

================================================================================
来源：http://oye.aibaodan.cn

O. 并发与异步
来源：http://wto.hcnkem.com

================================================================================
来源：http://ijb.tian-w.cn

[O01] 启动一个线程
来源：http://zzd.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rvx.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uyo.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gel.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://msv.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://bzp.gaohongyu789.top

Go:   go f()
来源：http://cxz.shangyingyoupin.top

Ruby: Thread.new { f }
来源：http://ocq.fengsongda.top

C#:   Task.Run(() => F());
来源：http://lww.fktsv.cn

[O02] 使用线程池
来源：http://qxj.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jka.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kqb.epnwcf.com

JS:   // worker_threads 线程池
来源：http://azi.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://hmj.tanke756.top

Java: Executors.newFixedThreadPool(4)
来源：http://whe.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wqj.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jgp.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mvk.xylfe.cn

[O03] 加锁保护共享数据
来源：http://ujl.fengsongda.top

Py:   with lock: shared += 1
来源：http://tuc.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://gbv.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ewy.sysykeji.top

TS:   // 同 JS
来源：http://ndb.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://qbj.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gfs.zycfv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://osk.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://ffu.mhx1999.top

[O04] 定义异步函数并等待
来源：http://wxx.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://bev.jyoumei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eza.ivvv.top

JS:   async function f() { await g(); }
来源：http://sun.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://twh.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xzp.yvedp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rhn.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://lkh.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://nid.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://lct.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://mos.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://avw.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://ins.nwbrower.top

TS:   await Promise.all(tasks)
来源：http://nve.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ggi.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sfv.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://ddc.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pzu.sxryk.cn

[O06] 使用进程池
来源：http://zzz.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lvy.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nhq.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://pjw.yj202588.top

TS:   // child_process / cluster 模块
来源：http://itb.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xnd.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aml.redwolf501.top

Ruby: // fork 块
来源：http://uhn.fengsongda.top

C#:   Parallel.For
来源：http://mcc.yuxming.cn

================================================================================
来源：http://yxi.hcnkem.com

P. 常用工具函数
来源：http://lib.jiagoushi.top

================================================================================
来源：http://dlp.jinqigufen.top

[P01] 生成 UUID
来源：http://cwt.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://gkj.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fka.ppjwa.cn

JS:   crypto.randomUUID()
来源：http://ubp.jqgfzy.top

TS:   crypto.randomUUID()
来源：http://bia.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://ylw.shangyingyoupin.top

Go:   // 用 github.com/google/uuid
来源：http://jxv.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://crb.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://eyp.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://was.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hfy.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkg.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vgg.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yrx.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fyg.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zre.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://txy.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bxw.zhengqikj.top

[P03] 生成短随机字符串
来源：http://lcr.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://htb.gotoacloud.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://has.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://akf.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obb.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eiw.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eep.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gjx.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rvk.xziqi.cn

[P04] 求长度
来源：http://tlz.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zgk.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxj.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxz.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kmz.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://zpn.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://abt.shzxlz.cn

Ruby: x.length;  x.size
来源：http://diq.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pge.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://ige.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eqj.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oyj.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xtb.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fro.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wkt.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cow.hywenlv.cn

Ruby: a == b
来源：http://mzn.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ndq.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tew.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dgv.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://sqh.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vij.vqdsnc.cn

TS:   if (x == null) {}
来源：http://nmw.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://til.52xcode.cn

Go:   if x == nil {}
来源：http://sil.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://duv.redwolf501.top

C#:   if (x is null) {}
来源：http://zke.yanxiufei.cn

[P07] 防抖与节流
来源：http://pkn.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wvm.jqgufenzy.top


<!-- 参考信息 -->