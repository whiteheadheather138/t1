代发 wailian999

TS:   process.cwd()
来源：http://gro.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://wug.guannengcc.top

Go:   os.Getwd()
来源：http://duf.sufxvd.cn

Ruby: Dir.pwd
来源：http://gkj.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://brp.tanke756.top

[M05] 设置退出码
来源：http://rkl.kuanghao11.cn

Py:   sys.exit(1)
来源：http://nqy.aizwys.cn

PHP:  exit(1);
来源：http://izu.dianchejie.cn

JS:   process.exit(1)
来源：http://hbf.andypj.xyz

TS:   process.exit(1)
来源：http://rfb.guowangkeji.top

Java: System.exit(1)
来源：http://pgd.cqqwz.cn

Go:   os.Exit(1)
来源：http://arj.chenzaomai.com

Ruby: exit 1
来源：http://wgc.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ern.jyoumei.cn

[M06] 向标准错误输出
来源：http://mdo.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://xtc.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oic.havefunace.top

JS:   console.error("err")
来源：http://oxf.guannengcc.top

TS:   console.error("err")
来源：http://gwj.jiagoushi.top

Java: System.err.println("err")
来源：http://pja.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tpd.sysykeji.top

Ruby: warn "err"
来源：http://tsb.redwolf501.top

C#:   Console.Error.WriteLine("err")
来源：http://byg.redwolf501.top

[M07] 判断是否为主入口
来源：http://mzm.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://zog.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fga.9152youxi.cn

JS:   require.main === module
来源：http://lzg.yonumen.top

TS:   require.main === module
来源：http://izq.shuidangran.top

Java: public static void main(String[] args)
来源：http://hwn.aibaodan.cn

Go:   func main()
来源：http://tzm.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tnr.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://qhi.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://yvq.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://dvu.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://txz.hysaishi.cn

JS:   process.platform;  process.version
来源：http://gac.tianlin.xyz

TS:   process.platform;  process.version
来源：http://rli.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hrf.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uey.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bfc.cashguo.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://suk.ppjwa.cn

================================================================================
来源：http://kjz.fanxiaobao.xyz

N. 数据结构与算法
来源：http://ybk.hnxiangtu.top

================================================================================
来源：http://wgq.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://fuz.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ibn.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zux.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ouk.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sgi.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mmk.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://rrt.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://csm.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ruj.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://jkh.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ogf.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lgz.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://gso.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://szi.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ypb.redwolf501.top

Go:   slices.Sort(arr)
来源：http://bfy.aizwys.cn

Ruby: arr.sort
来源：http://wpz.jyoumei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wzl.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://csv.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oga.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://pgr.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mog.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vog.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://znk.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gjt.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mdi.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qoq.yuanzhike.top

[N04] 斐波那契数列
来源：http://mpr.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yhh.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://glp.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cmv.jinqigfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqf.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mif.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yaq.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://anm.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cjw.ctjpmb.com

[N05] 最大公约数
来源：http://dtd.xuanzx.com

Py:   math.gcd(a, b)
来源：http://kzb.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oao.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gwz.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xkl.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iaa.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fjm.hywenlv.cn

Ruby: a.gcd(b)
来源：http://iin.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xwi.yuxming.cn

[N06] 判断回文字符串
来源：http://sdn.guowangkeji.top

Py:   s == s[::-1]
来源：http://hrk.aizwys.cn

PHP:  $s === strrev($s);
来源：http://etc.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://ras.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://flz.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ris.fzhhl.top

Go:   // 双指针从两端比较
来源：http://mpq.hnqzz.top

Ruby: s == s.reverse
来源：http://cxe.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sdd.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://nml.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oja.hammf.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://swk.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gjl.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://jhc.jiagoushi.top

Java: // 手写 HashMap
来源：http://uuc.birdmap.top

Go:   // 手写 map[int]int
来源：http://pdy.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://wxn.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://eml.hnxiangtu.top

[N08] 生成全排列
来源：http://qzg.bjfxy.top

Py:   itertools.permutations(arr)
来源：http://niq.yuxming.cn

PHP:  // 手写递归交换
来源：http://sgb.hywenlv.cn

JS:   // 手写回溯递归
来源：http://kze.shzxlz.cn

TS:   // 手写回溯递归
来源：http://ooj.yj20258888.top

Java: // 手写回溯递归
来源：http://pdb.pycfn.com

Go:   // 手写回溯递归
来源：http://skq.havefunace.top

Ruby: arr.permutation.to_a
来源：http://gmt.zhengqikj.top

C#:   // 手写回溯递归
来源：http://pgv.jqgufenzy.top

[N09] 栈与队列
来源：http://thz.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tmw.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vri.chenjidiqi.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wve.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ogw.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yyk.tian-w.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ibn.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uap.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kto.316326.xyz

[N10] 链表节点定义
来源：http://eli.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xug.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gwp.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://viy.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gkv.havefunace.top

