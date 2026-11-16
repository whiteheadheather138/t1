代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://buh.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bup.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zfj.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rhg.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kie.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://izq.gotoacloud.top

================================================================================
来源：http://btu.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://fsn.jqgfzy.top

================================================================================
来源：http://sti.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://jcz.zycfv.cn

Py:   sys.argv[1:]
来源：http://mgq.yj20258.top

PHP:  $argv;  $argc;
来源：http://ikn.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://dce.uphjek.com

TS:   process.argv.slice(2)
来源：http://gid.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://izg.aizwys.cn

Go:   os.Args[1:]
来源：http://vtj.shangyingyoupin.top

Ruby: ARGV
来源：http://dxd.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://azf.pengpengdd.cyou

[M02] 读取环境变量
来源：http://xnb.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://pmg.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jll.fehbvm.com

JS:   process.env.HOME
来源：http://aan.jqgfzy.top

TS:   process.env.HOME
来源：http://xmg.fengsongda.top

Java: System.getenv("HOME")
来源：http://eli.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gzb.bbcook.cn

Ruby: ENV["HOME"]
来源：http://twm.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vxw.aibaodan.cn

[M03] 执行外部命令
来源：http://gue.andypj.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ufx.xylfe.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rjt.sxryk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rke.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jxi.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tiv.feifeiyinyue.top

Go:   exec.Command("ls", "-l").Output()
来源：http://epm.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://cqf.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://yrp.gotoacloud.top

[M04] 获取当前工作目录
来源：http://zdr.guannengcc.top

Py:   os.getcwd()
来源：http://bea.yueranfly.top

PHP:  getcwd();
来源：http://yyk.gaohongyu789.top

JS:   process.cwd()
来源：http://one.yonumen.top

TS:   process.cwd()
来源：http://lkp.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://uvo.xziqi.cn

Go:   os.Getwd()
来源：http://duy.nanxinkj.top

Ruby: Dir.pwd
来源：http://snh.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://pcn.guowangkeji.top

[M05] 设置退出码
来源：http://sck.meibo888.top

Py:   sys.exit(1)
来源：http://feq.cqqwz.cn

PHP:  exit(1);
来源：http://kpq.tarul.cn

JS:   process.exit(1)
来源：http://xxg.yanxiufei.cn

TS:   process.exit(1)
来源：http://ced.52xcode.cn

Java: System.exit(1)
来源：http://iuh.cheryme.top

Go:   os.Exit(1)
来源：http://emk.zhongyouzk.top

Ruby: exit 1
来源：http://iad.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vuy.yuanzhike.top

[M06] 向标准错误输出
来源：http://omv.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://qqf.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vlk.tian-w.cn

JS:   console.error("err")
来源：http://dbg.yueranfly.top

TS:   console.error("err")
来源：http://zrs.xylfe.cn

Java: System.err.println("err")
来源：http://rvm.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://abx.zhijiandao.cn

Ruby: warn "err"
来源：http://yhg.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://yle.cashguo.top

[M07] 判断是否为主入口
来源：http://hlf.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://fhb.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zkg.jiagoushi.top

JS:   require.main === module
来源：http://ayv.chenjidiqi.icu

TS:   require.main === module
来源：http://wsx.gzhubu.top

Java: public static void main(String[] args)
来源：http://uei.hongshengwenyu.top

Go:   func main()
来源：http://vin.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lso.yvedp.cn

C#:   static void Main(string[] args)
来源：http://qkg.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://wpe.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://tse.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://wzw.havefunace.top

JS:   process.platform;  process.version
来源：http://qlo.ctjpmb.com

TS:   process.platform;  process.version
来源：http://nla.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqq.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jlb.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bns.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://mes.bbcook.cn

================================================================================
来源：http://chs.xuetiantiany.cn

N. 数据结构与算法
来源：http://wje.svipenyu.cn

================================================================================
来源：http://apg.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://lor.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://lqg.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yom.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uuf.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rar.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bpx.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://afh.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ctn.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pfg.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://cvt.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://lrq.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nkw.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://alk.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://yyx.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://seo.sysykeji.top

Go:   slices.Sort(arr)
来源：http://ysw.zdbjq.cn

Ruby: arr.sort
来源：http://crd.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dqx.yongpay.top

[N03] 快速排序（分治示例）
来源：http://tbw.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xtl.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://pgc.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rnq.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkc.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qiy.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fpt.yongpay.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zym.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://bej.tian-w.cn

[N04] 斐波那契数列
来源：http://uci.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wwu.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kqu.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dto.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dux.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://txe.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uni.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rny.yj20258888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://unm.smart0.xyz

[N05] 最大公约数
来源：http://vxl.tarul.cn

Py:   math.gcd(a, b)
来源：http://hwp.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vdv.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qny.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qlg.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lqt.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hrw.iojbl.cn

Ruby: a.gcd(b)
来源：http://buo.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hwt.zhijiandao.cn

[N06] 判断回文字符串
来源：http://dyp.cqqwz.cn

Py:   s == s[::-1]
来源：http://zns.tianlin.xyz

PHP:  $s === strrev($s);
来源：http://szc.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://btt.cqqwz.cn

