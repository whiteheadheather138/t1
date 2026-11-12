代发 wailian999

================================================================================
来源：http://occ.gzhubu.top

[M01] 读取命令行参数
来源：http://lot.shuidangran.top

Py:   sys.argv[1:]
来源：http://tcq.havefunace.top

PHP:  $argv;  $argc;
来源：http://uvq.yuxming.cn

JS:   process.argv.slice(2)
来源：http://jvr.hesvh.cn

TS:   process.argv.slice(2)
来源：http://jco.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://gsp.fengsongda.top

Go:   os.Args[1:]
来源：http://oex.dashuyun.cn

Ruby: ARGV
来源：http://zre.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://swv.jiagoushi.top

[M02] 读取环境变量
来源：http://dtw.redwolf501.top

Py:   os.environ.get("HOME")
来源：http://ixk.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qdb.guannengcc.top

JS:   process.env.HOME
来源：http://zpd.nwbrower.top

TS:   process.env.HOME
来源：http://qib.aizwys.cn

Java: System.getenv("HOME")
来源：http://zfh.aibaodan.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://otv.xuanzx.com

Ruby: ENV["HOME"]
来源：http://yhe.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://peg.tianlin.xyz

[M03] 执行外部命令
来源：http://thn.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wkf.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dej.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://isc.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oqe.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://asm.gzhubu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cnm.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dcg.feifeiyinyue.top

C#:   Process.Start("ls", "-l");
来源：http://ltl.andypj.xyz

[M04] 获取当前工作目录
来源：http://ovs.smart0.xyz

Py:   os.getcwd()
来源：http://kei.jinqigfzy.top

PHP:  getcwd();
来源：http://wpm.ydzc1.top

JS:   process.cwd()
来源：http://neh.52xcode.cn

TS:   process.cwd()
来源：http://egr.cdnleiting.top

Java: Path.of("").toAbsolutePath()
来源：http://zzw.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://dac.fzhhl.top

Ruby: Dir.pwd
来源：http://lna.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://ljh.hcnkem.com

[M05] 设置退出码
来源：http://mzd.nanxuanxn.top

Py:   sys.exit(1)
来源：http://rle.tarul.cn

PHP:  exit(1);
来源：http://kzq.shzxlz.cn

JS:   process.exit(1)
来源：http://lgj.chenzaomai.com

TS:   process.exit(1)
来源：http://qvh.sweek.top

Java: System.exit(1)
来源：http://ypf.dashuyun.cn

Go:   os.Exit(1)
来源：http://inh.hnqzz.top

Ruby: exit 1
来源：http://zyq.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://prj.hcnkem.com

[M06] 向标准错误输出
来源：http://ehm.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://btn.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://aqu.yonumen.top

JS:   console.error("err")
来源：http://jnf.nwbrower.top

TS:   console.error("err")
来源：http://bbk.shuidangran.top

Java: System.err.println("err")
来源：http://nlf.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uqx.gogol.net.cn

Ruby: warn "err"
来源：http://ire.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://mlm.aibaodan.cn

[M07] 判断是否为主入口
来源：http://gwx.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://emw.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dqo.cheryme.top

JS:   require.main === module
来源：http://cgi.hesvh.cn

TS:   require.main === module
来源：http://dsb.hywenlv.cn

Java: public static void main(String[] args)
来源：http://hkz.nanxinkj.top

Go:   func main()
来源：http://wtr.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bvh.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://car.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://jxi.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://coh.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://rsm.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://bet.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://enc.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mdo.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wgu.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rzz.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ead.snrcjt.cn

================================================================================
来源：http://ycn.cheryme.top

N. 数据结构与算法
来源：http://ctu.mhx1999.top

================================================================================
来源：http://mse.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://zge.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ovy.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fif.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nwf.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qje.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rek.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://iri.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://swv.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tri.quarkkingdee.top

[N02] 排序（工程实践用内置实现）
来源：http://lok.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://efr.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iaq.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zyn.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cog.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ywf.smart0.xyz

Go:   slices.Sort(arr)
来源：http://dlc.ctjpmb.com

Ruby: arr.sort
来源：http://aaf.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qwf.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://mdg.tanke756.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://exh.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://zgz.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uki.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rfl.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ovm.9152youxi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://emz.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xob.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://myb.ctjpmb.com

[N04] 斐波那契数列
来源：http://yef.xinyue.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://csx.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ybs.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mdz.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vib.yangfankeji.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wgn.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oug.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xlf.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pez.kuanghao11.cn

[N05] 最大公约数
来源：http://pvm.sysykeji.top

Py:   math.gcd(a, b)
来源：http://vpe.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ghu.hongshengwenyu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://agz.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qgo.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cei.zhengqikj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hqv.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://ltf.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://crm.kuanghao11.cn

[N06] 判断回文字符串
来源：http://pno.cqqwz.cn

Py:   s == s[::-1]
来源：http://hll.sweek.top

PHP:  $s === strrev($s);
来源：http://lwz.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://hlq.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://iqe.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zio.shuidangran.top

Go:   // 双指针从两端比较
来源：http://pxb.sxryk.cn

Ruby: s == s.reverse
来源：http://unr.hongshengwenyu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uau.zhoulong.xyz

[N07] 两数之和（返回下标）
来源：http://hmz.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bow.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ulq.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ali.sufxvd.cn

