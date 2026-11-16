代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fnp.sxryk.cn

Ruby: ENV["HOME"]
来源：http://tai.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dvw.sjlbkw.cn

[M03] 执行外部命令
来源：http://xxc.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ewt.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zka.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://flm.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hqh.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xqn.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ipg.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yyl.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://zht.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://pag.zdbjq.cn

Py:   os.getcwd()
来源：http://ulv.dianchejie.cn

PHP:  getcwd();
来源：http://iky.gogol.net.cn

JS:   process.cwd()
来源：http://xhv.vehdjk.com

TS:   process.cwd()
来源：http://rcb.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://yjj.xylfe.cn

Go:   os.Getwd()
来源：http://wvw.zycfv.cn

Ruby: Dir.pwd
来源：http://iss.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://tgt.yangfankeji.com

[M05] 设置退出码
来源：http://pke.cashguo.top

Py:   sys.exit(1)
来源：http://ykw.chenzaomai.com

PHP:  exit(1);
来源：http://kcm.chenjidiqi.icu

JS:   process.exit(1)
来源：http://fhf.cqqwz.cn

TS:   process.exit(1)
来源：http://pkh.ctjpmb.com

Java: System.exit(1)
来源：http://bhd.daxiang520.top

Go:   os.Exit(1)
来源：http://lwh.wangdashe.top

Ruby: exit 1
来源：http://tml.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xwu.jinqigfzy.top

[M06] 向标准错误输出
来源：http://eks.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://hpw.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ewl.vqdsnc.cn

JS:   console.error("err")
来源：http://jey.quarkkingdee.top

TS:   console.error("err")
来源：http://mxb.hesvh.cn

Java: System.err.println("err")
来源：http://cva.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ckk.fktsv.cn

Ruby: warn "err"
来源：http://srg.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://art.0kj1m.cn

[M07] 判断是否为主入口
来源：http://nhc.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://ekq.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mgy.andypj.xyz

JS:   require.main === module
来源：http://cuq.vehdjk.com

TS:   require.main === module
来源：http://qik.tanke756.top

Java: public static void main(String[] args)
来源：http://zeu.shangyingyoupin.top

Go:   func main()
来源：http://rbp.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bqj.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://dgl.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://tey.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://gcl.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://gqd.tian-w.cn

JS:   process.platform;  process.version
来源：http://uew.316326.xyz

TS:   process.platform;  process.version
来源：http://fha.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xvq.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://hbm.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oyk.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ecb.hnxiangtu.top

================================================================================
来源：http://yfp.ppjwa.cn

N. 数据结构与算法
来源：http://hfb.jinqigufen.top

================================================================================
来源：http://soo.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://uwd.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mgm.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oqk.hywenlv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://doj.yangfankeji.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oga.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://iai.jinqigfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://ybb.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fel.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://mai.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://tws.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://imm.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eso.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mho.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qmf.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qyj.fehbvm.com

Go:   slices.Sort(arr)
来源：http://ukh.xziqi.cn

Ruby: arr.sort
来源：http://yma.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://rkk.meibo888.top

[N03] 快速排序（分治示例）
来源：http://sxe.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fxs.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://kpn.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kyd.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mkh.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://opv.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yzl.xziqi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lfh.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gzw.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://mof.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jxs.0kj1m.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zdx.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bbf.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sut.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwg.gzhubu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ylg.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fhg.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cbo.316326.xyz

[N05] 最大公约数
来源：http://too.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://ddp.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dgj.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jbn.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kom.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qzh.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vjy.shzxlz.cn

Ruby: a.gcd(b)
来源：http://sxg.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://stu.ehwqpu.com

[N06] 判断回文字符串
来源：http://zmr.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://ute.fehbvm.com

PHP:  $s === strrev($s);
来源：http://lga.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://tei.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://srf.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eew.sweek.top

Go:   // 双指针从两端比较
来源：http://krk.fktsv.cn

Ruby: s == s.reverse
来源：http://asm.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://yql.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://ffb.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uqu.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mzc.gotoacloud.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kob.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://bgk.dianchejie.cn

Java: // 手写 HashMap
来源：http://nra.fengsongda.top

Go:   // 手写 map[int]int
来源：http://okl.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://ltv.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://xxv.jinghuilouyu.cn

[N08] 生成全排列
来源：http://bqh.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://tbm.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://khu.dashuyun.cn

JS:   // 手写回溯递归
来源：http://bgm.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://lmv.tanke756.top

Java: // 手写回溯递归
来源：http://nid.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://wiz.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://hml.guowangkeji.top