Java: class Node { int v; Node next; }
来源：http://zfr.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://uvx.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oww.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zpy.ybcxt.top

[N11] 二叉树中序遍历
来源：http://ung.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kki.gzhubu.top

PHP:  // 手写递归函数
来源：http://bul.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbi.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cpg.ybcxt.top

Java: // 手写递归
来源：http://lyh.fzhhl.top

Go:   // 手写递归
来源：http://tuh.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rkg.ppjwa.cn

C#:   // 手写递归
来源：http://jlj.jinqigufen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eso.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hvg.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rfw.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gvk.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dfk.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jyx.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jcg.chenjidiqi.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rer.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://txz.bbcook.cn

================================================================================
来源：http://ntu.ehwqpu.com

O. 并发与异步
来源：http://bbw.snrcjt.cn

================================================================================
来源：http://cxd.snrcjt.cn

[O01] 启动一个线程
来源：http://nfl.xinyue.icu

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wte.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ylt.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mtb.yj20258.top

TS:   // 同 JS
来源：http://muq.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://qpq.jqgufenzy.top

Go:   go f()
来源：http://ery.yangfankeji.com

Ruby: Thread.new { f }
来源：http://cpl.sxryk.cn

C#:   Task.Run(() => F());
来源：http://ozr.zhiwuduotai.top

[O02] 使用线程池
来源：http://cxu.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cco.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://irh.yvedp.cn

JS:   // worker_threads 线程池
来源：http://jig.yj202588.top

TS:   // worker_threads 线程池
来源：http://bcs.quarkkingdee.top

Java: Executors.newFixedThreadPool(4)
来源：http://bol.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ruq.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lxh.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://flh.cucudq.cn

[O03] 加锁保护共享数据
来源：http://ker.ydzc1.top

Py:   with lock: shared += 1
来源：http://vdt.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xzf.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tyk.cashguo.top

TS:   // 同 JS
来源：http://ljh.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://ygo.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vpr.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://psf.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://bfj.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://ttt.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://dng.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ead.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://gqi.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dcx.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xox.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kvu.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://eca.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://yyd.quarkkingdee.top

[O05] 并发执行并等待全部完成
来源：http://qxa.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://tki.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://juo.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://weq.guannengcc.top

TS:   await Promise.all(tasks)
来源：http://oao.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zvx.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eeh.bjfxy.top

Ruby: threads.map(&:join)
来源：http://sxk.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wbd.jinghuilouyu.cn

[O06] 使用进程池
来源：http://uib.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kxx.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dln.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://nln.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://jsc.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xbw.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pbk.gaohongyu789.top

Ruby: // fork 块
来源：http://ejk.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://gjq.xingfuxueyuan.xyz

================================================================================
来源：http://agg.dashuyun.cn

P. 常用工具函数
来源：http://hug.bjfxy.top

================================================================================
来源：http://tug.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://ugb.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://thy.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bnm.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://kqn.jianghu66.top

TS:   crypto.randomUUID()
来源：http://vuw.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://puw.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://dgz.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://ori.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://wtn.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://nud.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vfw.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jqi.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sop.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://por.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ovv.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hpz.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mem.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rtq.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://xha.sjlbkw.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mpt.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://whd.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gjx.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gka.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nqz.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hbx.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qot.yonumen.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cbs.nwbrower.top

[P04] 求长度
来源：http://iqw.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zrw.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uji.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mjv.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://htj.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://gyz.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://rvp.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://mci.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tfo.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://rlo.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rto.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zjv.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hyd.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tqt.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dhm.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://ier.xylfe.cn

Ruby: a == b
来源：http://mge.uphjek.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rkj.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qbz.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hto.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://cwx.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fpr.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://vov.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dqz.cdnleiting.top

Go:   if x == nil {}
来源：http://ujk.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://amb.shuidangran.top

C#:   if (x is null) {}
来源：http://fiq.yueranfly.top

[P07] 防抖与节流
来源：http://xet.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vdk.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://ver.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvy.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xow.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cyk.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ecb.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://bro.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://odj.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://nzb.tianlin.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wbw.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://afi.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ivy.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ysu.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://huw.zhoulong.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://utp.jyoumei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://msu.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dbw.birdmap.top

================================================================================
来源：http://osc.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ens.redwolf501.top

================================================================================
来源：http://seh.daria6918.cn

[Q01] 创建表
来源：http://yzo.shangyingyoupin.top

CREATE TABLE users (
来源：http://wnc.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fri.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://jis.svipenyu.cn

email VARCHAR(100) UNIQUE,
来源：http://qjp.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ypj.yonumen.top

);
来源：http://sjx.ehwqpu.com

[Q02] 创建带外键的表
来源：http://wst.tanke756.top

CREATE TABLE orders (
来源：http://ekf.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hvv.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://zak.yj202588.top

amount DECIMAL(10, 2),
来源：http://oet.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cmh.nwbrower.top


<!-- 参考信息 -->