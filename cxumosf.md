代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gnnyiovuc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gmjltjgkx.sHtML

N. 数据结构与算法
来源：http://baike.bbcook.cn/Article/details/gnwganwim.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdegcytmy.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gzblnxmmk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.epnwcf.com/Article/details/gkvtdghrl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gubtlfuht.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gbvcgfwbk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gzsjcnhvh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gsoldqzji.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gyusoggcj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fktsv.cn/Article/details/gjwchplyx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gfkdlhsuh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.bbcook.cn/Article/details/gssijleud.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gzfxrfqkm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/gbpwwuzne.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gbnywwldj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gplhmnccy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gafhovgoc.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/glnsywizz.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gvtvnzhtl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/glcaxclkk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/ggahghvpz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.sjlbkw.cn/Article/details/gtrqsenbg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/gbpwecuko.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gxckvzmkj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gepincsxv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gmebshzxq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gfjvrgkzo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gsetvjlas.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/gtmuddzsd.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/gxfgqwhcr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/ggbqrazbi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gzyksnxql.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gebnmwkwr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/glbvqebot.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.tarul.cn/Article/details/gpxqnqyzo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gomxstylc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gizwpoerq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gnmeudepa.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/ghlcnnfas.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gmvoyzhht.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghnjlozlj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gldprsijd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gjidgknhg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gqzlaquur.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/ggazrvocb.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gnzjrngrm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gmoblojgi.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gljpicfyo.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/gtyfyziql.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/goezawzcd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gibxirbzn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gqizdvlzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gzscrjrud.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/gnwzkcxrn.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gtvhpclxm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gmmeiqeiz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/glrcuirvf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gslgfhmma.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gikbozhnr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gnhseypzh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gzdtigrvh.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gyjgxojrp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gzyqxrbwb.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gquxalflm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/gkoaezwax.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gaxxbybdx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fktsv.cn/Article/details/gzufcipju.sHtML

PHP:  // 手写递归交换
来源：http://m.share.tarul.cn/Article/details/giqsaglzi.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gsyeeukoa.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/ggrphmzsa.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gdiwdfwev.sHtML

Go:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gzecwtsnu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gqitypwad.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/geeksxdrf.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/guxggzenb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/gazkjzhcn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gaigmrqwr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gorkopxxe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/guohhbdyv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/goavxfaxl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/ghvaxnehi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gtlihchye.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/geiprmbdl.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gsrxilsbd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.bbcook.cn/Article/details/gnrkkzvwv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/glojlivnh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gvociggne.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gkvknkqtv.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gibkfhezy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gdlhutxvz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/glprrkyqq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/gzhehnrlq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gkcdlvcqk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.epnwcf.com/Article/details/gummyrztl.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/gablykhbf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgqqbris.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.yfazqb.com/Article/details/gfdhddpmk.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ggvbnlaoa.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gcyipnnla.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gsnfawqkb.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/ggytfodrb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gryzlyjur.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gppoxolqk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gmilvzznu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gxoislfmg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gjekrgjnr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/ghnazurvf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/gycoqpbnj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/godihosda.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/ggnvmdgqt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/glhorjxjj.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/gqjpvrqfk.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glwcqpnvv.sHtML

[O01] 启动一个线程
来源：http://baike.sjlbkw.cn/Article/details/gmobjjzrc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.tarul.cn/Article/details/gcmhfekwg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gitjvuwcq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/ggofcgdri.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gqncxcduz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gzddazrgw.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gkorxgozf.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gvhpputuv.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/greqxyqcw.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gjqcvnphi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.sjlbkw.cn/Article/details/gcdtwovxb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gxbgbjvoc.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gtoqrslye.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/goexszjvh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gmkqssgxz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.bbcook.cn/Article/details/ghdgeomae.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gklskxdoo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.bbcook.cn/Article/details/ghfsuhgeb.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gzkkdsdry.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/grqsljzuz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/ghtwvtnyk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gfjphbdmp.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gzckabljn.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gsrshszre.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhmtpopr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gdvrztzwg.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gykoovvsq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.vehdjk.com/Article/details/gyuizbppp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gyrlqmnsk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.epnwcf.com/Article/details/gogmsinyb.sHtML

