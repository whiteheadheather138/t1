代发 wailian999

================================================================================
来源：http://enp.c1oappe.top

[M01] 读取命令行参数
来源：http://grk.cdnleiting.top

Py:   sys.argv[1:]
来源：http://cnz.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://lsf.ivvv.top

JS:   process.argv.slice(2)
来源：http://xfy.ybcxt.top

TS:   process.argv.slice(2)
来源：http://tdn.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://knx.ctjpmb.com

Go:   os.Args[1:]
来源：http://sfm.zhixingplan.top

Ruby: ARGV
来源：http://vxj.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://fon.pengpengdd.cyou

[M02] 读取环境变量
来源：http://zyl.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://zex.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqt.pycfn.com

JS:   process.env.HOME
来源：http://jdy.jlsjyb.cn

TS:   process.env.HOME
来源：http://blx.nanxinkj.top

Java: System.getenv("HOME")
来源：http://ghk.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uck.vehdjk.com

Ruby: ENV["HOME"]
来源：http://jbl.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zlf.uphjek.com

[M03] 执行外部命令
来源：http://pnf.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fiq.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vfz.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dtm.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://imw.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://plg.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://afz.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://zdh.cdnleiting.top

C#:   Process.Start("ls", "-l");
来源：http://lwi.gaohongyu789.top

[M04] 获取当前工作目录
来源：http://son.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://hsa.feifeiyinyue.top

PHP:  getcwd();
来源：http://fvd.gogol.net.cn

JS:   process.cwd()
来源：http://igr.jiagoushi.top

TS:   process.cwd()
来源：http://ssy.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://vqg.gogol.net.cn

Go:   os.Getwd()
来源：http://cgw.yvedp.cn

Ruby: Dir.pwd
来源：http://bth.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yhw.hammf.cn

[M05] 设置退出码
来源：http://svy.zhongyouzk.top

Py:   sys.exit(1)
来源：http://aja.jinghuilouyu.cn

PHP:  exit(1);
来源：http://bso.pengpengdd.cyou

JS:   process.exit(1)
来源：http://qab.smart0.xyz

TS:   process.exit(1)
来源：http://mfa.iojbl.cn

Java: System.exit(1)
来源：http://cvz.tian-w.cn

Go:   os.Exit(1)
来源：http://tvb.yangfankeji.com

Ruby: exit 1
来源：http://okf.pengpengdd.cyou

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qvi.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://hkd.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://uzv.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kra.haohaochexian.top

JS:   console.error("err")
来源：http://fno.shuidangran.top

TS:   console.error("err")
来源：http://dvh.meibo888.top

Java: System.err.println("err")
来源：http://vmm.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rqf.yanxiufei.cn

Ruby: warn "err"
来源：http://egp.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://kyz.aizwys.cn

[M07] 判断是否为主入口
来源：http://krb.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://ufx.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ybt.gotoacloud.top

JS:   require.main === module
来源：http://zbc.fanxiaobao.xyz

TS:   require.main === module
来源：http://iin.hnqzz.top

Java: public static void main(String[] args)
来源：http://xbd.zhixingplan.top

Go:   func main()
来源：http://xae.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jbk.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://ezb.hammf.cn

[M08] 获取系统与运行时信息
来源：http://lpr.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://vmj.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://wkf.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://bfp.uphjek.com

TS:   process.platform;  process.version
来源：http://cyo.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wql.jiagoushi.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lkp.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qbk.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://prn.yj202588.top

================================================================================
来源：http://sey.sufxvd.cn

N. 数据结构与算法
来源：http://fcy.chenjidiqi.icu

================================================================================
来源：http://phk.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://cdn.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xmm.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://shi.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://otj.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://boz.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://ket.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://hfk.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pnn.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://lxq.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://zah.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://jyq.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oap.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dtx.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://syg.sjlbkw.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xxr.sysykeji.top

Go:   slices.Sort(arr)
来源：http://eri.0kj1m.cn

Ruby: arr.sort
来源：http://fer.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nki.havefunace.top

[N03] 快速排序（分治示例）
来源：http://xur.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://llk.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://mgm.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mra.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://khc.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zmc.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lbc.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ndp.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://udj.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://hop.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ovg.yonumen.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sxm.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gqf.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://taa.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fqx.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hkj.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yrf.ydjk.org.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xsy.meibo888.top

[N05] 最大公约数
来源：http://foa.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://ezs.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jbe.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dor.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iov.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://txf.hammf.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nxf.ehwqpu.com

Ruby: a.gcd(b)
来源：http://wdh.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pap.aibaodan.cn

[N06] 判断回文字符串
来源：http://yki.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://bkd.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://feq.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://oft.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://sec.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gbs.epnwcf.com

Go:   // 双指针从两端比较
来源：http://ect.quarkkingdee.top

Ruby: s == s.reverse
来源：http://tdi.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cns.havefunace.top

[N07] 两数之和（返回下标）
来源：http://lzq.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://afx.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ebf.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sfs.yj20258.top

TS:   // 手写 Map<string, number>
来源：http://ayd.cashguo.top

Java: // 手写 HashMap
来源：http://ldm.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://hmc.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://gqt.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sei.xuetiantiany.cn

