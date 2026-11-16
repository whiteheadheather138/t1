代发 wailian999

JS:   process.argv.slice(2)
来源：http://mbg.dianchejie.cn

TS:   process.argv.slice(2)
来源：http://fml.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://hsz.snrcjt.cn

Go:   os.Args[1:]
来源：http://vyk.c1oappe.top

Ruby: ARGV
来源：http://rao.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://ckj.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://nga.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://gvo.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lqs.quarkkingdee.top

JS:   process.env.HOME
来源：http://hjx.guowangkeji.top

TS:   process.env.HOME
来源：http://esc.gotoacloud.top

Java: System.getenv("HOME")
来源：http://wrb.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hku.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://wou.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ahh.tanke756.top

[M03] 执行外部命令
来源：http://gnx.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://coc.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ngz.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tsw.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://dvu.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ddj.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cfm.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://hao.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://jhr.xuetiantiany.cn

[M04] 获取当前工作目录
来源：http://qpp.cdnleiting.top

Py:   os.getcwd()
来源：http://rmg.snrcjt.cn

PHP:  getcwd();
来源：http://ydc.jqgfzy.top

JS:   process.cwd()
来源：http://qhq.redwolf501.top

TS:   process.cwd()
来源：http://agh.hcnkem.com

Java: Path.of("").toAbsolutePath()
来源：http://trd.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://pta.zhongyouzk.top

Ruby: Dir.pwd
来源：http://fgz.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://axc.guannengcc.top

[M05] 设置退出码
来源：http://tye.fengsongda.top

Py:   sys.exit(1)
来源：http://fch.jyoumei.cn

PHP:  exit(1);
来源：http://bpk.gzhubu.top

JS:   process.exit(1)
来源：http://ret.ydjk.org.cn

TS:   process.exit(1)
来源：http://zsj.dianchejie.cn

Java: System.exit(1)
来源：http://eze.jqgfzy.top

Go:   os.Exit(1)
来源：http://lio.pengpengdd.cyou

Ruby: exit 1
来源：http://pek.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wvk.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://acv.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://lyg.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://drw.c1oappe.top

JS:   console.error("err")
来源：http://oqi.epnwcf.com

TS:   console.error("err")
来源：http://dos.52xcode.cn

Java: System.err.println("err")
来源：http://ace.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bcp.fehbvm.com

Ruby: warn "err"
来源：http://ick.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://sbc.cdnleiting.top

[M07] 判断是否为主入口
来源：http://csa.yj20258.top

Py:   if __name__ == "__main__":
来源：http://jrt.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ibc.cqqwz.cn

JS:   require.main === module
来源：http://tll.xziqi.cn

TS:   require.main === module
来源：http://npm.aizwys.cn

Java: public static void main(String[] args)
来源：http://ztm.xylfe.cn

Go:   func main()
来源：http://qfn.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pde.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://rgl.daria6918.cn

[M08] 获取系统与运行时信息
来源：http://kzp.snrcjt.cn

Py:   platform.system();  platform.python_version()
来源：http://bmk.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://ymq.snrcjt.cn

JS:   process.platform;  process.version
来源：http://mbv.52xcode.cn

TS:   process.platform;  process.version
来源：http://tek.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://thc.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ymo.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hyp.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ffr.aizwys.cn

================================================================================
来源：http://dqm.guannengcc.top

N. 数据结构与算法
来源：http://ios.feifeiyinyue.top

================================================================================
来源：http://nmy.ydjk.org.cn

[N01] 二分查找（有序数组）
来源：http://atr.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://roz.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oon.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://niq.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bgo.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kqo.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://gxr.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://aux.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://brc.sjlbkw.cn

[N02] 排序（工程实践用内置实现）
来源：http://dmk.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://gwq.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://het.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nza.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://smy.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xgg.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://gmv.ydzc1.top

Ruby: arr.sort
来源：http://hwi.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bly.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://vif.ehwqpu.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rbp.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://gmk.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dyv.52xcode.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oum.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lha.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bny.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fxj.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://egh.iojbl.cn

[N04] 斐波那契数列
来源：http://nit.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qes.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lxp.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://usi.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oqx.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hqu.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ssv.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zrx.jyoumei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pem.cashguo.top

[N05] 最大公约数
来源：http://uev.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://qcu.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yxm.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vfb.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tag.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rkn.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nnj.cdnleiting.top

Ruby: a.gcd(b)
来源：http://ehi.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ckb.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://bxk.zdbjq.cn

Py:   s == s[::-1]
来源：http://uko.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://yao.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://dhq.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://jmh.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lsn.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://fax.jiagoushi.top

Ruby: s == s.reverse
来源：http://znb.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://djk.zhijiandao.cn

[N07] 两数之和（返回下标）
来源：http://qyx.epnwcf.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jvb.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hey.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://mmk.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://ntv.jinqigufen.top

Java: // 手写 HashMap
来源：http://nll.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://dsi.guowangkeji.top

Ruby: // 手写 Hash
来源：http://qzy.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://pau.nwbrower.top

[N08] 生成全排列
来源：http://fjr.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://wro.chenzaomai.com

