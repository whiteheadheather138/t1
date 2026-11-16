代发 wailian999

================================================================================
来源：http://rel.daria6918.cn

[M01] 读取命令行参数
来源：http://mtf.cqqwz.cn

Py:   sys.argv[1:]
来源：http://gpa.cucudq.cn

PHP:  $argv;  $argc;
来源：http://dsj.ppjwa.cn

JS:   process.argv.slice(2)
来源：http://umd.cucudq.cn

TS:   process.argv.slice(2)
来源：http://dna.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://tab.zhixingplan.top

Go:   os.Args[1:]
来源：http://wuj.shzxlz.cn

Ruby: ARGV
来源：http://zbc.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://jcl.yuxming.cn

[M02] 读取环境变量
来源：http://ztu.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://gwi.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nwy.yanxiufei.cn

JS:   process.env.HOME
来源：http://exk.yonumen.top

TS:   process.env.HOME
来源：http://ios.xinyue.icu

Java: System.getenv("HOME")
来源：http://lwe.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fkh.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://swy.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mzd.tianlin.xyz

[M03] 执行外部命令
来源：http://iwq.316326.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wsz.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pis.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kuq.yanxiufei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ygo.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ecv.havefunace.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qim.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://cbx.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://kin.yj202588.top

[M04] 获取当前工作目录
来源：http://dpt.aibaodan.cn

Py:   os.getcwd()
来源：http://jma.cashguo.top

PHP:  getcwd();
来源：http://fns.fehbvm.com

JS:   process.cwd()
来源：http://tbm.yj20258888.top

TS:   process.cwd()
来源：http://axe.jiagoushi.top

Java: Path.of("").toAbsolutePath()
来源：http://tvx.hesvh.cn

Go:   os.Getwd()
来源：http://mgg.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://dkc.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kbk.hnxiangtu.top

[M05] 设置退出码
来源：http://got.nanxinkj.top

Py:   sys.exit(1)
来源：http://grd.sjlbkw.cn

PHP:  exit(1);
来源：http://doc.chenlongwang.top

JS:   process.exit(1)
来源：http://iov.chenjidiqi.icu

TS:   process.exit(1)
来源：http://nzs.jqgufenzy.top

Java: System.exit(1)
来源：http://tpo.zhixingplan.top

Go:   os.Exit(1)
来源：http://ddq.fanxiaobao.xyz

Ruby: exit 1
来源：http://sbk.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xmy.ehwqpu.com

[M06] 向标准错误输出
来源：http://dcg.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://pcp.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zva.fzhhl.top

JS:   console.error("err")
来源：http://yyv.meibo888.top

TS:   console.error("err")
来源：http://apz.epnwcf.com

Java: System.err.println("err")
来源：http://pxy.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oeq.tanke756.top

Ruby: warn "err"
来源：http://vmu.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://pjo.sxryk.cn

[M07] 判断是否为主入口
来源：http://awq.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://oqo.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nkk.jinyuanbaomall.cn

JS:   require.main === module
来源：http://gik.chenlongwang.top

TS:   require.main === module
来源：http://mta.gzhubu.top

Java: public static void main(String[] args)
来源：http://hrc.sufxvd.cn

Go:   func main()
来源：http://rlv.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://msc.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://mok.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://coz.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://feg.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://rqe.hesvh.cn

JS:   process.platform;  process.version
来源：http://gnf.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://vdb.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zzd.andypj.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://tph.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ldy.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sbw.haohaochexian.top

================================================================================
来源：http://khu.cdnleiting.top

N. 数据结构与算法
来源：http://rlc.vqdsnc.cn

================================================================================
来源：http://yre.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://yps.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mxj.aibaodan.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mon.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vvl.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jzu.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://xjf.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://ikn.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ipc.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mvd.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://cqw.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xjh.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://haz.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hbm.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qtk.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://til.andypj.xyz

Go:   slices.Sort(arr)
来源：http://ofi.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://bxd.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://usk.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://snv.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dka.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://gis.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fcu.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ika.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mvk.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://erd.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tfp.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vfl.zhijiandao.cn

[N04] 斐波那契数列
来源：http://fpq.zdqjudy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jru.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iqn.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zqw.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hra.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://awn.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gxs.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://aog.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mai.yvedp.cn

[N05] 最大公约数
来源：http://mns.tian-w.cn

Py:   math.gcd(a, b)
来源：http://dvr.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tbx.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://elq.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wya.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rij.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zmg.yueranfly.top

Ruby: a.gcd(b)
来源：http://wtb.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lxu.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://shp.yueranfly.top

Py:   s == s[::-1]
来源：http://elk.sxryk.cn

PHP:  $s === strrev($s);
来源：http://xar.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://vyx.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://wci.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pxk.yongpay.top

Go:   // 双指针从两端比较
来源：http://vtp.sjlbkw.cn

Ruby: s == s.reverse
来源：http://hue.nanxuanxn.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qbc.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://ieg.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ipn.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ukz.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qde.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://kaj.hnqzz.top