[N08] 生成全排列
来源：http://sjv.meibo888.top

Py:   itertools.permutations(arr)
来源：http://gsg.cdnleiting.top

PHP:  // 手写递归交换
来源：http://mcb.nanxinkj.top

JS:   // 手写回溯递归
来源：http://hhe.guowangkeji.top

TS:   // 手写回溯递归
来源：http://twz.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://qjk.daria6918.cn

Go:   // 手写回溯递归
来源：http://jgq.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://khw.nanxinkj.top

C#:   // 手写回溯递归
来源：http://pbu.hesvh.cn

[N09] 栈与队列
来源：http://hod.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://quz.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rau.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://syg.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pks.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bli.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bwx.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sjw.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dek.xuetiantiany.cn

[N10] 链表节点定义
来源：http://gxo.pycfn.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ktf.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sho.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fby.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sia.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://idl.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://etk.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yeh.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pvp.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://wrz.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xea.zdbjq.cn

PHP:  // 手写递归函数
来源：http://vzy.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kwe.xinyue.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfl.mhx1999.top

Java: // 手写递归
来源：http://gqk.chenzaomai.com

Go:   // 手写递归
来源：http://tel.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://shf.zycfv.cn

C#:   // 手写递归
来源：http://gng.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blc.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://afk.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://apw.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pvf.tian-w.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://czi.316326.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jeq.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nco.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tzl.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hhf.sxryk.cn

================================================================================
来源：http://ivm.zhongyouzk.top

O. 并发与异步
来源：http://uhs.zycfv.cn

================================================================================
来源：http://zxi.kuanghao11.cn

[O01] 启动一个线程
来源：http://uwp.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gtd.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://whk.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bbb.ppjwa.cn

TS:   // 同 JS
来源：http://ccz.hnqzz.top

Java: new Thread(() -> f()).start()
来源：http://ntm.yuanzhike.top

Go:   go f()
来源：http://ymi.birdmap.top

Ruby: Thread.new { f }
来源：http://dba.zycfv.cn

C#:   Task.Run(() => F());
来源：http://flq.zycfv.cn

[O02] 使用线程池
来源：http://pmr.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rns.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qtk.jlsjyb.cn

JS:   // worker_threads 线程池
来源：http://dai.snrcjt.cn

TS:   // worker_threads 线程池
来源：http://vjm.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://zyv.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mal.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pey.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hbo.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://dib.jiagoushi.top

Py:   with lock: shared += 1
来源：http://ucu.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://eet.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qtb.fanxiaobao.xyz

TS:   // 同 JS
来源：http://kej.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://vnw.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jcv.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cbq.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://elt.bjfxy.top

[O04] 定义异步函数并等待
来源：http://ubh.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://hjd.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dth.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://mtl.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kbc.tian-w.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jsm.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zko.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nyk.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://ort.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://vkk.zhengqikj.top

Py:   asyncio.gather(*tasks)
来源：http://ycp.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cxm.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://iid.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://bew.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://saj.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ijv.yuxming.cn

Ruby: threads.map(&:join)
来源：http://cel.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://pda.ivvv.top

[O06] 使用进程池
来源：http://gyk.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ggb.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nfb.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://bho.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://emr.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gre.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xli.yanxiufei.cn

Ruby: // fork 块
来源：http://bte.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://rsf.ydjk.org.cn

================================================================================
来源：http://ujn.cucudq.cn

P. 常用工具函数
来源：http://kcr.zdbjq.cn

================================================================================
来源：http://jjw.52xcode.cn

[P01] 生成 UUID
来源：http://iwp.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://wdp.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xce.xylfe.cn

JS:   crypto.randomUUID()
来源：http://zit.fengsongda.top

TS:   crypto.randomUUID()
来源：http://cbe.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://pck.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ycn.cdnleiting.top

Ruby: SecureRandom.uuid
来源：http://dro.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://bar.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://jzm.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://klv.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://llp.svipenyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ujr.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tcq.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oun.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gyt.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qft.svipenyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nli.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://jng.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ehj.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hhf.ybcxt.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ojr.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wyw.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yll.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ifh.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lsm.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://omg.tarul.cn

[P04] 求长度
来源：http://nnc.jqgfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lyo.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zks.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rod.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mye.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://ofs.nanxuanxn.top

Go:   len(arr);  len(m)
来源：http://cmi.ehwqpu.com

Ruby: x.length;  x.size
来源：http://flf.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xli.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://zum.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mtd.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ucp.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jjx.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://myu.yonumen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bci.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://ykq.gogol.net.cn

Ruby: a == b
来源：http://pkk.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jyo.yueranfly.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bzm.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://utx.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://ckd.ppjwa.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ozf.9152youxi.cn

TS:   if (x == null) {}
来源：http://uen.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://xym.316326.xyz

Go:   if x == nil {}
来源：http://oqa.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ncf.zdbjq.cn

C#:   if (x is null) {}
来源：http://wdh.vqdsnc.cn

[P07] 防抖与节流
来源：http://djx.cheryme.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eww.hongshengwenyu.top


<!-- 参考信息 -->