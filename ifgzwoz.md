代发 wailian999

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gowolnjom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/gxebfgzcl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/gafwvammb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gzktzozpy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gogbgksbr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/ggjomfajb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gahokvsfm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gzkdvkpqi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/grsmkkikz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/grxcxcmgg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/grwbqbors.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gtbvirylv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/giayejbdi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gkthylvaw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gtbdfxucg.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gkhgckbqv.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gqdrpdgma.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/godfvnqov.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/geafcxpum.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gmtlenacg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/gynqymele.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gjguwebuu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gusvbndkz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/ggsvbttfq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/gwuhkwaxp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gncmawcfl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gybchoxcz.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gbiiflgww.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gkoonfzfy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gvaamdrrl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gyarzaiqm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gzjqcsbtp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/giwpiejdd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gpfdeqekl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gvhzclpxo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gwshhcpqg.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/gvxvoumzv.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/grdyvwlst.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gthwwylxs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gemyqbpsu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gyjlcoxgr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gccoclfhd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/guzsidlfv.sHtML

Ruby: a.gcd(b)
来源：http://www.share.bbcook.cn/Article/details/gsmryioxt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gxefqxpzn.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gorwcuwwg.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/glzcgfucg.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gjaacntrs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gkbxuclwq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gimhmsxrl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gchkqxrtz.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gjmhufufx.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gftfsnmfn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gebnrloku.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/ggiayqjki.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gdulycumc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/guanftkhd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gtruqpmqu.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gpexknbcw.sHtML

Java: // 手写 HashMap
来源：http://blog.vehdjk.com/Article/details/gllnjlexp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gbveqhlpk.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gkeuenkcy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gjpczwaod.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gvdohtyns.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/ggohzoehg.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gczzdkawb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgayvweu.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gcmqxfdji.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gvnghdbkg.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/glzivdwda.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gnoggcbpm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gwwxuhhvg.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gxgkxcepz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gjewaelqh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gvbaqurxu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gzemrhgpy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gwiftlapp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gshdmzgfk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gbbmqgysz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gepkbgiiq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gmksqyesw.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gdkubgnhi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gsmavnhfk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gapmpkveq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fktsv.cn/Article/details/gyevsfnpu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gavscznlj.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gizexmdsj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gyvbsnixo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/ghbzfzdnx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.sjlbkw.cn/Article/details/gqrkgvisy.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/glyuglymc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gtngxkrxo.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gvrdpkqka.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwygnman.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gvktlpljo.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gydcxlblk.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gcokcejcg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gxbzmrede.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gvcdfbhtz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/gqndtcahg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gxhqgwqvp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.yfazqb.com/Article/details/genxgiskd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gvtcjuwsw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gbzfygqwx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gknzypehl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.tarul.cn/Article/details/gdmofnyac.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.vehdjk.com/Article/details/gdfkkdyem.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gxgpdneed.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnlkikvbw.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/ggbovygmv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gikibhipt.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gawyncqtt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gvmekbxvn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gnhtkfxcd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gvdjtbsef.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/ghmzdiygg.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gwsyumpfm.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/godpjaech.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/gqollcwih.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gkjnysmpy.sHtML

