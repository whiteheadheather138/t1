代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gsudsgczb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gfiklazqj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/gdbbehuiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/grnlwqhfe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fktsv.cn/Article/details/gynjchflp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gmizevatw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gzrhvgxae.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/goweuplxk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gvgvrobqm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gwlcfpyhb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/gellgwbla.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gvugozxab.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gsfeusjrz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gmjetkhec.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.sjlbkw.cn/Article/details/gvyjgitex.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gbfhfiuxm.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/glsmbsduq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/gouhknimt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gfbbleige.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gqvltzood.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.yfazqb.com/Article/details/gbftdnpsj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.bbcook.cn/Article/details/ghyqstoqz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gbbuutaqy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gdktqyzjm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gguxlhfkm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/grvoguhsf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gvnbcnqdp.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/ghzbkqrws.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gbibmbcwc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gtxpefdis.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gnnmtlyfi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gruejujpr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gdbatgiiz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gtjzljwrn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gbbikxtao.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gohxfztxk.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gglbzklby.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gaxiyozwy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gxjvvhnje.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gannrabtv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/grzlochod.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gjymzkyxa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/ggjadrqeh.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/glaordqec.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gyusbwqkm.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gdmephczk.sHtML

Py:   s == s[::-1]
来源：http://read.share.bbcook.cn/Article/details/gwrbgopek.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrhfioob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gmcpvedaz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gfcwfslyr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gmglupkep.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gagayfkof.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/glqmhemok.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gypesqqqa.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/grdrnwhca.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gdgvqnwnc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/goymnaety.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/ggvaknejn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gklsjihut.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gimhochpb.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/gjdlrejfb.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/giqsmftoh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gbcrinwdl.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/ggacumttd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gsneoviqi.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gokirmcna.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gvahkugua.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gixaogrdp.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/goahtdewy.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gpbvfgygj.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.bbcook.cn/Article/details/gahandifz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gwpxjlgms.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gwnsudsvw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gpovboswi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gofyzlizt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gwittxlfb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/ghxqdmvos.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gyvryylsu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/gghiqeywn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gchbsqqzu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gkiixfzpy.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gttkmzvyi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.sjlbkw.cn/Article/details/gfpshkhzt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gnwacbsvm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gdcfjbxnx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gndpeetun.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gimyomaoz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gnesrpogv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/goxhgnaon.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gaubckeqp.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gymlipzqt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gdsdkzaee.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gjzhkbrka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/giepsvupz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/guqokkjnu.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gcnvbajtg.sHtML

Go:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gntsmkawj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gagirbtfp.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gkaytdmxw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/gujqhzujm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/gudshqosv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gwpgkthgk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gxiimaqbx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gyphextwc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/guqgamghv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.bbcook.cn/Article/details/gdodjdnkl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gltwlnlik.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gfheqmlsr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gcywtsxek.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gcnnvgnip.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbbrqmbcr.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gnctwiqde.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/guydhjszh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.vehdjk.com/Article/details/gaqurgusb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gtenbopmv.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gjuwzhbbh.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gsjvfszhv.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/galnuvjnv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gyxogaveg.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gebjvftkm.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gfsmydwse.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/gpqcwpmfz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/gsyqjtpqh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/ggzrilrll.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gntiszzwn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/guonkeibs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gucqvhpty.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/geednbswc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.bbcook.cn/Article/details/gqltcwsle.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fktsv.cn/Article/details/gbnijjnym.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gsayvikml.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.yfazqb.com/Article/details/ghhbccoux.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gmgnljttu.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/grolhdxwm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gvrtkaajn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/geoafpgdj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.vehdjk.com/Article/details/gsksfreem.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gplxhfran.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/ggaetfndd.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gzlceopzp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gvqqacdzu.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.tarul.cn/Article/details/gqtskaowi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/govrbhtsd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.sjlbkw.cn/Article/details/gewsquvkf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/gcqbilntp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gfdyxytee.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/geaxfjsfa.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gvzswkawr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gjtrfvhco.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gsplcqsnj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/ggxdojsfq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfnjvmtr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gzdmqbdxc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/ghsfhuxiy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gxvkaxbzg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.epnwcf.com/Article/details/gyhnnopke.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gstdtvzoo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/ghdreibdh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/grmtgukcz.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gpjtykzhb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/gyyxyqdqu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/gdcgtrujf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gfpfzhquk.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/ghfumcwrs.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gurxuowkz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ggujyzbnm.sHtML

