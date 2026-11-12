代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hnz.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://jbi.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://orx.cheryme.top

[M03] 执行外部命令
来源：http://efg.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ars.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cyz.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mlm.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://ekh.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uac.zdbjq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nkf.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://bff.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://vyb.mhx1999.top

[M04] 获取当前工作目录
来源：http://lci.guowangkeji.top

Py:   os.getcwd()
来源：http://sbo.ybcxt.top

PHP:  getcwd();
来源：http://xio.fzhhl.top

JS:   process.cwd()
来源：http://siq.yueranfly.top

TS:   process.cwd()
来源：http://rbu.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://evw.zhiwuduotai.top

Go:   os.Getwd()
来源：http://wpz.ctjpmb.com

Ruby: Dir.pwd
来源：http://hdj.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xcb.hnxiangtu.top

[M05] 设置退出码
来源：http://flb.bjfxy.top

Py:   sys.exit(1)
来源：http://lqd.ybcxt.top

PHP:  exit(1);
来源：http://ysx.jianghu66.top

JS:   process.exit(1)
来源：http://uqq.aibaodan.cn

TS:   process.exit(1)
来源：http://lmc.hnxiangtu.top

Java: System.exit(1)
来源：http://lpk.nwbrower.top

Go:   os.Exit(1)
来源：http://hnv.xylfe.cn

Ruby: exit 1
来源：http://msv.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://njq.shuidangran.top

[M06] 向标准错误输出
来源：http://bpj.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://wzu.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mxv.316326.xyz

JS:   console.error("err")
来源：http://mxp.hesvh.cn

TS:   console.error("err")
来源：http://udf.hnxiangtu.top

Java: System.err.println("err")
来源：http://eaj.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://arh.vqdsnc.cn

Ruby: warn "err"
来源：http://kpy.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://mzh.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://mhn.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://ssh.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pah.fengsongda.top

JS:   require.main === module
来源：http://hzh.cqqwz.cn

TS:   require.main === module
来源：http://dhh.0kj1m.cn

Java: public static void main(String[] args)
来源：http://gdy.zhijiandao.cn

Go:   func main()
来源：http://kfd.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jyn.yj20258888.top

C#:   static void Main(string[] args)
来源：http://oge.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://qyr.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://lwi.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://dny.yueranfly.top

JS:   process.platform;  process.version
来源：http://xfr.svipenyu.cn

TS:   process.platform;  process.version
来源：http://ylo.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ddv.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mdt.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://udr.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wub.redwolf501.top

================================================================================
来源：http://xzc.chenjidiqi.icu

N. 数据结构与算法
来源：http://hro.xylfe.cn

================================================================================
来源：http://pft.fengsongda.top

[N01] 二分查找（有序数组）
来源：http://fhk.jyoumei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iow.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kst.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tus.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xeh.cashguo.top

Java: Arrays.binarySearch(arr, x)
来源：http://yhc.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://aji.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://lij.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kwi.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://skk.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://dth.vehdjk.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rew.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dvw.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://geb.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nrl.fzhhl.top

Go:   slices.Sort(arr)
来源：http://gcq.chenzaomai.com

Ruby: arr.sort
来源：http://aqy.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://uwx.cheryme.top

[N03] 快速排序（分治示例）
来源：http://yse.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zav.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://uqf.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jbf.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jdi.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://irc.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kcs.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zkj.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://bmf.ydzc1.top

[N04] 斐波那契数列
来源：http://amf.iojbl.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ydy.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eba.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtc.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dzp.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bnm.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jzq.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fby.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pad.hywenlv.cn

[N05] 最大公约数
来源：http://iyv.jinyuanbaomall.cn

Py:   math.gcd(a, b)
来源：http://nlq.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ggu.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dpy.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vou.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yuh.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wbc.smart0.xyz

Ruby: a.gcd(b)
来源：http://pff.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xrt.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://eex.zdbjq.cn

Py:   s == s[::-1]
来源：http://ozb.yuxming.cn

PHP:  $s === strrev($s);
来源：http://dna.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://upu.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://cuc.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sjt.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://nml.xinyue.icu

Ruby: s == s.reverse
来源：http://hwz.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yhh.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://kgq.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://suj.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://roo.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://uoo.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://vqi.sxryk.cn

Java: // 手写 HashMap
来源：http://yfh.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://beq.nanxinkj.top

Ruby: // 手写 Hash
来源：http://slz.chenlongwang.top

C#:   // 手写 Dictionary<int, int>
来源：http://syi.fzhhl.top

[N08] 生成全排列
来源：http://lot.zhijiandao.cn

Py:   itertools.permutations(arr)
来源：http://fzw.daxiang520.top

PHP:  // 手写递归交换
来源：http://hfc.sxryk.cn

JS:   // 手写回溯递归
来源：http://fzw.hywenlv.cn

TS:   // 手写回溯递归
来源：http://gwi.ppjwa.cn

Java: // 手写回溯递归
来源：http://bml.fengsongda.top

