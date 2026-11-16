代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oog.jianghu66.top

JS:   process.env.HOME
来源：http://zqc.yuanzhike.top

TS:   process.env.HOME
来源：http://upw.0kj1m.cn

Java: System.getenv("HOME")
来源：http://swd.sweek.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://umv.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://afn.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kpz.jqgfzy.top

[M03] 执行外部命令
来源：http://nnh.yuanzhike.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vgl.316326.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fgy.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ife.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wgx.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kyu.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yta.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xfo.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://gon.fengsongda.top

[M04] 获取当前工作目录
来源：http://uqs.ydzc1.top

Py:   os.getcwd()
来源：http://rou.yueranfly.top

PHP:  getcwd();
来源：http://ztl.aibaodan.cn

JS:   process.cwd()
来源：http://ujv.snrcjt.cn

TS:   process.cwd()
来源：http://aes.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://wyt.hywenlv.cn

Go:   os.Getwd()
来源：http://bbu.zhoulong.xyz

Ruby: Dir.pwd
来源：http://nih.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://cij.daria6918.cn

[M05] 设置退出码
来源：http://xyj.dianchejie.cn

Py:   sys.exit(1)
来源：http://jop.redwolf501.top

PHP:  exit(1);
来源：http://oyu.c1oappe.top

JS:   process.exit(1)
来源：http://ybc.zhixingplan.top

TS:   process.exit(1)
来源：http://ycp.xziqi.cn

Java: System.exit(1)
来源：http://phc.9152youxi.cn

Go:   os.Exit(1)
来源：http://hai.gzhubu.top

Ruby: exit 1
来源：http://ykl.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fdd.zhoulong.xyz

[M06] 向标准错误输出
来源：http://gar.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://acc.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zts.feifeiyinyue.top

JS:   console.error("err")
来源：http://gfd.quarkkingdee.top

TS:   console.error("err")
来源：http://fnx.hnxiangtu.top

Java: System.err.println("err")
来源：http://rtp.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sov.jlsjyb.cn

Ruby: warn "err"
来源：http://pdf.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://uaa.zdbjq.cn

[M07] 判断是否为主入口
来源：http://aqa.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://fun.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://asf.uphjek.com

JS:   require.main === module
来源：http://stq.daxiang520.top

TS:   require.main === module
来源：http://ygj.cashguo.top

Java: public static void main(String[] args)
来源：http://aux.sysykeji.top

Go:   func main()
来源：http://lmi.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uai.xuanzx.com

C#:   static void Main(string[] args)
来源：http://cyf.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://upp.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://wtg.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://xsa.hywenlv.cn

JS:   process.platform;  process.version
来源：http://rrs.yj20258888.top

TS:   process.platform;  process.version
来源：http://zha.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hvm.quarkkingdee.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zna.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gtk.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hnf.aizwys.cn

================================================================================
来源：http://ltt.xinyue.icu

N. 数据结构与算法
来源：http://dco.shzxlz.cn

================================================================================
来源：http://kxl.chenjidiqi.icu

[N01] 二分查找（有序数组）
来源：http://kxp.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://rac.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hxe.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msv.kuanghao11.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsk.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://nuu.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://mcx.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://srx.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://bfa.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://ywa.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://etx.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lrz.yj20258888.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qap.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pxw.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ypc.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://uxd.hongshengwenyu.top

Ruby: arr.sort
来源：http://jqa.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pkk.pycfn.com

[N03] 快速排序（分治示例）
来源：http://azf.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jdh.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://soz.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nlb.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wfe.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jpj.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhg.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://osv.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ljf.epnwcf.com

[N04] 斐波那契数列
来源：http://uyk.feifeiyinyue.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pby.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vra.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ppz.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jgb.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ghd.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://awo.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://exy.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cpw.zycfv.cn

[N05] 最大公约数
来源：http://irc.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://rub.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zym.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://euj.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://two.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aty.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zqo.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://nwv.hongshengwenyu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://phb.hysaishi.cn

[N06] 判断回文字符串
来源：http://vug.iojbl.cn

Py:   s == s[::-1]
来源：http://yti.sxryk.cn

PHP:  $s === strrev($s);
来源：http://qix.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://bmc.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://cmp.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ppv.gzhubu.top

Go:   // 双指针从两端比较
来源：http://gmf.xylfe.cn

Ruby: s == s.reverse
来源：http://sen.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://uhr.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://wpy.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uyc.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ins.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://thq.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://jwf.haohaochexian.top

Java: // 手写 HashMap
来源：http://vhi.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://dad.zhengqikj.top

Ruby: // 手写 Hash
来源：http://vnt.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bpe.fktsv.cn

[N08] 生成全排列
来源：http://jsj.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://kly.zhengqikj.top

PHP:  // 手写递归交换
来源：http://why.yj20258.top

JS:   // 手写回溯递归
来源：http://xew.andypj.xyz

TS:   // 手写回溯递归
来源：http://cew.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://meq.zdbjq.cn

Go:   // 手写回溯递归
来源：http://mls.tianlin.xyz

