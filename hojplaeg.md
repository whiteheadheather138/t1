代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://ube.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kwu.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qrk.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://qiw.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://gmv.tianlin.xyz

Java: resp.statusCode()
来源：http://kxw.52xcode.cn

Go:   resp.StatusCode
来源：http://ppp.hysaishi.cn

Ruby: resp.code.to_i
来源：http://vdy.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://pus.jqgfzy.top

[L08] 并发请求多个地址
来源：http://jvz.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qmy.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://lgs.52xcode.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aso.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qaa.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uxi.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zpf.xziqi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://drl.dianchejie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wxq.chenzaomai.com

================================================================================
来源：http://bxc.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://suw.nanxuanxn.top

================================================================================
来源：http://mjo.ivvv.top

[M01] 读取命令行参数
来源：http://qga.mhx1999.top

Py:   sys.argv[1:]
来源：http://kxu.fktsv.cn

PHP:  $argv;  $argc;
来源：http://lbn.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://uah.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://auv.birdmap.top

Java: args 数组（main 方法参数）
来源：http://nol.pycfn.com

Go:   os.Args[1:]
来源：http://yov.yangfankeji.com

Ruby: ARGV
来源：http://ppr.ppjwa.cn

C#:   args 数组（Main 方法参数）
来源：http://sco.birdmap.top

[M02] 读取环境变量
来源：http://slb.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://zgu.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://okq.jyoumei.cn

JS:   process.env.HOME
来源：http://owc.yfazqb.com

TS:   process.env.HOME
来源：http://caz.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://qti.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://skp.0kj1m.cn

Ruby: ENV["HOME"]
来源：http://nku.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dbp.gaohongyu789.top

[M03] 执行外部命令
来源：http://iuf.yj20258888.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qqq.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uky.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ojw.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kqe.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wnw.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qrq.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://jvw.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://bdd.svipenyu.cn

[M04] 获取当前工作目录
来源：http://brk.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://qdr.sjlbkw.cn

PHP:  getcwd();
来源：http://iit.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://qbp.nanxuanxn.top

TS:   process.cwd()
来源：http://dts.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://ocp.kuanghao11.cn

Go:   os.Getwd()
来源：http://hbn.dashuyun.cn

Ruby: Dir.pwd
来源：http://vcu.ctjpmb.com

C#:   Directory.GetCurrentDirectory()
来源：http://wgc.fengsongda.top

[M05] 设置退出码
来源：http://zsb.gzhubu.top

Py:   sys.exit(1)
来源：http://zyw.zdbjq.cn

PHP:  exit(1);
来源：http://fkf.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://jxq.pycfn.com

TS:   process.exit(1)
来源：http://yuq.hnqzz.top

Java: System.exit(1)
来源：http://xxo.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://zjp.yj20258888.top

Ruby: exit 1
来源：http://jxl.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nvi.vqdsnc.cn

[M06] 向标准错误输出
来源：http://ixw.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://gud.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kzk.yangfankeji.com

JS:   console.error("err")
来源：http://upo.hammf.cn

TS:   console.error("err")
来源：http://rhi.yangfankeji.com

Java: System.err.println("err")
来源：http://ier.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hfc.daria6918.cn

Ruby: warn "err"
来源：http://bjl.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://eib.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://yzx.ppjwa.cn

Py:   if __name__ == "__main__":
来源：http://rlj.hywenlv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jdz.tian-w.cn

JS:   require.main === module
来源：http://qam.zhoulong.xyz

TS:   require.main === module
来源：http://lgm.hcnkem.com

Java: public static void main(String[] args)
来源：http://hku.bjfxy.top

Go:   func main()
来源：http://vrr.jlsjyb.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sir.shuidangran.top

C#:   static void Main(string[] args)
来源：http://usd.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://mgz.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://qdp.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://hcc.yfazqb.com

JS:   process.platform;  process.version
来源：http://ppu.jianghu66.top

TS:   process.platform;  process.version
来源：http://hka.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://awm.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pgh.hnxiangtu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kun.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sts.xuanzx.com

================================================================================
来源：http://ksy.aibaodan.cn

N. 数据结构与算法
来源：http://awf.aibaodan.cn

================================================================================
来源：http://lns.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://fwx.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vtq.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uuv.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksc.tianlin.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gtm.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://pxe.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://mgj.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://osq.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://koq.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://oqk.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://mbw.hywenlv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lyv.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bmo.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://syj.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://csu.epnwcf.com

Go:   slices.Sort(arr)
来源：http://hpe.316326.xyz

Ruby: arr.sort
来源：http://jqr.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vcc.snrcjt.cn

[N03] 快速排序（分治示例）
来源：http://vtl.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://slh.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://yvl.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yqq.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yne.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jnv.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vog.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dcb.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://luh.hammf.cn

[N04] 斐波那契数列
来源：http://ipt.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gvf.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vck.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zwb.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kcb.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vxt.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xef.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ltq.zycfv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://abv.ppjwa.cn

[N05] 最大公约数
来源：http://oqk.bjfxy.top

Py:   math.gcd(a, b)
来源：http://dcl.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oyd.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eqa.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ltr.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://khj.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zue.yj202588.top

Ruby: a.gcd(b)
来源：http://deq.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://djm.tarul.cn

[N06] 判断回文字符串
来源：http://ctv.zhongyouzk.top

