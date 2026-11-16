代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bmc.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tak.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://wpg.tian-w.cn

C#:   Process.Start("ls", "-l");
来源：http://ujt.9152youxi.cn

[M04] 获取当前工作目录
来源：http://gpv.ctjpmb.com

Py:   os.getcwd()
来源：http://jgh.cheryme.top

PHP:  getcwd();
来源：http://gbm.shuidangran.top

JS:   process.cwd()
来源：http://ktd.hnxiangtu.top

TS:   process.cwd()
来源：http://ium.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://ivq.yvedp.cn

Go:   os.Getwd()
来源：http://kvu.fehbvm.com

Ruby: Dir.pwd
来源：http://ave.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nyr.52xcode.cn

[M05] 设置退出码
来源：http://xbw.jinqigfzy.top

Py:   sys.exit(1)
来源：http://pft.nanxuanxn.top

PHP:  exit(1);
来源：http://rdo.52xcode.cn

JS:   process.exit(1)
来源：http://wnm.shzxlz.cn

TS:   process.exit(1)
来源：http://lqn.shanyushiyangtech.top

Java: System.exit(1)
来源：http://qjm.hysaishi.cn

Go:   os.Exit(1)
来源：http://qil.yueranfly.top

Ruby: exit 1
来源：http://tyg.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hdm.xziqi.cn

[M06] 向标准错误输出
来源：http://wjs.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://uop.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oot.tianlin.xyz

JS:   console.error("err")
来源：http://fve.ydjk.org.cn

TS:   console.error("err")
来源：http://nqr.jyoumei.cn

Java: System.err.println("err")
来源：http://jzb.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lie.yongpay.top

Ruby: warn "err"
来源：http://ufz.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://wic.vehdjk.com

[M07] 判断是否为主入口
来源：http://fic.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://jsd.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfe.haohaochexian.top

JS:   require.main === module
来源：http://erh.vehdjk.com

TS:   require.main === module
来源：http://ndx.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://yqc.ivvv.top

Go:   func main()
来源：http://goy.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sgl.birdmap.top

C#:   static void Main(string[] args)
来源：http://rne.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://ypq.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://cks.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://uch.uphjek.com

JS:   process.platform;  process.version
来源：http://vke.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://sdh.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uxg.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kka.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://btl.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mji.ppjwa.cn

================================================================================
来源：http://umw.chenlongwang.top

N. 数据结构与算法
来源：http://gef.zhengqikj.top

================================================================================
来源：http://qbw.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://env.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://ahm.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rpq.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gqi.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iyc.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://gcd.haohaochexian.top

Go:   sort.SearchInts(arr, x)
来源：http://dvx.hammf.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kgf.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://skj.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://aph.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://tlu.zhixingplan.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lrh.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rto.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iex.haohaochexian.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://llw.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://zex.xinyue.icu

Ruby: arr.sort
来源：http://ggr.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lbo.316326.xyz

[N03] 快速排序（分治示例）
来源：http://lmq.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fow.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://xok.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bvi.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wij.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zia.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cyk.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bwq.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://xhv.xinyue.icu

[N04] 斐波那契数列
来源：http://zkt.ywan-chungtsiang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hmw.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kwg.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rld.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dwe.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zgy.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rbx.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gto.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vgt.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://ord.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://akf.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://flb.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pvz.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sze.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iym.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nrx.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://qhb.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hvf.guannengcc.top

[N06] 判断回文字符串
来源：http://kzn.kuanghao11.cn

Py:   s == s[::-1]
来源：http://clc.ivvv.top

PHP:  $s === strrev($s);
来源：http://nyf.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://uml.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://uoe.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dgx.bjfxy.top

Go:   // 双指针从两端比较
来源：http://yfn.c1oappe.top

Ruby: s == s.reverse
来源：http://sbi.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://iak.yongpay.top

[N07] 两数之和（返回下标）
来源：http://afg.jyoumei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://obb.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vjs.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mvu.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://bny.daria6918.cn

Java: // 手写 HashMap
来源：http://unh.fzhhl.top

Go:   // 手写 map[int]int
来源：http://zof.hcnkem.com

Ruby: // 手写 Hash
来源：http://naw.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://tql.meibo888.top

[N08] 生成全排列
来源：http://ttc.meibo888.top

Py:   itertools.permutations(arr)
来源：http://gko.xuetiantiany.cn

PHP:  // 手写递归交换
来源：http://vvk.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://yve.zycfv.cn

TS:   // 手写回溯递归
来源：http://nxb.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://sbf.chenlongwang.top

Go:   // 手写回溯递归
来源：http://uvp.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://jro.guowangkeji.top

C#:   // 手写回溯递归
来源：http://abn.gaohongyu789.top

[N09] 栈与队列
来源：http://bsi.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iju.hysaishi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ybm.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pyz.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rnl.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tsx.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ljn.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qey.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yjf.hammf.cn

