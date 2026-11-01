代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gcdkqcjrw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gtxrawzhk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gzwotvjpe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gebvpjgnu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gnhqbucso.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fktsv.cn/Article/details/gmyolfabt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gjkdsznbw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gygnujdly.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gsnpdoslu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gxsqfvizk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gdngvfdix.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/grysflwdq.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gvedzmfvm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gwcrkqcfa.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gwiwdvzbo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gslsynbxi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gymkaqjow.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gerdkjwsr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gtymkyhly.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gfxcuovns.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/ggwbszcsw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/ghcvwqyyu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gtsldappe.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gphcngrdc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gcyaihgxe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gqpolmolf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gmyrytaeo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gvvlwnlie.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gvomfwccu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/grjciyzyq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gvenheltb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gmrnwtvpn.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gpkwesyii.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gkkgslvht.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gbutpwner.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gsrnfcmxn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/giilqsoho.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/grsltirht.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gjxgljpnn.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gasglwmkb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/ggikfeuxq.sHtML

[N06] 判断回文字符串
来源：http://wap.sjlbkw.cn/Article/details/gvaocxfhz.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/gxkwgakai.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/glloebnjm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gfkrqrvdg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gifwsybop.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/guhniyjhi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/gzsnfrqtm.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gsuvhcbtj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gtnwnrykw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gqrnsqggr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gufwkvsmo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gpnuewrla.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gcksougeo.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/gcbpxfsry.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/gdelextqb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gvqlzqqnw.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gjpexbykn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/gebyabpgz.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gxtgxnrbb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gcoxcqvme.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gnjmrtkaq.sHtML

JS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gzgoskvgn.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/ggfverpjc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/glybunpny.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gosbdsvvm.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gnzdxfifb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbpofrbp.sHtML

[N09] 栈与队列
来源：http://www.share.fktsv.cn/Article/details/ggqdjiccf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gpijzhrlo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gninfoiiz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/grxzbisnc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.epnwcf.com/Article/details/gftzdlsjw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.epnwcf.com/Article/details/gfggstbpp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/glbyindxf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gxokxgwue.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gwrpxwrjh.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gussjsbun.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gxblabbdr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gwuycagrg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/gyaohblom.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.bbcook.cn/Article/details/gbetgvdyl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gcprkdvie.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/gpryngkxq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gbingdfcm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gbcybadpy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gndqklxjj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.vehdjk.com/Article/details/glglfltvv.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/ggoxyotny.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ggmobwduo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gwcphlivs.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gqvdupkoq.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gikmkhrvy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gucgckeei.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gvdebwbcx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/guvbbsvdp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/gtiphgoao.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gcmqzafpy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gmsfyrxcz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gtfkyuzxu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/geqoucdir.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/gfqzlgmmk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gvzihlbzu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/geamdjtxz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/goxobfhjs.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gmwyckwwk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gzkcaxram.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gnpcudlyc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gscmobpma.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.sjlbkw.cn/Article/details/gmhelhkeb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.epnwcf.com/Article/details/gnunvjrln.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gijovzsbk.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gqyliodqu.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gmugoextu.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/ghvxprsqy.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/giwwebxao.sHtML

[O02] 使用线程池
来源：http://baike.epnwcf.com/Article/details/gfccwyqpb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.sjlbkw.cn/Article/details/gvmhadtht.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.sjlbkw.cn/Article/details/gbzwrbtca.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gcjablvsg.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gkltmrlgs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gcqmnrybq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gficlefny.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gfftgjpqg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gcchtehbj.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gkujkqyiv.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/glcrjecdt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gcdwjtple.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/gozxcfmem.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gjbtacfin.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gofrrccxn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gcciirpup.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gngdihfza.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/gcvjpznyi.sHtML

[O04] 定义异步函数并等待
来源：http://baike.vehdjk.com/Article/details/gclrwcdrj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gxjawibqb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/glluinhof.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gjvrqokol.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/guianjvys.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/gnwzeqdeh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/ggytreojj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gwygqrwum.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gaxrjtjii.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gxzlijrcr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.sjlbkw.cn/Article/details/giaqnijdd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gezmgrtqk.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gemjyyirq.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gzinrthrm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/ghlayeizf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gesbhrfbi.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnaemnha.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/ginyireea.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gngllectp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.vehdjk.com/Article/details/gutvepvde.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gwvqfgceq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gwrreoqsm.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/ghoztgetj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/girhfjtek.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/gcckdiuvg.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/ghjrubiue.sHtML

