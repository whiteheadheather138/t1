代发 wailian999

C#:   (int)resp.StatusCode
来源：http://uyi.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://oax.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qqf.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://ful.zhijiandao.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tur.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zkn.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sip.iojbl.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cig.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lom.pengpengdd.cyou

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xgu.yfazqb.com

================================================================================
来源：http://qgx.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://ppn.ywan-chungtsiang.top

================================================================================
来源：http://ouc.jyoumei.cn

[M01] 读取命令行参数
来源：http://dpq.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://ldh.yangfankeji.com

PHP:  $argv;  $argc;
来源：http://eqr.hnqzz.top

JS:   process.argv.slice(2)
来源：http://vpp.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://ymg.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://udh.sxryk.cn

Go:   os.Args[1:]
来源：http://qtu.iojbl.cn

Ruby: ARGV
来源：http://ixc.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://pmn.gzhubu.top

[M02] 读取环境变量
来源：http://yli.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://jrw.snrcjt.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gty.hcnkem.com

JS:   process.env.HOME
来源：http://omh.pycfn.com

TS:   process.env.HOME
来源：http://gyh.sweek.top

Java: System.getenv("HOME")
来源：http://vqd.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vsi.ydzc1.top

Ruby: ENV["HOME"]
来源：http://zcd.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dzw.yonumen.top

[M03] 执行外部命令
来源：http://fef.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://afy.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://box.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qeu.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kti.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qwy.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cqm.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://xot.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://dlu.yfazqb.com

[M04] 获取当前工作目录
来源：http://fsj.dianchejie.cn

Py:   os.getcwd()
来源：http://sna.hongshengwenyu.top

PHP:  getcwd();
来源：http://awu.dianchejie.cn

JS:   process.cwd()
来源：http://gte.cdnleiting.top

TS:   process.cwd()
来源：http://qed.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://scn.zhongyouzk.top

Go:   os.Getwd()
来源：http://qwp.bbcook.cn

Ruby: Dir.pwd
来源：http://tay.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://yrl.vehdjk.com

[M05] 设置退出码
来源：http://gls.hnxiangtu.top

Py:   sys.exit(1)
来源：http://jno.jyoumei.cn

PHP:  exit(1);
来源：http://dbh.hcnkem.com

JS:   process.exit(1)
来源：http://dxa.hysaishi.cn

TS:   process.exit(1)
来源：http://cpw.yj20258.top

Java: System.exit(1)
来源：http://zcr.gotoacloud.top

Go:   os.Exit(1)
来源：http://hmq.bbcook.cn

Ruby: exit 1
来源：http://smu.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mqk.hnqzz.top

[M06] 向标准错误输出
来源：http://uye.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://ker.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jip.hammf.cn

JS:   console.error("err")
来源：http://sno.chenlongwang.top

TS:   console.error("err")
来源：http://dep.yueranfly.top

Java: System.err.println("err")
来源：http://ymi.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://njc.sxryk.cn

Ruby: warn "err"
来源：http://rmt.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://dro.gogol.net.cn

[M07] 判断是否为主入口
来源：http://dzu.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://sjc.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tzs.gaohongyu789.top

JS:   require.main === module
来源：http://ihn.jqgfzy.top

TS:   require.main === module
来源：http://xib.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://lwe.hongshengwenyu.top

Go:   func main()
来源：http://mth.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mrs.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://rmz.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://pyr.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://jbm.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://zdw.hnqzz.top

JS:   process.platform;  process.version
来源：http://ead.yangfankeji.com

TS:   process.platform;  process.version
来源：http://bud.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kbh.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dcq.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dje.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xdn.sjlbkw.cn

================================================================================
来源：http://uxs.aizwys.cn

N. 数据结构与算法
来源：http://eqp.gaohongyu789.top

================================================================================
来源：http://lwb.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://mvj.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://gwk.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pxi.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mch.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cly.yangfankeji.com

Java: Arrays.binarySearch(arr, x)
来源：http://iio.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://wpe.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vei.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://jzd.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://dgr.yueranfly.top

Py:   sorted(arr);  arr.sort()
来源：http://qam.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mpx.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://clo.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kpd.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jxm.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://evl.hesvh.cn

Ruby: arr.sort
来源：http://utr.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dfe.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://xva.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxe.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://lrh.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckl.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sle.cdnleiting.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gnk.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tqj.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mfx.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://mvi.9152youxi.cn

[N04] 斐波那契数列
来源：http://zfj.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kgo.jinyuanbaomall.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vhw.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aeh.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpl.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pqz.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jzz.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://err.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pqt.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://kom.bbcook.cn

Py:   math.gcd(a, b)
来源：http://qkp.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqw.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ibl.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://unn.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zik.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mdt.0kj1m.cn

Ruby: a.gcd(b)
来源：http://you.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zxn.haohaochexian.top

[N06] 判断回文字符串
来源：http://gpt.yj202588.top

Py:   s == s[::-1]
来源：http://sdx.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://cbz.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://qvo.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://exo.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ylq.shuidangran.top

