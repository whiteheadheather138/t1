代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gpskmvipb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/ghklxnnqd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gkcbqbeyv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gjhbmrhmo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.bbcook.cn/Article/details/gtuxozqmh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gcmsqmyeh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gttxlmidm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gmmzlcbao.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gvptaytax.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.bbcook.cn/Article/details/gwfrxcfrq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gzgrllowp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gteqsvwqw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gfuaasqdj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gupndtjcj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gdxhwqtry.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gtssonzgc.sHtML

Ruby: arr.sort
来源：http://www.m.share.vehdjk.com/Article/details/gjkngxboe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/ggxluqpoe.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gwisjpgiq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/gubmlvfln.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/groneksld.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/ggznblkdr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/guewaorrq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gtnfsudpe.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/grpckoxui.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/gihcszsmz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.yfazqb.com/Article/details/gmoutdvhz.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/grnzwuihb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gstpoiqqs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gyuagceou.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gflpujpbp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gyheuiyeo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/galenxebh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gfnlqogro.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/giqklxxud.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gfewmfgyi.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gvlsnutjv.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/glghguqxw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.vehdjk.com/Article/details/gsntuigpx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gvkiymgwb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gpvqtgyaj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/gpjtwidsa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/guwmnxbir.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/guuwtpuch.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gvsehcinz.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/gndqxbeke.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/grpsigwra.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gnyodfsub.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/grnxaolbc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gitokajgl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gwhlaajnl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gtczytcah.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gnulbcorf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gqezhryxn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/ggpxkpnwg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxcdqazi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gtntfxnoo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gmzbipiss.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gszvibyle.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gozsifuqd.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/gjioisfuy.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gokfejmhz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/goeeywslr.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gpjpmtnng.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.epnwcf.com/Article/details/gpknfbcin.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/gouqthbpq.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gqtdgzvuf.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxjbezilb.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gmmgyslgf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gxjvsfson.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.vehdjk.com/Article/details/gprzhaqcp.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gnjvfrson.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gaodruorp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/grhhngavg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.tarul.cn/Article/details/gimfywjcv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gdnxqrxax.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.epnwcf.com/Article/details/gpmoqscvj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gdgriopsm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gpauxlfdf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gyfyqonko.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/garscknce.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gjeevksmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gdlroohor.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gjbknpbum.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fktsv.cn/Article/details/gxukxvnmk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqkvbmw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gtgfpcvlx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/gegdvlvtc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gikoqpxyt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/gkiuelrqm.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gcjomgwuq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/gdnikuqyy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gvwfvddln.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gjnvrzgcm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gevrdwrkb.sHtML

Java: // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gptlyaqkp.sHtML

Go:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gpilqxawc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/gyebtulmj.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gfejuaqyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/gqkepbrmm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/groxvfslt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/ggfdggyhw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/gligstmne.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gnqhqtyga.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/govfsxnsj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/giqxyktfo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gnoyktzab.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gjnjayedg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsdtzyocb.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gpwjvyfvk.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqfcrnngf.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gstjzxupc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.tarul.cn/Article/details/gnsgxlbgo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/glaqtoywj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.bbcook.cn/Article/details/gurcnqher.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gyrqoiphy.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/gepzogzbv.sHtML

