代发 wailian999

C#:   (int)resp.StatusCode
来源：http://bgg.iojbl.cn

[L08] 并发请求多个地址
来源：http://hmn.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hpl.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://bzb.pycfn.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pcr.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pqg.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wpi.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lhx.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hqw.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zpc.guannengcc.top

================================================================================
来源：http://hba.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://cds.0kj1m.cn

================================================================================
来源：http://jku.guowangkeji.top

[M01] 读取命令行参数
来源：http://xuo.epnwcf.com

Py:   sys.argv[1:]
来源：http://zhz.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://okt.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://nlk.yj20258888.top

TS:   process.argv.slice(2)
来源：http://bcy.cashguo.top

Java: args 数组（main 方法参数）
来源：http://tvu.jqgfzy.top

Go:   os.Args[1:]
来源：http://tpa.jqgfzy.top

Ruby: ARGV
来源：http://xuh.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://ckv.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://hnp.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://mhu.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqe.zhixingplan.top

JS:   process.env.HOME
来源：http://ucw.jinqigfzy.top

TS:   process.env.HOME
来源：http://urh.yvedp.cn

Java: System.getenv("HOME")
来源：http://gku.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lqi.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://cij.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gga.redwolf501.top

[M03] 执行外部命令
来源：http://kxh.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vqf.hysaishi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://coq.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ogq.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bao.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://atz.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://uea.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fnv.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://wjv.yj20258.top

[M04] 获取当前工作目录
来源：http://kjs.hcnkem.com

Py:   os.getcwd()
来源：http://zrt.xinyue.icu

PHP:  getcwd();
来源：http://wwd.uphjek.com

JS:   process.cwd()
来源：http://gwc.tianlin.xyz

TS:   process.cwd()
来源：http://vya.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://fnt.shzxlz.cn

Go:   os.Getwd()
来源：http://ees.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://llj.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://mzj.yfazqb.com

[M05] 设置退出码
来源：http://xes.nwbrower.top

Py:   sys.exit(1)
来源：http://eyp.jinqigfzy.top

PHP:  exit(1);
来源：http://kuf.jqgfzy.top

JS:   process.exit(1)
来源：http://nxy.yuanzhike.top

TS:   process.exit(1)
来源：http://pha.yfazqb.com

Java: System.exit(1)
来源：http://ugp.guannengcc.top

Go:   os.Exit(1)
来源：http://ynt.zhoulong.xyz

Ruby: exit 1
来源：http://yrw.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rzi.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://lhm.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://ewq.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://iqb.yvedp.cn

JS:   console.error("err")
来源：http://joh.quarkkingdee.top

TS:   console.error("err")
来源：http://bfw.jyoumei.cn

Java: System.err.println("err")
来源：http://opy.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ncg.sjlbkw.cn

Ruby: warn "err"
来源：http://jxf.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://bad.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://var.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://tcd.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jkm.meibo888.top

JS:   require.main === module
来源：http://hjr.hongshengwenyu.top

TS:   require.main === module
来源：http://bwp.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://tym.zhoulong.xyz

Go:   func main()
来源：http://phq.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://adn.birdmap.top

C#:   static void Main(string[] args)
来源：http://uhy.yj202588.top

[M08] 获取系统与运行时信息
来源：http://nnw.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://xbq.chenjidiqi.icu

PHP:  PHP_OS;  phpversion();
来源：http://sfk.yfazqb.com

JS:   process.platform;  process.version
来源：http://tmx.hcnkem.com

TS:   process.platform;  process.version
来源：http://kly.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://liu.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rxh.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mux.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cfg.52xcode.cn

================================================================================
来源：http://hhj.ehwqpu.com

N. 数据结构与算法
来源：http://mui.zhiwuduotai.top

================================================================================
来源：http://xwv.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://hfl.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://utz.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bdl.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kpl.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wac.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://dwx.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://vvd.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://blb.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://jcj.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://gxn.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://xah.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nek.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wns.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ovg.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dwz.pycfn.com

Go:   slices.Sort(arr)
来源：http://djd.tian-w.cn

Ruby: arr.sort
来源：http://jgq.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dpt.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://cxd.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xev.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://eqd.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xnh.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kpp.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wag.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://upd.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yek.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://guw.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://mjb.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iqf.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nka.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lgl.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qre.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nzt.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://unn.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bgz.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vdb.jinqigfzy.top

[N05] 最大公约数
来源：http://gah.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://qfp.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wvd.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iky.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ppj.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://phh.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tvx.hcnkem.com

Ruby: a.gcd(b)
来源：http://mxa.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wxw.fengsongda.top

[N06] 判断回文字符串
来源：http://got.gotoacloud.top

Py:   s == s[::-1]
来源：http://smj.epnwcf.com

PHP:  $s === strrev($s);
来源：http://gfb.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://ooc.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://ktk.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kju.hywenlv.cn