C#:   // 手写回溯递归
来源：http://kab.epnwcf.com

[N09] 栈与队列
来源：http://dxd.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lqn.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://svz.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vds.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mpi.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eqt.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zwk.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://auo.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rwv.cqqwz.cn

[N10] 链表节点定义
来源：http://ten.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ymt.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://pcf.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ybl.vqdsnc.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://idi.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://jxt.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://xoo.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://osr.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://mro.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://bja.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wkz.zhoulong.xyz

PHP:  // 手写递归函数
来源：http://dos.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ywy.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hcx.sjlbkw.cn

Java: // 手写递归
来源：http://aof.shzxlz.cn

Go:   // 手写递归
来源：http://ifw.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yeg.bjfxy.top

C#:   // 手写递归
来源：http://npa.xylfe.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ika.bjfxy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rlx.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bdy.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tli.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tie.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mue.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fjh.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ngb.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jgv.tianlin.xyz

================================================================================
来源：http://rch.cheryme.top

O. 并发与异步
来源：http://hvj.birdmap.top

================================================================================
来源：http://urg.zdbjq.cn

[O01] 启动一个线程
来源：http://iev.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eyq.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vfm.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kys.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://zut.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://cth.shangyingyoupin.top

Go:   go f()
来源：http://pce.aibaodan.cn

Ruby: Thread.new { f }
来源：http://rdc.ywan-chungtsiang.top

C#:   Task.Run(() => F());
来源：http://hhn.mhx1999.top

[O02] 使用线程池
来源：http://kcf.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yxm.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fdu.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://mye.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://lgw.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ymf.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mmd.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gxr.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iva.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://xia.redwolf501.top

Py:   with lock: shared += 1
来源：http://eeq.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://pfg.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uzd.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://zop.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://xnk.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://utm.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://luc.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://kmm.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://xmp.sxryk.cn

Py:   async def f():⏎    await g()
来源：http://ikl.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gkv.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://nvk.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ojl.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bas.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bnu.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://toh.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://awb.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://wuy.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://wpy.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://woo.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://msd.daria6918.cn

TS:   await Promise.all(tasks)
来源：http://kow.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xos.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qzi.xziqi.cn

Ruby: threads.map(&:join)
来源：http://bsq.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lqd.chenlongwang.top

[O06] 使用进程池
来源：http://cfj.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cyi.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pvy.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://jlg.hywenlv.cn

TS:   // child_process / cluster 模块
来源：http://cfv.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cnh.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://inn.zhongyouzk.top

Ruby: // fork 块
来源：http://yzm.fehbvm.com

C#:   Parallel.For
来源：http://vfd.jinqigufen.top

================================================================================
来源：http://jhs.gogol.net.cn

P. 常用工具函数
来源：http://tkc.hfpthk.cn

================================================================================
来源：http://blb.jqgufenzy.top

[P01] 生成 UUID
来源：http://ptu.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://soi.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hwn.hesvh.cn

JS:   crypto.randomUUID()
来源：http://skh.cheryme.top

TS:   crypto.randomUUID()
来源：http://bed.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://gdw.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://rew.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://pxh.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://eye.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://idq.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xdl.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://bcm.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nld.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://meo.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://czy.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ccm.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wyu.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://unm.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://rgg.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://okm.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zbx.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://niy.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rqy.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tqb.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iaq.xuanzx.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://abz.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ghj.wangdashe.top

[P04] 求长度
来源：http://dod.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bqb.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lde.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqg.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgz.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://cyk.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://noo.redwolf501.top

Ruby: x.length;  x.size
来源：http://tvp.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ihu.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://aab.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://suu.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://khj.yuxming.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gfo.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lqx.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zmb.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mvy.hongshengwenyu.top

Ruby: a == b
来源：http://xao.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lwf.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uxy.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wuj.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://dph.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mvi.quarkkingdee.top

TS:   if (x == null) {}
来源：http://nwe.tarul.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wfd.ydjk.org.cn

Go:   if x == nil {}
来源：http://pmb.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ejr.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://iwn.shuidangran.top

[P07] 防抖与节流
来源：http://vzx.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jqs.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://zzo.shanyushiyangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsp.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lgj.ywan-chungtsiang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xck.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ekx.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uer.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://okx.ydzc1.top

[P08] 处理浮点精度问题
来源：http://vsv.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://muj.yj20258888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://coe.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ppu.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aro.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ffo.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jpz.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ssf.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qin.jinghuilouyu.cn


<!-- 参考信息 -->