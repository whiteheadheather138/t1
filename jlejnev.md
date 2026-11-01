代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gijjxdixq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gwsauuech.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gydjipaek.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grmmcojwx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/ggmnkgkqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gbnhfgtjj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gzquhhggu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/grveygfih.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gjgobodsa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/ghvlorcki.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gysvnjomu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gchvhqlrt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/grktruhwv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/ggunjdmtt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/genbubzxn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gfndguzxt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gfcxjqpgc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gohemacor.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.sjlbkw.cn/Article/details/gzpsokljx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fktsv.cn/Article/details/gsvhlhcxq.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gdkbttxxe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gqhfkwqto.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gfaeamkou.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gctgiksbs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/goywmvyae.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gdbfnjtvd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gxtgmjngr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.yfazqb.com/Article/details/gqrcpdesn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gcwcyupvq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.yfazqb.com/Article/details/gekvvygzu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.sjlbkw.cn/Article/details/guuudsjfh.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gnddkddjt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gglsgukqm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gaeghkyyp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gjieoreea.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gsrnjhvju.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gjnzhnqss.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gpcfbovtl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gygsyjkrc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gmpuohatd.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gkqaylzhs.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/ggweopgxv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gckwcydru.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gpwsoxdfb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gdslcrtna.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.bbcook.cn/Article/details/gnggfikyi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/geqyctjuh.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gkppcuajw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gwepwrsaz.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/geypacvxr.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gjzeaaoms.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gffisnnjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/genzrhjuu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gkiycuxle.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gabidssnq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/ggnjcjksx.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gynsqoaxq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/grrdgjpxp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gbqencawl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/guvxyikba.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/gzozlxtah.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gpkvnysgs.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/ghwbvsjws.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gqdzzelek.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/geijactjy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.vehdjk.com/Article/details/guwazsmuh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gihhapyxo.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gnubahzqb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.epnwcf.com/Article/details/gjoapjucc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/glzjzipkd.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gdejkblyz.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gibgaugzw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gpbbcytka.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gxdvvbhvp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gponexrmk.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/grxgdhomi.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/geshxgwec.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gcefggawm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/goylvdyip.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsqustsw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/glycwyndl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/geghvcggl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gisorwclm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gomujbazl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gfpwsybop.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/ghuybefie.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gjnemajrx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/grgnximcy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gzpvavftw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/gfkhosnut.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/grfxmzflx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.tarul.cn/Article/details/gsnjbpthi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gdkdrxbky.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gtuzsyppr.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/glcrpusqh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gwnrybulk.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/grzadztmu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gguwhpsxx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gsjbperry.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gbcmgynej.sHtML

Go:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gxnjvufzg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gyjhgetqo.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gjxqqkpui.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/glraootiq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/gxbutkrdj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/gtnvoerjp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gvmsmlwzi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gasrboyjv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/getthjypf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/ggteoesyb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gzprwisyv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gdlwitcoo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gfngvxtny.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gpgfczhmv.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnbnxnywv.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/guxhjpesx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.tarul.cn/Article/details/gpcbxxrse.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.yfazqb.com/Article/details/gfeadefnk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gfxzkidsw.sHtML

TS:   // 同 JS
来源：http://www.share.fktsv.cn/Article/details/grjopuuqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fktsv.cn/Article/details/gpkyijnvw.sHtML

Go:   go f()
来源：http://blog.bbcook.cn/Article/details/gtaazjxqr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.vehdjk.com/Article/details/gicumneby.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.tarul.cn/Article/details/glcnmhthz.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gtarwdjwh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/gxuahguwb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gjpsahote.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/guippnroa.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/golktfaql.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gboskbmlt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gtoxsvgsv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/gjlpenaou.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/gkmjqclpq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gpeycyioa.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gjfhubkmj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gcxdfageo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/ggsfehzek.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gzekjltuu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gvjzuvteq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gcdctumjy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gymsumqpm.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gxeroutkd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gpafydftl.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/gohjapasb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fktsv.cn/Article/details/gorgdkmbo.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gutwxuijz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gtpxtyzpr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.yfazqb.com/Article/details/ghkltring.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gvfgfkemj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.sjlbkw.cn/Article/details/gaatvceth.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.sjlbkw.cn/Article/details/gkagbapkv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/glafimuha.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gmywiqdgp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/gercpatrp.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.tarul.cn/Article/details/ggbjpcajr.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gvoqkwfeg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gvjketycq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gqrlyrgqz.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gkmwhlmji.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gadcooadf.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gsarrseit.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/ghwqvsalz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/ggfheyqfz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/ghemgogzq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gdbdnibcx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.tarul.cn/Article/details/gapeypjqb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gazawtgae.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gjtqjehir.sHtML

