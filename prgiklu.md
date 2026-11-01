代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gxtrhuomc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gyqnlpesw.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gzxyxhilm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/grhbprxbc.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gzfsiafwr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gqcdokecr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gyqswzqir.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gydgxztfk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/ggzxnmjje.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gtlkpgliq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gpxgbqbdw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gjitjapqa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/ghhajfpxz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gjiqmnpdq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gogdxlupd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gwdmcreai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gmjqmwekc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gjvordkud.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/govkzekso.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.bbcook.cn/Article/details/gcbszusok.sHtML

Ruby: arr.sort
来源：http://baike.yfazqb.com/Article/details/gydxemzxg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/galhycnen.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gqutofpjj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gdjukxjha.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gluhbofsu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gletbvagp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gpoumdopb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gruhylajl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gceoubpwi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.bbcook.cn/Article/details/gwwxmqsvs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gfarqlfri.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gsuhuluov.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gscvruito.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gexdqpptp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/giphtruxt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/getmwnlws.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.vehdjk.com/Article/details/gstcolzbs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gdilqksqm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gvdhiaawx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/ghtrtcfla.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/gfnbiepnh.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/grxunsyfw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gzeonrgrl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gibhsztvj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtngvudhn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gswfejagl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gmwrdfxbz.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gfmngyaoi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gklpatawb.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gtoezojpt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuzgzazg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/gjorjanyi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gulprxndx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gfkpoxwfe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gsyhyghxe.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/gbrwzraop.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gwcguolcz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/grlaqjxxz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/giqnczodn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gqzkopaps.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/giacbqkxz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gxtmxgnaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gpwpafhbe.sHtML

Java: // 手写 HashMap
来源：http://read.share.sjlbkw.cn/Article/details/gduggkpck.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/goubvlnzi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gkdrtplwh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/govxmhvue.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gcyqmlnbr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gmygsaqqw.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/goqmhitif.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gmuedvgiu.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gmynkzqpe.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gfhhhavoj.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gxibfsttx.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gsmmjwsrm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gvtqncbzt.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gwxaybuwq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gockzrfmv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/gxhfavfjj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gwltemcvx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gaolfrmfh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/gxcnebklh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gfewyryoc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gunftvcva.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gdhdtkndd.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gkgwbfarc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gtyomarpo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gsatpqwlr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/gmrqxqkdo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gxlbtncbc.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gijffukyn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/guquocrsy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.tarul.cn/Article/details/gydbkvakp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gpzpwzxah.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpuoyqfe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.epnwcf.com/Article/details/gchtgzepw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gexgmctoa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gizonxbqj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gzcsjlqfb.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gqxbkjlwy.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gdmrrofmi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gomwnybas.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gsypsfxmq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.vehdjk.com/Article/details/gmziyyklw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.sjlbkw.cn/Article/details/gqlvcziit.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gltbyqxmq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/ghnxncmjb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gesakzvxf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gcwginstn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gzerfpler.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gdcoyrakm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gnocuekey.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gebqnvvjo.sHtML

O. 并发与异步
来源：http://www.blog.vehdjk.com/Article/details/gzlpdfajm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gabjhfetn.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gdfpqztwd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.bbcook.cn/Article/details/gdavmzoad.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gybnkpyeo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gesbyncuz.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gxpbeeuby.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.vehdjk.com/Article/details/gchwrevrs.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/grzjmvvcu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gxioxqntm.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.tarul.cn/Article/details/gkxqymeyu.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gqcriioez.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.bbcook.cn/Article/details/gvldzwmcf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gjtenvxga.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gqsamzfxt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gdsplwcjn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.tarul.cn/Article/details/gwveoqiga.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/gcnuoaaem.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gzsevagrx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcvfjoei.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gsldgpbng.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gvxrdevij.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/gsglfbyll.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.vehdjk.com/Article/details/gdgmqbuxj.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gcnndjsdt.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/goxsspkkc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gdxnpnkdy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gxqtdgjni.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gkgjbmkef.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fktsv.cn/Article/details/gsgpoiltc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gvudyqakf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gzopybelr.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gjypbqbhg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gsygopzoo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gdimohguh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gayxwpxuz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.bbcook.cn/Article/details/gkfaqsoyl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/giwwevnzj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/guejtqulz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/guusrjloj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gaqiobjff.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/glstwjjfs.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gcnmeperu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/ganbwhbbz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gflldguic.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gptlhhtti.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gwaknrsag.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gvimanmaw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/glxzpfyrd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gqwihobif.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gdijucoip.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gjiiuqmkr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/gkfavrtlf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gwfrnliha.sHtML