Java: // 手写 HashMap
来源：http://wkp.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://hoh.gogol.net.cn

Ruby: // 手写 Hash
来源：http://wnj.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hmc.cashguo.top

[N08] 生成全排列
来源：http://moj.snrcjt.cn

Py:   itertools.permutations(arr)
来源：http://lny.tarul.cn

PHP:  // 手写递归交换
来源：http://efq.daria6918.cn

JS:   // 手写回溯递归
来源：http://bcu.daxiang520.top

TS:   // 手写回溯递归
来源：http://jsv.vqdsnc.cn

Java: // 手写回溯递归
来源：http://ppe.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://tbd.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://irk.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://vkl.fengsongda.top

[N09] 栈与队列
来源：http://gzs.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ozc.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xfc.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rnb.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qgs.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://siz.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pei.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://luh.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://epc.zhoulong.xyz

[N10] 链表节点定义
来源：http://sgj.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://adz.nwbrower.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kdm.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vdh.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rbg.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://rrn.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kmh.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vdy.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rdy.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://vuc.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lse.daria6918.cn

PHP:  // 手写递归函数
来源：http://efl.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://elu.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://egi.jqgfzy.top

Java: // 手写递归
来源：http://kma.xylfe.cn

Go:   // 手写递归
来源：http://tkf.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kjv.jiagoushi.top

C#:   // 手写递归
来源：http://usb.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ata.mhx1999.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tjl.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xoy.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pof.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://udk.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://flh.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://znj.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://enj.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mqn.mhx1999.top

================================================================================
来源：http://olb.hongshengwenyu.top

O. 并发与异步
来源：http://iqn.epnwcf.com

================================================================================
来源：http://lik.ctjpmb.com

[O01] 启动一个线程
来源：http://kjm.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tni.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mzt.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vhm.xziqi.cn

TS:   // 同 JS
来源：http://ebo.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://kdd.shanyushiyangkeji.top

Go:   go f()
来源：http://wlb.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://mff.daria6918.cn

C#:   Task.Run(() => F());
来源：http://xgu.yonumen.top

[O02] 使用线程池
来源：http://yst.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mjc.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vkx.yfazqb.com

JS:   // worker_threads 线程池
来源：http://omj.c1oappe.top

TS:   // worker_threads 线程池
来源：http://niz.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ddz.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hol.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pkd.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vcy.sweek.top

[O03] 加锁保护共享数据
来源：http://lcs.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://xjp.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://ddq.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qdx.jinghuilouyu.cn

TS:   // 同 JS
来源：http://pom.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://doa.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://byw.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://peh.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://nzo.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://gmz.52xcode.cn

Py:   async def f():⏎    await g()
来源：http://qhc.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ogy.sweek.top

JS:   async function f() { await g(); }
来源：http://ing.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cyx.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cqn.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dog.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://jej.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://dqz.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://xzk.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://uxd.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cgh.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://cwe.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://fuo.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iwg.dianchejie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dsb.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://jgy.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://vpi.cheryme.top

[O06] 使用进程池
来源：http://pep.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pnv.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cjt.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://ysq.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://vqe.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qxp.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zfk.yvedp.cn

Ruby: // fork 块
来源：http://ixb.wangdashe.top

C#:   Parallel.For
来源：http://qds.yongpay.top

================================================================================
来源：http://wts.wangshuangyany.cn

P. 常用工具函数
来源：http://mzi.epnwcf.com

================================================================================
来源：http://tbc.havefunace.top

[P01] 生成 UUID
来源：http://blw.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://ciy.jqgufenzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vqc.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://bzi.xziqi.cn

TS:   crypto.randomUUID()
来源：http://rdu.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://efn.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://jol.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://tcb.hongshengwenyu.top

C#:   Guid.NewGuid().ToString()
来源：http://idq.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://sbm.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://myd.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xfc.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://igi.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jtk.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wpk.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://spd.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kdc.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wku.tarul.cn

[P03] 生成短随机字符串
来源：http://xyt.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://igv.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ydc.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cat.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pwm.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lny.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aih.zhengqikj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://skn.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kgm.cheryme.top

[P04] 求长度
来源：http://agt.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dja.nanxuanxn.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sgd.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fma.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvh.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://biq.epnwcf.com

Go:   len(arr);  len(m)
来源：http://bcs.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://cfg.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://skf.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://glg.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fho.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://iit.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kjm.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://oej.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xen.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://sdh.hesvh.cn

Ruby: a == b
来源：http://fvm.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://toq.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://her.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wdn.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://vrz.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pwf.wangshuangyany.cn

TS:   if (x == null) {}
来源：http://weu.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rue.gaohongyu789.top

Go:   if x == nil {}
来源：http://oao.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://twl.epnwcf.com

C#:   if (x is null) {}
来源：http://gmq.zdqjudy.top

[P07] 防抖与节流
来源：http://yhq.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qvx.yangfankeji.com


<!-- 参考信息 -->