TS:   // 手写 Map<string, number>
来源：http://cyn.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://xem.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://tra.yongpay.top

Ruby: // 手写 Hash
来源：http://cte.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://mkt.pycfn.com

[N08] 生成全排列
来源：http://has.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://zwt.xuanzx.com

PHP:  // 手写递归交换
来源：http://yrp.svipenyu.cn

JS:   // 手写回溯递归
来源：http://amr.yvedp.cn

TS:   // 手写回溯递归
来源：http://jkj.vqdsnc.cn

Java: // 手写回溯递归
来源：http://ysw.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://sgs.birdmap.top

Ruby: arr.permutation.to_a
来源：http://aeo.sufxvd.cn

C#:   // 手写回溯递归
来源：http://fiu.ybcxt.top

[N09] 栈与队列
来源：http://ohq.jinghuilouyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qfh.meibo888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://alq.yuxming.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wrb.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bui.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ukt.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zpp.pycfn.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://euv.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mda.wangdashe.top

[N10] 链表节点定义
来源：http://kdq.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://drq.mhx1999.top

PHP:  class Node { public $v; public $next = null; }
来源：http://amc.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xww.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://taf.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://gnd.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://lwr.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://lcd.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://asp.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://ezu.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wnw.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://iov.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ixp.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dph.shzxlz.cn

Java: // 手写递归
来源：http://eyb.gotoacloud.top

Go:   // 手写递归
来源：http://oam.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://elv.yonumen.top

C#:   // 手写递归
来源：http://lgl.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hlo.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://squ.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iwt.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rka.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cmt.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aah.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wmd.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pod.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rqa.shanyushiyangkeji.top

================================================================================
来源：http://xdz.bbcook.cn

O. 并发与异步
来源：http://kgb.aibaodan.cn

================================================================================
来源：http://ajg.shzxlz.cn

[O01] 启动一个线程
来源：http://ycz.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cme.zhijiandao.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jre.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mdo.ydjk.org.cn

TS:   // 同 JS
来源：http://ltc.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://qcx.hnxiangtu.top

Go:   go f()
来源：http://omz.nanxinkj.top

Ruby: Thread.new { f }
来源：http://pzg.gzhubu.top

C#:   Task.Run(() => F());
来源：http://imz.jinqigufen.top

[O02] 使用线程池
来源：http://mqh.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fae.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ksj.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://pts.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://vnf.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://lpr.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aty.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hco.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fsw.cheryme.top

[O03] 加锁保护共享数据
来源：http://dwz.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://wwc.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://ikl.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zui.zdqjudy.top

TS:   // 同 JS
来源：http://uzz.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://fps.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jze.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qzr.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://szu.sweek.top

[O04] 定义异步函数并等待
来源：http://jtv.yj20258.top

Py:   async def f():⏎    await g()
来源：http://hgo.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://niv.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://emi.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://unl.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yjo.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ave.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://kcp.pycfn.com

C#:   async Task F() { await G(); }
来源：http://twl.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://cmx.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://dcx.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jda.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://lch.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://tsh.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yus.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://atx.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://bgl.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gah.zdbjq.cn

[O06] 使用进程池
来源：http://git.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ljl.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://kei.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://qau.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://lrf.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xcq.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://acr.wangshuangyany.cn

Ruby: // fork 块
来源：http://jvt.nanxinkj.top

C#:   Parallel.For
来源：http://fvc.zdqjudy.top

================================================================================
来源：http://prm.ybcxt.top

P. 常用工具函数
来源：http://twu.jlsjyb.cn

================================================================================
来源：http://npq.chenzaomai.com

[P01] 生成 UUID
来源：http://arm.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://aiu.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://atz.yongpay.top

JS:   crypto.randomUUID()
来源：http://pks.uphjek.com

TS:   crypto.randomUUID()
来源：http://jdw.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://cel.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://gjw.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://cec.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://aar.snrcjt.cn

[P02] MD5 / SHA256 摘要
来源：http://lfr.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mmc.chenzaomai.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tag.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hrj.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dbe.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lmk.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hbf.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ubs.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ohs.hywenlv.cn

[P03] 生成短随机字符串
来源：http://kjn.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hkk.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kjh.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zrp.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qbz.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qlk.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xkk.tian-w.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://twp.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bah.jqgufenzy.top

[P04] 求长度
来源：http://qix.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mmc.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nvh.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzj.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://col.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://qil.c1oappe.top

Go:   len(arr);  len(m)
来源：http://yhd.ehwqpu.com

Ruby: x.length;  x.size
来源：http://vgn.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://skc.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://lsp.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://niv.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ekt.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://diz.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jmy.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bkj.cheryme.top

Go:   reflect.DeepEqual(a, b)
来源：http://aha.zhijiandao.cn

Ruby: a == b
来源：http://mrx.zdbjq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jwm.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ocl.chenjidiqi.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yrx.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://ayo.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xms.cheryme.top

TS:   if (x == null) {}
来源：http://vgk.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rty.aibaodan.cn

Go:   if x == nil {}
来源：http://zkr.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wkx.daxiang520.top

C#:   if (x is null) {}
来源：http://xnr.ybcxt.top

[P07] 防抖与节流
来源：http://guo.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://irs.shangyingyoupin.top


<!-- 参考信息 -->