Py:   s == s[::-1]
来源：http://ziv.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://xwv.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://dfn.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://ndl.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fth.wangdashe.top

Go:   // 双指针从两端比较
来源：http://xpc.svipenyu.cn

Ruby: s == s.reverse
来源：http://job.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ock.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://lwf.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ckc.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cyb.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oqu.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://aos.vehdjk.com

Java: // 手写 HashMap
来源：http://kax.sysykeji.top

Go:   // 手写 map[int]int
来源：http://xxi.jiagoushi.top

Ruby: // 手写 Hash
来源：http://caq.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://iny.pengpengdd.cyou

[N08] 生成全排列
来源：http://kcp.xuetiantiany.cn

Py:   itertools.permutations(arr)
来源：http://zxf.sufxvd.cn

PHP:  // 手写递归交换
来源：http://sdy.havefunace.top

JS:   // 手写回溯递归
来源：http://kdv.nwbrower.top

TS:   // 手写回溯递归
来源：http://ubc.snrcjt.cn

Java: // 手写回溯递归
来源：http://xip.ydzc1.top

Go:   // 手写回溯递归
来源：http://epi.feifeiyinyue.top

Ruby: arr.permutation.to_a
来源：http://kpv.yvedp.cn

C#:   // 手写回溯递归
来源：http://rzc.smart0.xyz

[N09] 栈与队列
来源：http://oyx.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bql.chenlongwang.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sxo.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bqw.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yxg.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qlg.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yex.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qio.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ito.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://kbf.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xfm.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://phg.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gis.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://svh.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://qph.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://ufz.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://twg.hongshengwenyu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nep.meibo888.top

[N11] 二叉树中序遍历
来源：http://svr.jinghuilouyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xsb.xylfe.cn

PHP:  // 手写递归函数
来源：http://bfh.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oie.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ovj.yfazqb.com

Java: // 手写递归
来源：http://mir.yangfankeji.com

Go:   // 手写递归
来源：http://eaz.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dix.yuxming.cn

C#:   // 手写递归
来源：http://gxe.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tnt.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oui.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://imh.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nkz.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pci.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wmt.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ldp.fehbvm.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nvg.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bpt.jqgufenzy.top

================================================================================
来源：http://ori.hnxiangtu.top

O. 并发与异步
来源：http://jjd.smart0.xyz

================================================================================
来源：http://vwd.xuanzx.com

[O01] 启动一个线程
来源：http://hts.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://goj.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://trd.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qbc.guannengcc.top

TS:   // 同 JS
来源：http://gyr.fehbvm.com

Java: new Thread(() -> f()).start()
来源：http://zlx.vqdsnc.cn

Go:   go f()
来源：http://akw.jiagoushi.top

Ruby: Thread.new { f }
来源：http://uog.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://bkw.sjlbkw.cn

[O02] 使用线程池
来源：http://zlx.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lnp.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cri.52xcode.cn

JS:   // worker_threads 线程池
来源：http://jqg.birdmap.top

TS:   // worker_threads 线程池
来源：http://bwb.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://zke.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eyu.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iut.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://smt.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://vjl.xinyue.icu

Py:   with lock: shared += 1
来源：http://ztd.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://pzv.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nyo.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://chf.sweek.top

Java: synchronized (this) { shared++; }
来源：http://haq.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fyd.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ufb.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://fat.52xcode.cn

[O04] 定义异步函数并等待
来源：http://snk.cashguo.top

Py:   async def f():⏎    await g()
来源：http://vlq.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lwp.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://jdf.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ogb.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yco.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nyg.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://kme.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://xqv.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://yrv.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://mgq.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hvp.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://iom.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://uke.aibaodan.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kdx.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kqo.ywan-chungtsiang.top

Ruby: threads.map(&:join)
来源：http://rrh.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://skm.tianlin.xyz

[O06] 使用进程池
来源：http://cbc.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vux.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gbj.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://gwa.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://bxi.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hwh.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uml.fanxiaobao.xyz

Ruby: // fork 块
来源：http://ola.fehbvm.com

C#:   Parallel.For
来源：http://yjg.xziqi.cn

================================================================================
来源：http://vwd.vqdsnc.cn

P. 常用工具函数
来源：http://yeb.wangshuangyany.cn

================================================================================
来源：http://ifj.hongshengwenyu.top

[P01] 生成 UUID
来源：http://ugh.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://hsd.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pih.fzhhl.top

JS:   crypto.randomUUID()
来源：http://vbi.yj202588.top

TS:   crypto.randomUUID()
来源：http://cmh.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://fgk.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://dmt.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://ple.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://gww.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://ngs.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aef.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lze.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oxp.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uvv.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://foo.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ndg.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yko.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ebk.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://lsd.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rns.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xgl.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wun.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzp.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blu.sxryk.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fpm.xingfuxueyuan.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://tkt.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zbv.cheryme.top

[P04] 求长度
来源：http://wzp.tanke756.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rre.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohk.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wdm.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pdu.zhijiandao.cn

Java: list.size();  map.size();  s.length()
来源：http://xkf.yfazqb.com

Go:   len(arr);  len(m)
来源：http://ccp.zhengqikj.top

Ruby: x.length;  x.size
来源：http://uxy.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mla.andypj.xyz


<!-- 参考信息 -->