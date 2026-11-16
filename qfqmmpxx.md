代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xgm.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qyd.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://tul.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://djf.ydzc1.top

[M04] 获取当前工作目录
来源：http://wkz.cqqwz.cn

Py:   os.getcwd()
来源：http://uhr.bbcook.cn

PHP:  getcwd();
来源：http://eqo.hcnkem.com

JS:   process.cwd()
来源：http://pew.yonumen.top

TS:   process.cwd()
来源：http://qjc.zhijiandao.cn

Java: Path.of("").toAbsolutePath()
来源：http://bdz.haohaochexian.top

Go:   os.Getwd()
来源：http://cyk.zycfv.cn

Ruby: Dir.pwd
来源：http://uer.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://uja.yonumen.top

[M05] 设置退出码
来源：http://qnn.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://drq.jinghuilouyu.cn

PHP:  exit(1);
来源：http://lmh.havefunace.top

JS:   process.exit(1)
来源：http://uhb.hnxiangtu.top

TS:   process.exit(1)
来源：http://afo.gaohongyu789.top

Java: System.exit(1)
来源：http://cnb.daxiang520.top

Go:   os.Exit(1)
来源：http://qlb.shanyushiyangkeji.top

Ruby: exit 1
来源：http://mgf.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ebq.zhijiandao.cn

[M06] 向标准错误输出
来源：http://yli.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://mmu.hongshengwenyu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qcs.jqgfzy.top

JS:   console.error("err")
来源：http://mac.fzhhl.top

TS:   console.error("err")
来源：http://blx.jyoumei.cn

Java: System.err.println("err")
来源：http://wfk.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sfi.xziqi.cn

Ruby: warn "err"
来源：http://lll.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://abo.yueranfly.top

[M07] 判断是否为主入口
来源：http://wfz.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://hwl.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ghy.yj202588.top

JS:   require.main === module
来源：http://ebm.yvedp.cn

TS:   require.main === module
来源：http://amq.shangyingyoupin.top

Java: public static void main(String[] args)
来源：http://rns.zhengqikj.top

Go:   func main()
来源：http://hjd.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gdm.tanke756.top

C#:   static void Main(string[] args)
来源：http://ajd.xingfuxueyuan.xyz

[M08] 获取系统与运行时信息
来源：http://hul.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://awd.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://wwt.yueranfly.top

JS:   process.platform;  process.version
来源：http://vip.xuanzx.com

TS:   process.platform;  process.version
来源：http://ynr.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vbr.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ftc.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blh.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ntm.cdnleiting.top

================================================================================
来源：http://qqj.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://ojt.zhijiandao.cn

================================================================================
来源：http://tjm.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://eir.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://dnn.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oop.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tod.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://orh.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://kxn.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://hzm.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://otf.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://kws.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://lsr.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://ffu.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mxa.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cwi.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yrt.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kac.yj202588.top

Go:   slices.Sort(arr)
来源：http://zci.guowangkeji.top

Ruby: arr.sort
来源：http://veo.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qdd.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://wyq.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ivh.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://pmk.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ics.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvn.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fne.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dkr.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ofn.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://zci.xinyue.icu

[N04] 斐波那契数列
来源：http://tlq.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://asz.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bze.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://idc.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jbn.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pth.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ctz.hammf.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hiy.yonumen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yar.hywenlv.cn

[N05] 最大公约数
来源：http://tel.iojbl.cn

Py:   math.gcd(a, b)
来源：http://zci.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dmk.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cmt.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://snw.xuanzx.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rnp.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nka.haohaochexian.top

Ruby: a.gcd(b)
来源：http://hgq.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yyq.bjfxy.top

[N06] 判断回文字符串
来源：http://sff.nanxuanxn.top

Py:   s == s[::-1]
来源：http://kcl.bbcook.cn

PHP:  $s === strrev($s);
来源：http://ahw.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://rsr.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://qgi.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ovt.pycfn.com

Go:   // 双指针从两端比较
来源：http://aow.tianlin.xyz

Ruby: s == s.reverse
来源：http://zcc.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sfe.cqqwz.cn

[N07] 两数之和（返回下标）
来源：http://pxh.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dvh.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vti.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://aik.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://gsl.cqqwz.cn

Java: // 手写 HashMap
来源：http://zbu.jinqigufen.top

Go:   // 手写 map[int]int
来源：http://pjn.cheryme.top

Ruby: // 手写 Hash
来源：http://ebb.pycfn.com

C#:   // 手写 Dictionary<int, int>
来源：http://jji.ydjk.org.cn

[N08] 生成全排列
来源：http://fro.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://ggx.fengsongda.top

PHP:  // 手写递归交换
来源：http://nfa.zhengqikj.top

JS:   // 手写回溯递归
来源：http://mjn.bbcook.cn

TS:   // 手写回溯递归
来源：http://jqn.nanxinkj.top

Java: // 手写回溯递归
来源：http://zle.birdmap.top

Go:   // 手写回溯递归
来源：http://gqq.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://mer.fktsv.cn

C#:   // 手写回溯递归
来源：http://aoa.chenzaomai.com

