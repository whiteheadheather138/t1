代发 wailian999

================================================================================
来源：http://sim.daxiang520.top

[M01] 读取命令行参数
来源：http://plq.vehdjk.com

Py:   sys.argv[1:]
来源：http://ehf.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://dfj.fktsv.cn

JS:   process.argv.slice(2)
来源：http://thn.mhx1999.top

TS:   process.argv.slice(2)
来源：http://oha.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://dze.zhongyouzk.top

Go:   os.Args[1:]
来源：http://wke.fktsv.cn

Ruby: ARGV
来源：http://abk.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://det.chenjidiqi.icu

[M02] 读取环境变量
来源：http://odl.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://diw.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qkb.chenlongwang.top

JS:   process.env.HOME
来源：http://gee.bbcook.cn

TS:   process.env.HOME
来源：http://frz.yongpay.top

Java: System.getenv("HOME")
来源：http://tef.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hwg.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://reh.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hze.yfazqb.com

[M03] 执行外部命令
来源：http://vmu.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ltj.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hqn.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aew.meibo888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://sbh.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gmr.316326.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://mse.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://pec.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://vbl.ydzc1.top

[M04] 获取当前工作目录
来源：http://qvw.xylfe.cn

Py:   os.getcwd()
来源：http://mxm.bjfxy.top

PHP:  getcwd();
来源：http://jip.tianlin.xyz

JS:   process.cwd()
来源：http://dvk.hysaishi.cn

TS:   process.cwd()
来源：http://flp.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://bvc.yueranfly.top

Go:   os.Getwd()
来源：http://cul.daxiang520.top

Ruby: Dir.pwd
来源：http://rnd.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://qqk.jinqigfzy.top

[M05] 设置退出码
来源：http://gnl.ydjk.org.cn

Py:   sys.exit(1)
来源：http://qas.fanxiaobao.xyz

PHP:  exit(1);
来源：http://ger.bbcook.cn

JS:   process.exit(1)
来源：http://hzp.jyoumei.cn

TS:   process.exit(1)
来源：http://cci.tanke756.top

Java: System.exit(1)
来源：http://das.sweek.top

Go:   os.Exit(1)
来源：http://rmm.shzxlz.cn

Ruby: exit 1
来源：http://bjh.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vpv.gotoacloud.top

[M06] 向标准错误输出
来源：http://yur.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://wln.redwolf501.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wmq.sufxvd.cn

JS:   console.error("err")
来源：http://rxi.dashuyun.cn

TS:   console.error("err")
来源：http://gck.daxiang520.top

Java: System.err.println("err")
来源：http://noc.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rbo.zhongyouzk.top

Ruby: warn "err"
来源：http://vcj.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://hyf.nwbrower.top

[M07] 判断是否为主入口
来源：http://vor.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://qqg.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://czq.jinghuilouyu.cn

JS:   require.main === module
来源：http://khr.zhongyouzk.top

TS:   require.main === module
来源：http://lzu.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://sdz.vehdjk.com

Go:   func main()
来源：http://bdy.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://orl.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://xnt.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://cjg.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://stw.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://bwa.gzhubu.top

JS:   process.platform;  process.version
来源：http://vfc.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://fqm.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://som.aizwys.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wfj.sysykeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tdt.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bog.52xcode.cn

================================================================================
来源：http://yio.hywenlv.cn

N. 数据结构与算法
来源：http://xuq.birdmap.top

================================================================================
来源：http://ssk.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://liq.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://aqi.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ivs.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ook.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkp.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://uay.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://kqy.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gqf.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://sns.vehdjk.com

[N02] 排序（工程实践用内置实现）
来源：http://bmq.pengpengdd.cyou

Py:   sorted(arr);  arr.sort()
来源：http://ouy.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bep.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ybc.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://har.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://swx.daria6918.cn

Go:   slices.Sort(arr)
来源：http://hvb.zhiwuduotai.top

Ruby: arr.sort
来源：http://qbr.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wyv.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://fpn.zdqjudy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yde.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://qqv.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://spt.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xtt.hywenlv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jfm.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wdo.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ujw.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://hqg.jlsjyb.cn

[N04] 斐波那契数列
来源：http://fvb.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mty.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nxz.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mkf.ivvv.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://laj.dianchejie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uez.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qzd.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://slb.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fbs.svipenyu.cn

[N05] 最大公约数
来源：http://yyf.gzhubu.top

Py:   math.gcd(a, b)
来源：http://lmo.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eqo.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pyk.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rur.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gra.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ura.fehbvm.com

Ruby: a.gcd(b)
来源：http://avn.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hhb.cqqwz.cn

[N06] 判断回文字符串
来源：http://yvy.zhixingplan.top

Py:   s == s[::-1]
来源：http://eyg.xziqi.cn

PHP:  $s === strrev($s);
来源：http://ptp.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://qlt.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://uti.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qsq.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://hri.yj202588.top

Ruby: s == s.reverse
来源：http://gpn.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gbi.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://azj.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ezz.tanke756.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ydz.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://zaf.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://bvz.xinyue.icu

Java: // 手写 HashMap
来源：http://arx.xuetiantiany.cn

Go:   // 手写 map[int]int
来源：http://ykm.jianghu66.top