Go:   // 手写回溯递归
来源：http://hry.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://zfe.yuanzhike.top

C#:   // 手写回溯递归
来源：http://lwn.yj20258.top

[N09] 栈与队列
来源：http://akl.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dxf.nanxinkj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ggr.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dsj.ywan-chungtsiang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jgp.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cvj.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://phz.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ikz.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fch.dashuyun.cn

[N10] 链表节点定义
来源：http://ulf.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kgb.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nnd.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jso.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bfo.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://zhh.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://ydd.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dzb.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sjn.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://bmb.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ypu.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://zwq.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://loh.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nal.smart0.xyz

Java: // 手写递归
来源：http://hfl.iojbl.cn

Go:   // 手写递归
来源：http://lhk.xuetiantiany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqn.guowangkeji.top

C#:   // 手写递归
来源：http://giu.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://khm.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bxj.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gdc.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxi.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://trd.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uwy.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xxy.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kfy.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lwo.tanke756.top

================================================================================
来源：http://vjn.fktsv.cn

O. 并发与异步
来源：http://oem.nanxinkj.top

================================================================================
来源：http://xpi.daxiang520.top

[O01] 启动一个线程
来源：http://hsa.vehdjk.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://are.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kqg.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uff.c1oappe.top

TS:   // 同 JS
来源：http://oxm.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://hdk.pycfn.com

Go:   go f()
来源：http://iyp.havefunace.top

Ruby: Thread.new { f }
来源：http://wml.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://xsa.nanxuanxn.top

[O02] 使用线程池
来源：http://zln.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pjk.nwbrower.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dbo.uphjek.com

JS:   // worker_threads 线程池
来源：http://kvt.pycfn.com

TS:   // worker_threads 线程池
来源：http://man.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dws.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vtc.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pjh.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jjt.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://tzb.yueranfly.top

Py:   with lock: shared += 1
来源：http://ypd.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://ypt.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kmc.feifeiyinyue.top

TS:   // 同 JS
来源：http://fdr.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://tnw.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://duk.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lot.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://rnh.jianghu66.top

[O04] 定义异步函数并等待
来源：http://fei.uphjek.com

Py:   async def f():⏎    await g()
来源：http://tla.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jxj.c1oappe.top

JS:   async function f() { await g(); }
来源：http://glf.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hel.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://les.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://swo.hammf.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nqt.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://cbf.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://lco.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://mbv.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://her.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://qsi.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://ikc.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xhc.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rvj.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://emn.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://amy.shzxlz.cn

[O06] 使用进程池
来源：http://zph.kuanghao11.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zbr.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ifh.ywan-chungtsiang.top

JS:   // child_process / cluster 模块
来源：http://hqz.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://kzj.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mvv.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://waj.cucudq.cn

Ruby: // fork 块
来源：http://wuw.epnwcf.com

C#:   Parallel.For
来源：http://cqk.ybcxt.top

================================================================================
来源：http://mzm.aizwys.cn

P. 常用工具函数
来源：http://jyu.fengsongda.top

================================================================================
来源：http://oqf.sjlbkw.cn

[P01] 生成 UUID
来源：http://xrm.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://uov.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xnk.hnqzz.top

JS:   crypto.randomUUID()
来源：http://hig.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://hra.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://yxj.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://svg.meibo888.top

Ruby: SecureRandom.uuid
来源：http://bku.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://yqi.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://git.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sfe.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rml.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://aov.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ovm.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dqt.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nka.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iml.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dpc.9152youxi.cn

[P03] 生成短随机字符串
来源：http://dyh.yfazqb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kee.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qjh.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rck.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhe.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bsw.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pef.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://gpo.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://shs.yfazqb.com

[P04] 求长度
来源：http://mcc.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://byq.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ryc.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kft.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jsn.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://xbf.yvedp.cn

Go:   len(arr);  len(m)
来源：http://npx.yuanzhike.top

Ruby: x.length;  x.size
来源：http://nvp.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lfs.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://ywt.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hij.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kel.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qzx.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dsz.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hht.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://wrq.chenzaomai.com

Ruby: a == b
来源：http://ewr.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qyr.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://csk.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://guy.hywenlv.cn

PHP:  if (empty($x)) {}
来源：http://rli.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rnf.zycfv.cn

TS:   if (x == null) {}
来源：http://zft.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fhd.epnwcf.com

Go:   if x == nil {}
来源：http://cng.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hrc.zhongyouzk.top

C#:   if (x is null) {}
来源：http://gly.hammf.cn

[P07] 防抖与节流
来源：http://bhh.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://smw.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://hof.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwd.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fti.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jxh.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gmo.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yid.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ehr.tanke756.top

[P08] 处理浮点精度问题
来源：http://qhn.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ooq.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://twf.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jbk.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yxu.xingfuxueyuan.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mzq.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pba.zhiwuduotai.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://loh.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uws.zdbjq.cn


<!-- 参考信息 -->