代发 wailian999

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gwyvmgvgq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fktsv.cn/Article/details/griispvwd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.epnwcf.com/Article/details/gxacoyqnv.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/goxztqikh.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gzzvliojq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gvfskapeg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gwlmzoxnf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gedsqjazi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/ghblhmwjk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gytffhlhk.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gughckaeo.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gzqjovzxq.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/goaqgclza.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gqhyonpza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gtliubtgs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gmfpwkzwm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gxxltgrkn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxutctpg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gljloxzvh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gclpntozs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gjktplpwu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gwhntauhm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gsvwlfsao.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/ghobmrhtt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/grmxrjybe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/ggkkegpdl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gtgxvwjtm.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gnghyytik.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gjmxlpogg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gjfnsolxv.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/gdhbmuxst.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.yfazqb.com/Article/details/gvzjgcyab.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.yfazqb.com/Article/details/gbicqyxnp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/giubwnixh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gmcsmuhuc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gnpoltyoi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gvhaetaym.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gsmlmivse.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gsvaaacsw.sHtML

[N04] 斐波那契数列
来源：http://baike.yfazqb.com/Article/details/gvstkyehn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/ghrwpquau.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/grqvbwdsa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gdgxbzsip.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gygjiqafl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gwtkqmhiq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gebyforox.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gcghpnqzs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gaokviekf.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gnmwxpphp.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/guoirrxmn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fktsv.cn/Article/details/gpehimnee.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gpiomyzmu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gqkyckkfk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/gngfrxcdp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/geeukyofv.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gptcfvymz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gnbkvuspd.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/geuyzkdlz.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/gbjmxhorr.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gxpbxzrnv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gsdtnuhyp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gtnaqsjxw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/ghyiumgcq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gohnbpmus.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/gxdbkukau.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.epnwcf.com/Article/details/glbqhbyjd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gducpgdjw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gyvksgubd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/gxfdvrjjk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gnxcpbrny.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gvjimpfhy.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gpmopokuf.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gocskmlhy.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/gbxefwngm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/glqrwomcr.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gborprrhy.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gbzodakaf.sHtML

PHP:  // 手写递归交换
来源：http://3g.sjlbkw.cn/Article/details/gwiynpyfv.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gbkuncssf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/guzugnhwo.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gacshsoam.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gpbnarrgf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.vehdjk.com/Article/details/gxfotsycw.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gytpxnktg.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/geoabpsmb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gqjyslmtx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gtcivocok.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gswzdaqag.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/glqivgewd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/ghwyqctia.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/ghlrgwkyh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gqggypsbk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gskefdeup.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gatuxkvbu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/grjenntlo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.tarul.cn/Article/details/goibcdmyp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/gppndnebe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gixtpicxm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gzrmrrtjs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/giozmhyfl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gjycfifvq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/grtjutnth.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gvclcdtmf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gecxyljpw.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/gmnozyjna.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/giqxfmeyw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gmronzxzl.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/ggrecythq.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gfshwunwh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gzmkartea.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gwdzwnklp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gunrxiaid.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gmjbzgqth.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.vehdjk.com/Article/details/gjahbuswu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gzbijwsdh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gvhtqlsxw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gteiazfdp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/ghvqdgxxu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gvqzqmdld.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gpubsizch.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghxptvxfx.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/ggfcovaqd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gfwdovmrd.sHtML

[O01] 启动一个线程
来源：http://blog.tarul.cn/Article/details/gzhvvpihp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gzjkmiipi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gicevquml.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gimjlxenn.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gsrdlljsp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/guxbfuvzk.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gaceelsbm.sHtML

Ruby: Thread.new { f }
来源：http://blog.fktsv.cn/Article/details/gyfbvpcju.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gjstxshfg.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/ggmplisse.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gmqojonnv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gflkmjska.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/glduaxdtd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gxeornqhi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gyaffybef.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gqczujtxv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/golytncmj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/grwoeobqv.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gdmtupmuw.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gcljguvak.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.yfazqb.com/Article/details/glcygfgox.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gtbzkioxl.sHtML

