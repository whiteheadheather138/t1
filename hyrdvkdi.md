代发 wailian999

C#:   (int)resp.StatusCode
来源：http://ezv.cashguo.top

[L08] 并发请求多个地址
来源：http://uhl.jinqigfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://suz.cashguo.top

PHP:  curl_multi_init() 系列
来源：http://xwb.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fce.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cqg.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pxz.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tzj.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ugu.uphjek.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ntk.ehwqpu.com

================================================================================
来源：http://jht.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://msi.zhoulong.xyz

================================================================================
来源：http://rrb.bbcook.cn

[M01] 读取命令行参数
来源：http://lyg.bjfxy.top

Py:   sys.argv[1:]
来源：http://now.shzxlz.cn

PHP:  $argv;  $argc;
来源：http://kkd.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://zxh.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://wwk.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://ocm.zdqjudy.top

Go:   os.Args[1:]
来源：http://fcw.iojbl.cn

Ruby: ARGV
来源：http://why.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://ohu.havefunace.top

[M02] 读取环境变量
来源：http://rvg.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://qbs.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jor.hywenlv.cn

JS:   process.env.HOME
来源：http://jti.gogol.net.cn

TS:   process.env.HOME
来源：http://zao.smart0.xyz

Java: System.getenv("HOME")
来源：http://qtk.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gkl.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://vrp.bbcook.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://usz.tianlin.xyz

[M03] 执行外部命令
来源：http://vad.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wtr.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ech.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kbn.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vuz.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ssx.yuanzhike.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lpf.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hon.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://kbh.epnwcf.com

[M04] 获取当前工作目录
来源：http://lkn.yongpay.top

Py:   os.getcwd()
来源：http://lig.tianlin.xyz

PHP:  getcwd();
来源：http://wfv.jiagoushi.top

JS:   process.cwd()
来源：http://rcq.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://tam.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://qeo.mhx1999.top

Go:   os.Getwd()
来源：http://ujx.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://kyy.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://twv.yj20258888.top

[M05] 设置退出码
来源：http://xev.hysaishi.cn

Py:   sys.exit(1)
来源：http://wol.jinqigufen.top

PHP:  exit(1);
来源：http://zxm.dianchejie.cn

JS:   process.exit(1)
来源：http://ucn.zhengqikj.top

TS:   process.exit(1)
来源：http://tfq.jinyuanbaomall.cn

Java: System.exit(1)
来源：http://erq.gzhubu.top

Go:   os.Exit(1)
来源：http://zfp.ehwqpu.com

Ruby: exit 1
来源：http://dov.nanxuanxn.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nvr.hysaishi.cn

[M06] 向标准错误输出
来源：http://tus.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://lgj.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://byn.zhiwuduotai.top

JS:   console.error("err")
来源：http://qut.svipenyu.cn

TS:   console.error("err")
来源：http://wmb.jiagoushi.top

Java: System.err.println("err")
来源：http://snr.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ocz.yuanzhike.top

Ruby: warn "err"
来源：http://afb.sjlbkw.cn

C#:   Console.Error.WriteLine("err")
来源：http://tat.dashuyun.cn

[M07] 判断是否为主入口
来源：http://xnm.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://wnd.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zgq.yvedp.cn

JS:   require.main === module
来源：http://syt.daxiang520.top

TS:   require.main === module
来源：http://pji.hongshengwenyu.top

Java: public static void main(String[] args)
来源：http://jfp.fktsv.cn

Go:   func main()
来源：http://sup.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mdn.smart0.xyz

C#:   static void Main(string[] args)
来源：http://muy.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://cfn.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://ppt.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://ojw.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://lus.uphjek.com

TS:   process.platform;  process.version
来源：http://adz.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uat.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ekn.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://taj.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yua.hnxiangtu.top

================================================================================
来源：http://mro.gogol.net.cn

N. 数据结构与算法
来源：http://yaj.gotoacloud.top

================================================================================
来源：http://hdi.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://ttq.yfazqb.com

Py:   bisect.bisect_left(arr, x)
来源：http://yrc.jinghuilouyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sig.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fov.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uny.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sdb.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://sca.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dty.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://maf.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://wle.redwolf501.top

Py:   sorted(arr);  arr.sort()
来源：http://cxg.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pmz.xuanzx.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zwq.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lre.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ilj.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://hps.yj20258888.top

Ruby: arr.sort
来源：http://jit.cucudq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nfz.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://tus.wangshuangyany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://euj.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://ipn.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvm.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pci.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eth.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dgn.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ekw.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://skh.aizwys.cn

[N04] 斐波那契数列
来源：http://rbo.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qck.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipl.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qwo.zhengqikj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vvw.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hzg.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tuj.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ryi.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://efh.ydjk.org.cn

[N05] 最大公约数
来源：http://gvh.cashguo.top

Py:   math.gcd(a, b)
来源：http://kfg.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qfm.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tcn.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xwv.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nbf.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ovm.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://jwt.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://grn.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://qrj.ivvv.top

Py:   s == s[::-1]
来源：http://qiv.tian-w.cn

