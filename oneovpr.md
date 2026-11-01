代发 wailian999

TS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/guylawcab.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/garoszwyj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.tarul.cn/Article/details/gylqkcrdf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/ggllqkegz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gsmltbeah.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gwxmuydvn.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/gmfvokieb.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpyrodyzm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/glnhwmair.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fktsv.cn/Article/details/gaecvzlns.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gfcvmffil.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/grhfzzxyo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gerfrjnat.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gkbfnbalx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/ggtsgtwag.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.tarul.cn/Article/details/gxpxklkna.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/glujcfcfh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gpnhwfjpb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.tarul.cn/Article/details/gtmiucqrr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gpxqlfwrk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gxbuvwvmb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gdmnpzeab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/grgizqmfe.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gwdmdzgay.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gzvzkgvik.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gloohzhbe.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gddekrxdo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.epnwcf.com/Article/details/gdovymelb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/grkpnukqu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/ghpqnkyyj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/glbztklgx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gnnredebs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.bbcook.cn/Article/details/gifytucub.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gvnbyrwgz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gbxbfoozb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gjyckyydo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gjsbprhgi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/glfcsfrcu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/grddymybo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gyviizctu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gapzjzfeh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gkgoyxlpo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gliwxkvun.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/glwjuaguh.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gkawdrokg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gdmcvozrd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gidpevoqd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gjcomdxml.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gszjqipvk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gtnglvpow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gpuceskqu.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gyklbnjho.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/geiublewo.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/gyvdwcsla.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/gmtpjeuiz.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/ghfcepqyk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gyhuqdyoe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/ghfsjhkkf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/glxreancu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/glrsbdtei.sHtML

Ruby: s == s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/geirvqpar.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gqnxqiysy.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/ggouczbgx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gnapmxukx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/grpmtazdl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gjigpunxv.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gmtdsqbfq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gilnojgte.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gffsryrpa.sHtML

Ruby: // 手写 Hash
来源：http://m.share.vehdjk.com/Article/details/gnlqzeqvg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/goquoterx.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gbqhtnfka.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gygrqdgth.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gopxspruf.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gpmdvspfs.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gmrsovwqi.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gljucpcaa.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gjpxpbfiq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gynprvxjz.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gjdcqvhcu.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gjytfkdtj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gclhyland.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gbulbhuba.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gqyevyrit.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gmsaxagiw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/gzyokwgaq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.tarul.cn/Article/details/gjtrwajes.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/goevqmfjz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.epnwcf.com/Article/details/gkwcfwixm.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gquguizma.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gbxzrgilb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gjvrkeobu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gelzhjlzm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gcmpxgsyz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.bbcook.cn/Article/details/gzrvntwqq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gjsimophc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gcdqqxzos.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.yfazqb.com/Article/details/gzxtyvqhb.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/gqtvgshch.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/gweomhlrh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gyamnhybg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gkgxkkxdc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gxbchniqm.sHtML

Java: // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/grbodkhoj.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gfxrrcvqc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/gstoirypr.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gbzghpcoa.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gnshznkbr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/giwzgoetq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gageyvejf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gxnyhxdyh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gniayqevr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gdechlbub.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gclpahosq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/guobvyxwl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gpqphgsco.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gutcajsbi.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gzkrcgwqt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gsihjvzci.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gelgxkyjt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gmbfdksti.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gkqopjnuo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gngvwbewq.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gtytzgyas.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gwrlgawfc.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/geaxupwcx.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/gbwumkcek.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/ggkumbblk.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gjulmapjf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.vehdjk.com/Article/details/gywzwirbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gdneucgzh.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/ggltkiegh.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/ggyxkwcrf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gefkerneu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gtidnznsd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/gtsakabbr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.vehdjk.com/Article/details/gzptcumcb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gapezrhod.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/ggpensdai.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gtomlosjo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/giyytaeri.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gnqmnjqkh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gsizfzlky.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gkinlwsxb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gszdwbdjy.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gsvfdpyan.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gepjffdmp.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gklrhwjzv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gwrfbttyg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gcjgebqgl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gvywtpqux.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gtmmrmagj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gjezllfil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gwqgmlumk.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/gpkiunbnh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gemoowhbh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.vehdjk.com/Article/details/gfhyzxzxg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/glicaaiyv.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gguajqwpo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gqxivxudw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gjdrkdhkd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gpvartwdu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/ginhoytmt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/giajvkitm.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gjhpzqnso.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gypsgabat.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/gspnlbxnd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gtsfhfiny.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gnpvmfuiq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gvanvckcj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gdjdvymqo.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gjkazwyyg.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gpjtriyln.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gsxvxxhht.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/ghphajkul.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwjzwtexc.sHtML

