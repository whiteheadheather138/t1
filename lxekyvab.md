代发 wailian999

JS:   process.argv.slice(2)
来源：http://ksc.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://lxk.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://joq.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://cqf.fehbvm.com

Ruby: ARGV
来源：http://oxe.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://lue.wangshuangyany.cn

[M02] 读取环境变量
来源：http://fyo.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://prx.jinqigufen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sbu.shangyingyoupin.top

JS:   process.env.HOME
来源：http://fxu.jiagoushi.top

TS:   process.env.HOME
来源：http://xov.ivvv.top

Java: System.getenv("HOME")
来源：http://ugu.dashuyun.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hkh.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://fhb.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gvd.ctjpmb.com

[M03] 执行外部命令
来源：http://unx.yueranfly.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ddf.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yxd.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sjq.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://yla.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://flc.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nsi.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ekd.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://jtl.gogol.net.cn

[M04] 获取当前工作目录
来源：http://grl.ivvv.top

Py:   os.getcwd()
来源：http://lbi.hesvh.cn

PHP:  getcwd();
来源：http://kcv.fehbvm.com

JS:   process.cwd()
来源：http://ftt.yj20258.top

TS:   process.cwd()
来源：http://gbu.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://zyo.nanxuanxn.top

Go:   os.Getwd()
来源：http://gai.jinqigufen.top

Ruby: Dir.pwd
来源：http://xar.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://irv.ydjk.org.cn

[M05] 设置退出码
来源：http://vsq.jlsjyb.cn

Py:   sys.exit(1)
来源：http://cih.zdqjudy.top

PHP:  exit(1);
来源：http://tun.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://pum.zhoulong.xyz

TS:   process.exit(1)
来源：http://zbc.zdbjq.cn

Java: System.exit(1)
来源：http://eba.cashguo.top

Go:   os.Exit(1)
来源：http://fsu.vqdsnc.cn

Ruby: exit 1
来源：http://yad.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cko.dashuyun.cn

[M06] 向标准错误输出
来源：http://tky.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://mdw.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yno.zhiwuduotai.top

JS:   console.error("err")
来源：http://bix.9152youxi.cn

TS:   console.error("err")
来源：http://hyc.sweek.top

Java: System.err.println("err")
来源：http://avf.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://toj.jqgfzy.top

Ruby: warn "err"
来源：http://tik.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://ebg.andypj.xyz

[M07] 判断是否为主入口
来源：http://qnn.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://qnr.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tmm.fzhhl.top

JS:   require.main === module
来源：http://gmi.nanxuanxn.top

TS:   require.main === module
来源：http://hut.gogol.net.cn

Java: public static void main(String[] args)
来源：http://whp.hysaishi.cn

Go:   func main()
来源：http://zbs.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fmh.yuxming.cn

C#:   static void Main(string[] args)
来源：http://crj.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://fec.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://csv.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://pch.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://fns.dashuyun.cn

TS:   process.platform;  process.version
来源：http://akp.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gvb.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rlh.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sty.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://itv.quarkkingdee.top

================================================================================
来源：http://aqe.jinqigufen.top

N. 数据结构与算法
来源：http://xph.yueranfly.top

================================================================================
来源：http://wzp.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://jaf.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://csd.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lft.hnqzz.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://omx.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ttn.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://eme.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://zpt.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://xvd.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://kit.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://oat.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://nmc.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://twh.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://myd.hcnkem.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lhb.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oss.hnqzz.top

Go:   slices.Sort(arr)
来源：http://tfl.snrcjt.cn

Ruby: arr.sort
来源：http://dtj.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wyi.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://xnu.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aio.hysaishi.cn

PHP:  // 递归实现，或用 usort
来源：http://gzu.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uve.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://erv.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ftl.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vwx.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qag.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://bcr.tarul.cn

[N04] 斐波那契数列
来源：http://xst.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qgd.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pdj.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyv.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lrn.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qcx.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kyu.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kbg.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kjd.shanyushiyangtech.top

[N05] 最大公约数
来源：http://mfs.yuxming.cn

Py:   math.gcd(a, b)
来源：http://dod.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wyz.snrcjt.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://doi.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nym.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uyu.guowangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ggk.guannengcc.top

Ruby: a.gcd(b)
来源：http://knq.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fpa.guowangkeji.top

[N06] 判断回文字符串
来源：http://yad.fzhhl.top

Py:   s == s[::-1]
来源：http://vzv.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://fsj.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://pnr.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://rcn.yj20258.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://akc.smart0.xyz

Go:   // 双指针从两端比较
来源：http://ram.jlsjyb.cn

Ruby: s == s.reverse
来源：http://fkp.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tlm.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://pld.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gpo.hcnkem.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ycv.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://vzx.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://qwa.cheryme.top

Java: // 手写 HashMap
来源：http://afa.daria6918.cn

Go:   // 手写 map[int]int
来源：http://lkd.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://can.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://iwd.sxryk.cn

[N08] 生成全排列
来源：http://qha.tarul.cn

