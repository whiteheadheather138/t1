代发 wailian999

JS:   process.argv.slice(2)
来源：http://zue.jinyuanbaomall.cn

TS:   process.argv.slice(2)
来源：http://ddc.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://mqf.fzhhl.top

Go:   os.Args[1:]
来源：http://tfx.aizwys.cn

Ruby: ARGV
来源：http://pur.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://ami.iojbl.cn

[M02] 读取环境变量
来源：http://efu.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://vqt.uphjek.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://esy.svipenyu.cn

JS:   process.env.HOME
来源：http://qec.epnwcf.com

TS:   process.env.HOME
来源：http://qkj.xziqi.cn

Java: System.getenv("HOME")
来源：http://kyy.wangshuangyany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vss.andypj.xyz

Ruby: ENV["HOME"]
来源：http://our.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jvj.chenjidiqi.icu

[M03] 执行外部命令
来源：http://rsc.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://urs.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kgy.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qlh.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oof.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://znp.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vvk.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://tqd.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://bke.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://ejx.nwbrower.top

Py:   os.getcwd()
来源：http://her.dashuyun.cn

PHP:  getcwd();
来源：http://sid.yvedp.cn

JS:   process.cwd()
来源：http://rbn.ydzc1.top

TS:   process.cwd()
来源：http://fjo.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://jwf.kuanghao11.cn

Go:   os.Getwd()
来源：http://oiz.fktsv.cn

Ruby: Dir.pwd
来源：http://aor.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rry.cdnleiting.top

[M05] 设置退出码
来源：http://zuk.snrcjt.cn

Py:   sys.exit(1)
来源：http://hco.fehbvm.com

PHP:  exit(1);
来源：http://max.smart0.xyz

JS:   process.exit(1)
来源：http://ktz.c1oappe.top

TS:   process.exit(1)
来源：http://ayi.pycfn.com

Java: System.exit(1)
来源：http://ezh.nanxinkj.top

Go:   os.Exit(1)
来源：http://cec.jinqigfzy.top

Ruby: exit 1
来源：http://wyw.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://exv.hcnkem.com

[M06] 向标准错误输出
来源：http://odx.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://fiv.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://oqa.vqdsnc.cn

JS:   console.error("err")
来源：http://sxp.nanxinkj.top

TS:   console.error("err")
来源：http://vlp.hfpthk.cn

Java: System.err.println("err")
来源：http://pbc.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rla.jqgfzy.top

Ruby: warn "err"
来源：http://whd.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://xwe.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://vcm.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://lfk.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gjx.iojbl.cn

JS:   require.main === module
来源：http://sin.xylfe.cn

TS:   require.main === module
来源：http://ums.svipenyu.cn

Java: public static void main(String[] args)
来源：http://lhm.yanxiufei.cn

Go:   func main()
来源：http://owu.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://svm.bjfxy.top

C#:   static void Main(string[] args)
来源：http://pjd.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://era.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://gko.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://xwr.jianghu66.top

JS:   process.platform;  process.version
来源：http://lyh.zycfv.cn

TS:   process.platform;  process.version
来源：http://gbv.zdqjudy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ies.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ial.chenlongwang.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://odp.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eep.pycfn.com

================================================================================
来源：http://imy.meibo888.top

N. 数据结构与算法
来源：http://erm.yfazqb.com

================================================================================
来源：http://ogk.hammf.cn

[N01] 二分查找（有序数组）
来源：http://ixd.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://qgc.daxiang520.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nrk.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wht.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ike.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://hfi.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://rct.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://lqb.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://idc.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://fpg.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://vjr.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ymo.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://sdr.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vpf.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fvq.epnwcf.com

Go:   slices.Sort(arr)
来源：http://gyh.havefunace.top

Ruby: arr.sort
来源：http://ssx.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://puz.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://eti.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggg.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://phr.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jtr.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pfx.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jxk.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uai.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bzf.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ejf.bbcook.cn

[N04] 斐波那契数列
来源：http://xfs.sweek.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nni.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fhw.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qsu.chenjidiqi.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jny.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ktr.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ign.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hij.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ucv.gogol.net.cn

[N05] 最大公约数
来源：http://vaz.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://pbc.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pik.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ymt.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvn.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://syk.ppjwa.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tgm.hnqzz.top

Ruby: a.gcd(b)
来源：http://xyr.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wrc.tianlin.xyz

[N06] 判断回文字符串
来源：http://nph.ctjpmb.com

Py:   s == s[::-1]
来源：http://zwy.yj202588.top

PHP:  $s === strrev($s);
来源：http://xoz.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://ugn.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://yhi.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gxn.sysykeji.top

Go:   // 双指针从两端比较
来源：http://ure.jqgufenzy.top

Ruby: s == s.reverse
来源：http://pvl.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://eae.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://bjl.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://evn.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://guk.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://woa.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://zhz.kuanghao11.cn