TS:   s === [...s].reverse().join("")
来源：http://fgk.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kht.ydzc1.top

Go:   // 双指针从两端比较
来源：http://aiz.sjlbkw.cn

Ruby: s == s.reverse
来源：http://nbl.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ssl.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://knm.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uba.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://alu.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dhv.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://sjr.mhx1999.top

Java: // 手写 HashMap
来源：http://xoe.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://kqe.shanyushiyangkeji.top

Ruby: // 手写 Hash
来源：http://izi.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://xac.yuanzhike.top

[N08] 生成全排列
来源：http://ecl.yanxiufei.cn

Py:   itertools.permutations(arr)
来源：http://sza.jiagoushi.top

PHP:  // 手写递归交换
来源：http://vpo.jiagoushi.top

JS:   // 手写回溯递归
来源：http://vvb.tianlin.xyz

TS:   // 手写回溯递归
来源：http://zyn.haohaochexian.top

Java: // 手写回溯递归
来源：http://ylh.sufxvd.cn

Go:   // 手写回溯递归
来源：http://lad.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://eja.yuxming.cn

C#:   // 手写回溯递归
来源：http://vwq.aibaodan.cn

[N09] 栈与队列
来源：http://qdj.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fpm.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pns.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tma.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://akn.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://iuy.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cfs.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tmz.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ujv.chenjidiqi.icu

[N10] 链表节点定义
来源：http://rph.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nqr.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zrq.ydzc1.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pja.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pnd.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://eat.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://ayy.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vty.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ieh.epnwcf.com

[N11] 二叉树中序遍历
来源：http://roi.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://egv.zhixingplan.top

PHP:  // 手写递归函数
来源：http://szj.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tta.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jlb.zycfv.cn

Java: // 手写递归
来源：http://ofx.zhixingplan.top

Go:   // 手写递归
来源：http://drt.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://chj.cucudq.cn

C#:   // 手写递归
来源：http://yvq.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tkg.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zbx.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://okq.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vvs.epnwcf.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://spe.yuanzhike.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://amt.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vyo.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zjm.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jcz.cdnleiting.top

================================================================================
来源：http://jyj.yj202588.top

O. 并发与异步
来源：http://ecb.sufxvd.cn

================================================================================
来源：http://pfc.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://lag.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jvl.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bec.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://egz.mhx1999.top

TS:   // 同 JS
来源：http://nnr.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://fez.bbcook.cn

Go:   go f()
来源：http://zvk.fehbvm.com

Ruby: Thread.new { f }
来源：http://huj.tanke756.top

C#:   Task.Run(() => F());
来源：http://wgi.zhijiandao.cn

[O02] 使用线程池
来源：http://sjo.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pjm.cqqwz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fxk.52xcode.cn

JS:   // worker_threads 线程池
来源：http://bdk.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://ajo.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://cib.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ohe.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xuz.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://adl.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://ftb.zhengqikj.top

Py:   with lock: shared += 1
来源：http://yph.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://rku.pengpengdd.cyou

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwb.yj20258.top

TS:   // 同 JS
来源：http://fbf.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://mxu.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yxb.cdnleiting.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kes.zdqjudy.top

C#:   lock (gate) { shared++; }
来源：http://bth.fengsongda.top

[O04] 定义异步函数并等待
来源：http://nda.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://xvg.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fkw.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://gid.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fdd.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xdl.shanyushiyangtech.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rwx.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dur.tarul.cn

C#:   async Task F() { await G(); }
来源：http://jwk.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://igm.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://bqt.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lih.havefunace.top

JS:   await Promise.all(tasks)
来源：http://bai.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://kzp.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://apz.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zvv.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://bdl.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://odq.ivvv.top

[O06] 使用进程池
来源：http://uzc.quarkkingdee.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://csa.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xsg.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://drp.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://rpq.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hgs.zhiwuduotai.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://smo.redwolf501.top

Ruby: // fork 块
来源：http://kkq.fzhhl.top

C#:   Parallel.For
来源：http://acl.0kj1m.cn

================================================================================
来源：http://xwf.wangshuangyany.cn

P. 常用工具函数
来源：http://etb.ydjk.org.cn

================================================================================
来源：http://dpa.cashguo.top

[P01] 生成 UUID
来源：http://bap.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://kvp.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rwj.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://ytx.xziqi.cn

TS:   crypto.randomUUID()
来源：http://kcn.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://ucm.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://xbv.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://qwi.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://mwp.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://ilr.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://edp.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gdb.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vkr.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oif.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mhq.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uyn.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zem.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kfq.jiagoushi.top

[P03] 生成短随机字符串
来源：http://dgq.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rwo.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pxk.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ezf.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obn.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://npo.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://glm.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://idu.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rvc.tarul.cn

[P04] 求长度
来源：http://scs.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vza.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hsg.gotoacloud.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wlv.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxe.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://jfq.hesvh.cn

Go:   len(arr);  len(m)
来源：http://boi.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://ihd.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lyo.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://pdf.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cul.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rwt.feifeiyinyue.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sjd.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://znw.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pof.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xqv.chenlongwang.top

Ruby: a == b
来源：http://qpc.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mqm.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mmi.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://glq.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://nfv.gotoacloud.top


<!-- 参考信息 -->