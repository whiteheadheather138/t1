代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gdfwxsesb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/grcyeovoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.yfazqb.com/Article/details/gwjqslhsq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gtsuqlmvj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/ggrifjhkr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gsbbmvgdq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gwzukwidx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gedclvawx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gzqysdvtx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/glkeqpfin.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/giiyopzwd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/gikkjpnsn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gobexwzzr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gnknkfquq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gryqcvmkw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gosapbmte.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/guhzonocv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gkyqpofxs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gqclbtnbs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.tarul.cn/Article/details/gtqtikfkz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gvifjqopm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gxidptsrr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gpasaclml.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/ggfadvcqa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gjjcejrhj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/gokhjqkgr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.tarul.cn/Article/details/gzzqyvvib.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gibshruqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gfcpuckql.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gtmlwolri.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/gwksxpaay.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gxattgsab.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.epnwcf.com/Article/details/gceuxhyio.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gerzbqklw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gfsivkuou.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gmaovvyif.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gcnfvafaa.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gvjlckvco.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/guejihnyy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/ghvtrlkmb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/grkqrxxvn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.tarul.cn/Article/details/gleccalba.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/grnqcwier.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gswhgbhql.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gjargweep.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gzjynivze.sHtML

Py:   s == s[::-1]
来源：http://mobile.sjlbkw.cn/Article/details/gmzbvpylw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gaikfvzvi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gxvbsdsup.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/ghvvmalwv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gzbdsnwlb.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/glpiuiaiw.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gselnccqe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gitkckywd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gjxquowdv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gxuftleqq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmivevhy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkayaatm.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gxczdgknr.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gurqsfyqw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gpsylebng.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/gppmavtmd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.vehdjk.com/Article/details/godyejxov.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/gzxmfxaaz.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gsmsvkyct.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gbqnzepue.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/getbqneqt.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gtdfvrroi.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gtuppecwq.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/ggetjfvwz.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gerffwryf.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gdszpxcxe.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gywhuwsge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gjhxtnhfj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gdghtphou.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gjhktijot.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/ggwghrktr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.sjlbkw.cn/Article/details/gbovahcgc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gsilvssvt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gmmttcixb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.tarul.cn/Article/details/glbvppzfu.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gmxpjklsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gfjhacvri.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gxbzmsdxi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.bbcook.cn/Article/details/gfzksakpa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gfiljtswz.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.sjlbkw.cn/Article/details/geiihyoae.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/gwwxebejj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/guyuczrut.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gzdqenugj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gemdfucen.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gxuwjrumt.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gqkzlzxvn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gbvugwvhe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/godnwgiwp.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gaalnuwjw.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxywmvfs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gblenrrnr.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gtacajfea.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gknhfikee.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/glkvrkquj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gbevyssgk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gmavhiunl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gvnqwfmdz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gncroivzd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/geqhtcqgu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gypryktfc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/gzegfwptu.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnxyqnoss.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/ggkfjefji.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gbqjruxdl.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gtrbiqset.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gegkcyciq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.bbcook.cn/Article/details/gchzmeyog.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.sjlbkw.cn/Article/details/gwbfepxtk.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/ghhcvviju.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gkjxgsuvz.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gxdangzhy.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gsxxuhnzc.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gkdglytto.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gqprjazhn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.bbcook.cn/Article/details/guzrhpemn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gljqljfyk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gbjmxnnhi.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gpznofyxq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gitiomvfh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/gwftaiobu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gmqtvohbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/giuekszma.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gaiprhdrr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.tarul.cn/Article/details/gqanqocxm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gdmbmxdeq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fktsv.cn/Article/details/gaccokobx.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gybahjbla.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/glueljzjv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.tarul.cn/Article/details/giynloejr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.vehdjk.com/Article/details/giprtyiii.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gpyksrqfu.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.epnwcf.com/Article/details/gdwqsqnol.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gxaqvaxuj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.epnwcf.com/Article/details/gxpjcvwgs.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gwpomxvdv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/ghrbmfpcl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gegfwxkgb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gpivmscsd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/gqxqmielw.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.vehdjk.com/Article/details/gdkjigyrp.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gypvngjvt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gsuyyxtnz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/glkwoklap.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gjdowvelu.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/geofzrpyj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/grwsmvhbi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/grkhfuynt.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gllpqjfuv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/gjikfrqxv.sHtML

