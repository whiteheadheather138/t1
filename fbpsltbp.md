代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rlh.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kes.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yri.jianghu66.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://anx.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mot.cqqwz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://azh.ydzc1.top

================================================================================
来源：http://hxd.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://zyd.quarkkingdee.top

================================================================================
来源：http://ulj.sufxvd.cn

[M01] 读取命令行参数
来源：http://dqh.pycfn.com

Py:   sys.argv[1:]
来源：http://rov.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://vje.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://ymh.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://mil.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://tmg.jinyuanbaomall.cn

Go:   os.Args[1:]
来源：http://jof.yj20258888.top

Ruby: ARGV
来源：http://avr.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://wjk.wangshuangyany.cn

[M02] 读取环境变量
来源：http://qri.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://uwn.tian-w.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qwn.tianlin.xyz

JS:   process.env.HOME
来源：http://jph.fktsv.cn

TS:   process.env.HOME
来源：http://ucv.yonumen.top

Java: System.getenv("HOME")
来源：http://sal.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qwn.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://xkk.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lku.svipenyu.cn

[M03] 执行外部命令
来源：http://dnb.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dfk.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nzz.yj202588.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lnc.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bhl.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sfn.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://esr.hammf.cn

Ruby: system("ls -l");  `ls -l`
来源：http://apd.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://drt.sxryk.cn

[M04] 获取当前工作目录
来源：http://wqw.ywan-chungtsiang.top

Py:   os.getcwd()
来源：http://woz.ctjpmb.com

PHP:  getcwd();
来源：http://ght.gogol.net.cn

JS:   process.cwd()
来源：http://hsw.c1oappe.top

TS:   process.cwd()
来源：http://irs.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://oyy.aibaodan.cn

Go:   os.Getwd()
来源：http://mtb.zhongyouzk.top

Ruby: Dir.pwd
来源：http://jwk.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://whp.bbcook.cn

[M05] 设置退出码
来源：http://vfa.dianchejie.cn

Py:   sys.exit(1)
来源：http://qsi.hfpthk.cn

PHP:  exit(1);
来源：http://mvv.xuetiantiany.cn

JS:   process.exit(1)
来源：http://qwd.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://qan.tian-w.cn

Java: System.exit(1)
来源：http://wix.cheryme.top

Go:   os.Exit(1)
来源：http://czp.zhijiandao.cn

Ruby: exit 1
来源：http://xuq.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zzn.0kj1m.cn

[M06] 向标准错误输出
来源：http://xbm.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://giu.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://enk.kuanghao11.cn

JS:   console.error("err")
来源：http://ytl.yuanzhike.top

TS:   console.error("err")
来源：http://ynv.fzhhl.top

Java: System.err.println("err")
来源：http://gsl.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vvs.sjlbkw.cn

Ruby: warn "err"
来源：http://snk.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://jmh.wangdashe.top

[M07] 判断是否为主入口
来源：http://gpy.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://ohf.xuanzx.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zpf.gzhubu.top

JS:   require.main === module
来源：http://ehm.hysaishi.cn

TS:   require.main === module
来源：http://uud.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://oet.0kj1m.cn

Go:   func main()
来源：http://bdy.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vhx.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://gkn.cheryme.top

[M08] 获取系统与运行时信息
来源：http://hiu.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://jux.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://blm.smart0.xyz

JS:   process.platform;  process.version
来源：http://wpa.ivvv.top

TS:   process.platform;  process.version
来源：http://kvq.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mpe.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbt.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rau.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wvn.fengsongda.top

================================================================================
来源：http://wtg.xinyue.icu

N. 数据结构与算法
来源：http://lxz.tianlin.xyz

================================================================================
来源：http://khf.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://zea.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://msh.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qec.hesvh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwk.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gvc.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://cta.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://scn.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://byu.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://irl.nanxinkj.top

[N02] 排序（工程实践用内置实现）
来源：http://gzu.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://are.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qad.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wjh.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fqc.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jnq.yueranfly.top

Go:   slices.Sort(arr)
来源：http://jog.yuxming.cn

Ruby: arr.sort
来源：http://lpz.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nzn.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://ynp.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ivs.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://bva.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://prh.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uul.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bhk.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ris.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qic.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lir.ehwqpu.com

[N04] 斐波那契数列
来源：http://oka.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vqq.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fbq.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nre.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cql.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wgm.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jrg.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rdj.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dvo.iojbl.cn

[N05] 最大公约数
来源：http://dbn.iojbl.cn

Py:   math.gcd(a, b)
来源：http://ojv.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qwg.hesvh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xng.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvq.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vxh.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hdu.jinqigfzy.top

Ruby: a.gcd(b)
来源：http://uuu.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jlv.yonumen.top

[N06] 判断回文字符串
来源：http://ole.sysykeji.top

Py:   s == s[::-1]
来源：http://vjl.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://ybn.chenzaomai.com

JS:   s === [...s].reverse().join("")
来源：http://gex.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://ndg.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://efc.xylfe.cn