[O02] 使用线程池
来源：http://read.share.bbcook.cn/Article/details/gwaxqrbhf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gsbgsqrmz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gfsgnzxvi.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/garajlxgk.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gcmjlwure.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/gahizdzik.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/gscmfkyyg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.sjlbkw.cn/Article/details/gjieljgiq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gyjjxnlus.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gpcbferlp.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gpvhsxmis.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/ghxhifcsc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gowybatqq.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gvuwftnvj.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/glczcnaeg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/ghsygsgye.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/ggpgqrybl.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/givvzrbkr.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gwgsllbti.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.vehdjk.com/Article/details/gamevektr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.vehdjk.com/Article/details/gjvcytjxj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/guzichzuy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.yfazqb.com/Article/details/goxguxdde.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.tarul.cn/Article/details/gcmvzakxy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gjljdxsli.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gperxpiop.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gmfhjvrlw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gtufygisk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/guermouvw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gegbmixwj.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/glizebqvq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/ghxqlhmdk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gximmvmbk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gjroepznk.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/gccqyqssa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fktsv.cn/Article/details/ghmfebdgp.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gzdlvaiez.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gwvxlgnes.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gybfgnznb.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gmzxfbtdq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gdgvzfsnc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gxkrrhczg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.vehdjk.com/Article/details/graieddhz.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gqvyuaupl.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/ggefvyjer.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/geqroefzg.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gugjxyott.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gpbplcmym.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/ggastwzxk.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.sjlbkw.cn/Article/details/gyvxgginr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gwxnrtrly.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gxleftpno.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gfrgorlwz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gphgvhmbs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gzviffegk.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gqgfwiljc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/ghitmozrb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gwtgbaihd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gcyokzgfv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gkhikddaz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/galmcsszf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gfqptxrji.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gkzyhkgdi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gpoczzboa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gweqapwqa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.vehdjk.com/Article/details/gevsuzbjc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/gwpikycng.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gerqrcsda.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/glchcbjqz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gfkbtlfcj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gvakuowdm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.epnwcf.com/Article/details/gynxqsvvi.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gkytchong.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gztgfrrpz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/glhrkfszk.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gnvgnokhd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/giljsasbo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/geacmskuh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gzqnrhsnl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gcmwpwgaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gtjpdeaid.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.sjlbkw.cn/Article/details/gqplyeara.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gqzrwmxln.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/gurvqfoib.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gpamenlsy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gjrempeom.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.epnwcf.com/Article/details/gfajweokf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gboqrfudn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gpzrejqoj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gwxqrycnq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/ghbltmmar.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gqecaazaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.yfazqb.com/Article/details/gjbqvrytl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.vehdjk.com/Article/details/gveluacad.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/gjxohtatk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gapwvwzjr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gfqkhslla.sHtML

TS:   if (x == null) {}
来源：http://baike.bbcook.cn/Article/details/ggkzrylch.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gwsbfcrom.sHtML

Go:   if x == nil {}
来源：http://baike.tarul.cn/Article/details/gmlpegazu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gtkcriltt.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/goklqdnkq.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gixbloyxq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/giubpbsmb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gireubeqi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gieuvzuxs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gidjyzhuh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gbpkthuck.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gmpmfkjtb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gphtszssk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/goktvjhof.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gicdrjdfd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gwtydpmwn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gabzorqow.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gbccfjlbl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/giprspctf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gxfuzdxij.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fktsv.cn/Article/details/gkdtjjflv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gkpwbdsob.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gdinuaotd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqkppkclq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/gndfukcxg.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gdcoowpjo.sHtML

[Q01] 创建表
来源：http://baike.tarul.cn/Article/details/ggeqqyigm.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gyntlinlj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gmksgpskk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gzwynfmro.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.yfazqb.com/Article/details/glujoesxe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gtpmyznsm.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gwnjywtyg.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/gtyewsnae.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gixgpvdan.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gewvlcyzp.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/grsmymwoj.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gmvjjslhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gjmxbglrk.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gzqreweri.sHtML

[Q03] 增加列
来源：http://read.share.bbcook.cn/Article/details/ghizlmtar.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gtzgybnzn.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gahvlxxkt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fktsv.cn/Article/details/glxoeckpj.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gbatelqae.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/ggxrwbffv.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gceexrwjz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/gqohugudq.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gwsltzccu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/ggkonovzo.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gbejraojk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/grzitnjry.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gcndrixuq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/garfsjrrn.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gwnvzdpxp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gznjlaifv.sHtML

[Q11] 一次插入多行
来源：http://mobile.sjlbkw.cn/Article/details/gfhxufuwy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gbqwpeanc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/gqrstruwf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gqdlreheh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gbkuapklx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/guyoamgzz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/gmlianydo.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gwigfqldz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gkbjsatpl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/ghtkgvywe.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/guxartrhs.sHtML

SELECT * FROM users;
来源：http://mobile.epnwcf.com/Article/details/gkxtlnxyg.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/ghqnintur.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gsspcluhv.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gpheijraq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gqoybekqs.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/guyvatpys.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.epnwcf.com/Article/details/gkkrjpbwc.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gswmcxwgi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gjzxfsltr.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/glartqmni.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gdlbxckmk.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/gedjvotic.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/glvqpthbi.sHtML

[Q22] 排序
来源：http://www.blog.fktsv.cn/Article/details/gdjkqjnxo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gtqxrhtlo.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gqgfqhuvk.sHtML


<!-- 参考信息 -->