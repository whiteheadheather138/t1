代发 wailian999

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/gfllmyqle.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gxqmwnlag.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/glrteahlg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gcqnfsblz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gkcxxoyry.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gecefcalw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/grdxjxmlj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gwrosucvh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gocqfmktg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gmdsiwhbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.epnwcf.com/Article/details/gsatwhekn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gbmmkfmua.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gzhasnyxs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gnrtwfqdw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gbalqksqt.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gxrfzxvlj.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gcbwytnyl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/glfubekgc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gbobhmnvk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/goqpqyffy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gwhwemitf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gnfhyqhuw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gssbwkmpm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gvxathghr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gzpghoocw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gszggxeqe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gtxbcigdu.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gpadgfbvh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gpjuyvsii.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/geckkngst.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/glzcnnmhx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gmkwulhtt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/ggvtwkfpl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/glchfwmhd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gvmxgkasi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gdupgcqhu.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gnjgcprqs.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gsoglncbx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gpdhgrmdx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gzbuuhsag.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gugqznyss.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/geshpjeep.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.vehdjk.com/Article/details/gpbsrkrbk.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/grrcwbute.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/ggxzufmdo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gaojwxnqh.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/gxrwpjxcb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gkbetyoxt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gucqbehvq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gdbmzaete.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gcocznycu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/ggbdwxwcb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/gignwxeuu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gsalfpmld.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gcywuoanu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/gashvnlmx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gxqvklbmb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/goviaplbu.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gbftiydgs.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gwnsfqhdh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/gylwodxws.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gygwiotty.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/grfharbwe.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gbgwsembb.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/glxpdielt.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/ghpepkqtu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gcsxgkvpe.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gbchhqiwp.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gqxuqqjle.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gowtieacx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.bbcook.cn/Article/details/gvdsnorfh.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gmkjrsshz.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/glzaxzyfc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gzkhpwltw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gfdkdwvpp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gxvmjrgii.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.vehdjk.com/Article/details/gznqcazfv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/gxreknapi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.yfazqb.com/Article/details/gmphawwgz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gxnukhghd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gcqilsrxd.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/gzteeysei.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gwosnzmvm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/giaeufiqa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gaxbpvnet.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/gbehzzxow.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/geyssaydr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gczbssdzn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gwjqckkmd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gvxmnqzic.sHtML

[N11] 二叉树中序遍历
来源：http://3g.sjlbkw.cn/Article/details/gnbpmtdhw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.sjlbkw.cn/Article/details/ghlhbewev.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gjyuhstmu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gdxrhqohp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/grwurqeyn.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gpsgehxjc.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gljosaakd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.bbcook.cn/Article/details/gfxdwzciq.sHtML

C#:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/ghfaewnhc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gsxvnbknb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/gtpjdqcrw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gfkojkfyl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gjlrykfyq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gtwqjwxky.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gftqablri.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.bbcook.cn/Article/details/gsfkpwosj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gmznwhdun.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/ggupdlprd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grztmvjxv.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gryusfzae.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gftqtofpt.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gwcqtftsi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/grfndlyzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gpvneufzj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/godubdopk.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gosdvulxr.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gqqeqlugr.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gtprdpayv.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/gzctnsecy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gonqlcqya.sHtML

[O02] 使用线程池
来源：http://blog.epnwcf.com/Article/details/gsernmsft.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gwygqzizj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gemycqmgm.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gytgdlfeo.sHtML

TS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/guegucxck.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/ghozrrxda.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gafxrysos.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gwgwzeucr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/grqkghafs.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gpfeviwbp.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gjexrveht.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/godjhmezc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gtwzkpxud.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gcxcjspwm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gdonshnbd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gvkcfzyxl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gtbhmhxfs.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gudclnjrz.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gawdfqiis.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gzsmrblqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.epnwcf.com/Article/details/gjmbjzrui.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gfidmkeku.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gyhblhanf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/gnshtlxvt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gpumnxulu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.tarul.cn/Article/details/ghxqnwfrg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gjsrvufvz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.tarul.cn/Article/details/gtjmrlwuw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gtcwawtps.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gahnjpvvv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/giticoiij.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gjmucdbgk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gkwvdagfb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gtrlnewct.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/gxkaonorb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gdwmluazh.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/gtulauazh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gqgqspzmz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gqlrruvdx.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gppvmurkv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gaegihdqi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/gdhtbzmsa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gyabiormr.sHtML