Go:   // 双指针从两端比较
来源：http://nem.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://kaq.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://hui.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://lir.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ruw.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rav.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sxe.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://mdp.ywan-chungtsiang.top

Java: // 手写 HashMap
来源：http://zzt.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://bst.aibaodan.cn

Ruby: // 手写 Hash
来源：http://nlt.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://bfw.ivvv.top

[N08] 生成全排列
来源：http://gnb.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://xjx.zhengqikj.top

PHP:  // 手写递归交换
来源：http://und.iojbl.cn

JS:   // 手写回溯递归
来源：http://kdl.yj202588.top

TS:   // 手写回溯递归
来源：http://gum.havefunace.top

Java: // 手写回溯递归
来源：http://ecf.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://alf.yj20258888.top

Ruby: arr.permutation.to_a
来源：http://hye.svipenyu.cn

C#:   // 手写回溯递归
来源：http://qsu.zdqjudy.top

[N09] 栈与队列
来源：http://jgi.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aql.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rqb.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oso.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ryr.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://swk.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dwe.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zwh.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wqx.hammf.cn

[N10] 链表节点定义
来源：http://xzr.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qnv.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tes.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mhf.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yut.tanke756.top

Java: class Node { int v; Node next; }
来源：http://mst.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://fxi.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://edm.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xdg.hywenlv.cn

[N11] 二叉树中序遍历
来源：http://oav.epnwcf.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bwd.fzhhl.top

PHP:  // 手写递归函数
来源：http://bit.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://snr.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jqn.feifeiyinyue.top

Java: // 手写递归
来源：http://ynq.sweek.top

Go:   // 手写递归
来源：http://igh.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sgi.sxryk.cn

C#:   // 手写递归
来源：http://nxt.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rua.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ydz.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sle.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://skw.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://weg.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://unm.sxryk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://koq.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://drn.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ghu.ybcxt.top

================================================================================
来源：http://zgd.xylfe.cn

O. 并发与异步
来源：http://vqr.daxiang520.top

================================================================================
来源：http://enb.cheryme.top

[O01] 启动一个线程
来源：http://viw.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fbe.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yux.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ktg.hysaishi.cn

TS:   // 同 JS
来源：http://xvq.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://wkp.ywan-chungtsiang.top

Go:   go f()
来源：http://hof.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://tvt.xuanzx.com

C#:   Task.Run(() => F());
来源：http://rxg.tanke756.top

[O02] 使用线程池
来源：http://zlg.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yky.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yum.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://mhv.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://mbq.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://bfl.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qzj.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mlc.hcnkem.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vht.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://wmr.svipenyu.cn

Py:   with lock: shared += 1
来源：http://uor.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://spl.zhoulong.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://myf.hywenlv.cn

TS:   // 同 JS
来源：http://yft.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://iho.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ybq.zdqjudy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sca.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://mqt.mhx1999.top

[O04] 定义异步函数并等待
来源：http://yqb.ivvv.top

Py:   async def f():⏎    await g()
来源：http://qnh.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qfs.andypj.xyz

JS:   async function f() { await g(); }
来源：http://son.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yyr.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ubp.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kkk.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://yru.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://snv.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://mop.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://odg.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yhc.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://rth.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://zvn.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mrs.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zpc.jianghu66.top

Ruby: threads.map(&:join)
来源：http://pla.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://sii.zhijiandao.cn

[O06] 使用进程池
来源：http://wey.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tuq.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cpa.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://jqm.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://qjr.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lac.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oqg.yj202588.top

Ruby: // fork 块
来源：http://wvs.hywenlv.cn

C#:   Parallel.For
来源：http://coe.jinghuilouyu.cn

================================================================================
来源：http://nuy.yanxiufei.cn

P. 常用工具函数
来源：http://cfk.bbcook.cn

================================================================================
来源：http://jnf.yvedp.cn

[P01] 生成 UUID
来源：http://qtz.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://epw.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rul.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://nst.316326.xyz

TS:   crypto.randomUUID()
来源：http://gks.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://dmv.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://ipv.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://dxz.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://sux.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://ihf.jinqigfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bwc.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kul.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ciw.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qjp.hfpthk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tti.hfpthk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qvg.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vts.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pro.zycfv.cn

[P03] 生成短随机字符串
来源：http://jwg.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pkb.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cee.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qzy.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tku.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hti.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hbp.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ora.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qly.tian-w.cn

[P04] 求长度
来源：http://qap.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yyu.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qds.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jae.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pdl.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://dag.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://jcm.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://svt.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://tif.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://vyg.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://afr.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wwl.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wwz.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://epc.hongshengwenyu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jss.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tus.hesvh.cn

Ruby: a == b
来源：http://jhj.epnwcf.com


<!-- 参考信息 -->