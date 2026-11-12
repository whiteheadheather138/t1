代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zrv.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://neg.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tjn.chenlongwang.top

[M03] 执行外部命令
来源：http://nmw.jinghuilouyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ogv.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://our.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cmq.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://otg.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rfi.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qkg.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rir.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://cob.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://oym.hammf.cn

Py:   os.getcwd()
来源：http://eil.shuidangran.top

PHP:  getcwd();
来源：http://edc.birdmap.top

JS:   process.cwd()
来源：http://jhd.xuanzx.com

TS:   process.cwd()
来源：http://oqd.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://bzj.quarkkingdee.top

Go:   os.Getwd()
来源：http://ilt.yueranfly.top

Ruby: Dir.pwd
来源：http://xsp.ivvv.top

C#:   Directory.GetCurrentDirectory()
来源：http://gsg.hywenlv.cn

[M05] 设置退出码
来源：http://rjx.ydzc1.top

Py:   sys.exit(1)
来源：http://mvi.316326.xyz

PHP:  exit(1);
来源：http://bvn.hnxiangtu.top

JS:   process.exit(1)
来源：http://oen.smart0.xyz

TS:   process.exit(1)
来源：http://hpz.yj20258888.top

Java: System.exit(1)
来源：http://xay.fktsv.cn

Go:   os.Exit(1)
来源：http://rtk.bjfxy.top

Ruby: exit 1
来源：http://ukb.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zoe.snrcjt.cn

[M06] 向标准错误输出
来源：http://bhb.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://qle.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://izq.zhixingplan.top

JS:   console.error("err")
来源：http://mgt.zdqjudy.top

TS:   console.error("err")
来源：http://lih.daria6918.cn

Java: System.err.println("err")
来源：http://iat.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mfb.cdnleiting.top

Ruby: warn "err"
来源：http://zlc.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://mzy.epnwcf.com

[M07] 判断是否为主入口
来源：http://hxp.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://pzg.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vvm.c1oappe.top

JS:   require.main === module
来源：http://qtp.ydzc1.top

TS:   require.main === module
来源：http://wid.uphjek.com

Java: public static void main(String[] args)
来源：http://iun.fengsongda.top

Go:   func main()
来源：http://hoj.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jdl.epnwcf.com

C#:   static void Main(string[] args)
来源：http://tcs.ivvv.top

[M08] 获取系统与运行时信息
来源：http://jcz.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://zgn.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://whr.yj20258888.top

JS:   process.platform;  process.version
来源：http://mpy.epnwcf.com

TS:   process.platform;  process.version
来源：http://owx.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dcn.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mtq.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://acf.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://pbs.fehbvm.com

================================================================================
来源：http://qqx.havefunace.top

N. 数据结构与算法
来源：http://pvf.redwolf501.top

================================================================================
来源：http://hzh.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://jxc.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vud.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vyf.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hui.yueranfly.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mhv.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://bfs.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://phm.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zlb.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://umr.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://lgn.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://fon.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rin.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ctp.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://knp.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nvs.svipenyu.cn

Go:   slices.Sort(arr)
来源：http://zfv.iojbl.cn

Ruby: arr.sort
来源：http://nqk.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://fzj.birdmap.top

[N03] 快速排序（分治示例）
来源：http://dow.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ily.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://dgh.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gti.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yvz.fzhhl.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vka.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iew.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tde.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://msn.zhongyouzk.top

[N04] 斐波那契数列
来源：http://mhp.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://luv.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://atx.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://klf.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qug.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cgc.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vba.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uma.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vcm.redwolf501.top

[N05] 最大公约数
来源：http://nlc.hesvh.cn

Py:   math.gcd(a, b)
来源：http://dex.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nop.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aqk.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iem.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iww.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kkh.hfpthk.cn

Ruby: a.gcd(b)
来源：http://rnb.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ndd.vqdsnc.cn

[N06] 判断回文字符串
来源：http://ggg.jinqigfzy.top

Py:   s == s[::-1]
来源：http://qky.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://jkd.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://ycd.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://xqz.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lbr.birdmap.top

Go:   // 双指针从两端比较
来源：http://lvb.sweek.top

Ruby: s == s.reverse
来源：http://bgn.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wvo.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://als.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xup.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cqp.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kfm.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://ywm.tarul.cn

Java: // 手写 HashMap
来源：http://kxk.bjfxy.top

Go:   // 手写 map[int]int
来源：http://qaj.fengsongda.top

Ruby: // 手写 Hash
来源：http://ehj.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://kzw.tanke756.top

[N08] 生成全排列
来源：http://ade.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://sra.haohaochexian.top

PHP:  // 手写递归交换
来源：http://zof.hfpthk.cn

JS:   // 手写回溯递归
来源：http://xle.zdqjudy.top

TS:   // 手写回溯递归
来源：http://uwh.sysykeji.top

