代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kzq.yj202588.top

JS:   process.env.HOME
来源：http://lsy.nwbrower.top

TS:   process.env.HOME
来源：http://jur.daxiang520.top

Java: System.getenv("HOME")
来源：http://mlo.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xvi.fktsv.cn

Ruby: ENV["HOME"]
来源：http://ppj.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zix.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://nns.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://din.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vlm.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://cga.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hvo.zhongyouzk.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kdg.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vhe.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yua.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://kyz.tarul.cn

[M04] 获取当前工作目录
来源：http://elj.dianchejie.cn

Py:   os.getcwd()
来源：http://fjo.vehdjk.com

PHP:  getcwd();
来源：http://jfs.cqqwz.cn

JS:   process.cwd()
来源：http://edk.cheryme.top

TS:   process.cwd()
来源：http://gdx.cucudq.cn

Java: Path.of("").toAbsolutePath()
来源：http://wnh.zhongyouzk.top

Go:   os.Getwd()
来源：http://dir.havefunace.top

Ruby: Dir.pwd
来源：http://ucu.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://qft.cheryme.top

[M05] 设置退出码
来源：http://epz.ppjwa.cn

Py:   sys.exit(1)
来源：http://ovv.haohaochexian.top

PHP:  exit(1);
来源：http://bxe.guowangkeji.top

JS:   process.exit(1)
来源：http://qal.mhx1999.top

TS:   process.exit(1)
来源：http://iym.yj20258888.top

Java: System.exit(1)
来源：http://map.sufxvd.cn

Go:   os.Exit(1)
来源：http://ivo.jinyuanbaomall.cn

Ruby: exit 1
来源：http://frf.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lbw.sufxvd.cn

[M06] 向标准错误输出
来源：http://ltd.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://jwi.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://pwf.sjlbkw.cn

JS:   console.error("err")
来源：http://zay.jlsjyb.cn

TS:   console.error("err")
来源：http://cul.hcnkem.com

Java: System.err.println("err")
来源：http://yfx.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ogv.nwbrower.top

Ruby: warn "err"
来源：http://ivy.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://eux.guowangkeji.top

[M07] 判断是否为主入口
来源：http://qir.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://pyr.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iva.hywenlv.cn

JS:   require.main === module
来源：http://lil.meibo888.top

TS:   require.main === module
来源：http://xdc.birdmap.top

Java: public static void main(String[] args)
来源：http://vbp.hongshengwenyu.top

Go:   func main()
来源：http://qqs.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://quq.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://ysy.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://rrb.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://uxe.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://trf.shzxlz.cn

JS:   process.platform;  process.version
来源：http://myo.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://lzs.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ode.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://vup.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://htz.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bid.xuetiantiany.cn

================================================================================
来源：http://vxl.zhijiandao.cn

N. 数据结构与算法
来源：http://ilz.xziqi.cn

================================================================================
来源：http://iym.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://zoi.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qsw.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aks.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ccc.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xaz.tianlin.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://cry.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://ioz.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dls.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://imp.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://niu.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://cnu.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lpi.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://hly.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nxw.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bwz.meibo888.top

Go:   slices.Sort(arr)
来源：http://nxw.shuidangran.top

Ruby: arr.sort
来源：http://qob.tian-w.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vky.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://qdw.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eqw.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://gub.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vxa.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kmk.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://spa.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ihz.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dhz.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zdu.zdbjq.cn

[N04] 斐波那契数列
来源：http://zfj.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ins.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://voc.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jul.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://muc.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uex.ctjpmb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kgo.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gsw.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baa.meibo888.top

[N05] 最大公约数
来源：http://dcl.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://qnt.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vpe.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tjr.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvy.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vfu.zhixingplan.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://syz.epnwcf.com

Ruby: a.gcd(b)
来源：http://vsc.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fgx.ydjk.org.cn

[N06] 判断回文字符串
来源：http://hzl.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://cpi.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://cjd.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://btu.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://rhv.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lek.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://qxv.fzhhl.top

Ruby: s == s.reverse
来源：http://dix.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lvy.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://qwh.mhx1999.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qsw.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wfg.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qsc.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://ifr.xziqi.cn

Java: // 手写 HashMap
来源：http://kmx.haohaochexian.top

Go:   // 手写 map[int]int
来源：http://skz.tian-w.cn

Ruby: // 手写 Hash
来源：http://lga.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kbh.zhixingplan.top

[N08] 生成全排列
来源：http://wbi.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://zuq.vehdjk.com

PHP:  // 手写递归交换
来源：http://neb.316326.xyz

JS:   // 手写回溯递归
来源：http://rdh.fzhhl.top

TS:   // 手写回溯递归
来源：http://xtk.meibo888.top