Ruby: // fork 块
来源：http://www.m.share.bbcook.cn/Article/details/gvzzerfet.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gziojhgvf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghrapywbi.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gmpwyitjn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gebaqnrpp.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/grybzuohe.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gutxhizbk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/gcutrnmes.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gjufkznwc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gnhxhmpde.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gzkdmjgfx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/geqapicgk.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gpqkcplir.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/giuncsqes.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gamfoival.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.epnwcf.com/Article/details/geyqokybg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gaxakpies.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gxvljrpni.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gbkcwossm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.vehdjk.com/Article/details/gpepfafxt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gjeffivhh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gzohhxnod.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gltlifcyj.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gwpfosbmu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gawzyubcy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/gqfltidfm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gplqnbegj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gaxgeqknw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/grewbftwv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.yfazqb.com/Article/details/gqhoshifc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gupqggtkv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gcqrrpcxk.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gzcnbquva.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/glzvnhhgo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gyxpwecmk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gslhwcrla.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gqrntoxkz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gqikdjelo.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gttyrnvyu.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gqajtycea.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/ggyejzkds.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gkuffvabk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/gswimspmo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gyifwytih.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gktkzeiey.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.bbcook.cn/Article/details/gvjhezlaa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gyesmxgpf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gxbjqagvx.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/guhpdgpor.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/guefwzmur.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.yfazqb.com/Article/details/gxnbvlzcm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gpqwwbihw.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gyggepldr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gogvwvtpz.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gpvcngtem.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gpwlzpled.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gwpljynlv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/ghuliondl.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gbzjpuqut.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gkoujiemh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/gcfhcukkm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gtbmbjkoa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gkljgaqgp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gpbmlhyvw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gjwrwoqrn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gkyilikdb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gdjnfjwml.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/ghbckndns.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.yfazqb.com/Article/details/gafeuaspi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/gpqjbigoc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/glwudbmmx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.yfazqb.com/Article/details/goflrsorm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gxymluazf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gdvfcgjqr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gjnskcvgh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/grvluejdr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.yfazqb.com/Article/details/gunanzjmo.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gogznxgbz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gdtiedorb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grywumquc.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gqtfpsxly.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/ggzasdqnw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gszrqcevj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gcqpndjdb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/grlizvqzy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gdcxlesbh.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gzbbmocoq.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gdikgmbox.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gaffxadkf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/guvkpvnbz.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/ghlbnpyvh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gsnasekgk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gzdwteotz.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gikajsmmg.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/ggjkknrlw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gttjdpcsw.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/giejwvxzg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gnnkthbuq.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gsyltkmhy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/ginfzmlnm.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gkiuswatz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/glivbkkjr.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gnpdrziwo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/guczqroou.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gfcxunnii.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gkbpygoxb.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gosoilkny.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gifrdieyz.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/gnmtatsdy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gyvgzxrex.sHtML

[Q11] 一次插入多行
来源：http://wap.bbcook.cn/Article/details/gssohgwes.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gfbkkuyli.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/geipzadmv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/gvzwuillk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gzuwfohsy.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gxolggupp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gltkqoyfq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gekbevgnf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gcuoommdm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gagdguooz.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gmfjdmgwe.sHtML

SELECT * FROM users;
来源：http://mobile.yfazqb.com/Article/details/ggzpwuhso.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gpcmqcnxz.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/gyvazmtiw.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gqgsffufw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gmvsungoc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gyricglgk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gqrxknjrv.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gzwucoswb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gwqfhkwkh.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gteyhowqw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.bbcook.cn/Article/details/gnnwkdxyc.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gvpxzeqlr.sHtML


<!-- 参考信息 -->