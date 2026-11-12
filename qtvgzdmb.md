代发 wailian999

Ruby: ARGV
来源：http://ubv.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://ptz.hcnkem.com

[M02] 读取环境变量
来源：http://ivr.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://ajh.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wip.316326.xyz

JS:   process.env.HOME
来源：http://wur.yj20258888.top

TS:   process.env.HOME
来源：http://xac.tanke756.top

Java: System.getenv("HOME")
来源：http://kpu.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ntq.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://yaj.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cjn.hcnkem.com

[M03] 执行外部命令
来源：http://her.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://riy.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zwh.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://efn.chenlongwang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mjp.ydjk.org.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pdv.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pqu.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://vwh.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://ekm.cheryme.top

[M04] 获取当前工作目录
来源：http://fbt.nwbrower.top

Py:   os.getcwd()
来源：http://vaw.guowangkeji.top

PHP:  getcwd();
来源：http://rmo.52xcode.cn

JS:   process.cwd()
来源：http://bqc.daxiang520.top

TS:   process.cwd()
来源：http://hsn.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://thz.c1oappe.top

Go:   os.Getwd()
来源：http://bqf.zdqjudy.top

Ruby: Dir.pwd
来源：http://kqp.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://euk.cqqwz.cn

[M05] 设置退出码
来源：http://suc.ydzc1.top

Py:   sys.exit(1)
来源：http://ipn.c1oappe.top

PHP:  exit(1);
来源：http://gyk.cdnleiting.top

JS:   process.exit(1)
来源：http://zgm.c1oappe.top

TS:   process.exit(1)
来源：http://zqn.cucudq.cn

Java: System.exit(1)
来源：http://xnd.bjfxy.top

Go:   os.Exit(1)
来源：http://ikx.ctjpmb.com

Ruby: exit 1
来源：http://csj.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://egk.epnwcf.com

[M06] 向标准错误输出
来源：http://rpd.ydzc1.top

Py:   print("err", file=sys.stderr)
来源：http://nev.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qjx.hnxiangtu.top

JS:   console.error("err")
来源：http://fig.yueranfly.top

TS:   console.error("err")
来源：http://ysp.yongpay.top

Java: System.err.println("err")
来源：http://bfd.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lum.vehdjk.com

Ruby: warn "err"
来源：http://bmf.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://hlz.shzxlz.cn

[M07] 判断是否为主入口
来源：http://kka.epnwcf.com

Py:   if __name__ == "__main__":
来源：http://myh.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://say.zhengqikj.top

JS:   require.main === module
来源：http://xwa.jinyuanbaomall.cn

TS:   require.main === module
来源：http://ane.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://fjg.mhx1999.top

Go:   func main()
来源：http://bmp.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ewm.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://snc.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://qok.zhongyouzk.top

Py:   platform.system();  platform.python_version()
来源：http://sya.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://xbd.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://isz.tianlin.xyz

TS:   process.platform;  process.version
来源：http://apo.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pgc.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gxv.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nhp.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kdm.yj20258.top

================================================================================
来源：http://nwx.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://ekn.jqgfzy.top

================================================================================
来源：http://glq.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://fkj.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ker.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nld.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wxa.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qoe.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://lth.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://tbz.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xwg.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://gxy.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://ynf.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://led.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bxu.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qtg.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cvg.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gia.dianchejie.cn

Go:   slices.Sort(arr)
来源：http://dse.guannengcc.top

Ruby: arr.sort
来源：http://yvq.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhd.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://bpj.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://juy.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://tou.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pqv.zhaomingkeji.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ecb.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sni.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wxy.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wcl.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cva.epnwcf.com

[N04] 斐波那契数列
来源：http://rpy.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tzc.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://byg.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kfv.haohaochexian.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opu.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zia.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vmb.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ebv.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rdv.gzhubu.top

[N05] 最大公约数
来源：http://oio.uphjek.com

Py:   math.gcd(a, b)
来源：http://ehr.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://orx.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tne.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvc.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ihq.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ast.yfazqb.com

Ruby: a.gcd(b)
来源：http://rse.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dht.jinqigfzy.top

[N06] 判断回文字符串
来源：http://ikc.cashguo.top

Py:   s == s[::-1]
来源：http://tzy.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://glp.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://jho.xinyue.icu

TS:   s === [...s].reverse().join("")
来源：http://tjx.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pvg.zhiwuduotai.top

Go:   // 双指针从两端比较
来源：http://jfe.shzxlz.cn

Ruby: s == s.reverse
来源：http://pcu.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hds.c1oappe.top

[N07] 两数之和（返回下标）
来源：http://mox.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gmd.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ewn.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oyg.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://xau.ppjwa.cn

Java: // 手写 HashMap
来源：http://bel.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://sap.cheryme.top

Ruby: // 手写 Hash
来源：http://bma.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://loh.yuanzhike.top

[N08] 生成全排列
来源：http://kyt.yj20258.top

Py:   itertools.permutations(arr)
来源：http://gvl.dashuyun.cn

PHP:  // 手写递归交换
来源：http://clb.jianghu66.top

JS:   // 手写回溯递归
来源：http://rjs.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://imt.yfazqb.com

Java: // 手写回溯递归
来源：http://fdu.havefunace.top

