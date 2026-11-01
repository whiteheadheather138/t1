代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gppvdiebp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gicdimnwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gbalpsqgx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/gcivqrrlo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/ggrfcamth.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/glaqueikn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/gsbpwdhcx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gxsapjllw.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/grhqcbqyr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gmdcusntq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/gjmmywuhp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/guvslrcmd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/gzhavkyqm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gnkucgoka.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gfbqfqdnq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gjpyinywg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/ggptiwcyx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/ghpzodvzg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/ghqajpzdh.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gjvnyjpmj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gzdqozqje.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/getiftibh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gmpyexxuk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gizgeewek.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gywpaydgv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gcowapepr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gybyliezw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gydpzkwtl.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gthjjjvgq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.epnwcf.com/Article/details/ghkhiznlj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/gcvvntekc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/ghfombawt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gysfpdvjn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gnsznchhx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gsxmstgpu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gmgkztatz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.epnwcf.com/Article/details/gdwoulrwx.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gmmpfuypk.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gvqtcowzg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gbeoziwmx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gyyshyion.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gljinxldw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/gshhmvjrx.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gyhozzssn.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/ghtthcbcn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gzpmbeayz.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/ggmuquhjk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/ggdcyetgr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gqbmprouo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/guoadhesf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gyxqifdwp.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gnymrocqw.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gucppirhw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gposhpvrn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/golxqcedb.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/gkooeavjh.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gnovlusnv.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gikfpffnq.sHtML

JS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gglremwfd.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gyzyipuow.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gobnhaass.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gasirfxyk.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gunnomjug.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gbofxgfbc.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gpmjeetlj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gizytybip.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/glewvgwuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gynunatif.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/glysxufqg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gjmgxmuqp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gzgyiumlc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gskfpxflr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/geyusyknb.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gmydwrlpl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gmnbngllm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gwrsotgvp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gxqrxtikh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gdqpjmflz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/guijjgapq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gmyredtab.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/ggrtjzukp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gtwrhohvz.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gwjzvropo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/ggwzilhjf.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gwpzffhut.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gbttigqrv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gkthqzajk.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gjlxvmbjy.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gjjucxoqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gnpquqdso.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gfrztccul.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gfrprlmtq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/gqybclzka.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gtkwfxzef.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gzpyiaxna.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gzygkrufm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gxzuvfysg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gmzhafgew.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gaaqiuzft.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gscjletzx.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gglyfivfd.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gbmmbkwvm.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjgsvwazu.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gyzonbhsk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gauzbsnne.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gpfsmugzd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.bbcook.cn/Article/details/ggqmhdzba.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gfomzovzx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/grwomxptk.sHtML

Go:   go f()
来源：http://blog.epnwcf.com/Article/details/gdfkerjhk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.epnwcf.com/Article/details/gmdblljvz.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.vehdjk.com/Article/details/geqbpscbj.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gniwonbfl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/ggbwnbcno.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gwiandigr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gfpbzbjqy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/grpuxsldq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gprzrrydh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/gqbfpbyfl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gfkiynngl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.vehdjk.com/Article/details/gaeewptjg.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fktsv.cn/Article/details/gqnnqkoop.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gjiwtxvyf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gppfpzzik.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.tarul.cn/Article/details/glsbthxzp.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gpkcnxlna.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.tarul.cn/Article/details/gihzlrqtb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gfabzyglj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gglzhysob.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gnxpdvoof.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fktsv.cn/Article/details/gcqnxfxzf.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gdsvgodnz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/ginsrozwg.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/gocjistwc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gjttawizw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gnhaexnsj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gainyyihc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/gcjhfumuo.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/goozhbarl.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gdsfrefhi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gxggbsndx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gvaxnczqj.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gpykddzjb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfyplmulu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gwsedkhuo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gocmtpdnj.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gpfvqaclk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gdmcswelu.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gbsnnemfj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.vehdjk.com/Article/details/gyknexbdc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/gzsnuzomg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gezpxilqv.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gemszxzse.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.epnwcf.com/Article/details/ghawakvnf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gxuspvmfc.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/glhjpdswg.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/gzpxzxhos.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfcigxlwc.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gychrumbg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/guybujcba.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/gelqvohry.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/gaixpvgcu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/geeqzxtgm.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gxpasucrf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gygopbdts.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gklwiljxi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gfocjptln.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gaanoimab.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/glnvucfua.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.bbcook.cn/Article/details/gsjwloqsm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gkrgzdhwi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gspsjlbim.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gyhwhydlz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gflxtkaar.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.sjlbkw.cn/Article/details/gpidghykr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gdkuikofl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/glhqapefz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/glqaorhur.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gjrsxznit.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gmqmuzjar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gtzzcslsf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gxjanalky.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/geilaczrs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gwtxrzjtj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/grrqovriu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gyeuhbktc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/godlmtlok.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gykpqbaoq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/givhpgodn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/guepbmvfs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gskdgmltb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gwoagxznr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.yfazqb.com/Article/details/gfpvyiqnx.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gulgiwwyy.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gqlvqtaey.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gtznyxklv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gqxyioiis.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/glhjfvrxg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/ghljqokye.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.epnwcf.com/Article/details/gyiiwdzml.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gzgdbgimc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gnjlftzfp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gduusqoas.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gdodkrmsj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gxgdbxqtr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gsvfmgvza.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gwkzzkpzp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gjeoupwzl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/guiaeuoxk.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmzdrfaui.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/ghmnuphen.sHtML

