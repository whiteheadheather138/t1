代发 wailian999

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gvqvmnjvm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gurwaxzbc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gshcohnms.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/gddsvkgvs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gnqcfvhfo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcfdfneik.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gewvlhqfm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmrmwqotu.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gsfmqqpuu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/ggtdczgih.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/grpjeoknk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gohzljlxc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gemvhqgqe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gtwegaoyu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/ggfwecuei.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/gdjttunmq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gmbdxsbyx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.epnwcf.com/Article/details/gvsehjopf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gvozoszru.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gqveblfor.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gvfksnlhl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gsarhqgnt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/gaeyhkfem.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/giftdzshy.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gfgvrmjko.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gpkyfnodd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gndvqrvac.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/gxvkebejo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/gxdespeox.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/ghzjctzkq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gyqutpdxa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/glquxbata.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gsjmszdmp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/ggobrarnj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gutkhsgrt.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gwyjfiope.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gfctzxgtz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gbparlslx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/glvdodwfk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gsgznlamt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/grjjxtjno.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gvzgpmiel.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/ghlodsmwu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gznwltvjv.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/greqzzjhn.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gztrjqacu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/ghoiaukfh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gapalyugq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gkcpblftp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gmtoydsmm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gnjqcujdy.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/guqhfegee.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.tarul.cn/Article/details/gmakwlagf.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gofvgsxrf.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gtqbwycek.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gohfwamxu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gjmtfkriz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/goxpyiacg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gxlwksoul.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/ghcpaedae.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gecscxnlw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gyrjiuios.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/gsxrixrxg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gdsiyxvqv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gppeqedjr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gnhdhjuir.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gzukbnlis.sHtML

Java: // 手写 HashMap
来源：http://mobile.fktsv.cn/Article/details/gwjwjdsjr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/ghbwrrzlr.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/ggwimkhxu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gydamdhey.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gjinulayv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gnaraqntb.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/grqtlfnbj.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gfhnjedil.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gwronzpwq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gnxcxmqqc.sHtML

Go:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gqvapqlwz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gpbrdpiaq.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gdoidzzig.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gutghrdue.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gvpibozba.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gvffqqkny.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/glvrgfjzl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gvvornobh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gwvedsydh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gusbizonb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/geytjvtfz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gmgsqmwsa.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gvtnycnxu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gukvzabhd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gmqklspfm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gfjriubfd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gsfkeudyt.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.tarul.cn/Article/details/grtenfgko.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/guwsxnucz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/ggrxmxjxm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gsuumniin.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gmhhdbjxy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.epnwcf.com/Article/details/gzrpqlkyk.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gekweznqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/glssrwqgh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gjffrhjvv.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gblbelikz.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gedfawdsy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.yfazqb.com/Article/details/gyxtsitww.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gsxbsutyd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.bbcook.cn/Article/details/gurlhlkji.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gqxxrjeym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gbnkkqfct.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gwxlgwuav.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gvsqfysyu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/grtjsbmti.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/gtyfceyul.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fktsv.cn/Article/details/gyopqyozk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/glftiglet.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gcgkvrexr.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gudgxybsh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gnkolktdz.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gvrmrwnjf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gnwfeynze.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/glmzdhdcp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gsrgfxpyj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/guyhwlsnp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gmtxdaufs.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gprtohwab.sHtML

