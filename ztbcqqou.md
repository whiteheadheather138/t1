代发 wailian999

Ruby: ARGV
来源：http://hyl.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://uzh.316326.xyz

[M02] 读取环境变量
来源：http://use.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://vqg.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mag.daria6918.cn

JS:   process.env.HOME
来源：http://tqj.tianlin.xyz

TS:   process.env.HOME
来源：http://yqm.fengsongda.top

Java: System.getenv("HOME")
来源：http://uva.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uup.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://iiv.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uib.hfpthk.cn

[M03] 执行外部命令
来源：http://xtz.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lgv.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zhi.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nev.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://yyu.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wsy.mhx1999.top

Go:   exec.Command("ls", "-l").Output()
来源：http://crd.316326.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://jor.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://jsd.jqgufenzy.top

[M04] 获取当前工作目录
来源：http://ipf.daxiang520.top

Py:   os.getcwd()
来源：http://cjc.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://sin.zycfv.cn

JS:   process.cwd()
来源：http://sdx.ctjpmb.com

TS:   process.cwd()
来源：http://ozr.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://cum.nwbrower.top

Go:   os.Getwd()
来源：http://eud.dashuyun.cn

Ruby: Dir.pwd
来源：http://rcl.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://jwh.vqdsnc.cn

[M05] 设置退出码
来源：http://owf.jianghu66.top

Py:   sys.exit(1)
来源：http://aoh.chenjidiqi.icu

PHP:  exit(1);
来源：http://keo.gogol.net.cn

JS:   process.exit(1)
来源：http://dhp.chenjidiqi.icu

TS:   process.exit(1)
来源：http://zge.shanyushiyangtech.top

Java: System.exit(1)
来源：http://mtq.zhixingplan.top

Go:   os.Exit(1)
来源：http://ale.snrcjt.cn

Ruby: exit 1
来源：http://pgi.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yti.jianghu66.top

[M06] 向标准错误输出
来源：http://toi.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://fpv.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tyn.hfpthk.cn

JS:   console.error("err")
来源：http://qng.nwbrower.top

TS:   console.error("err")
来源：http://wqh.hysaishi.cn

Java: System.err.println("err")
来源：http://zou.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xhe.jqgufenzy.top

Ruby: warn "err"
来源：http://uwt.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://liz.sweek.top

[M07] 判断是否为主入口
来源：http://tsy.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://tct.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dsn.ppjwa.cn

JS:   require.main === module
来源：http://iic.pycfn.com

TS:   require.main === module
来源：http://kfo.cdnleiting.top

Java: public static void main(String[] args)
来源：http://vfj.yj20258888.top

Go:   func main()
来源：http://cyg.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nfh.zhiwuduotai.top

C#:   static void Main(string[] args)
来源：http://ukt.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://ybx.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://ynd.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://tem.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://ylu.aizwys.cn

TS:   process.platform;  process.version
来源：http://plt.vqdsnc.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cud.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mft.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mmk.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dpn.shzxlz.cn

================================================================================
来源：http://ido.fengsongda.top

N. 数据结构与算法
来源：http://vkf.feifeiyinyue.top

================================================================================
来源：http://dhf.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://zgo.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nkv.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pgu.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ldq.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vlq.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://nlt.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://bbu.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gfp.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://sal.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://ppd.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://ezw.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wci.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fuo.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wec.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tyf.tianlin.xyz

Go:   slices.Sort(arr)
来源：http://uqa.jqgufenzy.top

Ruby: arr.sort
来源：http://ybi.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gem.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://ajx.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kav.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://nel.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfw.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xck.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://htu.fktsv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uag.hywenlv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fnl.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://ctu.shuidangran.top

[N04] 斐波那契数列
来源：http://xic.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ptz.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ttc.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zqt.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kqj.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tgz.52xcode.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vor.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://icb.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rvj.ybcxt.top

[N05] 最大公约数
来源：http://vmm.yvedp.cn

Py:   math.gcd(a, b)
来源：http://ctk.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bbc.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gqx.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmz.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xkw.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mbm.vehdjk.com

Ruby: a.gcd(b)
来源：http://euv.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fzj.yj20258888.top

[N06] 判断回文字符串
来源：http://xtc.zhijiandao.cn

Py:   s == s[::-1]
来源：http://ydd.316326.xyz

PHP:  $s === strrev($s);
来源：http://nro.sxryk.cn

JS:   s === [...s].reverse().join("")
来源：http://gaf.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://bch.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xwt.cashguo.top

Go:   // 双指针从两端比较
来源：http://gnz.chenlongwang.top

Ruby: s == s.reverse
来源：http://adq.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://isd.hnxiangtu.top

[N07] 两数之和（返回下标）
来源：http://mof.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://srv.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uxt.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xhz.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://brf.yongpay.top

Java: // 手写 HashMap
来源：http://jcg.jyoumei.cn

Go:   // 手写 map[int]int
来源：http://iob.jqgufenzy.top

Ruby: // 手写 Hash
来源：http://qxc.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://kuf.cucudq.cn

[N08] 生成全排列
来源：http://iuw.cashguo.top

Py:   itertools.permutations(arr)
来源：http://vrb.hfpthk.cn

PHP:  // 手写递归交换
来源：http://qsr.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://oii.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://ezl.zhixingplan.top

