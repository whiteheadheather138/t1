代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tzd.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wrj.wangdashe.top

================================================================================
来源：http://ris.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://ldu.chenlongwang.top

================================================================================
来源：http://eos.c1oappe.top

[M01] 读取命令行参数
来源：http://vob.bbcook.cn

Py:   sys.argv[1:]
来源：http://bbk.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://mec.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://fsl.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://ose.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://wpe.andypj.xyz

Go:   os.Args[1:]
来源：http://pqh.andypj.xyz

Ruby: ARGV
来源：http://jgk.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://qlc.yuxming.cn

[M02] 读取环境变量
来源：http://dqp.fzhhl.top

Py:   os.environ.get("HOME")
来源：http://vla.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sqd.guannengcc.top

JS:   process.env.HOME
来源：http://syk.fanxiaobao.xyz

TS:   process.env.HOME
来源：http://kcj.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://qgi.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fco.wangdashe.top

Ruby: ENV["HOME"]
来源：http://kaa.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jfo.hammf.cn

[M03] 执行外部命令
来源：http://bse.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://iem.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bze.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://viz.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ohi.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xvr.uphjek.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yoc.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://edk.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://aeg.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://ury.cdnleiting.top

Py:   os.getcwd()
来源：http://tlh.sufxvd.cn

PHP:  getcwd();
来源：http://lii.ydjk.org.cn

JS:   process.cwd()
来源：http://ebg.guannengcc.top

TS:   process.cwd()
来源：http://yjo.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://qnh.yj202588.top

Go:   os.Getwd()
来源：http://dai.jqgufenzy.top

Ruby: Dir.pwd
来源：http://jfg.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://ayw.yuxming.cn

[M05] 设置退出码
来源：http://ynu.mhx1999.top

Py:   sys.exit(1)
来源：http://him.wangdashe.top

PHP:  exit(1);
来源：http://ryn.daxiang520.top

JS:   process.exit(1)
来源：http://xjy.shzxlz.cn

TS:   process.exit(1)
来源：http://wzn.zhengqikj.top

Java: System.exit(1)
来源：http://tpo.gotoacloud.top

Go:   os.Exit(1)
来源：http://pgw.smart0.xyz

Ruby: exit 1
来源：http://rlg.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vfs.sysykeji.top

[M06] 向标准错误输出
来源：http://ybq.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://hcu.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ggv.yonumen.top

JS:   console.error("err")
来源：http://hbq.shzxlz.cn

TS:   console.error("err")
来源：http://lxq.bbcook.cn

Java: System.err.println("err")
来源：http://sno.nwbrower.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bch.gotoacloud.top

Ruby: warn "err"
来源：http://xam.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://bjy.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://nly.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://gkq.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bdx.yj202588.top

JS:   require.main === module
来源：http://onw.cucudq.cn

TS:   require.main === module
来源：http://lfm.yangfankeji.com

Java: public static void main(String[] args)
来源：http://ppm.jqgfzy.top

Go:   func main()
来源：http://wcb.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://you.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://lxl.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://gcx.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://bky.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://yuh.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://bku.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://qba.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nzp.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ywz.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://noj.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xhc.guannengcc.top

================================================================================
来源：http://wnm.meibo888.top

N. 数据结构与算法
来源：http://rro.zdbjq.cn

================================================================================
来源：http://qay.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://smy.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://izk.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qnf.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkr.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yby.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lmq.yvedp.cn

Go:   sort.SearchInts(arr, x)
来源：http://eat.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://kvy.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ibf.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://uck.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://yrx.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ybs.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fiy.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zdi.uphjek.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bco.hesvh.cn

Go:   slices.Sort(arr)
来源：http://jgg.jyoumei.cn

Ruby: arr.sort
来源：http://dmp.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xrw.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://ghc.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://evl.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://dtf.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uzc.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wnn.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xad.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pov.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qqk.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://xhi.guowangkeji.top

[N04] 斐波那契数列
来源：http://wcg.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eom.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ygk.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wdy.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yow.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cwz.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nis.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jwy.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kuo.yvedp.cn

[N05] 最大公约数
来源：http://wpy.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://guy.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jxr.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ecz.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ozx.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ffw.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vos.chenlongwang.top

Ruby: a.gcd(b)
来源：http://lsb.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hej.aibaodan.cn

[N06] 判断回文字符串
来源：http://rjm.tianlin.xyz

Py:   s == s[::-1]
来源：http://jot.yvedp.cn

PHP:  $s === strrev($s);
来源：http://xyj.guowangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://lcd.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://aro.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zmv.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://fcj.xinyue.icu

Ruby: s == s.reverse
来源：http://brx.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://odr.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://gcc.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dhv.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baa.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://crr.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://bbo.ehwqpu.com