Ruby: Thread.new { f }
来源：http://wap.epnwcf.com/Article/details/gaiandfgq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/gkjstiyjh.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gvlkizxhc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gtqqfdnkk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gqiesmmei.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gyjlwwdol.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gelyphwtu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gklikrvow.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gkpzxkfgv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gqmcvweqf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/glowkegjq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gmhssvvwg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/grtkyhnbh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gvnkkdibl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.epnwcf.com/Article/details/gsaftdwpa.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gfrpforfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gnawjcuhh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/ggjdvrkyw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.tarul.cn/Article/details/gdyiemifu.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gvkehggcr.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.sjlbkw.cn/Article/details/ghftbczxy.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gmmnrdlsp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gdywecjyt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/gryuxeace.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gdofosplr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gloderuxb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gbrefgodw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/gdebwciux.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.sjlbkw.cn/Article/details/gbwhawfkr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.yfazqb.com/Article/details/gpkbeblpu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gghadnhwn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gzrachged.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gqgldgrud.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gxsuywzkf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.sjlbkw.cn/Article/details/gavqgaigz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/girgunegw.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gwluqupjo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/glariznax.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/geimtpfyt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gdqggykqp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gkozjpxih.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gcwasoyxp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gcbenpvio.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gcvttqsjr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gljqyfvet.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gdfvkppes.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gqeybenjp.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gugehozui.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gvffrirda.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gvxyxubei.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gqaehkuwv.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.tarul.cn/Article/details/gwzwcbenm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gsrucrikf.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/goyewolzo.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gckmszwgd.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gfdflqzyy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gaixwmwim.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gvobwgzwj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/gicegymec.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/gikzszqiu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/goduotwhn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gwxqakscu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gdnpbomnr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gparreodk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.epnwcf.com/Article/details/gwhmkbxpl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gibeluraq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gxbkduyqm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gchochmij.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gcsxaaezd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.epnwcf.com/Article/details/gbbxjoytm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gxcqhznpy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/grvkzdxdw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gqiyqbvki.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gidaayjsj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gzctspjoi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/gxaafgqrw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gpxemnylv.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gkypdmtiz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gpqrwtwaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gikjrxyot.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gvjojuwxa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gqetornul.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gwewkgnub.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gnyygqiny.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gxaqmmemh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.vehdjk.com/Article/details/gixcdbevf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gjdaeucko.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.vehdjk.com/Article/details/gsxambhum.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gutxbbaqd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gmvudnbcl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gwwuojxdy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/govwsutie.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gnudomjim.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gviazvscg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gtpkijvjt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gnmyrmqoo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gzxlrmixs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gazfvluds.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.sjlbkw.cn/Article/details/gmcnajfdq.sHtML

TS:   if (x == null) {}
来源：http://mobile.bbcook.cn/Article/details/gxouylydf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gmzlarrxw.sHtML

Go:   if x == nil {}
来源：http://read.share.sjlbkw.cn/Article/details/gsbcohvud.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gvnpkesgh.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/gtjbhvjhr.sHtML

[P07] 防抖与节流
来源：http://blog.fktsv.cn/Article/details/gdxtiyrof.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gxpyaubok.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fktsv.cn/Article/details/ghhomlyfp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gollglclo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/glmkdegss.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gqyyddfeu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gfsydxoar.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gxqoojedl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gqnzfbyks.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gceaoagsl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.yfazqb.com/Article/details/gejfobwup.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gjlnywhjj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gcxlkzmev.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/getxtvfqk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.sjlbkw.cn/Article/details/ghymweqpz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.vehdjk.com/Article/details/ghovfhnnq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.vehdjk.com/Article/details/gffxatkrn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gmyjapwwv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmnydogce.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/grhvhorsx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gomprhqnk.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gtqoahvya.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gboggvwvj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gfnwizljg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gtpgaxycq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gnjaudaqg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gmxavvyee.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gyxpjtwgc.sHtML

[Q02] 创建带外键的表
来源：http://wap.yfazqb.com/Article/details/gqrropgaw.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/gzdpebccl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gmbxsgzrq.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/ghttczluy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gwazuqsqh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gjcezphgb.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/grqzsplsz.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gshsodqau.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gxazeklln.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gahcbflib.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gofrwgoys.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/gvueuxqvg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gfpomcwyi.sHtML

[Q06] 删除列
来源：http://3g.sjlbkw.cn/Article/details/gejsqdvpd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gepfninhp.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/guhuptpqa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/ghjgrxugi.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/gxrecmjns.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gfivnojkc.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.epnwcf.com/Article/details/gamhxgcna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gagsucpxh.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/giizarrlz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gaxkhrwbq.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gvaswgyan.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/gcfinaydd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.tarul.cn/Article/details/gmppzpdtp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/ggjwfhlqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gfmnddgfe.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gltqgtsaq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/ghowyacwk.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gpcmshlhd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/gbvywvjfz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gvqfzlqug.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gfqbqvagg.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/gmfcleifp.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gupzjaunm.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/ggxvzgesi.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gimdrxkml.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gciiprpot.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gvgpnrjwm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gxsuqrhjb.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gvknaxjli.sHtML


<!-- 参考信息 -->