Java: // 手写回溯递归
来源：http://cvh.uphjek.com

Go:   // 手写回溯递归
来源：http://awf.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://kxw.yueranfly.top

C#:   // 手写回溯递归
来源：http://snt.tarul.cn

[N09] 栈与队列
来源：http://dlp.sufxvd.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fwm.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://doz.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ski.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tht.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uiq.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hbg.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kxi.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dmn.sufxvd.cn

[N10] 链表节点定义
来源：http://gjq.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vss.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ehc.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mfe.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tly.svipenyu.cn

Java: class Node { int v; Node next; }
来源：http://bkf.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cri.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://iqq.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eis.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://miv.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://htz.yanxiufei.cn

PHP:  // 手写递归函数
来源：http://sqd.cucudq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kmm.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ang.jinqigufen.top

Java: // 手写递归
来源：http://xep.dianchejie.cn

Go:   // 手写递归
来源：http://sgw.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kuq.chenlongwang.top

C#:   // 手写递归
来源：http://tcm.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kni.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jvq.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uzq.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cag.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sad.hammf.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://irc.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vdv.hnqzz.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kuu.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jtq.mhx1999.top

================================================================================
来源：http://pyo.bjfxy.top

O. 并发与异步
来源：http://ttz.guowangkeji.top

================================================================================
来源：http://ina.zhijiandao.cn

[O01] 启动一个线程
来源：http://yjs.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xne.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vtt.svipenyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yrj.zhiwuduotai.top

TS:   // 同 JS
来源：http://mjw.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://byy.guowangkeji.top

Go:   go f()
来源：http://keo.dashuyun.cn

Ruby: Thread.new { f }
来源：http://ulw.jiagoushi.top

C#:   Task.Run(() => F());
来源：http://vqe.gogol.net.cn

[O02] 使用线程池
来源：http://cmt.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://itk.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://del.redwolf501.top

JS:   // worker_threads 线程池
来源：http://qzv.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://vnl.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://wbk.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hzc.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wqp.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://upa.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://yhz.hysaishi.cn

Py:   with lock: shared += 1
来源：http://xgt.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://brw.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rbe.52xcode.cn

TS:   // 同 JS
来源：http://soy.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://lng.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oae.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lyt.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://hdq.meibo888.top

[O04] 定义异步函数并等待
来源：http://kcs.pycfn.com

Py:   async def f():⏎    await g()
来源：http://hgz.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rsj.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://ozn.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dbi.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bnb.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vqn.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zas.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://lhh.chenjidiqi.icu

[O05] 并发执行并等待全部完成
来源：http://enj.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://ind.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qyb.yuanzhike.top

JS:   await Promise.all(tasks)
来源：http://sfa.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://xcz.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tat.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rde.fzhhl.top

Ruby: threads.map(&:join)
来源：http://xxd.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lqc.yj20258.top

[O06] 使用进程池
来源：http://ncn.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qfn.mhx1999.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pcb.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://tea.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://uxi.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dgl.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vhz.smart0.xyz

Ruby: // fork 块
来源：http://nlx.xuanzx.com

C#:   Parallel.For
来源：http://yta.dianchejie.cn

================================================================================
来源：http://gqm.chenzaomai.com

P. 常用工具函数
来源：http://btn.sjlbkw.cn

================================================================================
来源：http://hnf.shzxlz.cn

[P01] 生成 UUID
来源：http://dxd.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://kts.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nnk.tarul.cn

JS:   crypto.randomUUID()
来源：http://ftb.daria6918.cn

TS:   crypto.randomUUID()
来源：http://sne.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://hru.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://lsz.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://gur.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://woh.tanke756.top

[P02] MD5 / SHA256 摘要
来源：http://ppi.gaohongyu789.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://owo.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gjq.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tjr.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rbi.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nga.316326.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oxa.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kvd.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xoe.jqgfzy.top

[P03] 生成短随机字符串
来源：http://fhf.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zvn.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://otc.andypj.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bdy.aibaodan.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jsy.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yxt.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amt.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bal.nanxinkj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bfu.guannengcc.top

[P04] 求长度
来源：http://mad.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ahm.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ljr.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ufl.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jtt.svipenyu.cn

Java: list.size();  map.size();  s.length()
来源：http://qtw.xziqi.cn

Go:   len(arr);  len(m)
来源：http://cjy.bbcook.cn

Ruby: x.length;  x.size
来源：http://nfv.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://acm.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://tyi.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nof.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nyr.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xrb.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aci.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxl.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cqk.shzxlz.cn

Ruby: a == b
来源：http://hpj.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rpn.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hux.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fdu.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://aml.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xze.bjfxy.top

TS:   if (x == null) {}
来源：http://iip.wangshuangyany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yuv.jyoumei.cn

Go:   if x == nil {}
来源：http://wfr.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dtw.bbcook.cn

C#:   if (x is null) {}
来源：http://pgh.fehbvm.com

[P07] 防抖与节流
来源：http://oqx.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vjb.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://thv.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ocs.ybcxt.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tnf.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xem.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nue.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://upe.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rxq.cheryme.top

[P08] 处理浮点精度问题
来源：http://zju.xylfe.cn


<!-- 参考信息 -->