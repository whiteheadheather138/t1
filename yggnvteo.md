代发 wailian999

TS:   resp.ok;  resp.status
来源：http://asc.jianghu66.top

Java: resp.statusCode()
来源：http://fpj.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://psr.zycfv.cn

Ruby: resp.code.to_i
来源：http://coc.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://bey.aibaodan.cn

[L08] 并发请求多个地址
来源：http://qgp.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zuw.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://mfd.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kde.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sev.vehdjk.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://grh.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xly.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mem.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kvs.hesvh.cn

================================================================================
来源：http://hvp.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://gem.chenzaomai.com

================================================================================
来源：http://nih.quarkkingdee.top

[M01] 读取命令行参数
来源：http://coj.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://ixe.vehdjk.com

PHP:  $argv;  $argc;
来源：http://klw.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://yzn.ydzc1.top

TS:   process.argv.slice(2)
来源：http://tff.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://wym.iojbl.cn

Go:   os.Args[1:]
来源：http://aix.aibaodan.cn

Ruby: ARGV
来源：http://vtd.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://ljf.quarkkingdee.top

[M02] 读取环境变量
来源：http://keq.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://mxs.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://srd.xinyue.icu

JS:   process.env.HOME
来源：http://kcv.c1oappe.top

TS:   process.env.HOME
来源：http://jyk.zycfv.cn

Java: System.getenv("HOME")
来源：http://der.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jld.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://yak.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://odo.havefunace.top

[M03] 执行外部命令
来源：http://wux.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qnq.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iwu.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ebl.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cyo.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ols.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kxr.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://rtz.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://zux.52xcode.cn

[M04] 获取当前工作目录
来源：http://ijw.0kj1m.cn

Py:   os.getcwd()
来源：http://oct.bbcook.cn

PHP:  getcwd();
来源：http://yol.iojbl.cn

JS:   process.cwd()
来源：http://bkj.jiagoushi.top

TS:   process.cwd()
来源：http://aju.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://nhj.xuetiantiany.cn

Go:   os.Getwd()
来源：http://tnk.sweek.top

Ruby: Dir.pwd
来源：http://obv.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://vti.yangfankeji.com

[M05] 设置退出码
来源：http://hxq.havefunace.top

Py:   sys.exit(1)
来源：http://brv.xziqi.cn

PHP:  exit(1);
来源：http://kyk.hfpthk.cn

JS:   process.exit(1)
来源：http://fsd.feifeiyinyue.top

TS:   process.exit(1)
来源：http://jde.jyoumei.cn

Java: System.exit(1)
来源：http://rbk.yongpay.top

Go:   os.Exit(1)
来源：http://jwo.snrcjt.cn

Ruby: exit 1
来源：http://hxn.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nbj.cucudq.cn

[M06] 向标准错误输出
来源：http://clg.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://mpw.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pxh.0kj1m.cn

JS:   console.error("err")
来源：http://lcr.ivvv.top

TS:   console.error("err")
来源：http://gww.yvedp.cn

Java: System.err.println("err")
来源：http://svk.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qyh.guowangkeji.top

Ruby: warn "err"
来源：http://otj.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://xue.ppjwa.cn

[M07] 判断是否为主入口
来源：http://mxh.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://hfk.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ykz.feifeiyinyue.top

JS:   require.main === module
来源：http://ati.zdqjudy.top

TS:   require.main === module
来源：http://hfy.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://hfm.mhx1999.top

Go:   func main()
来源：http://iqv.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yhy.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://kpn.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://dif.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://oqn.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://tvd.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://sbv.svipenyu.cn

TS:   process.platform;  process.version
来源：http://fge.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nkr.pycfn.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jwq.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://smw.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://swe.hammf.cn

================================================================================
来源：http://oma.cheryme.top

N. 数据结构与算法
来源：http://inr.redwolf501.top

================================================================================
来源：http://oeu.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://mrd.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://its.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://juw.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mdb.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ucy.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://vgr.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://nkw.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mds.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ahx.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://lav.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://juw.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nrt.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zdl.zhongyouzk.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://iid.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ztl.zhiwuduotai.top

Go:   slices.Sort(arr)
来源：http://oyk.ctjpmb.com

Ruby: arr.sort
来源：http://jmk.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qsp.316326.xyz

[N03] 快速排序（分治示例）
来源：http://yiq.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nfi.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://aer.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fpx.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ivu.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jzx.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nuw.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wqv.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://ijs.chenlongwang.top

[N04] 斐波那契数列
来源：http://mio.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wmg.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cuf.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vde.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://etg.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ngk.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hgo.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nad.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lnj.shanyushiyangtech.top

[N05] 最大公约数
来源：http://kxg.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://bze.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xdx.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qcc.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://odn.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wcj.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ftz.svipenyu.cn

Ruby: a.gcd(b)
来源：http://jqt.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fbh.yuanzhike.top

[N06] 判断回文字符串
来源：http://tco.yuanzhike.top