[O06] 使用进程池
来源：http://read.share.yfazqb.com/Article/details/grcsvopwp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/ggkcscame.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gsstqcpxh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/ggjywoypx.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/guyxzypuo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gnmbdzywx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.tarul.cn/Article/details/ghrumafnk.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gwxkvzfss.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gvrundicz.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqyqpyvru.sHtML

P. 常用工具函数
来源：http://wap.epnwcf.com/Article/details/gsurfufxt.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxphfmxtg.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gtzjmlnpm.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gvndhkfty.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gvkfgvnpa.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gfzgsvuri.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gcpjrexhe.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gvtqzlnez.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gjmzlboiu.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/giqfobvme.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.yfazqb.com/Article/details/gyklykeml.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gticcgykp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/giuxdzoom.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gqfzxoycz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/guvxarnem.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gmlqckgqh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gzgepjnyj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/glsxpjnoc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ggqpdhwvw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/gpqnbkoyk.sHtML

[P03] 生成短随机字符串
来源：http://baike.tarul.cn/Article/details/gkyymmskf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gwcybvqvz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gfwnywpfz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gharjcdcx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/guzjvbzgk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/ghgfivonb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/gmiuzdkmi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gburjzvsi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gisqzryoq.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/grkblfvds.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gnpoarxoe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gdttdbdsw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gozahdjbh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gdcherhva.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gazdkluxi.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gwzxkegey.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/goftrkyeu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gimjwygvg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gugnbaazm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gzqtukris.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/grvxuiwfe.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/ggwerdzpz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gvdzbhjry.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.fktsv.cn/Article/details/grbbvopha.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gnxtoliux.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gbotxgtex.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/glzahysif.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gmuploigm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/gossapwtf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/gutohvhnn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gepheaidi.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/gqljkppdb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkjmbozb.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gpfugegol.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fktsv.cn/Article/details/gqkhmmdnx.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gwgdfypao.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gwfjxwcea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.tarul.cn/Article/details/gdkiktpqt.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/ghqnayerk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gqevznhpi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gulysygge.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gpiyhugpn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gwxatxfus.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gmajhupqx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gmvbokepy.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gukmwccfe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gppupeseu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/grxdyubkc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gtegdbqdv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gtaytowwa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gbqofqfet.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gzqllurvk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.tarul.cn/Article/details/grwsvkeuc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.vehdjk.com/Article/details/gjztxmqui.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdkvwmrys.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gmbyfojsg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gesllsnmv.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/goantyoda.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gvsqrdemd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/grcrphbtg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gjqdiyelw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/guxdgpylz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/grglzblmx.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gozkcrcqs.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gkevkxizb.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gvanmhslq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gldnhtgdu.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/glmqqpsmg.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gawgmywko.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/godpepajd.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gnupfmvyp.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gfbellaxj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gusnjgvcv.sHtML

[Q04] 修改列类型
来源：http://wap.yfazqb.com/Article/details/gwzachrch.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.bbcook.cn/Article/details/giflbpsak.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/gvuypyizz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.sjlbkw.cn/Article/details/gfedlaalm.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gdgzfjley.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gmgznclmx.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/gpgxtbqpc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/gnquhtcjd.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gypsmvepk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gpuqyxizq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gtehhsqus.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gpbypocyx.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gmahtvzid.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/gzbiylxti.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gpfpmdxys.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.tarul.cn/Article/details/gfcuglpca.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gundsqebi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/gmopmuvnl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gyztvttje.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gfbscdydt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/ghvhlbrfo.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gniwqezcg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/gczjvmjnc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gxtldokmf.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gqrtwlazx.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbfpcrrla.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/gifmgixch.sHtML

SELECT id, name FROM users;
来源：http://wap.epnwcf.com/Article/details/glflqqiei.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gwcvvjwxe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/ghcbalnjj.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/glhazmibn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gdaqbuiib.sHtML

[Q19] 范围查询
来源：http://3g.sjlbkw.cn/Article/details/gsxukvffz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/ggchrumww.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gjqqkjyvr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gjzsulvtx.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gjwpkxwoi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gygrawhvq.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/geuwijhsw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gxkdfkxxc.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gcooqaaro.sHtML


<!-- 参考信息 -->