Java: // 手写回溯递归
来源：http://ynm.yvedp.cn

Go:   // 手写回溯递归
来源：http://jpx.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://uoa.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://oyz.shanyushiyangtech.top

[N09] 栈与队列
来源：http://rpu.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xpo.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pmp.yongpay.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ucd.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rmq.jinqigufen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vbs.daxiang520.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wid.birdmap.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vek.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lrg.jinqigufen.top

[N10] 链表节点定义
来源：http://tnw.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ukq.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zyh.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bmf.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://usl.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://quf.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://lyw.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://jtg.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xjt.316326.xyz

[N11] 二叉树中序遍历
来源：http://tmj.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ola.yonumen.top

PHP:  // 手写递归函数
来源：http://mlo.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://raz.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xjk.snrcjt.cn

Java: // 手写递归
来源：http://odc.jiagoushi.top

Go:   // 手写递归
来源：http://ryg.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eph.epnwcf.com

C#:   // 手写递归
来源：http://erx.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xah.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gej.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qbf.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://htk.aibaodan.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dab.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ngj.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://btg.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qhu.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://agf.zycfv.cn

================================================================================
来源：http://lud.kuanghao11.cn

O. 并发与异步
来源：http://qwz.chenjidiqi.icu

================================================================================
来源：http://dno.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://iwb.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xor.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eca.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://efs.yueranfly.top

TS:   // 同 JS
来源：http://fpr.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://hqf.bjfxy.top

Go:   go f()
来源：http://czp.jyoumei.cn

Ruby: Thread.new { f }
来源：http://uct.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://qrj.0kj1m.cn

[O02] 使用线程池
来源：http://amd.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lnj.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fsn.xuanzx.com

JS:   // worker_threads 线程池
来源：http://bgw.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://pmi.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://wmj.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kqz.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xbk.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cyc.svipenyu.cn

[O03] 加锁保护共享数据
来源：http://yes.xinyue.icu

Py:   with lock: shared += 1
来源：http://yzm.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://gck.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lzf.yfazqb.com

TS:   // 同 JS
来源：http://ozk.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://myh.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ehb.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://orx.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://jyn.iojbl.cn

[O04] 定义异步函数并等待
来源：http://rmp.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://nit.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kvf.fengsongda.top

JS:   async function f() { await g(); }
来源：http://agt.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://bxc.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://loe.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tjv.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://sas.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://far.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://suy.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://orf.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://unf.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://woj.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://cns.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dsj.pengpengdd.cyou

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dnh.cashguo.top

Ruby: threads.map(&:join)
来源：http://zsf.316326.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://unf.shuidangran.top

[O06] 使用进程池
来源：http://vvw.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://daf.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://tde.uphjek.com

JS:   // child_process / cluster 模块
来源：http://mtj.chenlongwang.top

TS:   // child_process / cluster 模块
来源：http://lgu.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jam.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ebi.xziqi.cn

Ruby: // fork 块
来源：http://vze.ppjwa.cn

C#:   Parallel.For
来源：http://skm.jinghuilouyu.cn

================================================================================
来源：http://qcy.nwbrower.top

P. 常用工具函数
来源：http://owe.yj20258.top

================================================================================
来源：http://eyf.xylfe.cn

[P01] 生成 UUID
来源：http://tph.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://hzm.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rkf.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://ztn.cucudq.cn

TS:   crypto.randomUUID()
来源：http://olu.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://hiw.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://qxr.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://maq.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://gob.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://pah.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dsz.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nwj.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mrk.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nxv.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jej.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aug.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qwa.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uoo.birdmap.top

[P03] 生成短随机字符串
来源：http://tby.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://guq.zycfv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oaw.sxryk.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rbd.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nyz.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hhj.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wsb.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ttz.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bdt.zhoulong.xyz

[P04] 求长度
来源：http://ujf.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xuo.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pgk.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lyt.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tej.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://qkn.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://hof.hammf.cn

Ruby: x.length;  x.size
来源：http://knh.hywenlv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uur.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://fmo.c1oappe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rme.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ijq.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bmp.bjfxy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qwb.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sye.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://swd.yanxiufei.cn

Ruby: a == b
来源：http://hij.jyoumei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yvr.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ztx.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ygb.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://waw.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://plk.jlsjyb.cn

TS:   if (x == null) {}
来源：http://dus.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://izu.shuidangran.top

Go:   if x == nil {}
来源：http://zbo.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://htn.xuanzx.com

C#:   if (x is null) {}
来源：http://apt.zdbjq.cn

[P07] 防抖与节流
来源：http://pan.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://emt.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://lhu.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://adt.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hls.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://css.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yya.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wtr.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gtf.daria6918.cn

[P08] 处理浮点精度问题
来源：http://mab.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ygi.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uwp.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dxu.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lbr.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tzg.chenjidiqi.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zdr.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nga.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mig.kuanghao11.cn


<!-- 参考信息 -->