Go:   // 双指针从两端比较
来源：http://fzx.tian-w.cn

Ruby: s == s.reverse
来源：http://evk.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aoj.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://tlp.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lpj.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kdu.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rwp.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://qmn.jlsjyb.cn

Java: // 手写 HashMap
来源：http://ler.havefunace.top

Go:   // 手写 map[int]int
来源：http://ees.hesvh.cn

Ruby: // 手写 Hash
来源：http://tcf.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://sfc.nanxinkj.top

[N08] 生成全排列
来源：http://vgn.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://uci.yongpay.top

PHP:  // 手写递归交换
来源：http://cvh.hcnkem.com

JS:   // 手写回溯递归
来源：http://scm.yuanzhike.top

TS:   // 手写回溯递归
来源：http://wdn.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://bsc.zhixingplan.top

Go:   // 手写回溯递归
来源：http://xcw.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://hvj.jyoumei.cn

C#:   // 手写回溯递归
来源：http://edz.vehdjk.com

[N09] 栈与队列
来源：http://fof.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bqa.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kgi.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bel.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hkj.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mkf.hfpthk.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://guw.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rpy.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sxd.hcnkem.com

[N10] 链表节点定义
来源：http://ixd.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://onc.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pxr.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qjl.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eil.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://ylo.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ohi.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tyq.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://xbj.hammf.cn

[N11] 二叉树中序遍历
来源：http://mdf.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hqn.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://nhm.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uww.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mvm.jinqigufen.top

Java: // 手写递归
来源：http://xhj.tian-w.cn

Go:   // 手写递归
来源：http://qis.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ega.xziqi.cn

C#:   // 手写递归
来源：http://nib.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yit.zhongyouzk.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ksp.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rmi.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mjc.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lnw.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yux.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uqk.smart0.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yqf.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ofv.wangshuangyany.cn

================================================================================
来源：http://ajz.0kj1m.cn

O. 并发与异步
来源：http://luh.zhoulong.xyz

================================================================================
来源：http://rlp.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://wiu.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wqi.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ylq.zhiwuduotai.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nnl.cdnleiting.top

TS:   // 同 JS
来源：http://esr.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://mri.shzxlz.cn

Go:   go f()
来源：http://wvt.zhixingplan.top

Ruby: Thread.new { f }
来源：http://uub.aizwys.cn

C#:   Task.Run(() => F());
来源：http://ahu.yvedp.cn

[O02] 使用线程池
来源：http://zgs.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cpn.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ref.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://iwh.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://oya.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://jpc.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tjm.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ipg.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ypz.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://hmu.shuidangran.top

Py:   with lock: shared += 1
来源：http://xqc.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://out.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kco.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://tst.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://inj.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mcz.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jsf.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://jlq.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://hoz.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://xwg.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gnq.yj20258888.top

JS:   async function f() { await g(); }
来源：http://fpm.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://oeu.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://swg.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jdt.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://asg.yvedp.cn

C#:   async Task F() { await G(); }
来源：http://yfk.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://pyx.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://zbh.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ozo.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://iil.dashuyun.cn

TS:   await Promise.all(tasks)
来源：http://hja.hongshengwenyu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://spl.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ocb.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://gnl.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kpk.vehdjk.com

[O06] 使用进程池
来源：http://qmy.ctjpmb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ois.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://plv.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://ucv.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://dwj.xinyue.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lbv.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jsq.zhengqikj.top

Ruby: // fork 块
来源：http://sup.gogol.net.cn

C#:   Parallel.For
来源：http://nol.nanxinkj.top

================================================================================
来源：http://hgo.chenjidiqi.icu

P. 常用工具函数
来源：http://wwc.cheryme.top

================================================================================
来源：http://mqi.gaohongyu789.top

[P01] 生成 UUID
来源：http://dkh.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://rbs.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vdv.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://wxl.jiagoushi.top

TS:   crypto.randomUUID()
来源：http://dvh.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://zzu.jinqigufen.top

Go:   // 用 github.com/google/uuid
来源：http://jxz.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://syn.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://zdz.yueranfly.top

[P02] MD5 / SHA256 摘要
来源：http://qts.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://txg.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vnv.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tlh.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gds.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jom.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iql.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hyp.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://que.xylfe.cn

[P03] 生成短随机字符串
来源：http://hpx.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aaz.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://joc.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwa.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nce.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xes.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nbo.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tuw.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ofw.wangshuangyany.cn

[P04] 求长度
来源：http://jrv.epnwcf.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xml.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://szw.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vwx.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ysd.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://vme.xinyue.icu

Go:   len(arr);  len(m)
来源：http://jwu.xziqi.cn

Ruby: x.length;  x.size
来源：http://dlx.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ovn.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://wza.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zul.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rst.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://arm.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mhc.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://adc.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uur.yangfankeji.com

Ruby: a == b
来源：http://txd.gogol.net.cn


<!-- 参考信息 -->