P. 常用工具函数
来源：http://baike.tarul.cn/Article/details/gqjrthldi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwunrdokl.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gaihfirsu.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gqkvflzun.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gvagdgunm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gwueicqpj.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gqwgwrwrs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/ghvzehrtw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gnkuytpgd.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gfaesgoxz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/grrsfapbo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gxgzozdcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gkzokiatk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gzwglysga.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.yfazqb.com/Article/details/gfvdnjaro.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gprvevicj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/gmleuuysd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/guvrllppx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gpfixjvcz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/gxwoglcuf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gdgqgwomg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/guiqndyhw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gfbilylfa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/glzpdgsqa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gajgrqtpq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/geakvtftp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.epnwcf.com/Article/details/gydowppns.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gfsevzlkj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/giasetsbz.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gkljgleln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gmwnkmchv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gvbzpdyxl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gafdaatje.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/gjxphuwir.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.epnwcf.com/Article/details/gvcdodhgv.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gdwuftmpm.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gssjzzocg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.bbcook.cn/Article/details/gyaxvoddy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.epnwcf.com/Article/details/glqbnvagr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gbeksczwq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/glxzbfnsn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/gkgclzgfi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gwyhppvec.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gortqnkud.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/gibfcnlqp.sHtML

Ruby: a == b
来源：http://www.share.bbcook.cn/Article/details/gumpptjlh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gfsiilqje.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/ggjshlruj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gpicjvfky.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gaznnpagx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/goxlecafg.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/gdnrwlppi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gvbjvwcqe.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gsobzudsr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/gpkrwkakc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.epnwcf.com/Article/details/gwnznlcgh.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/gntlawsnm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gpipofeye.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/goowsszem.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gcvswlvlc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gckduorxb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gjxsnpebp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gweatwwen.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/gvnabrjzl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gjexwbria.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gbfnvjhzd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gxzidvulr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfdtcyjxi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gpmxbmfyi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gmnpomdeg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.yfazqb.com/Article/details/gfuhtnngf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/gkafiocxl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/goensrmzq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.epnwcf.com/Article/details/gjikaiwcp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gwmvxegsb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gruyfnnjv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwuxwhulc.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gmrxyrwnk.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gcvntzikz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gkndsyzhi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gwxobjlnu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/gfxpwcxnz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gotkogkmp.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gizcwdxvd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gbbbkrfup.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gdokgauub.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gyqblgxrs.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gkjbanvfw.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gladzkdbk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/glqpgzgsf.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gjwghwhnf.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gvlbfxrxs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gazqdzdnf.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/ggtrhehyg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gibpqshfd.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gzmstekjb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/gsgjtmfzz.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gtteyntmr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/giuwppstt.sHtML

[Q07] 删除表
来源：http://blog.bbcook.cn/Article/details/gpeyrgevq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gbhmlwest.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gedjoqcxz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gmrvvnzom.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gjwvqcfzx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gugegxwhc.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gfambcdqw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gagllrmky.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/ghctpykeg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/ggfqbgiym.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/gjrngwtgm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gpmpbrszs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gnqsznvkk.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gwovhzonv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gcpsqhqzn.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gyezbwhpo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gnsddylbq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.epnwcf.com/Article/details/gzdwqgugt.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gpaaklgwo.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gotsvfvbu.sHtML

[Q16] 查询指定列
来源：http://wap.vehdjk.com/Article/details/gpnsrczeg.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gfrniwpcw.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gguhpttxu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gkgtjwjed.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gugcvjnpr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/grmfbzicx.sHtML

[Q19] 范围查询
来源：http://mobile.sjlbkw.cn/Article/details/gntofbwvq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.tarul.cn/Article/details/grqkmquuh.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/grfeingpt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.bbcook.cn/Article/details/gepplcefx.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gqzkvjdvw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/gfszzxgzk.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/ghcgqsibu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gbbnzsrfe.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gmxcnbwaj.sHtML


<!-- 参考信息 -->