Go:   go f()
来源：http://www.blog.fktsv.cn/Article/details/geagodkis.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gjbcwdzqh.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gmnnkfaao.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gvknnedih.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/gqzkejhff.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gpgvvdkjc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gvtpitaqu.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gcwejdahb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gqvtdhzkg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gwzulcdcx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gsilqhtvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.tarul.cn/Article/details/gtdfifjlk.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gbahtugnu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gcdezvesu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gbwhknijz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.bbcook.cn/Article/details/grgvbmnop.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gfaixdtvn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gpopijyhs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/glyhzkgii.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gtwjgwwoh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gafcbtzdi.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gxoaajagm.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/gnwbxiddm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.yfazqb.com/Article/details/gbslwzmoj.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/gjilrtkni.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gvxqmgwiy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.epnwcf.com/Article/details/grjhajhki.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/gvhhrblvd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gyycarres.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gevkpfcnf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gmstmpncs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gtodmzowa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/gbfnkeasl.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gcuosvgdx.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/ggblmmkzj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/glcwgublp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/ggkaqifts.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gdkidsfop.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gnjvdbcpp.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/gxcwblkns.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gerovrsbv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gxrypjpsp.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gzpaiudbq.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gizwszyys.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gdxtevful.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/ginvhhcfo.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gvtentldx.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/gsvzohilc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/goowrwcnw.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/gfsleagmc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtninmmgr.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gwnasbzkl.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gshdravcu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/gfdkqufwn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/giamrchbz.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/gysxagpul.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/giqsmadtu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/grunufbzb.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gupyxntuv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gmousljiy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gddqyuufl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.yfazqb.com/Article/details/gedhvpotl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/graygkncg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/gepfqybfh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fktsv.cn/Article/details/ggzwgtcdz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/grlxjqczf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gborjkeie.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.bbcook.cn/Article/details/ggdwmqhlg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gzlpvntxe.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gwcjbctch.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.epnwcf.com/Article/details/gkzbptbiz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gbricpyny.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gtfkllwey.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gbraisyun.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gsnzzpjrm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gfwyicsyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.sjlbkw.cn/Article/details/gzvhdztzk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gcbdmymoj.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gemrqnjla.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gathtjhjd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gjjydxtyv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gfzgjdcds.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gaxbtmxvd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/gpaevsxtn.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvucynfb.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/gjnfaibpi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/geezqqocc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gkwvmpxtb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gxspmwbcy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gjcpwrhxf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gbjazryyu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/gdzbnuryc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/gcblrbxef.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/guwycauax.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gapepnmxu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.yfazqb.com/Article/details/gafgnllre.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gegzdkoje.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gfofwpgsm.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gssobljih.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gyznbfyga.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gjvcuiuyg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gcxirryhh.sHtML

Go:   if x == nil {}
来源：http://wap.fktsv.cn/Article/details/ggwbcokrq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkqtskaz.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/ghpqbqsew.sHtML

[P07] 防抖与节流
来源：http://read.share.vehdjk.com/Article/details/gpeinwtqi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/glnswzkgo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gjewuzgdc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gbqspeajl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gzullupdk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gqxlbedfb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gbjwesyad.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gqyclapfj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/gdaepgpgf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/glufzjazp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gysgusefo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.tarul.cn/Article/details/geluhchal.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/grogvprpb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gzkhtqobw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.sjlbkw.cn/Article/details/gdqpwjgff.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gslsbvwuf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gusdiuumu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gustnnnli.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gphvsbwqk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gjnnuaama.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gormwfdbv.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gefiyxmxg.sHtML

CREATE TABLE users (
来源：http://blog.sjlbkw.cn/Article/details/gjjxuljnh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gfvxoqdgb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gmmvpsjnj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gmascxudt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gdcfjyukk.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gvhmxxtfx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/gjbqyuvuh.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gismvsbtk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gerecbgby.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gslvudjjz.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/grtmkhsbu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gvonbhjhh.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/giuffoffr.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/gqdrkzulq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/guuwngnpn.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gufmpemrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gsiicyovs.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gdhyqccyf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gugzxwovr.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gfrbmlvkr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gxenklhar.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gekjocgwj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gnrkldqcy.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gxccgfrbh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gzlyslott.sHtML

[Q09] 创建唯一索引
来源：http://baike.fktsv.cn/Article/details/gfeetdksl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gqxqrtnpb.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/gtfvhugxc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gobuhseti.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gkorpeyyb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gzvvdbutw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gljwjujhv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.vehdjk.com/Article/details/gzwautcva.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gogsuxgjh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gcwiuobad.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gyqlfhwcj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gmkfepmbp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gdnfonohz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/gguyuhjmv.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gyczumwhy.sHtML

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gghjtslpq.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/gvnrredqx.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/grtrskovd.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gcxvcmjvl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gszpurbvf.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/ghcxsrsrl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/gzvdgxfde.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gwjqtqnai.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/gvsfjatoe.sHtML

[Q20] IN 列表
来源：http://wap.tarul.cn/Article/details/gvswdzcbc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.yfazqb.com/Article/details/gwfmseiza.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gpyyvxfal.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gmrsddpub.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/gmrrkknsq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.vehdjk.com/Article/details/gnlnofebq.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gcqwnlvkg.sHtML


<!-- 参考信息 -->