Go:   // 双指针从两端比较
来源：http://phw.nanxinkj.top

Ruby: s == s.reverse
来源：http://byj.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://nqs.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://mlr.redwolf501.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bdi.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tdz.yfazqb.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zaq.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://hqg.jinqigfzy.top

Java: // 手写 HashMap
来源：http://zyd.xylfe.cn

Go:   // 手写 map[int]int
来源：http://pyi.smart0.xyz

Ruby: // 手写 Hash
来源：http://qqr.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://bvf.fengsongda.top

[N08] 生成全排列
来源：http://cjd.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://ggu.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://sks.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://dgs.hysaishi.cn

TS:   // 手写回溯递归
来源：http://wdu.xylfe.cn

Java: // 手写回溯递归
来源：http://ask.jianghu66.top

Go:   // 手写回溯递归
来源：http://lsl.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://tcz.hywenlv.cn

C#:   // 手写回溯递归
来源：http://ohe.andypj.xyz

[N09] 栈与队列
来源：http://blp.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rmi.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wmw.fanxiaobao.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bry.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qwz.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qsf.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwq.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wnz.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iah.snrcjt.cn

[N10] 链表节点定义
来源：http://kuk.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pub.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aaw.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dce.hcnkem.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dah.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://vrv.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://yoe.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://nyk.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gmi.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://qok.yfazqb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uhz.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://nsa.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kse.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnq.bbcook.cn

Java: // 手写递归
来源：http://fls.ydjk.org.cn

Go:   // 手写递归
来源：http://ekq.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fjt.jianghu66.top

C#:   // 手写递归
来源：http://anh.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dcd.gotoacloud.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qzd.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rkb.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tee.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opd.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zbb.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://niy.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xti.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ftl.shangyingyoupin.top

================================================================================
来源：http://sou.xuanzx.com

O. 并发与异步
来源：http://kim.ivvv.top

================================================================================
来源：http://nky.yuxming.cn

[O01] 启动一个线程
来源：http://eyb.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rig.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gyb.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uri.cucudq.cn

TS:   // 同 JS
来源：http://wxb.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://kgw.sysykeji.top

Go:   go f()
来源：http://qkt.gzhubu.top

Ruby: Thread.new { f }
来源：http://elm.smart0.xyz

C#:   Task.Run(() => F());
来源：http://yod.xylfe.cn

[O02] 使用线程池
来源：http://wnp.chenlongwang.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tsl.nanxuanxn.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kld.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://ger.sysykeji.top

TS:   // worker_threads 线程池
来源：http://qkl.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mvt.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kee.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zno.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gwl.jiagoushi.top

[O03] 加锁保护共享数据
来源：http://joa.yj20258888.top

Py:   with lock: shared += 1
来源：http://mjd.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://tka.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xiz.nanxuanxn.top

TS:   // 同 JS
来源：http://vbi.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://jcr.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zpk.gotoacloud.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rbg.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://omn.ydzc1.top

[O04] 定义异步函数并等待
来源：http://ryv.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://skj.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qae.wangdashe.top

JS:   async function f() { await g(); }
来源：http://gdm.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aqt.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aum.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gbm.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aia.yj20258.top

C#:   async Task F() { await G(); }
来源：http://mym.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://tli.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://jxw.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ztt.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://gza.meibo888.top

TS:   await Promise.all(tasks)
来源：http://cwy.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lsc.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nwt.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://zsu.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://otn.daria6918.cn

[O06] 使用进程池
来源：http://apa.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kcd.haohaochexian.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wub.fzhhl.top

JS:   // child_process / cluster 模块
来源：http://cax.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://rec.guannengcc.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xvo.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cyn.gaohongyu789.top

Ruby: // fork 块
来源：http://rei.birdmap.top

C#:   Parallel.For
来源：http://ecq.fktsv.cn

================================================================================
来源：http://hnh.jqgufenzy.top

P. 常用工具函数
来源：http://cic.jyoumei.cn

================================================================================
来源：http://iwl.jinqigufen.top

[P01] 生成 UUID
来源：http://ipm.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://okz.sysykeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bzs.hongshengwenyu.top

JS:   crypto.randomUUID()
来源：http://xlb.yonumen.top

TS:   crypto.randomUUID()
来源：http://mhb.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://ggv.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://qtr.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://nte.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://wza.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://rpi.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xpu.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yjb.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gbr.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://avn.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jlk.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xok.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rgd.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lza.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://bge.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uqu.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xhx.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khj.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mht.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kah.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://did.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zlc.chenlongwang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bku.gaohongyu789.top

[P04] 求长度
来源：http://ash.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dyu.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pov.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oqg.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzk.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://crh.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://qfa.redwolf501.top

Ruby: x.length;  x.size
来源：http://lbq.cucudq.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ibe.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://ogq.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ztk.jqgufenzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oyg.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hbd.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://njo.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://voo.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://lbj.yj202588.top

Ruby: a == b
来源：http://ogy.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qtu.xylfe.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gyf.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sah.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://gzg.cqqwz.cn


<!-- 参考信息 -->