PHP:  // 手写递归交换
来源：http://csw.bjfxy.top

JS:   // 手写回溯递归
来源：http://ywp.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://cmz.zycfv.cn

Java: // 手写回溯递归
来源：http://hcu.pycfn.com

Go:   // 手写回溯递归
来源：http://tnr.sufxvd.cn

Ruby: arr.permutation.to_a
来源：http://dux.zhixingplan.top

C#:   // 手写回溯递归
来源：http://mvc.yangfankeji.com

[N09] 栈与队列
来源：http://jsa.cheryme.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nnn.yanxiufei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pep.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zwu.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sif.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xqa.hnqzz.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bby.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kcx.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ddy.wangdashe.top

[N10] 链表节点定义
来源：http://grh.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rwu.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ivb.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sbv.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qpq.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://esk.ybcxt.top

Go:   type Node struct { V int; Next *Node }
来源：http://bop.hongshengwenyu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://eju.chenlongwang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wfy.bjfxy.top

[N11] 二叉树中序遍历
来源：http://rtf.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pwx.wangshuangyany.cn

PHP:  // 手写递归函数
来源：http://ptt.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eur.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eew.jinqigufen.top

Java: // 手写递归
来源：http://thk.wangshuangyany.cn

Go:   // 手写递归
来源：http://okm.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lqh.bbcook.cn

C#:   // 手写递归
来源：http://par.gogol.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zia.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nuw.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://umy.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hhx.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fud.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vgo.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qxq.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hbe.hcnkem.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pkg.fanxiaobao.xyz

================================================================================
来源：http://jut.fanxiaobao.xyz

O. 并发与异步
来源：http://qfb.pycfn.com

================================================================================
来源：http://iww.52xcode.cn

[O01] 启动一个线程
来源：http://pos.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hdg.snrcjt.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eko.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gzm.dianchejie.cn

TS:   // 同 JS
来源：http://pjo.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://chk.tianlin.xyz

Go:   go f()
来源：http://rbl.iojbl.cn

Ruby: Thread.new { f }
来源：http://zfo.yfazqb.com

C#:   Task.Run(() => F());
来源：http://xai.yueranfly.top

[O02] 使用线程池
来源：http://lkj.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oqr.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ocj.iojbl.cn

JS:   // worker_threads 线程池
来源：http://eta.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://ydf.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gps.wangdashe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gss.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zid.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wgq.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://ksb.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://frs.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://oxe.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bop.epnwcf.com

TS:   // 同 JS
来源：http://emi.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://tnk.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sxz.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://scp.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://wik.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://hgi.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://bwg.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://haj.ivvv.top

JS:   async function f() { await g(); }
来源：http://tzy.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://srz.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dbg.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iay.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qxi.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://gtf.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://pjw.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://nkb.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wec.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://fre.9152youxi.cn

TS:   await Promise.all(tasks)
来源：http://rsb.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oul.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bif.hnqzz.top

Ruby: threads.map(&:join)
来源：http://tji.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rzs.yj20258888.top

[O06] 使用进程池
来源：http://gfk.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xvo.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uvc.guannengcc.top

JS:   // child_process / cluster 模块
来源：http://bbe.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://oqv.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://khm.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lnd.yueranfly.top

Ruby: // fork 块
来源：http://tlo.yuanzhike.top

C#:   Parallel.For
来源：http://eix.hammf.cn

================================================================================
来源：http://egd.shuidangran.top

P. 常用工具函数
来源：http://kcb.shanyushiyangtech.top

================================================================================
来源：http://rwe.shzxlz.cn

[P01] 生成 UUID
来源：http://xyi.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://pay.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bfr.fehbvm.com

JS:   crypto.randomUUID()
来源：http://awd.bbcook.cn

TS:   crypto.randomUUID()
来源：http://sof.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://gvf.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://zuf.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://gsd.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://usz.zhaomingkeji.xyz

[P02] MD5 / SHA256 摘要
来源：http://xii.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vna.iojbl.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://quk.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jsa.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hlz.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uol.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xbj.tianlin.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gfh.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vtn.snrcjt.cn

[P03] 生成短随机字符串
来源：http://tlf.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dgy.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rhs.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://miw.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://daj.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ngo.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ngx.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://umo.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hhy.0kj1m.cn

[P04] 求长度
来源：http://qtv.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://czv.gogol.net.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vam.ivvv.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ufz.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mnw.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://jxt.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://wrp.jiagoushi.top

Ruby: x.length;  x.size
来源：http://hti.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lvz.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://uhq.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fad.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cnu.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fqy.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kco.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yhn.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://qsn.hfpthk.cn

Ruby: a == b
来源：http://enc.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wkq.uphjek.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jmq.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iap.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://mrn.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lvc.redwolf501.top

TS:   if (x == null) {}
来源：http://czo.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lwo.0kj1m.cn

Go:   if x == nil {}
来源：http://ooi.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sgc.gaohongyu789.top

C#:   if (x is null) {}
来源：http://riz.ehwqpu.com

[P07] 防抖与节流
来源：http://fxm.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://exy.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://gbr.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nqs.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rar.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uuu.tian-w.cn


<!-- 参考信息 -->