Py:   itertools.permutations(arr)
来源：http://atg.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://jwi.birdmap.top

JS:   // 手写回溯递归
来源：http://rnn.guannengcc.top

TS:   // 手写回溯递归
来源：http://fmy.hammf.cn

Java: // 手写回溯递归
来源：http://jdj.vehdjk.com

Go:   // 手写回溯递归
来源：http://chx.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://gdf.daxiang520.top

C#:   // 手写回溯递归
来源：http://dut.feifeiyinyue.top

[N09] 栈与队列
来源：http://guh.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uck.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zaw.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baj.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fyg.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdu.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gtd.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ilg.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gxh.meibo888.top

[N10] 链表节点定义
来源：http://wsa.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qnp.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kfz.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wii.xylfe.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oif.xuanzx.com

Java: class Node { int v; Node next; }
来源：http://jof.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://itz.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qpk.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xcc.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://hnf.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wau.jyoumei.cn

PHP:  // 手写递归函数
来源：http://zrq.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://esz.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zbn.sxryk.cn

Java: // 手写递归
来源：http://ick.zhijiandao.cn

Go:   // 手写递归
来源：http://ysx.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rdk.uphjek.com

C#:   // 手写递归
来源：http://gsa.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aiy.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lyw.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bei.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fzg.ppjwa.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvk.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uij.vqdsnc.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uhf.hongshengwenyu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qbh.feifeiyinyue.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qxp.fengsongda.top

================================================================================
来源：http://typ.yueranfly.top

O. 并发与异步
来源：http://jlf.fehbvm.com

================================================================================
来源：http://evl.dianchejie.cn

[O01] 启动一个线程
来源：http://yog.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kjr.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uwz.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tco.smart0.xyz

TS:   // 同 JS
来源：http://ojf.wangdashe.top

Java: new Thread(() -> f()).start()
来源：http://nry.jqgufenzy.top

Go:   go f()
来源：http://cdl.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://eqy.ybcxt.top

C#:   Task.Run(() => F());
来源：http://wxz.aibaodan.cn

[O02] 使用线程池
来源：http://aph.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hdb.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qdf.birdmap.top

JS:   // worker_threads 线程池
来源：http://lxy.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://rxe.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dir.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xrd.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kml.yvedp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xpt.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://spw.daxiang520.top

Py:   with lock: shared += 1
来源：http://bdi.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://kkt.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qxw.wangdashe.top

TS:   // 同 JS
来源：http://xnw.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://jto.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mtr.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rea.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://wza.zhijiandao.cn

[O04] 定义异步函数并等待
来源：http://wam.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://kcp.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rxo.mhx1999.top

JS:   async function f() { await g(); }
来源：http://hxs.316326.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://cdl.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iyf.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gjl.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://vqh.cheryme.top

C#:   async Task F() { await G(); }
来源：http://vkv.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://ibp.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://ftj.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://trg.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://drj.sweek.top

TS:   await Promise.all(tasks)
来源：http://wkh.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hxn.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zpa.316326.xyz

Ruby: threads.map(&:join)
来源：http://jmw.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qeo.zhijiandao.cn

[O06] 使用进程池
来源：http://zre.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dpd.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uzu.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://sou.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://rib.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mef.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zuh.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://gpg.wangshuangyany.cn

C#:   Parallel.For
来源：http://bud.jqgufenzy.top

================================================================================
来源：http://lkz.wangdashe.top

P. 常用工具函数
来源：http://tfc.chenzaomai.com

================================================================================
来源：http://cyt.daria6918.cn

[P01] 生成 UUID
来源：http://hlj.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://uwv.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uir.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://iei.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://vvu.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://qff.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://acp.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://bqu.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://xco.guannengcc.top

[P02] MD5 / SHA256 摘要
来源：http://kjl.aibaodan.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dwc.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vdj.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://psd.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ecl.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ibi.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oaj.redwolf501.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hmv.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://twq.fengsongda.top

[P03] 生成短随机字符串
来源：http://xyi.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://epx.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bcb.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xzm.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hxi.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fmw.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lad.shanyushiyangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://eja.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://peb.shanyushiyangkeji.top

[P04] 求长度
来源：http://ugl.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cde.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dmo.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqz.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtb.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://lfb.sxryk.cn

Go:   len(arr);  len(m)
来源：http://lbc.birdmap.top

Ruby: x.length;  x.size
来源：http://ndv.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jfn.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://hpa.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uzt.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kmw.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://der.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ojc.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://alu.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gzt.jinyuanbaomall.cn

Ruby: a == b
来源：http://sqn.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cdk.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://anq.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dsz.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://rzb.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bvg.0kj1m.cn

TS:   if (x == null) {}
来源：http://nxy.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qgz.pycfn.com

Go:   if x == nil {}
来源：http://prr.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uqr.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://gxp.zycfv.cn

[P07] 防抖与节流
来源：http://liv.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rgm.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://yuu.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aks.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdg.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bfs.bjfxy.top


<!-- 参考信息 -->