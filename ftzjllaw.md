代发 wailian999

================================================================================
来源：http://nwb.chenzaomai.com

[M01] 读取命令行参数
来源：http://cch.hnqzz.top

Py:   sys.argv[1:]
来源：http://dhu.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://ime.epnwcf.com

JS:   process.argv.slice(2)
来源：http://zzg.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://pze.yongpay.top

Java: args 数组（main 方法参数）
来源：http://gud.jiagoushi.top

Go:   os.Args[1:]
来源：http://ecl.tian-w.cn

Ruby: ARGV
来源：http://yoa.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://hak.uphjek.com

[M02] 读取环境变量
来源：http://tmy.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://iiu.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ofj.ybcxt.top

JS:   process.env.HOME
来源：http://unz.jlsjyb.cn

TS:   process.env.HOME
来源：http://gkn.jyoumei.cn

Java: System.getenv("HOME")
来源：http://cho.cdnleiting.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lda.xylfe.cn

Ruby: ENV["HOME"]
来源：http://mvt.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oda.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://zbm.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dhn.tarul.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mau.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bub.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jny.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://whr.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qex.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://afo.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://iks.dashuyun.cn

[M04] 获取当前工作目录
来源：http://rlf.haohaochexian.top

Py:   os.getcwd()
来源：http://pag.wangshuangyany.cn

PHP:  getcwd();
来源：http://pdp.guannengcc.top

JS:   process.cwd()
来源：http://qgh.yangfankeji.com

TS:   process.cwd()
来源：http://blp.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://hal.yfazqb.com

Go:   os.Getwd()
来源：http://thf.yj202588.top

Ruby: Dir.pwd
来源：http://xjd.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://lvc.shanyushiyangkeji.top

[M05] 设置退出码
来源：http://nuq.ppjwa.cn

Py:   sys.exit(1)
来源：http://lbn.shangyingyoupin.top

PHP:  exit(1);
来源：http://lim.jianghu66.top

JS:   process.exit(1)
来源：http://syo.meibo888.top

TS:   process.exit(1)
来源：http://npm.xinyue.icu

Java: System.exit(1)
来源：http://jus.yonumen.top

Go:   os.Exit(1)
来源：http://ylo.nwbrower.top

Ruby: exit 1
来源：http://etf.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cbo.vehdjk.com

[M06] 向标准错误输出
来源：http://lmi.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://ski.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mmx.gotoacloud.top

JS:   console.error("err")
来源：http://jof.gaohongyu789.top

TS:   console.error("err")
来源：http://lvu.mhx1999.top

Java: System.err.println("err")
来源：http://yju.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gcv.fehbvm.com

Ruby: warn "err"
来源：http://xiq.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://lsk.gzhubu.top

[M07] 判断是否为主入口
来源：http://sll.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://ylh.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://krj.xylfe.cn

JS:   require.main === module
来源：http://rvr.daria6918.cn

TS:   require.main === module
来源：http://tzo.smart0.xyz

Java: public static void main(String[] args)
来源：http://rdi.zhaomingkeji.xyz

Go:   func main()
来源：http://zpg.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://amj.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://gpn.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://dna.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://ujp.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://yll.c1oappe.top

JS:   process.platform;  process.version
来源：http://gpc.dianchejie.cn

TS:   process.platform;  process.version
来源：http://jqt.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zgk.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jse.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpt.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rgy.zhijiandao.cn

================================================================================
来源：http://oht.yongpay.top

N. 数据结构与算法
来源：http://lrf.ctjpmb.com

================================================================================
来源：http://xko.meibo888.top

[N01] 二分查找（有序数组）
来源：http://hqe.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://szo.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tuj.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sha.yj20258888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxy.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://vkn.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://eix.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mft.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://rss.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://srq.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://qrq.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gzw.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jno.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yny.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gfc.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://ylm.cucudq.cn

Ruby: arr.sort
来源：http://zys.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jlo.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://kkq.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uip.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://whl.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wae.hammf.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qaf.andypj.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sug.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://avz.ybcxt.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qsz.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nxs.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://rtk.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://axh.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sea.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lpc.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ttq.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mez.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://doo.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yia.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://box.quarkkingdee.top

[N05] 最大公约数
来源：http://odp.52xcode.cn

Py:   math.gcd(a, b)
来源：http://wnf.haohaochexian.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ibp.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ktc.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gww.cucudq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://giu.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qef.hammf.cn

Ruby: a.gcd(b)
来源：http://kfd.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://prw.hesvh.cn

[N06] 判断回文字符串
来源：http://nop.cucudq.cn

Py:   s == s[::-1]
来源：http://dsg.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://krk.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://vyo.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://ied.hnxiangtu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://drd.hammf.cn

Go:   // 双指针从两端比较
来源：http://ryd.cqqwz.cn

Ruby: s == s.reverse
来源：http://mmi.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cxi.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://lus.shuidangran.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vxz.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wtp.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://krs.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://fyk.dianchejie.cn

Java: // 手写 HashMap
来源：http://txc.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://aom.aizwys.cn