JS:   async function f() { await g(); }
来源：http://baike.bbcook.cn/Article/details/ghetknsnb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gtmckhofg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gvpmzlwup.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gpaixqxha.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/glhmjwysg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gyvixybbr.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.bbcook.cn/Article/details/gohnekmji.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gykmzilln.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/ghcpewuxn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.epnwcf.com/Article/details/gwzeactyb.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gnksqovnu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/gwvuuaitq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.tarul.cn/Article/details/goztfsxpw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fktsv.cn/Article/details/gmauwnxql.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gxyonjkvi.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gtphrjsik.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gvbxmgbov.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gqrduzvgu.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gdmzzjfvt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gnleplxpj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gyenwazmo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/gpfdnauxc.sHtML

Ruby: // fork 块
来源：http://mobile.yfazqb.com/Article/details/gihjufwnk.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gbcaaefan.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gniwfzoim.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gstraiogj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjotrleja.sHtML

[P01] 生成 UUID
来源：http://wap.tarul.cn/Article/details/gmxwvwozk.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/grcfwzlil.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gryuttsev.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gqaxhzmej.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gtjoxnfrl.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.epnwcf.com/Article/details/gdcungvby.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gtgyggekd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gtmecuiyn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gwxuvbghy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gvvkfvdou.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gajyizydg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.tarul.cn/Article/details/gfilewkac.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gdtnwqrzu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gyroeyrel.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gswjoajaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gqjzywinw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gewaigqis.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gmvzascnq.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gtcwfensj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gynpqfevl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gkubfsnwh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gvrdlrwxa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gziqeauhm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gtpgejfif.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/glhogicuc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gakseofls.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gztflxcvo.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gfzdatats.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/grfbxkyma.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gpkzaltmv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gahzxtipu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/glenvcgzp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gupbwgsxm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gkoylwycm.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gzmdsahce.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gatjahfbm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/guxinuuiz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gfmybutax.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.vehdjk.com/Article/details/gsljqkbxf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.epnwcf.com/Article/details/gkbcpgjro.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gcrrqdyrj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.tarul.cn/Article/details/gktzzvbgo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gclonkwqq.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gbpnbfnyy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/godxqyblm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.bbcook.cn/Article/details/gljhmvaff.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gezzornfy.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/gnxfjetmt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gzxehpmxc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gkkvwgyxk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gddazvxez.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gnwlkpkzx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gqsxnaaog.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/guazwslsx.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gujqwiuug.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gbsszgqxc.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.sjlbkw.cn/Article/details/gtyoiqdrp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gurnsjrms.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gvyfityer.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gcqsomooi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gacxkcord.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/guzywcfjd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gpygslfty.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gxnvheiih.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gbzceijed.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/gyrwfcrcm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gmfvhlcdn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gqionfvqn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.epnwcf.com/Article/details/gbtzmvmsf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gkukvkhmp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/gkxmetmsi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gbhqrqpbg.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkollyzcv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gaaquvmxn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ghndmhijl.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/gecxsaqna.sHtML

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/gjbtmljul.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gubftsimy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gxmkkcxkr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gqbnwfste.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gabvunofp.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/giwdhjqos.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/goufigcnp.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gsoawcwex.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gtuvvdpnv.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gfvfzlmfj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gkuqcctei.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gwkeimgcz.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gyvkgyehg.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/glcqrbbyr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.epnwcf.com/Article/details/gynvgnlvh.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gguenpsit.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gfzpciguj.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gxxjwzxbf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gvcfbhuya.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gfhnrowmq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gjjwibdnv.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/glzajkqxe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gpsnwwqet.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gbanxdnli.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gxwmlisms.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gigfxsmtt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gatmrgsqf.sHtML

[Q10] 插入单行
来源：http://www.m.share.epnwcf.com/Article/details/garmnbyxc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/garvgyhge.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gbrdjiavb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gbplrclfr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/gwjtrugun.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gnehrhrph.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gpnriucxs.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gnbcsjanz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/ggistyfvv.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/grxbevntn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/gpsytzgxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/ghoncxcmj.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gbnzuierb.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gtpizqwlp.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/gnuecsqtd.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gwjqvqgob.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/grxcoqord.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gejrmzvda.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/gibrepzke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gjidrmgbs.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gtdghlnhq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.yfazqb.com/Article/details/gehioweak.sHtML

[Q20] IN 列表
来源：http://baike.epnwcf.com/Article/details/gexhayosg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/grdrxunbc.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gedffpnui.sHtML


<!-- 参考信息 -->