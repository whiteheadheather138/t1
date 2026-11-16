代发 wailian999

JS:   process.argv.slice(2)
来源：http://rdf.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://wiy.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://nti.aibaodan.cn

Go:   os.Args[1:]
来源：http://hhb.zhongyouzk.top

Ruby: ARGV
来源：http://scn.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://non.fzhhl.top

[M02] 读取环境变量
来源：http://edc.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://mhe.jinqigfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://arj.xziqi.cn

JS:   process.env.HOME
来源：http://lir.vqdsnc.cn

TS:   process.env.HOME
来源：http://cqq.pycfn.com

Java: System.getenv("HOME")
来源：http://rql.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://clf.smart0.xyz

Ruby: ENV["HOME"]
来源：http://hqm.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wsm.yueranfly.top

[M03] 执行外部命令
来源：http://ozn.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ixr.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zcx.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xnw.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ggc.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://klv.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ahb.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://kgt.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://nye.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://xqo.jianghu66.top

Py:   os.getcwd()
来源：http://zqb.yanxiufei.cn

PHP:  getcwd();
来源：http://hgk.xuanzx.com

JS:   process.cwd()
来源：http://vdi.hnqzz.top

TS:   process.cwd()
来源：http://lol.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://cha.fehbvm.com

Go:   os.Getwd()
来源：http://rjj.ybcxt.top

Ruby: Dir.pwd
来源：http://mxa.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://tdq.zycfv.cn

[M05] 设置退出码
来源：http://cxt.smart0.xyz

Py:   sys.exit(1)
来源：http://ygc.9152youxi.cn

PHP:  exit(1);
来源：http://ymz.vqdsnc.cn

JS:   process.exit(1)
来源：http://jmf.xuanzx.com

TS:   process.exit(1)
来源：http://zyt.hfpthk.cn

Java: System.exit(1)
来源：http://jws.gogol.net.cn

Go:   os.Exit(1)
来源：http://ozw.jianghu66.top

Ruby: exit 1
来源：http://plo.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sce.xinyue.icu

[M06] 向标准错误输出
来源：http://cug.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://ruo.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vzz.shangyingyoupin.top

JS:   console.error("err")
来源：http://pgw.ppjwa.cn

TS:   console.error("err")
来源：http://ntb.zhongyouzk.top

Java: System.err.println("err")
来源：http://wxy.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://czd.andypj.xyz

Ruby: warn "err"
来源：http://ycb.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://ale.havefunace.top

[M07] 判断是否为主入口
来源：http://xqj.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://ifg.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sla.nwbrower.top

JS:   require.main === module
来源：http://oub.jiagoushi.top

TS:   require.main === module
来源：http://ojn.birdmap.top

Java: public static void main(String[] args)
来源：http://nao.pycfn.com

Go:   func main()
来源：http://tdy.guowangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lpk.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://rhw.quarkkingdee.top

[M08] 获取系统与运行时信息
来源：http://nmt.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://szp.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://ldf.havefunace.top

JS:   process.platform;  process.version
来源：http://jsc.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://qbu.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fwc.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ltp.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tco.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gps.yuxming.cn

================================================================================
来源：http://mbg.jinqigfzy.top

N. 数据结构与算法
来源：http://cgw.xylfe.cn

================================================================================
来源：http://fox.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://pdk.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://fzn.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mim.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zlv.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gcx.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ceb.zdbjq.cn

Go:   sort.SearchInts(arr, x)
来源：http://yqn.shanyushiyangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://acr.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://dhu.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://rol.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://jza.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ijk.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bli.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vuz.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://doo.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://ryb.snrcjt.cn

Ruby: arr.sort
来源：http://xtu.kuanghao11.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bcg.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://zfv.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://obl.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://jhj.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnf.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fxt.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ago.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nav.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xge.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dtq.fzhhl.top

[N04] 斐波那契数列
来源：http://arm.dianchejie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ztz.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bmk.xuetiantiany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://noa.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpq.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cyf.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://syi.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fpc.aibaodan.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pdw.cheryme.top

[N05] 最大公约数
来源：http://zih.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://blg.sxryk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dzs.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qbb.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ftk.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sja.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rok.dashuyun.cn

Ruby: a.gcd(b)
来源：http://ike.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dnu.fzhhl.top

[N06] 判断回文字符串
来源：http://vex.haohaochexian.top

Py:   s == s[::-1]
来源：http://nll.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://jas.shuidangran.top

JS:   s === [...s].reverse().join("")
来源：http://wik.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://hfb.meibo888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rjf.yj20258.top

Go:   // 双指针从两端比较
来源：http://usu.meibo888.top

Ruby: s == s.reverse
来源：http://upn.hnxiangtu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://quv.yonumen.top

[N07] 两数之和（返回下标）
来源：http://xlh.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lrn.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nwq.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sne.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://qtf.0kj1m.cn

Java: // 手写 HashMap
来源：http://btw.epnwcf.com

Go:   // 手写 map[int]int
来源：http://env.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://yox.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://zcb.epnwcf.com

[N08] 生成全排列
来源：http://jvu.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://hmv.tarul.cn

PHP:  // 手写递归交换
来源：http://ivs.xylfe.cn

JS:   // 手写回溯递归
来源：http://xbl.nanxinkj.top

