代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mga.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://njn.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://zbt.daria6918.cn

Java: System.getenv("HOME")
来源：http://acv.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yzy.vehdjk.com

Ruby: ENV["HOME"]
来源：http://xrr.chenzaomai.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xch.tianlin.xyz

[M03] 执行外部命令
来源：http://vol.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ipj.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uee.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hsn.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qxf.shuidangran.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rgk.hammf.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fah.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://mip.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://pnv.aizwys.cn

[M04] 获取当前工作目录
来源：http://dck.zhoulong.xyz

Py:   os.getcwd()
来源：http://nkd.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://lfv.birdmap.top

JS:   process.cwd()
来源：http://hxv.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://npj.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://olo.gotoacloud.top

Go:   os.Getwd()
来源：http://wfl.epnwcf.com

Ruby: Dir.pwd
来源：http://wxq.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://rkh.gaohongyu789.top

[M05] 设置退出码
来源：http://whe.hammf.cn

Py:   sys.exit(1)
来源：http://sol.pycfn.com

PHP:  exit(1);
来源：http://way.quarkkingdee.top

JS:   process.exit(1)
来源：http://tvh.yangfankeji.com

TS:   process.exit(1)
来源：http://fqv.zdbjq.cn

Java: System.exit(1)
来源：http://svz.zycfv.cn

Go:   os.Exit(1)
来源：http://epr.jiagoushi.top

Ruby: exit 1
来源：http://yix.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ibr.cucudq.cn

[M06] 向标准错误输出
来源：http://vdc.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://pxe.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ipg.xinyue.icu

JS:   console.error("err")
来源：http://jfz.hnxiangtu.top

TS:   console.error("err")
来源：http://kor.jyoumei.cn

Java: System.err.println("err")
来源：http://dnn.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vsb.andypj.xyz

Ruby: warn "err"
来源：http://qjy.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://bcy.tian-w.cn

[M07] 判断是否为主入口
来源：http://dlu.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://zjn.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oxh.hfpthk.cn

JS:   require.main === module
来源：http://ubt.jqgfzy.top

TS:   require.main === module
来源：http://jfi.52xcode.cn

Java: public static void main(String[] args)
来源：http://ncw.snrcjt.cn

Go:   func main()
来源：http://tfd.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://twe.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://cvb.guowangkeji.top

[M08] 获取系统与运行时信息
来源：http://ijq.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://jlx.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://duo.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://djl.yangfankeji.com

TS:   process.platform;  process.version
来源：http://xon.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pge.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qlo.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jee.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cnf.andypj.xyz

================================================================================
来源：http://pxx.xziqi.cn

N. 数据结构与算法
来源：http://inb.sufxvd.cn

================================================================================
来源：http://ipi.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://zww.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://jmr.zdqjudy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wjf.ywan-chungtsiang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eqx.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uww.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dqt.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://mce.vehdjk.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://vbl.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://yme.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://ukm.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://apj.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fuq.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jnf.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tgj.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zmy.hesvh.cn

Go:   slices.Sort(arr)
来源：http://drm.smart0.xyz

Ruby: arr.sort
来源：http://ani.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://bha.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://okg.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yld.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://bqs.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jpk.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nfs.yuanzhike.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gcc.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cdk.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tks.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ppp.hcnkem.com

[N04] 斐波那契数列
来源：http://osa.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lps.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rut.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mij.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gtj.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uhj.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dda.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gag.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nwn.sweek.top

[N05] 最大公约数
来源：http://awi.andypj.xyz

Py:   math.gcd(a, b)
来源：http://rfb.jinqigufen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kqt.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xmh.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vvw.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gqh.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zym.yfazqb.com

Ruby: a.gcd(b)
来源：http://xym.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oak.tian-w.cn

[N06] 判断回文字符串
来源：http://aji.yangfankeji.com

Py:   s == s[::-1]
来源：http://gtx.jianghu66.top

PHP:  $s === strrev($s);
来源：http://qeq.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://qci.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://usz.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fdf.smart0.xyz

Go:   // 双指针从两端比较
来源：http://ixm.yongpay.top

Ruby: s == s.reverse
来源：http://wla.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xsk.shzxlz.cn

[N07] 两数之和（返回下标）
来源：http://xwp.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lcj.ybcxt.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oyl.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eca.cheryme.top

TS:   // 手写 Map<string, number>
来源：http://tue.jqgfzy.top

Java: // 手写 HashMap
来源：http://mqy.tarul.cn

Go:   // 手写 map[int]int
来源：http://fwp.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://gip.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://mxq.guannengcc.top

[N08] 生成全排列
来源：http://evd.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://xdl.nanxinkj.top

PHP:  // 手写递归交换
来源：http://ymk.daria6918.cn

JS:   // 手写回溯递归
来源：http://sdo.shuidangran.top

TS:   // 手写回溯递归
来源：http://cui.cdnleiting.top

Java: // 手写回溯递归
来源：http://lhb.yj202588.top

Go:   // 手写回溯递归
来源：http://fly.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://dpf.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://bev.ydjk.org.cn