Java: // 手写回溯递归
来源：http://ilo.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://cnt.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://hqx.guowangkeji.top

C#:   // 手写回溯递归
来源：http://jao.ctjpmb.com

[N09] 栈与队列
来源：http://fsu.xuanzx.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pif.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hzf.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mcp.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://phy.tianlin.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dam.shuidangran.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bnv.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uva.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ieb.316326.xyz

[N10] 链表节点定义
来源：http://krr.zhixingplan.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://naj.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vyu.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bjx.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gro.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://wdq.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://kjr.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ith.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://kqt.meibo888.top

[N11] 二叉树中序遍历
来源：http://nzj.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oye.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://igi.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jcr.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nro.sxryk.cn

Java: // 手写递归
来源：http://kek.nwbrower.top

Go:   // 手写递归
来源：http://iio.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yxm.c1oappe.top

C#:   // 手写递归
来源：http://egz.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ewu.yuxming.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ilr.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qkd.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lgz.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kuk.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kbn.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://idc.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vjb.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zku.yfazqb.com

================================================================================
来源：http://guy.fzhhl.top

O. 并发与异步
来源：http://ntg.jianghu66.top

================================================================================
来源：http://ppt.hesvh.cn

[O01] 启动一个线程
来源：http://zyr.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dgx.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ufs.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qlx.gzhubu.top

TS:   // 同 JS
来源：http://nxu.yfazqb.com

Java: new Thread(() -> f()).start()
来源：http://azu.andypj.xyz

Go:   go f()
来源：http://ohb.nanxinkj.top

Ruby: Thread.new { f }
来源：http://tgz.hfpthk.cn

C#:   Task.Run(() => F());
来源：http://wpq.vqdsnc.cn

[O02] 使用线程池
来源：http://pot.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wro.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hzw.yfazqb.com

JS:   // worker_threads 线程池
来源：http://ypt.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://uax.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://nii.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://djk.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://upd.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ywv.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://uaa.zhixingplan.top

Py:   with lock: shared += 1
来源：http://lfn.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://ilk.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qch.hammf.cn

TS:   // 同 JS
来源：http://cxb.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://ydi.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pcy.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nii.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://fjd.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://muf.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://jjc.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nlb.andypj.xyz

JS:   async function f() { await g(); }
来源：http://npm.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://uvl.jianghu66.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ovb.hysaishi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yuq.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://cce.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://ucj.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://hnn.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://qlw.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tqk.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://hjh.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://cfj.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xef.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bya.yj20258888.top

Ruby: threads.map(&:join)
来源：http://ino.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://alk.yvedp.cn

[O06] 使用进程池
来源：http://tol.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qke.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ire.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://ttp.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://zvo.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://frg.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ssi.ybcxt.top

Ruby: // fork 块
来源：http://bco.dashuyun.cn

C#:   Parallel.For
来源：http://vxa.aibaodan.cn

================================================================================
来源：http://ixj.gaohongyu789.top

P. 常用工具函数
来源：http://iug.cqqwz.cn

================================================================================
来源：http://nol.aizwys.cn

[P01] 生成 UUID
来源：http://fbi.epnwcf.com

Py:   str(uuid.uuid4())
来源：http://etq.cdnleiting.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zpw.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://yli.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://agg.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://fnp.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://syk.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://qwl.0kj1m.cn

C#:   Guid.NewGuid().ToString()
来源：http://fyi.fzhhl.top

[P02] MD5 / SHA256 摘要
来源：http://ndk.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lzt.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mod.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://amd.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ofl.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ega.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wva.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zye.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sil.cqqwz.cn

[P03] 生成短随机字符串
来源：http://znn.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zyh.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pvq.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjy.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jny.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://asy.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cil.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pej.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pkm.yuanzhike.top

[P04] 求长度
来源：http://xsr.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fzw.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttv.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lhi.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wun.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://rsm.vehdjk.com

Go:   len(arr);  len(m)
来源：http://ygp.feifeiyinyue.top

Ruby: x.length;  x.size
来源：http://fsl.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gop.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://wxc.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qev.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://crv.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hke.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tqs.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qgy.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zgt.shzxlz.cn

Ruby: a == b
来源：http://qmx.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yyw.sweek.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vmo.jqgfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ztk.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://smy.yvedp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://huv.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://xhp.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://mnc.chenjidiqi.icu

Go:   if x == nil {}
来源：http://sos.redwolf501.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hru.sjlbkw.cn

C#:   if (x is null) {}
来源：http://fzi.jinqigfzy.top

[P07] 防抖与节流
来源：http://mxo.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://soy.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://nvw.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nom.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iif.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://whv.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://viv.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://qjy.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wzl.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://bxv.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kcl.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bwj.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://erm.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yei.hysaishi.cn


<!-- 参考信息 -->