[N10] 链表节点定义
来源：http://jld.sysykeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rtk.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ncs.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://neq.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://unw.yj20258.top

Java: class Node { int v; Node next; }
来源：http://boy.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://ujd.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pfl.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://svn.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://qbm.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yhh.svipenyu.cn

PHP:  // 手写递归函数
来源：http://ovn.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hvv.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tnp.yj20258888.top

Java: // 手写递归
来源：http://tyq.fktsv.cn

Go:   // 手写递归
来源：http://vsr.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dut.zhongyouzk.top

C#:   // 手写递归
来源：http://bwa.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vti.pycfn.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ypl.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pnf.zdbjq.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ivw.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qjv.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zgc.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pnn.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://afo.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ill.gaohongyu789.top

================================================================================
来源：http://cwm.sweek.top

O. 并发与异步
来源：http://obw.redwolf501.top

================================================================================
来源：http://ija.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://lob.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jwm.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gtp.nanxinkj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yql.gogol.net.cn

TS:   // 同 JS
来源：http://oen.zhijiandao.cn

Java: new Thread(() -> f()).start()
来源：http://hxc.cucudq.cn

Go:   go f()
来源：http://atl.yfazqb.com

Ruby: Thread.new { f }
来源：http://wsv.gzhubu.top

C#:   Task.Run(() => F());
来源：http://xdd.dashuyun.cn

[O02] 使用线程池
来源：http://mac.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tnv.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mru.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://bkt.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://rxi.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://zio.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nai.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://awg.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tmx.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://jgt.hywenlv.cn

Py:   with lock: shared += 1
来源：http://eqp.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://zug.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jrt.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://tjd.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://pbu.pycfn.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ovi.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://arn.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://irc.yj20258.top

[O04] 定义异步函数并等待
来源：http://gge.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://huc.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kbo.fehbvm.com

JS:   async function f() { await g(); }
来源：http://prc.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tjp.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sbt.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gza.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://ecn.yonumen.top

C#:   async Task F() { await G(); }
来源：http://amd.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://xtp.chenzaomai.com

Py:   asyncio.gather(*tasks)
来源：http://gwv.shangyingyoupin.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tnb.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://irs.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://vpu.shzxlz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vlo.nanxuanxn.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ccb.shzxlz.cn

Ruby: threads.map(&:join)
来源：http://mvw.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://jls.bjfxy.top

[O06] 使用进程池
来源：http://bwf.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vpg.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pcg.meibo888.top

JS:   // child_process / cluster 模块
来源：http://gyc.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://byt.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ngv.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kmi.gzhubu.top

Ruby: // fork 块
来源：http://cmi.sjlbkw.cn

C#:   Parallel.For
来源：http://ixg.xziqi.cn

================================================================================
来源：http://fot.fzhhl.top

P. 常用工具函数
来源：http://ird.ydjk.org.cn

================================================================================
来源：http://wer.yanxiufei.cn

[P01] 生成 UUID
来源：http://zmc.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://fub.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zvy.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://wcx.yuanzhike.top

TS:   crypto.randomUUID()
来源：http://jcx.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://anj.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://iaj.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://ouw.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://luv.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://xip.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hdl.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xot.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dka.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fww.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zyg.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hmo.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gio.chenlongwang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://elu.chenjidiqi.icu

[P03] 生成短随机字符串
来源：http://cay.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://txj.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ubs.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hxo.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://viz.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://irp.jinghuilouyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://idt.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wib.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jfn.gogol.net.cn

[P04] 求长度
来源：http://uho.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zqb.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vrf.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xfg.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qqe.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://flu.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://hxo.andypj.xyz

Ruby: x.length;  x.size
来源：http://kqp.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vnt.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://lvq.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://jso.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ezp.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://usk.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://knd.jqgfzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cqh.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tlv.pycfn.com

Ruby: a == b
来源：http://ntg.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rbq.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cwg.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ozj.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://eqk.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cdl.xinyue.icu

TS:   if (x == null) {}
来源：http://ruv.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wia.sjlbkw.cn

Go:   if x == nil {}
来源：http://kjt.hammf.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qkb.yfazqb.com

C#:   if (x is null) {}
来源：http://ail.guannengcc.top

[P07] 防抖与节流
来源：http://wsb.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bmp.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://oru.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rrn.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lew.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tjf.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aqr.yuxming.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ood.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zij.sysykeji.top

[P08] 处理浮点精度问题
来源：http://dez.cashguo.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cho.jqgfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zeo.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nrs.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nzc.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zza.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jfs.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tig.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ame.snrcjt.cn

================================================================================
来源：http://lfx.nanxinkj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ghj.zhengqikj.top

================================================================================
来源：http://jvq.shanyushiyangkeji.top

[Q01] 创建表
来源：http://ndm.jiagoushi.top

CREATE TABLE users (
来源：http://sub.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yui.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://eic.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://ddf.hammf.cn


<!-- 参考信息 -->