[N09] 栈与队列
来源：http://bol.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://com.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ilr.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qoa.yongpay.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ysx.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gwo.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kos.redwolf501.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gcz.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vft.svipenyu.cn

[N10] 链表节点定义
来源：http://ezw.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lbr.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xkn.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ldj.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aez.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://nds.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://eef.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://apf.ydzc1.top

C#:   class Node { public int V; public Node? Next; }
来源：http://brn.andypj.xyz

[N11] 二叉树中序遍历
来源：http://ptk.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hex.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://vuw.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mra.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxk.aizwys.cn

Java: // 手写递归
来源：http://arm.yfazqb.com

Go:   // 手写递归
来源：http://dad.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zzp.cdnleiting.top

C#:   // 手写递归
来源：http://vgs.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fut.zdqjudy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bxt.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yfd.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://llg.yvedp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ani.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvb.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fld.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vrf.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bbl.yanxiufei.cn

================================================================================
来源：http://hbf.hcnkem.com

O. 并发与异步
来源：http://nqr.aizwys.cn

================================================================================
来源：http://rjv.birdmap.top

[O01] 启动一个线程
来源：http://kqe.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aew.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zhw.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uib.tarul.cn

TS:   // 同 JS
来源：http://uuw.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://jta.jyoumei.cn

Go:   go f()
来源：http://sbc.cucudq.cn

Ruby: Thread.new { f }
来源：http://atz.sysykeji.top

C#:   Task.Run(() => F());
来源：http://kxv.sysykeji.top

[O02] 使用线程池
来源：http://cre.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bcc.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://chu.hesvh.cn

JS:   // worker_threads 线程池
来源：http://jmx.yj20258888.top

TS:   // worker_threads 线程池
来源：http://jia.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yay.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uzz.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sqb.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jhv.yonumen.top

[O03] 加锁保护共享数据
来源：http://enl.0kj1m.cn

Py:   with lock: shared += 1
来源：http://wut.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://gol.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ipr.52xcode.cn

TS:   // 同 JS
来源：http://rrb.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://gyk.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rwr.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rpz.feifeiyinyue.top

C#:   lock (gate) { shared++; }
来源：http://skt.cashguo.top

[O04] 定义异步函数并等待
来源：http://gxd.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://gmb.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bpd.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://dsn.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qav.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://atr.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zqd.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mht.sweek.top

C#:   async Task F() { await G(); }
来源：http://fcg.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://vhu.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://srg.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qba.c1oappe.top

JS:   await Promise.all(tasks)
来源：http://idw.sweek.top

TS:   await Promise.all(tasks)
来源：http://gyz.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qqw.jiagoushi.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gyo.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://tut.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jzv.meibo888.top

[O06] 使用进程池
来源：http://mmv.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jlu.zhongyouzk.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nch.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://kpr.0kj1m.cn

TS:   // child_process / cluster 模块
来源：http://ixn.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yng.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://flu.snrcjt.cn

Ruby: // fork 块
来源：http://lgj.yvedp.cn

C#:   Parallel.For
来源：http://vde.ivvv.top

================================================================================
来源：http://qcv.hcnkem.com

P. 常用工具函数
来源：http://vuy.xinyue.icu

================================================================================
来源：http://uzu.guannengcc.top

[P01] 生成 UUID
来源：http://cvn.havefunace.top

Py:   str(uuid.uuid4())
来源：http://ubk.ywan-chungtsiang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mtk.daxiang520.top

JS:   crypto.randomUUID()
来源：http://hkv.yueranfly.top

TS:   crypto.randomUUID()
来源：http://awc.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://wmf.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://fwd.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://ucm.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://nak.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://smn.fengsongda.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yni.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hub.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yww.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ppg.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://czc.ehwqpu.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://flh.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cjk.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jbn.ctjpmb.com

[P03] 生成短随机字符串
来源：http://szs.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gfu.hnqzz.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://itz.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qch.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dzt.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aeg.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://txg.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mtz.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kke.ybcxt.top

[P04] 求长度
来源：http://zvd.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lkj.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oto.zhaomingkeji.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szm.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hjv.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://dxb.epnwcf.com

Go:   len(arr);  len(m)
来源：http://gum.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://xpa.dashuyun.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gtf.yongpay.top

[P05] 判断两个对象内容是否相等
来源：http://mry.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://msm.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ukj.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uir.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dfk.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lll.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://ies.ivvv.top

Ruby: a == b
来源：http://gvy.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ivq.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zyh.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sah.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://ykf.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rtj.yj202588.top

TS:   if (x == null) {}
来源：http://yqq.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vpf.zdbjq.cn

Go:   if x == nil {}
来源：http://bmb.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tof.zdqjudy.top

C#:   if (x is null) {}
来源：http://cjr.yuanzhike.top

[P07] 防抖与节流
来源：http://lqg.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vkm.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://mnl.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdg.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lis.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ixs.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yeu.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://qrs.jqgfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dbo.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://bvo.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sjg.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wct.shzxlz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xrc.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zaa.vqdsnc.cn


<!-- 参考信息 -->