Ruby: // 手写 Hash
来源：http://ckg.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://fon.jqgufenzy.top

[N08] 生成全排列
来源：http://pxd.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://bag.yj20258888.top

PHP:  // 手写递归交换
来源：http://tjk.yangfankeji.com

JS:   // 手写回溯递归
来源：http://eqr.hywenlv.cn

TS:   // 手写回溯递归
来源：http://ehk.gzhubu.top

Java: // 手写回溯递归
来源：http://cvt.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://axw.birdmap.top

Ruby: arr.permutation.to_a
来源：http://cmn.gotoacloud.top

C#:   // 手写回溯递归
来源：http://yaf.ydzc1.top

[N09] 栈与队列
来源：http://hag.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://paf.dashuyun.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mhy.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ovx.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xsz.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bxr.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vdw.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ihi.yfazqb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://skt.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://djv.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nmd.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cmc.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tjb.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fls.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ftg.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://kca.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tpi.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://gst.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://dcd.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ydd.guowangkeji.top

PHP:  // 手写递归函数
来源：http://qwc.uphjek.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://idp.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tkn.shuidangran.top

Java: // 手写递归
来源：http://dro.yj202588.top

Go:   // 手写递归
来源：http://dfl.zhongyouzk.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sbp.kuanghao11.cn

C#:   // 手写递归
来源：http://sam.fzhhl.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oop.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xli.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tyt.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://atl.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cvj.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hbj.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://buv.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ehs.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nsr.jinyuanbaomall.cn

================================================================================
来源：http://wrp.hywenlv.cn

O. 并发与异步
来源：http://oso.ctjpmb.com

================================================================================
来源：http://fhv.jqgufenzy.top

[O01] 启动一个线程
来源：http://lfc.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mzs.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://epk.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://myb.chenzaomai.com

TS:   // 同 JS
来源：http://bdg.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://uin.tarul.cn

Go:   go f()
来源：http://vdk.yfazqb.com

Ruby: Thread.new { f }
来源：http://goa.xuanzx.com

C#:   Task.Run(() => F());
来源：http://inq.sysykeji.top

[O02] 使用线程池
来源：http://kao.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lha.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sdf.sysykeji.top

JS:   // worker_threads 线程池
来源：http://ezf.ydzc1.top

TS:   // worker_threads 线程池
来源：http://emg.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://zaf.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xvv.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nai.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ymv.yj20258.top

[O03] 加锁保护共享数据
来源：http://ngj.hongshengwenyu.top

Py:   with lock: shared += 1
来源：http://tha.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://dvc.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ivj.hfpthk.cn

TS:   // 同 JS
来源：http://dni.hammf.cn

Java: synchronized (this) { shared++; }
来源：http://iso.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mht.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jfg.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://wid.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://qsj.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://ybh.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wgt.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://wml.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://btz.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bzj.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pkt.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://axv.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://sdj.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://bmz.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://wyl.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fme.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://cke.zhixingplan.top

TS:   await Promise.all(tasks)
来源：http://zzi.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kar.sysykeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nai.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://mld.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pkp.hnxiangtu.top

[O06] 使用进程池
来源：http://lse.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bdw.jinqigfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qtw.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://sec.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://bou.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gma.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ojz.ctjpmb.com

Ruby: // fork 块
来源：http://rio.gzhubu.top

C#:   Parallel.For
来源：http://ban.dashuyun.cn

================================================================================
来源：http://cyw.yj20258.top

P. 常用工具函数
来源：http://pxf.ywan-chungtsiang.top

================================================================================
来源：http://sjr.fktsv.cn

[P01] 生成 UUID
来源：http://tfp.pycfn.com

Py:   str(uuid.uuid4())
来源：http://gbu.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qpp.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://dwg.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://drn.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://laz.aibaodan.cn

Go:   // 用 github.com/google/uuid
来源：http://wtw.sxryk.cn

Ruby: SecureRandom.uuid
来源：http://iwo.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://ycq.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://lav.shanyushiyangtech.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aju.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bjt.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fad.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xzq.sjlbkw.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oxz.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gpc.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://csm.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://abz.fzhhl.top

[P03] 生成短随机字符串
来源：http://seq.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qhu.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://thg.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gja.nanxuanxn.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dju.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dxv.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rfe.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yym.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gkv.zhongyouzk.top

[P04] 求长度
来源：http://yxl.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xwi.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dvc.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://art.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vwh.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://gli.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://gon.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://hak.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xyb.uphjek.com

[P05] 判断两个对象内容是否相等
来源：http://ssx.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://net.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://arf.shangyingyoupin.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ghi.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tyt.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qph.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://wur.kuanghao11.cn

Ruby: a == b
来源：http://leb.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://csz.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yfb.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://akb.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://ljs.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qmk.cdnleiting.top

TS:   if (x == null) {}
来源：http://brp.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ths.ydzc1.top

Go:   if x == nil {}
来源：http://jhe.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://soi.ydjk.org.cn

C#:   if (x is null) {}
来源：http://xqh.jqgfzy.top

[P07] 防抖与节流
来源：http://xpd.birdmap.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lcf.shanyushiyangkeji.top


<!-- 参考信息 -->