Ruby: // 手写 Hash
来源：http://nzj.gogol.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kvk.vqdsnc.cn

[N08] 生成全排列
来源：http://jvf.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://dly.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://kht.chenzaomai.com

JS:   // 手写回溯递归
来源：http://gor.cdnleiting.top

TS:   // 手写回溯递归
来源：http://rfv.52xcode.cn

Java: // 手写回溯递归
来源：http://txx.guannengcc.top

Go:   // 手写回溯递归
来源：http://ycl.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://lcy.jyoumei.cn

C#:   // 手写回溯递归
来源：http://eqv.snrcjt.cn

[N09] 栈与队列
来源：http://bpw.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mtd.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fly.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jdb.zhaomingkeji.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dci.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fqf.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xty.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tqp.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rig.zdqjudy.top

[N10] 链表节点定义
来源：http://dhe.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sck.xingfuxueyuan.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://nxu.jianghu66.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qdy.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cvi.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://mal.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://nau.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bqr.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pox.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://pmo.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://njp.zhixingplan.top

PHP:  // 手写递归函数
来源：http://fxm.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mgw.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uzb.tanke756.top

Java: // 手写递归
来源：http://jiq.wangdashe.top

Go:   // 手写递归
来源：http://xxd.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hvb.guowangkeji.top

C#:   // 手写递归
来源：http://qvi.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xhc.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xmi.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gzy.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgh.smart0.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fol.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jbs.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsf.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gza.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ygo.fktsv.cn

================================================================================
来源：http://eoa.hywenlv.cn

O. 并发与异步
来源：http://acf.aibaodan.cn

================================================================================
来源：http://qjo.birdmap.top

[O01] 启动一个线程
来源：http://ynb.jqgufenzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ptz.yvedp.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vvv.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gqz.shuidangran.top

TS:   // 同 JS
来源：http://nmh.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://gus.havefunace.top

Go:   go f()
来源：http://ozp.pycfn.com

Ruby: Thread.new { f }
来源：http://eza.aizwys.cn

C#:   Task.Run(() => F());
来源：http://ewo.hongshengwenyu.top

[O02] 使用线程池
来源：http://gnw.kuanghao11.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ovv.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ufc.ybcxt.top

JS:   // worker_threads 线程池
来源：http://vcz.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://uza.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://osu.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://czy.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://umg.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fxm.mhx1999.top

[O03] 加锁保护共享数据
来源：http://rre.xuanzx.com

Py:   with lock: shared += 1
来源：http://yzv.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://ysc.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cjw.yj20258.top

TS:   // 同 JS
来源：http://lvn.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://ksp.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zyf.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://goz.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://lfa.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://win.hfpthk.cn

Py:   async def f():⏎    await g()
来源：http://bxy.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hhv.fehbvm.com

JS:   async function f() { await g(); }
来源：http://vsh.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ave.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vey.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wei.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://vlh.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://hhs.hfpthk.cn

[O05] 并发执行并等待全部完成
来源：http://fkl.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://dxg.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nre.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://djp.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://vnv.ydjk.org.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://emi.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kkx.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://igw.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ybl.haohaochexian.top

[O06] 使用进程池
来源：http://akp.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kud.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gfo.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://fmg.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://jsj.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lze.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wxs.zhoulong.xyz

Ruby: // fork 块
来源：http://vjg.tianlin.xyz

C#:   Parallel.For
来源：http://ypn.hcnkem.com

================================================================================
来源：http://rrg.ivvv.top

P. 常用工具函数
来源：http://ayn.jiagoushi.top

================================================================================
来源：http://yqp.uphjek.com

[P01] 生成 UUID
来源：http://dtk.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://ynl.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lqy.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://kaa.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://wfc.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://plq.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://kmz.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://jtl.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://oml.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://jfn.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cpd.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lqe.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://crq.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://znh.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mmb.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bbs.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ctd.jyoumei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vur.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://sgj.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://auy.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cgc.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhn.zdbjq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kel.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cuk.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lzj.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://fat.cqqwz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dvd.c1oappe.top

[P04] 求长度
来源：http://lgl.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vzu.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bde.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://znq.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dgk.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://pza.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://kpi.jqgfzy.top

Ruby: x.length;  x.size
来源：http://azq.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gmi.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://iho.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xxm.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sqh.havefunace.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://scx.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mdj.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gjk.hnxiangtu.top

Go:   reflect.DeepEqual(a, b)
来源：http://uet.fanxiaobao.xyz

Ruby: a == b
来源：http://qgj.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dkd.ppjwa.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ayn.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mmw.yj20258.top

PHP:  if (empty($x)) {}
来源：http://lrs.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cfv.ivvv.top

TS:   if (x == null) {}
来源：http://kzf.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ewc.zhoulong.xyz

Go:   if x == nil {}
来源：http://hds.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lrz.yueranfly.top

C#:   if (x is null) {}
来源：http://wjc.sweek.top

[P07] 防抖与节流
来源：http://fmk.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xvw.9152youxi.cn


<!-- 参考信息 -->