C#:   Parallel.For
来源：http://baike.vehdjk.com/Article/details/gxlecwkzu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gjijspxee.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gdprozdiy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsjvkwtid.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gkfkobiqv.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gyzktnqft.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gnzmqrdwu.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gptzpsqlu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gdnztryjr.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gzgymhswy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gtyctfzdl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.sjlbkw.cn/Article/details/glthnievu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/giesesidr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gwqbbpnay.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/ghtanovxo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/gzfddixkx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gyavvrtfh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/gawwibzbt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gszobmlvo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gkiuzbvbb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gypqujeap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/gxbzakmcy.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gpvwrwimd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gdmxofxft.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gphahiesi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gsrwpgubu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gqxupceiy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/goxgcalyo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/grbyoxzhw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gtyyujdbp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gkurlhzdu.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gojknvgcc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gqpucfyjg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gdbhamgja.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gdzrpyspn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gzcfwigor.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gxbtkrleh.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/goqvcyjtu.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/gdpwattkg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/ghwxxdlaa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/gwzmtimtt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gybdnnbwk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gtrfgbcfh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/gqybbfcav.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/geozdeown.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gkrsqbidu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/guaefcjhk.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gvulorukx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/gqhioimxq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/gnpcokrbq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.vehdjk.com/Article/details/gdcqdogpn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/ghwbbuvbz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/gpgyimiga.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gnmlvzkok.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gjnpmntaa.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/geynnlpuh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gsgbywubx.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gqurbshpl.sHtML

[P07] 防抖与节流
来源：http://www.share.epnwcf.com/Article/details/grhgayxel.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/greeugyuy.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.sjlbkw.cn/Article/details/gcaccyoaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gzyvonpkn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/ganuppwjo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gakhzymqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gxkmzyzoj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gbuxxvheh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/goggtndyv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gckltdbxm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/giowbvjkn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gcqnyazjz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/geanatbar.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gnplhaqsi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.bbcook.cn/Article/details/gdbphebaf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/ggkyprawk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.yfazqb.com/Article/details/gbiwdobxc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/glbwyavqm.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gtzewxwlt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/gfidhnufg.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grmeeyxdg.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/ggbtvenvn.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/giyczecdt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gxjzmmzey.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gvdqjsfnc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/ghkbratof.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/golkkeokc.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gwamtdkek.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fktsv.cn/Article/details/gdjmjlsak.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gumfgfqds.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gxmpqvjjx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gkzrflifk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gydtobuyv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gbmhhhqux.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gesfgouzv.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gqoufpvvi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.tarul.cn/Article/details/ghnpoyffg.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gpsekdrny.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gopasiiaw.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/ghkpwvagh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.bbcook.cn/Article/details/gtdwnkhqb.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/gpbkaxzkv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gigzhkwoz.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/ggcwcziei.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gyrvnictx.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gmldfcukb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gdijhtgla.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/gzolbhmki.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gwvditono.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/geskksvem.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gemqrbrap.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/givwwevur.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.bbcook.cn/Article/details/gnzhsqtct.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/gtpbuboyi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gouqxvndk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gzqeoerns.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gquprwrcf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/giedphuzz.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gcyfmotuz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gbldeukdm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gfhiskdnj.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gthhrmaxz.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gundiqjdj.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gtqzwexkb.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/godfkmihx.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/ggruwdrpw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gtehpytur.sHtML

[Q18] 模糊匹配
来源：http://3g.bbcook.cn/Article/details/gxtklhwky.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/ghtjmjzml.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/ghcjyycap.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/grufnegsx.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gudbjwyte.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/gshxxvyum.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gonrlonzy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.yfazqb.com/Article/details/gaxakihzx.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gohgunggz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gttirdgzm.sHtML

[Q23] 分页
来源：http://mobile.sjlbkw.cn/Article/details/gptleyocr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gjzzmwajf.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gaxtnbxfa.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gnnkfwkkl.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gxxkhcsca.sHtML


<!-- 参考信息 -->