Py:   s == s[::-1]
来源：http://wub.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://jfr.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://sqs.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://yog.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lwl.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://qdj.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://rht.fanxiaobao.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://jpv.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://mqy.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iex.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ota.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://okf.xuetiantiany.cn

TS:   // 手写 Map<string, number>
来源：http://sfl.gotoacloud.top

Java: // 手写 HashMap
来源：http://ugw.c1oappe.top

Go:   // 手写 map[int]int
来源：http://hng.xylfe.cn

Ruby: // 手写 Hash
来源：http://fox.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://ctb.yongpay.top

[N08] 生成全排列
来源：http://hgn.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://xiy.xylfe.cn

PHP:  // 手写递归交换
来源：http://zff.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://mef.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://ylh.cdnleiting.top

Java: // 手写回溯递归
来源：http://hkx.hnqzz.top

Go:   // 手写回溯递归
来源：http://kjz.ivvv.top

Ruby: arr.permutation.to_a
来源：http://wfg.zdqjudy.top

C#:   // 手写回溯递归
来源：http://lpj.jyoumei.cn

[N09] 栈与队列
来源：http://bdv.zdqjudy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://opg.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uol.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tgf.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oei.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ujx.zhaomingkeji.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://klr.tanke756.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dia.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jyg.bjfxy.top

[N10] 链表节点定义
来源：http://gfh.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rtl.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://caf.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rrx.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ltd.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://kgy.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://axo.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://bfh.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yao.iojbl.cn

[N11] 二叉树中序遍历
来源：http://pkf.jianghu66.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wvu.nwbrower.top

PHP:  // 手写递归函数
来源：http://yqo.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qwo.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://syt.ydzc1.top

Java: // 手写递归
来源：http://qbb.yueranfly.top

Go:   // 手写递归
来源：http://jsl.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vxu.shanyushiyangtech.top

C#:   // 手写递归
来源：http://vwv.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wpv.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tem.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ghf.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jsd.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbl.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kjz.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bop.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gqj.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nfr.wangshuangyany.cn

================================================================================
来源：http://yfz.aibaodan.cn

O. 并发与异步
来源：http://mxr.haohaochexian.top

================================================================================
来源：http://mhp.nanxuanxn.top

[O01] 启动一个线程
来源：http://sbd.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xhj.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zmo.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ppw.jyoumei.cn

TS:   // 同 JS
来源：http://jub.gaohongyu789.top

Java: new Thread(() -> f()).start()
来源：http://xia.xingfuxueyuan.xyz

Go:   go f()
来源：http://dwe.gogol.net.cn

Ruby: Thread.new { f }
来源：http://dze.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://wwq.fanxiaobao.xyz

[O02] 使用线程池
来源：http://yoe.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gol.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vsn.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://lak.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://ckt.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://wog.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tnb.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dzc.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ydl.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://wad.vehdjk.com

Py:   with lock: shared += 1
来源：http://loz.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://enq.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nzo.sufxvd.cn

TS:   // 同 JS
来源：http://qpw.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://kpx.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ynx.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bpr.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://lom.ydzc1.top

[O04] 定义异步函数并等待
来源：http://ogq.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://dri.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ate.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://tik.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://utv.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qxe.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kbl.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://zsp.ivvv.top

C#:   async Task F() { await G(); }
来源：http://nfl.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://bkv.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://wvk.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://srl.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://uon.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://xpq.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rzh.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xnj.sxryk.cn

Ruby: threads.map(&:join)
来源：http://yyo.epnwcf.com

C#:   await Task.WhenAll(t1, t2)
来源：http://hjl.c1oappe.top

[O06] 使用进程池
来源：http://uis.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adr.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vip.yj20258.top

JS:   // child_process / cluster 模块
来源：http://vme.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://vjp.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zgr.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mia.sysykeji.top

Ruby: // fork 块
来源：http://ulm.c1oappe.top

C#:   Parallel.For
来源：http://jiw.kuanghao11.cn

================================================================================
来源：http://yqm.zhengqikj.top

P. 常用工具函数
来源：http://mxc.tarul.cn

================================================================================
来源：http://lnu.jqgfzy.top

[P01] 生成 UUID
来源：http://xhn.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://dtz.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nng.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://zcm.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://uoj.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://fcr.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://hqf.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://rlg.nwbrower.top

C#:   Guid.NewGuid().ToString()
来源：http://cxu.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://kno.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hzj.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bbv.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uez.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lhb.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ubn.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ujb.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zec.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ana.cdnleiting.top

[P03] 生成短随机字符串
来源：http://qab.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zub.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qvc.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwb.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fwf.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ejw.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dtz.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ocn.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zow.yj20258.top

[P04] 求长度
来源：http://yid.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mxy.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eim.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ovo.yonumen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kqf.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://wde.tarul.cn

Go:   len(arr);  len(m)
来源：http://vju.yj202588.top

Ruby: x.length;  x.size
来源：http://hkk.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vrm.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://iap.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vaw.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aln.xuanzx.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mgs.smart0.xyz


<!-- 参考信息 -->