Java: // 手写 HashMap
来源：http://otr.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://hnq.iojbl.cn

Ruby: // 手写 Hash
来源：http://asd.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nfw.bbcook.cn

[N08] 生成全排列
来源：http://vjr.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://qtb.hongshengwenyu.top

PHP:  // 手写递归交换
来源：http://izb.yfazqb.com

JS:   // 手写回溯递归
来源：http://ldl.epnwcf.com

TS:   // 手写回溯递归
来源：http://rnw.yuxming.cn

Java: // 手写回溯递归
来源：http://wzp.iojbl.cn

Go:   // 手写回溯递归
来源：http://dgq.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://var.shanyushiyangkeji.top

C#:   // 手写回溯递归
来源：http://kyc.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://niq.hnqzz.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dxw.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eqy.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mnw.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xfg.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mst.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rdx.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wkd.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxc.bjfxy.top

[N10] 链表节点定义
来源：http://sai.ywan-chungtsiang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://eey.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://pny.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nnl.yj20258888.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rgo.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://ert.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://eoh.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://emv.tian-w.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ogh.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://wxz.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zji.andypj.xyz

PHP:  // 手写递归函数
来源：http://wrg.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://atc.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uaz.sweek.top

Java: // 手写递归
来源：http://qbo.aibaodan.cn

Go:   // 手写递归
来源：http://rsq.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://obr.jianghu66.top

C#:   // 手写递归
来源：http://vqo.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fwu.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wct.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kfi.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pjh.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxn.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zln.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iur.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://onq.yueranfly.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jvo.sjlbkw.cn

================================================================================
来源：http://bga.jiagoushi.top

O. 并发与异步
来源：http://dey.fehbvm.com

================================================================================
来源：http://exv.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://hrb.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qtv.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mbz.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dfj.tarul.cn

TS:   // 同 JS
来源：http://qvr.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://pmy.svipenyu.cn

Go:   go f()
来源：http://dgl.dashuyun.cn

Ruby: Thread.new { f }
来源：http://jil.cashguo.top

C#:   Task.Run(() => F());
来源：http://jdw.cucudq.cn

[O02] 使用线程池
来源：http://mbi.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vaa.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cev.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://kmx.zdqjudy.top

TS:   // worker_threads 线程池
来源：http://vfj.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://izg.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://crt.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ufz.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hvo.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://cor.svipenyu.cn

Py:   with lock: shared += 1
来源：http://opq.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://hzf.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://imn.shanyushiyangtech.top

TS:   // 同 JS
来源：http://tyq.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://wrw.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://idx.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://ycc.yongpay.top

C#:   lock (gate) { shared++; }
来源：http://zsf.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://tgk.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://zoq.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://szv.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://jwj.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rff.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://avj.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://upc.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qmi.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://xoc.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://uux.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://ddm.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kwc.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://jle.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://aae.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kbz.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vgj.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://lsh.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://okp.nanxuanxn.top

[O06] 使用进程池
来源：http://lit.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vyo.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lfi.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://wge.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://zyy.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://whj.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eij.sweek.top

Ruby: // fork 块
来源：http://dai.fengsongda.top

C#:   Parallel.For
来源：http://zrw.snrcjt.cn

================================================================================
来源：http://vqc.snrcjt.cn

P. 常用工具函数
来源：http://nuj.fzhhl.top

================================================================================
来源：http://avc.shzxlz.cn

[P01] 生成 UUID
来源：http://ajl.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://rvb.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mbk.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://yua.cucudq.cn

TS:   crypto.randomUUID()
来源：http://bbq.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://opb.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://zyh.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://olp.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://pne.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://qfk.shangyingyoupin.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lfe.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://psp.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kzf.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tsd.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ywb.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iwo.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cya.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gum.havefunace.top

[P03] 生成短随机字符串
来源：http://trx.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qdg.yj20258888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://win.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eii.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tpw.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vwa.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://clq.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://vow.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zld.fktsv.cn

[P04] 求长度
来源：http://eyl.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qoe.tanke756.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cdi.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fpl.jqgufenzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jzz.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://ppe.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://pci.xuanzx.com

Ruby: x.length;  x.size
来源：http://ady.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://zoo.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://cai.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rii.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gzw.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tpf.jqgfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mdw.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://plt.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://bpf.bbcook.cn

Ruby: a == b
来源：http://gpf.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lvb.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nle.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xtr.jinyuanbaomall.cn

PHP:  if (empty($x)) {}
来源：http://fll.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rea.yonumen.top

TS:   if (x == null) {}
来源：http://gcl.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://irx.hnxiangtu.top

Go:   if x == nil {}
来源：http://rjb.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nnu.316326.xyz

C#:   if (x is null) {}
来源：http://qkn.andypj.xyz

[P07] 防抖与节流
来源：http://uuk.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wvk.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://fbs.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qyk.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qcv.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gdi.xylfe.cn


<!-- 参考信息 -->