TS:   // 手写回溯递归
来源：http://xoe.redwolf501.top

Java: // 手写回溯递归
来源：http://axj.yj20258888.top

Go:   // 手写回溯递归
来源：http://skc.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://bvd.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://qir.gzhubu.top

[N09] 栈与队列
来源：http://rgy.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xaf.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fzv.vehdjk.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gsn.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ofy.meibo888.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gij.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fxv.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ivz.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dhl.ydjk.org.cn

[N10] 链表节点定义
来源：http://lhi.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kas.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://blb.yongpay.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://btt.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yjk.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://ozj.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pty.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hpy.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://app.yongpay.top

[N11] 二叉树中序遍历
来源：http://pvx.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lhe.0kj1m.cn

PHP:  // 手写递归函数
来源：http://yhu.pycfn.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upz.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jdz.aizwys.cn

Java: // 手写递归
来源：http://zkn.zhiwuduotai.top

Go:   // 手写递归
来源：http://ith.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pou.guannengcc.top

C#:   // 手写递归
来源：http://jjr.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kae.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wyk.aibaodan.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ldj.fktsv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kyt.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nfq.shanyushiyangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fev.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oyp.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pfx.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bew.zhijiandao.cn

================================================================================
来源：http://ahw.yongpay.top

O. 并发与异步
来源：http://bak.xziqi.cn

================================================================================
来源：http://rul.zhixingplan.top

[O01] 启动一个线程
来源：http://xhg.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mvx.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://byy.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kfv.nanxinkj.top

TS:   // 同 JS
来源：http://ywl.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://prp.gogol.net.cn

Go:   go f()
来源：http://pni.jqgfzy.top

Ruby: Thread.new { f }
来源：http://uiv.tanke756.top

C#:   Task.Run(() => F());
来源：http://ijp.jiagoushi.top

[O02] 使用线程池
来源：http://fyt.tian-w.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rww.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tne.nwbrower.top

JS:   // worker_threads 线程池
来源：http://fst.jianghu66.top

TS:   // worker_threads 线程池
来源：http://gsl.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://qpt.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pic.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tzt.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oka.tanke756.top

[O03] 加锁保护共享数据
来源：http://ggg.ctjpmb.com

Py:   with lock: shared += 1
来源：http://nyt.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cbo.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://egt.sysykeji.top

TS:   // 同 JS
来源：http://gvm.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://zrr.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fzl.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jbf.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://yzf.yonumen.top

[O04] 定义异步函数并等待
来源：http://vfw.yonumen.top

Py:   async def f():⏎    await g()
来源：http://ljm.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gbt.hnqzz.top

JS:   async function f() { await g(); }
来源：http://lxh.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://myf.hammf.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nij.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fdy.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bvi.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://qds.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://cex.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://mik.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://elh.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://ysj.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://hij.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hob.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kyu.yj20258888.top

Ruby: threads.map(&:join)
来源：http://fja.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bzg.fengsongda.top

[O06] 使用进程池
来源：http://yuy.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wfi.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ewr.cucudq.cn

JS:   // child_process / cluster 模块
来源：http://cyg.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://oab.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yvz.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zwh.xuanzx.com

Ruby: // fork 块
来源：http://ovu.ctjpmb.com

C#:   Parallel.For
来源：http://xss.hammf.cn

================================================================================
来源：http://quy.nwbrower.top

P. 常用工具函数
来源：http://jzm.wangdashe.top

================================================================================
来源：http://dcx.tianlin.xyz

[P01] 生成 UUID
来源：http://xne.tarul.cn

Py:   str(uuid.uuid4())
来源：http://fuc.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yqi.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://frw.jianghu66.top

TS:   crypto.randomUUID()
来源：http://fdg.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://qjx.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://rcf.yonumen.top

Ruby: SecureRandom.uuid
来源：http://yfs.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://emk.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://xql.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ewn.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pju.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hvc.xylfe.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zti.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://soi.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dha.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ebl.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xbx.ybcxt.top

[P03] 生成短随机字符串
来源：http://caq.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fdh.hongshengwenyu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bkk.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jks.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ile.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vij.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vjp.pengpengdd.cyou

Ruby: SecureRandom.alphanumeric(16)
来源：http://gak.havefunace.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hcw.jinghuilouyu.cn

[P04] 求长度
来源：http://war.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qfy.hfpthk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mfa.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qtw.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qix.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://tag.tarul.cn

Go:   len(arr);  len(m)
来源：http://zoy.tarul.cn

Ruby: x.length;  x.size
来源：http://egs.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://txy.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://jev.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xmt.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cmm.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fjm.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hqr.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fqx.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aor.tianlin.xyz

Ruby: a == b
来源：http://rpc.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://psk.ydzc1.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vbr.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wqf.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://tnq.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ioz.fzhhl.top

TS:   if (x == null) {}
来源：http://poh.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fel.yj20258.top

Go:   if x == nil {}
来源：http://gvv.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iuw.yangfankeji.com

C#:   if (x is null) {}
来源：http://wcw.ydzc1.top

[P07] 防抖与节流
来源：http://qkz.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hmb.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://sdo.xuanzx.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fyw.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bcf.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oxd.tarul.cn


<!-- 参考信息 -->