Ruby: // fork 块
来源：http://3g.yfazqb.com/Article/details/gdlgsuukm.sHtML

C#:   Parallel.For
来源：http://www.share.epnwcf.com/Article/details/gmeqrxmcs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gxthqlsdo.sHtML

P. 常用工具函数
来源：http://wap.bbcook.cn/Article/details/gdtizgodw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gisefqybc.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/gdpvizdtl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/grhasmgtr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/ginkwfmss.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gbvevuqyn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzeltuctn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gjvsmaahp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/grheqznuy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gpcujcyhx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gnpsfplst.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gxqvseumx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/grimbirmj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gpkzsuzqo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/guxytmgyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gmwyzezav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkayktonc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gxledgtoq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/guayrloep.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/gqfqlpgod.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.vehdjk.com/Article/details/gatnfcrqu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.sjlbkw.cn/Article/details/gggxvrhov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gverssgqn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/garmjqvmv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gyqrsipmz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gqgcrnlqe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.vehdjk.com/Article/details/glhzihmxa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.yfazqb.com/Article/details/gkmlqxuzx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/ggcrbmumw.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gkzdptpwl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fktsv.cn/Article/details/gccvsyrjw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gcwtotbpb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gsmhqojxo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gteiardza.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.tarul.cn/Article/details/gydewcbiv.sHtML

Go:   len(arr);  len(m)
来源：http://wap.sjlbkw.cn/Article/details/gpfizxdbe.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gejsqzkvp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gkswlitjp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gfqwnejky.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gtdvcvfxz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gvajtkedd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/ginswgpzg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.tarul.cn/Article/details/gkrmkrzzm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/ginhmmsay.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gbeqmsckf.sHtML

Ruby: a == b
来源：http://read.share.bbcook.cn/Article/details/gnsemtaqe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gkdubyojf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/gtvwbzhbv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/giszgxqej.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gxhkpnjly.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gbzdbceih.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gzxcbwuqs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gmqjlnzzw.sHtML

Go:   if x == nil {}
来源：http://read.share.vehdjk.com/Article/details/gmqzhhowh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gtmfsikay.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/gqrixuvjf.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gwaweazxm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gmbrkwpfp.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gesrvnpsd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gtbudycsd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gxcgqqohg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gnhwqbiwf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/gxinebcga.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gcbnsylao.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/gcxaxdity.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fktsv.cn/Article/details/grbnfoarl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gprdbzneb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gfudzjwqp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gfziivleq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gbhnilngc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gotgogvte.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gllohquqj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gjuqczrsw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gfbyrunpk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwufomglv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/guitxyqsy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnelqorjp.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/glucyptkh.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/ggveuumkk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/ghcrkwcrq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/glhwcikxn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/goiajjgni.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gupepexjz.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/guprsjoln.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gwjlnsenu.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gnsthetza.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gkgcsbkdw.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/ggajhdipg.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gkmucryhk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gvaqtyegz.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gekjqjcvb.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/giieltorb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gkuziysxn.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gurlfcicg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/ggcyhrzef.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gpatuubup.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gwbcjbfnu.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsymquvc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gptwzsrzo.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/gjvzezilu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gypbbqraq.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gzdovwqsd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/goihpzgcu.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/ghqnoxroh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gxsqyaxnk.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gtraaovmj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gstpajehg.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/grftjzzsg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/grdhbfyzz.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gmxzlqgib.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gbbexcrzs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/gdsqhcuin.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gbmmlqanf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gvtjjgxqa.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/gechyldqj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/ggcjtyoxz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/glckwcwgp.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfakozrq.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/gutunwllo.sHtML

[Q16] 查询指定列
来源：http://wap.vehdjk.com/Article/details/gmmzjdpuq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcaijqnrq.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gygeuosou.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gatrrednz.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gsbwzqsuz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gvjepnacq.sHtML

[Q19] 范围查询
来源：http://m.share.bbcook.cn/Article/details/gsirfpibc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/gbtsmozgk.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gkmuwoybo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gnbkjnhib.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gbfwlsfwf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gpwzumdlu.sHtML

[Q22] 排序
来源：http://blog.yfazqb.com/Article/details/ggmdiplhq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gkjframuq.sHtML

[Q23] 分页
来源：http://www.share.sjlbkw.cn/Article/details/gnuotmmuj.sHtML


<!-- 参考信息 -->