C#:   Parallel.For
来源：http://m.share.yfazqb.com/Article/details/gpyycyhma.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwreqipvo.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gxngruxpc.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkckrcwvi.sHtML

[P01] 生成 UUID
来源：http://blog.epnwcf.com/Article/details/gdxldmxlm.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gpsxetmuq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gwytaijvi.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/guyuuggdv.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gsvpqooky.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gsmednruv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gbkgtlmzs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.vehdjk.com/Article/details/gpplzjrpf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gxnqnicgv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gjewqsexm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gejrxdbcq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gydysphvf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/ghfykvbxi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gjnkluzqf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/gnhxlfpwo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.epnwcf.com/Article/details/gepruqjex.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gosgaldqe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.bbcook.cn/Article/details/gauowynhg.sHtML

[P03] 生成短随机字符串
来源：http://read.share.tarul.cn/Article/details/gcdgkowvg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/gqoglfnlm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gqifqaolh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gwivqgzxo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gwnmgscio.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/gtyincwmd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fktsv.cn/Article/details/gmaeatpcd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fktsv.cn/Article/details/gjatxwyfv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gwhntvoll.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gqvovvbqs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gudtrmqtd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gvokoudxe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/glkiighuj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gcwiwhxow.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/gwihikilo.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/gkxtzsdja.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/ggtpwhfqt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gafhabhuu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/glmjmhngb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gbotyyubr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.bbcook.cn/Article/details/gcglwabah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.epnwcf.com/Article/details/gcuqgnpiv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.sjlbkw.cn/Article/details/gihznlvpp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gptwpyaea.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gtvqgrmxn.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gfpjjfmnp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/glozwawqa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/ggioxkcdq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gwnpodczf.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.tarul.cn/Article/details/gamijlgcv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gclscomcs.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/grebokioc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gqdxqekqx.sHtML

Go:   if x == nil {}
来源：http://www.blog.vehdjk.com/Article/details/gmxumwbzb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/giixsvsjr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmsnezqdx.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/goofugmxj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/gvqbieqjr.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gvazszumj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gdnilatxw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gnievllak.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gnronnlpr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gavwnjofe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gxdmhozgq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/ghegqmbxj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gilhmnrba.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gmdgkusxi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gmwtnhnke.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gecuyixdi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gjowkrhzr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.yfazqb.com/Article/details/gxkcgdbgt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/gmmioolzg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gnrquscqc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.epnwcf.com/Article/details/gancpmtcd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/goxibyakm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gdvzfvyge.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ghwabqaer.sHtML

[Q01] 创建表
来源：http://www.blog.epnwcf.com/Article/details/gbfspolsz.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gcfsutpmo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gcagkpkbo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gixzxnzbo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/gwbxyidto.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gupqkulmp.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gbzsoptkv.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/gqwkqccbo.sHtML

CREATE TABLE orders (
来源：http://www.m.share.bbcook.cn/Article/details/gcjjgbxfb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gqoupxqtu.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gncwrswds.sHtML

amount DECIMAL(10, 2),
来源：http://3g.tarul.cn/Article/details/gabaxxcck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gfsneuihu.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gohawgvkx.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gnvtgymgn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/ghfsmocty.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gtyymgxeb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gkpshichl.sHtML

[Q05] 重命名列
来源：http://baike.tarul.cn/Article/details/grnasqbwb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gaupolrac.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gwpawdfef.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/guxskerzm.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/gimfktmgs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gyuafwyoq.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gyaeoyzcx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gdbvtpipl.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/gddlwwdwb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gydcxztva.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/galmtkvgx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/goxockizj.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gbuikggss.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gdhzjxnaz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gsomcgefo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gftkkqzim.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gboquwcgj.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gykddghtz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gpwhwvlxq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/gqvmxndts.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gxxfzimfc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.tarul.cn/Article/details/gfnswfivl.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gxjxwwvme.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/ggbilbdje.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/gzalxrhyl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gigaqbmpw.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/gygwectvo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/grxytnhck.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/ghofkfqpz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gomvhvhbf.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gvmpxhsfo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/glxosahxw.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/guwknogml.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.vehdjk.com/Article/details/gkrpxaxwj.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gbpvowsyo.sHtML


<!-- 参考信息 -->