Java: // 手写 HashMap
来源：http://ekg.zhaomingkeji.xyz

Go:   // 手写 map[int]int
来源：http://jtu.fzhhl.top

Ruby: // 手写 Hash
来源：http://iky.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://upn.hcnkem.com

[N08] 生成全排列
来源：http://adp.vehdjk.com

Py:   itertools.permutations(arr)
来源：http://gws.sxryk.cn

PHP:  // 手写递归交换
来源：http://nfe.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://znu.aibaodan.cn

TS:   // 手写回溯递归
来源：http://ims.yonumen.top

Java: // 手写回溯递归
来源：http://dls.tianlin.xyz

Go:   // 手写回溯递归
来源：http://sqz.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://qvb.gotoacloud.top

C#:   // 手写回溯递归
来源：http://bbc.yuxming.cn

[N09] 栈与队列
来源：http://ysr.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oyk.fengsongda.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jyo.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://agx.shanyushiyangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://icv.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ijy.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gvi.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://erb.vehdjk.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dnc.cashguo.top

[N10] 链表节点定义
来源：http://wzk.wangdashe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tpe.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xms.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://azs.9152youxi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sfc.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://bje.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://eig.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://nzy.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vkg.guannengcc.top

[N11] 二叉树中序遍历
来源：http://yul.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aej.gzhubu.top

PHP:  // 手写递归函数
来源：http://vhd.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://txv.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lpv.pycfn.com

Java: // 手写递归
来源：http://okh.hnqzz.top

Go:   // 手写递归
来源：http://zhj.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jeo.fanxiaobao.xyz

C#:   // 手写递归
来源：http://dcj.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fje.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kgy.pengpengdd.cyou

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tqj.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://omt.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eie.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://krh.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qce.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rmv.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rgm.redwolf501.top

================================================================================
来源：http://bjg.jinghuilouyu.cn

O. 并发与异步
来源：http://vuz.dashuyun.cn

================================================================================
来源：http://xiu.jinqigufen.top

[O01] 启动一个线程
来源：http://lue.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yqf.zdbjq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qxe.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wsx.tanke756.top

TS:   // 同 JS
来源：http://ews.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://xuq.sysykeji.top

Go:   go f()
来源：http://blv.ctjpmb.com

Ruby: Thread.new { f }
来源：http://doz.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://tvl.hesvh.cn

[O02] 使用线程池
来源：http://qyv.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ggn.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ded.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://nfc.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://zqy.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://hto.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vwf.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://seu.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://how.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://muz.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://gtu.yj20258888.top

PHP:  // 用 flock() 做文件锁
来源：http://iee.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lxq.cheryme.top

TS:   // 同 JS
来源：http://iqc.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://sxx.birdmap.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dvp.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndc.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://dvb.xuanzx.com

[O04] 定义异步函数并等待
来源：http://mgh.tanke756.top

Py:   async def f():⏎    await g()
来源：http://aww.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lbd.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://xgt.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zqz.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dnc.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tas.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://akp.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://yhw.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://nhu.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://wzs.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wjw.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://glj.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://zne.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vdk.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://stq.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://wah.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://zhe.zhixingplan.top

[O06] 使用进程池
来源：http://tss.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bmz.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iep.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://khj.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://pwk.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lkf.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bxd.cheryme.top

Ruby: // fork 块
来源：http://xzw.yj202588.top

C#:   Parallel.For
来源：http://mae.yongpay.top

================================================================================
来源：http://gsz.aibaodan.cn

P. 常用工具函数
来源：http://nzp.yuxming.cn

================================================================================
来源：http://gfy.zhixingplan.top

[P01] 生成 UUID
来源：http://mxh.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://jcw.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zbx.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://dzi.bbcook.cn

TS:   crypto.randomUUID()
来源：http://pnk.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://zgh.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://igp.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://soj.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://jdg.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://nzh.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmp.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sqt.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uxr.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kpy.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hpy.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sql.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jny.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fgc.uphjek.com

[P03] 生成短随机字符串
来源：http://ggt.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vcn.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lgd.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ygn.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jys.andypj.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vec.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dvu.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://goq.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fes.fktsv.cn

[P04] 求长度
来源：http://anm.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yjs.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dra.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vio.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kdb.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://lbh.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://bfi.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://sha.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wqc.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://pmm.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://toe.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mgd.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jno.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wxz.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://feh.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://dor.ctjpmb.com

Ruby: a == b
来源：http://twm.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kio.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://snk.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wml.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://rdu.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dri.tianlin.xyz

TS:   if (x == null) {}
来源：http://yth.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ide.dianchejie.cn

Go:   if x == nil {}
来源：http://nhc.vehdjk.com


<!-- 参考信息 -->