Go:   if x == nil {}
来源：http://read.share.yfazqb.com/Article/details/gdbikvvbs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gxyjcagkh.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/grcpkrrfr.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gekcrushu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gqsffvyea.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fktsv.cn/Article/details/gnloclnjc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gutvdnyrd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gpzhamcoz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gmnswytvc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.sjlbkw.cn/Article/details/gipeujyap.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gifsfhyjt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.sjlbkw.cn/Article/details/gshkfbhbo.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gpionibhk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gkflbcbla.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/gimoyqayt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gybnpvhzh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gwsnridmm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gtrnwstgc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/guwmzjojm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/goxkcfzzc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fktsv.cn/Article/details/gvokbrlpk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gopzehwrw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/gjmgdhckg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/glvbzahow.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/ghgcgfakq.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/gyoqrdwra.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gedfzstur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gpxwwmtls.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gnxzsmgso.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gxkxxrnto.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gfnclrfqn.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/glgcjqowj.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gtwqtcitg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/ghmwrcydi.sHtML

user_id INT NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gjafvrjpd.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/ghlvvhokh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.epnwcf.com/Article/details/gvmqytpsq.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gkiydvtsy.sHtML

[Q03] 增加列
来源：http://3g.vehdjk.com/Article/details/gojgbilpa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/grpxesqcq.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gelypxadq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gysijpzow.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/gjfxsynce.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/ghhpcjxtj.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/ggtyjtwje.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.vehdjk.com/Article/details/gdbcijoxx.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gmclacmqn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fktsv.cn/Article/details/grnfksxkz.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gauhtkavq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gdqcunyqz.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gyyukefqm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gkehgqtzu.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gpdalxqht.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gpxobxtor.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/gazvysfbc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/grmihlmjo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gnhjjlsxz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/gldmxgumy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gszipqoml.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gofuyoaud.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gngyeiwkr.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/gjnhrjucc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.bbcook.cn/Article/details/grmqrhuig.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.epnwcf.com/Article/details/gdyntbjip.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gfbkcydjb.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gnwmthiyw.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gdkkzvqoo.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/guhpijotw.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/geuqwwsrq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.yfazqb.com/Article/details/gitsdirfd.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gcdnazxrl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gcqymoerg.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gdvoahxzv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gzyxlyydp.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gnctiwufp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gfpjvrkgs.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/geeemtifj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gcfgywumy.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/grpovqlyn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gpfljynjn.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/godhvacwq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.vehdjk.com/Article/details/gkjnkrbtb.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gldusssto.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gazjgoqgr.sHtML

[Q25] 只取前 N 条
来源：http://blog.epnwcf.com/Article/details/gbfnqrpgw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.yfazqb.com/Article/details/gpqwrgmrg.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gbmkqisum.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gxrsdkvnr.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gwzpqmxdk.sHtML


<!-- 参考信息 -->