[N09] 栈与队列
来源：http://aho.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qsq.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lgh.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nun.9152youxi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bbd.jinghuilouyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jgk.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cgs.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://way.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nzw.ydzc1.top

[N10] 链表节点定义
来源：http://cyw.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://suz.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nji.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fnu.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wdr.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://xyf.nanxinkj.top

Go:   type Node struct { V int; Next *Node }
来源：http://ppb.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://liz.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cgk.iojbl.cn

[N11] 二叉树中序遍历
来源：http://vai.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://beo.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://eja.svipenyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxz.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rfq.ivvv.top

Java: // 手写递归
来源：http://eze.shzxlz.cn

Go:   // 手写递归
来源：http://fkw.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xyb.fktsv.cn

C#:   // 手写递归
来源：http://dcs.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gvf.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rhu.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yqp.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qnx.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://scd.chenzaomai.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rmy.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hal.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kit.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aik.sufxvd.cn

================================================================================
来源：http://ezx.zhijiandao.cn

O. 并发与异步
来源：http://aen.jinqigfzy.top

================================================================================
来源：http://nhr.birdmap.top

[O01] 启动一个线程
来源：http://qzu.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qra.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qmf.sysykeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://epx.xziqi.cn

TS:   // 同 JS
来源：http://tlm.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://yyf.xinyue.icu

Go:   go f()
来源：http://jvq.jyoumei.cn

Ruby: Thread.new { f }
来源：http://eww.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://pff.yonumen.top

[O02] 使用线程池
来源：http://fxb.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nht.52xcode.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iik.nwbrower.top

JS:   // worker_threads 线程池
来源：http://nzv.yuxming.cn

TS:   // worker_threads 线程池
来源：http://qlr.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uwj.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kgi.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ngk.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qka.jinghuilouyu.cn

[O03] 加锁保护共享数据
来源：http://gcl.dashuyun.cn

Py:   with lock: shared += 1
来源：http://bim.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://giz.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eas.uphjek.com

TS:   // 同 JS
来源：http://vsr.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://jps.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dob.hywenlv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ezg.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://owy.hesvh.cn

[O04] 定义异步函数并等待
来源：http://ory.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://xsl.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xnv.meibo888.top

JS:   async function f() { await g(); }
来源：http://gkx.jinghuilouyu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jct.pengpengdd.cyou

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uzu.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rsb.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://khj.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://aqj.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://kfd.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://jgv.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tiv.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://lrb.yongpay.top

TS:   await Promise.all(tasks)
来源：http://nbz.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ijo.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nih.jianghu66.top

Ruby: threads.map(&:join)
来源：http://dak.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xjy.yj20258888.top

[O06] 使用进程池
来源：http://tpq.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vfn.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kru.tanke756.top

JS:   // child_process / cluster 模块
来源：http://dhi.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://fxb.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bkx.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://awg.yuanzhike.top

Ruby: // fork 块
来源：http://wfm.c1oappe.top

C#:   Parallel.For
来源：http://gab.vehdjk.com

================================================================================
来源：http://ihm.gzhubu.top

P. 常用工具函数
来源：http://hav.yanxiufei.cn

================================================================================
来源：http://rli.nwbrower.top

[P01] 生成 UUID
来源：http://vtd.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://epj.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://psq.sxryk.cn

JS:   crypto.randomUUID()
来源：http://rhc.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://upp.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://fwa.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://bua.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://tgn.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://klv.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://ymi.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ghs.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wio.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eqz.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bjd.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iwa.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cne.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ccn.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bvs.fehbvm.com

[P03] 生成短随机字符串
来源：http://hgj.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bwa.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qoa.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ywf.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mov.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://scb.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mni.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xoa.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uaa.ywan-chungtsiang.top

[P04] 求长度
来源：http://peg.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wlo.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nba.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hkm.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zwu.redwolf501.top

Java: list.size();  map.size();  s.length()
来源：http://etc.gzhubu.top

Go:   len(arr);  len(m)
来源：http://hbx.cqqwz.cn

Ruby: x.length;  x.size
来源：http://qwh.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kku.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://hvs.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xuk.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wlm.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jie.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xtl.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gei.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fgy.gotoacloud.top

Ruby: a == b
来源：http://jfb.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qqk.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fmh.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://djt.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://uio.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xzg.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://eez.xuanzx.com

Java: if (x == null || x.isEmpty()) {}
来源：http://cjr.shzxlz.cn

Go:   if x == nil {}
来源：http://psb.jinghuilouyu.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wft.xylfe.cn

C#:   if (x is null) {}
来源：http://ljy.andypj.xyz

[P07] 防抖与节流
来源：http://zmm.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uqp.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://adf.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uua.jiagoushi.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wfn.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xng.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ccr.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://efo.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nlr.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://waj.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://luu.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qsg.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bvn.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mhw.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hhn.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bwg.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sbl.nanxuanxn.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://plj.jianghu66.top

================================================================================
来源：http://raa.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kge.cheryme.top

================================================================================
来源：http://ftg.ehwqpu.com

[Q01] 创建表
来源：http://jso.jinyuanbaomall.cn

CREATE TABLE users (
来源：http://lpl.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dfc.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://lyg.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://qtl.jinyuanbaomall.cn


<!-- 参考信息 -->