Ruby: arr.permutation.to_a
来源：http://gko.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://vag.sysykeji.top

[N09] 栈与队列
来源：http://ueq.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pns.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znz.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nzs.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oeu.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cfz.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dfq.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vdg.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://guo.zhiwuduotai.top

[N10] 链表节点定义
来源：http://jdd.shanyushiyangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sas.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fbz.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gsg.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rro.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://zus.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sgf.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mis.fehbvm.com

C#:   class Node { public int V; public Node? Next; }
来源：http://llh.cheryme.top

[N11] 二叉树中序遍历
来源：http://jvn.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bsj.andypj.xyz

PHP:  // 手写递归函数
来源：http://vge.xylfe.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ght.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mpz.jinqigfzy.top

Java: // 手写递归
来源：http://qmz.vqdsnc.cn

Go:   // 手写递归
来源：http://nbt.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vbi.daria6918.cn

C#:   // 手写递归
来源：http://qni.snrcjt.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ric.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cxl.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hkg.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bqk.guannengcc.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tnb.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vzq.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tag.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pzo.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://him.gogol.net.cn

================================================================================
来源：http://ovi.chenjidiqi.icu

O. 并发与异步
来源：http://zlf.fehbvm.com

================================================================================
来源：http://nus.52xcode.cn

[O01] 启动一个线程
来源：http://big.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://udx.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://smt.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fai.gaohongyu789.top

TS:   // 同 JS
来源：http://yvx.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://wvk.gotoacloud.top

Go:   go f()
来源：http://lxm.snrcjt.cn

Ruby: Thread.new { f }
来源：http://chx.fengsongda.top

C#:   Task.Run(() => F());
来源：http://rqd.yuxming.cn

[O02] 使用线程池
来源：http://lxb.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rie.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://goc.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://twc.pycfn.com

TS:   // worker_threads 线程池
来源：http://xzs.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://dtf.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hni.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://luk.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xgk.redwolf501.top

[O03] 加锁保护共享数据
来源：http://caw.meibo888.top

Py:   with lock: shared += 1
来源：http://soe.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://lau.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tqn.chenzaomai.com

TS:   // 同 JS
来源：http://nwq.ydzc1.top

Java: synchronized (this) { shared++; }
来源：http://npy.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afh.gzhubu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cgg.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://lab.52xcode.cn

[O04] 定义异步函数并等待
来源：http://lsj.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://uxy.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://slq.ivvv.top

JS:   async function f() { await g(); }
来源：http://mnq.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bqg.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fkn.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mna.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gok.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://vml.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://doa.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://nvb.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kxn.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://sib.meibo888.top

TS:   await Promise.all(tasks)
来源：http://vah.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://alt.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dlv.316326.xyz

Ruby: threads.map(&:join)
来源：http://rpu.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://lkf.nanxuanxn.top

[O06] 使用进程池
来源：http://xbm.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mhb.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ndq.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://uvo.birdmap.top

TS:   // child_process / cluster 模块
来源：http://aju.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qvp.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gvd.sweek.top

Ruby: // fork 块
来源：http://kyg.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://czy.mhx1999.top

================================================================================
来源：http://xdp.hfpthk.cn

P. 常用工具函数
来源：http://jvx.yuanzhike.top

================================================================================
来源：http://dxi.haohaochexian.top

[P01] 生成 UUID
来源：http://mcg.tarul.cn

Py:   str(uuid.uuid4())
来源：http://roz.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jam.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://oom.sjlbkw.cn

TS:   crypto.randomUUID()
来源：http://tzy.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://hov.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://jbb.sweek.top

Ruby: SecureRandom.uuid
来源：http://czh.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://xec.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://tyw.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dpb.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://sbd.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qti.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tyl.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zkp.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lws.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xql.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oke.chenzaomai.com

[P03] 生成短随机字符串
来源：http://bnp.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lxj.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://guh.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://slf.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kgu.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hij.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rvo.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jig.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ljv.pycfn.com

[P04] 求长度
来源：http://rel.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ulw.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gpx.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bus.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wrm.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://gda.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://fye.yuxming.cn

Ruby: x.length;  x.size
来源：http://saf.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://kzv.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://fho.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://mlk.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kms.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://etr.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hra.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nzy.aizwys.cn

Go:   reflect.DeepEqual(a, b)
来源：http://axb.hnxiangtu.top

Ruby: a == b
来源：http://qsn.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gbn.shangyingyoupin.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lfy.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yyl.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://fwm.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nvm.zhixingplan.top

TS:   if (x == null) {}
来源：http://pvs.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://otl.jinqigufen.top

Go:   if x == nil {}
来源：http://prk.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mxk.svipenyu.cn

C#:   if (x is null) {}
来源：http://ysa.tarul.cn

[P07] 防抖与节流
来源：http://utp.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fgl.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://aon.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gqr.vehdjk.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kxr.xingfuxueyuan.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qbb.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gor.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cjz.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cdo.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://cvt.epnwcf.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qnt.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://puz.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ffr.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kpk.cdnleiting.top


<!-- 参考信息 -->