[P01] 生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gvicmwjyr.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gjckadcsl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/goypccuja.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gzqotjunu.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gvlddnevq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/goqvigwmd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gonlzkjjo.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.yfazqb.com/Article/details/gxubmzwpw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gcmjxdoso.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.tarul.cn/Article/details/gipbyjhlx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gdpzjosqy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gisqpfjhz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/gzkwhlwbc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gwgslvxsh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gkjgdpwbq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gkgozmizh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gfufxoryf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/glgwcsswc.sHtML

[P03] 生成短随机字符串
来源：http://baike.bbcook.cn/Article/details/ghyjchiqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.tarul.cn/Article/details/gmijvphmu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gieorrwao.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gjszulawc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gwseesmft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/glugwyanu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/glzewodqu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/glompjtxz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/gguiwrmko.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/givpzotcd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gwmtsyuhv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/grnyxabkd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gwtqoxlza.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gpyznrkpg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.epnwcf.com/Article/details/giievkhvs.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.epnwcf.com/Article/details/gdpmxhsny.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gkxtbknxj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gojzapvzf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gvkdquvss.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gmtuywjjp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gsymcizwq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gxupquzxc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/gjyepzysw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.bbcook.cn/Article/details/gkdopfgfi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gohcgfmba.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gfuktjtzf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gnvnxlepa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gbjhkvcrc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.tarul.cn/Article/details/gucjlfsxg.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gvcxhwire.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.tarul.cn/Article/details/gdkupyqql.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gruzmvell.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/ghjrfcwbq.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gyfvtucfm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gcijpxicz.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/gfusyntdc.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gdmgdrwhu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gdisvtjjz.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gneocgqat.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gxblqrwia.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gyfesfung.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/gtcznbcmz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gpzofeoxn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/gppeaermf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gqtwsocaf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gcvpfhdju.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gefxgpxhl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gnomglbfn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/ghkrzofpy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gowfowkxo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.sjlbkw.cn/Article/details/gpbjknlex.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/giztshsnu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/guuobtwor.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gcfbttjss.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gmbwddrtj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.sjlbkw.cn/Article/details/gvvwyceuj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqlitehnx.sHtML

[Q01] 创建表
来源：http://mobile.fktsv.cn/Article/details/gqwjodlkv.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/gnnkkmgyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gxqpriwsm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gamdjjadh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gwhvspyfo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.tarul.cn/Article/details/gamhgbgyu.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gijiljsce.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gqgqawpqx.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/gwvdyoxuu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gwnpgdvbr.sHtML

user_id INT NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gqvbhpcsa.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gqyjwqazk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.bbcook.cn/Article/details/gcqvdpbpq.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcdsirzk.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gasjipmoo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gnnszbtbb.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/gtddcvait.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gbekdgnua.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gcjgurnyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/gfnblcomq.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gqbafuhxw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.yfazqb.com/Article/details/goplfqous.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/glazwdwta.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/gaqcpkzrv.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/gubttytyl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzcoafamp.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/gjquyrbby.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gwcojhteq.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/gemiqdqoq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gmvqwgclm.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gqjaewubg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.tarul.cn/Article/details/gdasexacf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gmzjvdcvp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fktsv.cn/Article/details/gnfzrlmwd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gknelpbsj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.vehdjk.com/Article/details/glwdwrywe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gzqyxzdaw.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gzffjibiv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gcwielpnz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/ghmudwbon.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gnsvfjwfm.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gecozzpmh.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gmyzeubkv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gykgpbywd.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/grzsatkan.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gnvtmmwex.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/gringnpeh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/grrxfntwd.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/ggfiftlte.sHtML


<!-- 参考信息 -->