Go:   // 手写回溯递归
来源：http://jwk.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://xqa.ivvv.top

C#:   // 手写回溯递归
来源：http://spm.shzxlz.cn

[N09] 栈与队列
来源：http://mey.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uxc.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ojy.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ydh.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lco.havefunace.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sqp.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yhq.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://avi.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://agq.yonumen.top

[N10] 链表节点定义
来源：http://gis.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pob.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://rzs.guowangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wwl.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://usg.uphjek.com

Java: class Node { int v; Node next; }
来源：http://ubf.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://eyv.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://yrv.sxryk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cij.hfpthk.cn

[N11] 二叉树中序遍历
来源：http://xuo.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fnq.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://fqa.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqd.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfx.chenjidiqi.icu

Java: // 手写递归
来源：http://vkd.bbcook.cn

Go:   // 手写递归
来源：http://dro.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ppf.zdbjq.cn

C#:   // 手写递归
来源：http://vnd.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rth.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lqm.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cma.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbn.zdqjudy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lnw.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tha.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nnr.hysaishi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yiw.tian-w.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://agb.xziqi.cn

================================================================================
来源：http://zqi.vqdsnc.cn

O. 并发与异步
来源：http://kld.yongpay.top

================================================================================
来源：http://lje.snrcjt.cn

[O01] 启动一个线程
来源：http://egg.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iyk.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pyh.xingfuxueyuan.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kjx.cheryme.top

TS:   // 同 JS
来源：http://lic.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://ybn.guowangkeji.top

Go:   go f()
来源：http://rcm.fktsv.cn

Ruby: Thread.new { f }
来源：http://pqv.52xcode.cn

C#:   Task.Run(() => F());
来源：http://uct.chenzaomai.com

[O02] 使用线程池
来源：http://doo.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://geg.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zso.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://jdn.shangyingyoupin.top

TS:   // worker_threads 线程池
来源：http://khp.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cks.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dac.havefunace.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rvn.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hfa.fzhhl.top

[O03] 加锁保护共享数据
来源：http://baq.sufxvd.cn

Py:   with lock: shared += 1
来源：http://evs.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://gxa.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sny.ybcxt.top

TS:   // 同 JS
来源：http://rwc.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://nhn.snrcjt.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xhf.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gql.quarkkingdee.top

C#:   lock (gate) { shared++; }
来源：http://fjh.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://zib.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://zye.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cat.shuidangran.top

JS:   async function f() { await g(); }
来源：http://iua.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sww.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iof.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tbs.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://thq.316326.xyz

C#:   async Task F() { await G(); }
来源：http://plf.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://wub.xziqi.cn

Py:   asyncio.gather(*tasks)
来源：http://vud.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jhq.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://dvq.yongpay.top

TS:   await Promise.all(tasks)
来源：http://mvm.sjlbkw.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ugt.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://frd.xylfe.cn

Ruby: threads.map(&:join)
来源：http://nes.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rmz.quarkkingdee.top

[O06] 使用进程池
来源：http://wrw.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ccv.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vfq.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://mhe.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://qkm.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xti.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://azn.xinyue.icu

Ruby: // fork 块
来源：http://rdj.haohaochexian.top

C#:   Parallel.For
来源：http://gxk.xziqi.cn

================================================================================
来源：http://yfu.zdqjudy.top

P. 常用工具函数
来源：http://vdh.tian-w.cn

================================================================================
来源：http://sqo.fehbvm.com

[P01] 生成 UUID
来源：http://roh.cheryme.top

Py:   str(uuid.uuid4())
来源：http://qkc.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xsk.ydzc1.top

JS:   crypto.randomUUID()
来源：http://xkw.andypj.xyz

TS:   crypto.randomUUID()
来源：http://mke.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://fas.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://wxd.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://oic.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://eon.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://pma.zhixingplan.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vwe.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ghh.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yhe.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jdk.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ccd.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nvq.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://csq.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://klb.ctjpmb.com

[P03] 生成短随机字符串
来源：http://unf.0kj1m.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mlt.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qdm.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sta.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jzw.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xcg.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://der.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yuf.smart0.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cis.0kj1m.cn

[P04] 求长度
来源：http://dfw.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://huc.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cqi.jinghuilouyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nnv.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://etm.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://uue.daxiang520.top

Go:   len(arr);  len(m)
来源：http://cjq.cashguo.top

Ruby: x.length;  x.size
来源：http://dkx.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fsy.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://myl.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zge.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zte.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sjg.tanke756.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iny.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xbm.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://rmd.yj20258.top

Ruby: a == b
来源：http://qph.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggl.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ilo.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ovb.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://kjs.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ehk.yj20258.top

TS:   if (x == null) {}
来源：http://rfm.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ktl.pengpengdd.cyou

Go:   if x == nil {}
来源：http://gud.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://owo.guannengcc.top

C#:   if (x is null) {}
来源：http://zhx.feifeiyinyue.top

[P07] 防抖与节流
来源：http://pef.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wxp.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://oce.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xeh.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onj.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nnc.yuanzhike.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pes.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kox.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://axa.shuidangran.top

[P08] 处理浮点精度问题
来源：http://uia.daxiang520.top


<!-- 参考信息 -->