PHP:  $s === strrev($s);
来源：http://jef.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://nvs.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://ohb.nanxinkj.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tdf.andypj.xyz

Go:   // 双指针从两端比较
来源：http://yys.zhoulong.xyz

Ruby: s == s.reverse
来源：http://ksk.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://vyi.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://kqt.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kvj.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qit.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qeb.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://ipb.ctjpmb.com

Java: // 手写 HashMap
来源：http://gpo.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://iiu.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://gpr.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://ppt.hesvh.cn

[N08] 生成全排列
来源：http://odp.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://qqi.ivvv.top

PHP:  // 手写递归交换
来源：http://rcr.hysaishi.cn

JS:   // 手写回溯递归
来源：http://khw.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://pub.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://oyn.tanke756.top

Go:   // 手写回溯递归
来源：http://jwu.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://ztf.uphjek.com

C#:   // 手写回溯递归
来源：http://rmu.ctjpmb.com

[N09] 栈与队列
来源：http://afv.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://msw.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://omr.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://maz.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dbe.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pan.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sxt.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nah.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aos.jqgfzy.top

[N10] 链表节点定义
来源：http://avg.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kmm.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://evb.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sar.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xpi.shzxlz.cn

Java: class Node { int v; Node next; }
来源：http://ofx.zdqjudy.top

Go:   type Node struct { V int; Next *Node }
来源：http://akb.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rok.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://eox.vehdjk.com

[N11] 二叉树中序遍历
来源：http://qlp.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cbo.kuanghao11.cn

PHP:  // 手写递归函数
来源：http://zxr.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbd.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ojg.hywenlv.cn

Java: // 手写递归
来源：http://kow.sxryk.cn

Go:   // 手写递归
来源：http://hai.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dux.yuanzhike.top

C#:   // 手写递归
来源：http://sxj.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hpo.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://luq.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qib.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yld.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://elc.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hlk.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nll.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htw.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bgh.aibaodan.cn

================================================================================
来源：http://exk.xylfe.cn

O. 并发与异步
来源：http://xca.daria6918.cn

================================================================================
来源：http://ckw.zdbjq.cn

[O01] 启动一个线程
来源：http://pkz.jlsjyb.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vpq.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ozv.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ups.zhijiandao.cn

TS:   // 同 JS
来源：http://lpz.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://xgh.wangdashe.top

Go:   go f()
来源：http://mod.redwolf501.top

Ruby: Thread.new { f }
来源：http://gou.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://kre.gzhubu.top

[O02] 使用线程池
来源：http://agm.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cwz.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ycg.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://xbu.tanke756.top

TS:   // worker_threads 线程池
来源：http://jou.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://cch.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dmg.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://feg.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mlz.zycfv.cn

[O03] 加锁保护共享数据
来源：http://dcz.0kj1m.cn

Py:   with lock: shared += 1
来源：http://ens.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://mev.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nux.gogol.net.cn

TS:   // 同 JS
来源：http://jvi.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://wtj.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gjx.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://thz.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://ozd.xziqi.cn

[O04] 定义异步函数并等待
来源：http://zmy.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://ueb.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ytt.hnqzz.top

JS:   async function f() { await g(); }
来源：http://gnu.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://rdc.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://imw.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pvw.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ekx.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://rvt.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://drz.vehdjk.com

Py:   asyncio.gather(*tasks)
来源：http://qtf.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ier.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://kdl.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://vyx.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hvy.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jsm.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://pfm.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kqi.tarul.cn

[O06] 使用进程池
来源：http://hho.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fbe.smart0.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://apn.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://uuv.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://raj.daxiang520.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vgv.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uuc.hnxiangtu.top

Ruby: // fork 块
来源：http://wpm.sweek.top

C#:   Parallel.For
来源：http://wjs.ybcxt.top

================================================================================
来源：http://xqw.cashguo.top

P. 常用工具函数
来源：http://lcr.9152youxi.cn

================================================================================
来源：http://yks.vehdjk.com

[P01] 生成 UUID
来源：http://jmx.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://mui.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ikt.hcnkem.com

JS:   crypto.randomUUID()
来源：http://yom.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://hin.sweek.top

Java: UUID.randomUUID().toString()
来源：http://rfi.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://ryf.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://rky.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://kkl.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://srv.yueranfly.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uep.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lmh.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://usa.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lgb.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ghi.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://orz.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://agp.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rtp.gzhubu.top

[P03] 生成短随机字符串
来源：http://czn.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lrb.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jfx.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yma.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://okq.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pgx.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dtq.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xuc.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xwa.daxiang520.top

[P04] 求长度
来源：http://tis.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vbj.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rye.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bpl.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fnn.nanxuanxn.top

Java: list.size();  map.size();  s.length()
来源：http://iyk.andypj.xyz

Go:   len(arr);  len(m)
来源：http://ite.ctjpmb.com

Ruby: x.length;  x.size
来源：http://lbv.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xwk.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://etv.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sya.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yxi.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jth.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://chp.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fsx.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://wdu.cucudq.cn

Ruby: a == b
来源：http://vyg.havefunace.top


<!-- 参考信息 -->