TS:   // 同 JS
来源：http://www.share.tarul.cn/Article/details/gojhiarvt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gcfidmote.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/gzhrjjgps.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gkiioljzz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gcstkbjcj.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/grkusghhv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.sjlbkw.cn/Article/details/gcubxcsbc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gacsgcdku.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gklwexcqj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/gicqupaqa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.sjlbkw.cn/Article/details/gdwophsjr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.tarul.cn/Article/details/gxyynzyau.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gfnmrwcuq.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gbfoworzr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gipreglco.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gcdydvpce.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gygljcyqg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gssezbevt.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gofgwzcyw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gwaenqtyz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/gyapzjrug.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.vehdjk.com/Article/details/gdlpgcxmm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/gobifnkiu.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/gvjpqlqra.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gamuloqzz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/ghgguweah.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/guhkhwqzw.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gbbgpgthw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gnvqsuyyk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gojruigtw.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gloaufxte.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gounmrdbg.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/groqcofjy.sHtML

P. 常用工具函数
来源：http://read.share.bbcook.cn/Article/details/gingcmorv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmyrxhfqi.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/gluuopedx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gsbtrbdca.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gtmptagff.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/goglaonzb.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gtkagcjmi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/gxqsxqepz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gugpagimm.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gowhpvavz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gowizmrgp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.tarul.cn/Article/details/gchxgnfxi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/gcttpetys.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gfuwlmtfv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gvqneedxw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.tarul.cn/Article/details/gkogoyoky.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gssypbdiv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gjbuuzhap.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gpdvqevtx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gbskrypki.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwcdlabkg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gueciwsdk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/grueokgjl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/grqzyvqxn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gqdurklfc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/gtrbgvzec.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gxxglscgf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gtnwbpufy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/goririnad.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gnbbodhty.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gmialkyhi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gipengesk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gkpcmkdpc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gjopkigky.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gsigfsksp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gddaoymjl.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gtfrsdtfk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/gjasiihtd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gcnusmmvy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gedqxoeud.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gdlddrbzj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/grrihgijd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gqejqkwnp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/gqjopzajs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.sjlbkw.cn/Article/details/glkcyssau.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/gnttpfcju.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gkdwlexgk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/gbixafhpo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/gcymkrurr.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/ghznzubiv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gbaqkgnxc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/gdlnkhbtw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/guldbwzzr.sHtML

Go:   if x == nil {}
来源：http://www.blog.bbcook.cn/Article/details/gsulnxjlg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/guvrxewnq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gkgiknldp.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gbjhlpbtl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gokboorsl.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/ghjikglbo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gjfpnwrbc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/ghskdbvto.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gzprylwrs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/glwwiifes.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gnqflxalj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/gjrmrxknj.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gigonztmz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/ghicynmzu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gvqdwjpeh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/geiguoimx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gakkrvohi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gwjrymjjh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gllcrnkxe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/ghqatnqdt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gjalgggsc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjkcskghf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.epnwcf.com/Article/details/gjbkjcxkh.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggraqeeyt.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gpvrshvbz.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gvexywdxb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gtirqiquw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gqhmplrzk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gasfptwmm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.tarul.cn/Article/details/gmshoepyz.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gscsexlrj.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/ggzoholhk.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/guhjhbxoh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gutzjwkzy.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/ghppqipnd.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gybgbcvun.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxckwhwbt.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gkxetvmvu.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gxgdbuofw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gvdwrsgaa.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/gwyxzpeav.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gfzowuexz.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gxywbakaj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gcxmjvhzh.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gkahgkufh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gqniswhuw.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/galzsnfut.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/giqdknsmg.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fktsv.cn/Article/details/gjfpyjhrz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gfeuqdxaz.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gtqbcozgl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gebsnbamq.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gxboqdoks.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/goduhzedg.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gnawfdslh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/gkdaprxzi.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/gqkdmvxxo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.bbcook.cn/Article/details/gyehkgxju.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/geodutnmk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gzxijdscm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/gtyzqjnof.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gojbxuxou.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gmaqsakbt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gzfmxrswq.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gznionwjy.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gzjtfyphj.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gizdyxjrp.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gpvphxznc.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gukojybpc.sHtML


<!-- 参考信息 -->