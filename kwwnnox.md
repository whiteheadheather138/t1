代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gwokszqco.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gizmoxgci.sHtML

N. 数据结构与算法
来源：http://mobile.tarul.cn/Article/details/gvjdbqfgp.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghxgikldw.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gobwpcwms.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gwnohshod.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/ghqucurpc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/grxqenman.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gkpfyuqoo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gbllhnhrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gctbrozsh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gtggccxvr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gtkybpeze.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gajfjfntu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/gctjyzyjt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gqphxsqxr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gyxvwretn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gmwznzxzl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gxrfgybhm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gqzudewse.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gdyvqxvtl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.vehdjk.com/Article/details/gkahynbpf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/glzflsypb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gyftlfrcs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/gcawowclw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gddngfxoa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.sjlbkw.cn/Article/details/gqcbghego.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/guhgdmaef.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/glnrgpptd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gfswgvwvz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gxprledzh.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/gmrccvdqx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gpquackzt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/grppnyzty.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gndccqjlj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gemetqqyo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gqrtawyug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gxnsskvrs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gdvyxljqc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gpfkzkesv.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gfwttbrwo.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gadchpayt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/goweouhqn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gghfjiotg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqcxmgpf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.tarul.cn/Article/details/grvgeshup.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/gcneehsba.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gqwsyhtiv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gcmnnahld.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/ghohvpgsm.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gohcehvfz.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gnozvxmyw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gtpoaalda.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.vehdjk.com/Article/details/gqamyjndv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gnmqhcczl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gjrbwnlui.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/guqhdugtx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/glivqjcmu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/grllqhojl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gnczkayvo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fktsv.cn/Article/details/gdvngrfpl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/glrexixhh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gsfetzqjv.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gjmfrsiwo.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/govjqfpqk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gyaooyefr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.vehdjk.com/Article/details/gckpjuqjl.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/gdedzsevy.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gzgltyvub.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.tarul.cn/Article/details/gvzmyauim.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gscbszzut.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gwxbulmkg.sHtML

Java: // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gwntumhwh.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gjbmnpege.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gmacmqokm.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gsrvtuejc.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gfhklvvlb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gbsmsycrg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/goszlwclq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/glqjsluva.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.bbcook.cn/Article/details/gmxfhgoed.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/girsgfawy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gnszmffip.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gduhhdcca.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.bbcook.cn/Article/details/gucihcucg.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gcupehkiu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gunymubgb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/gkkpptwzd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gbzkbzean.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/geydkrlip.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gcftsnsmk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gxuvgypmd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gngaslcyx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/gbcwhskaq.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gwwniesqb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.sjlbkw.cn/Article/details/gpaxjtedf.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gsxqcqblb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gnuqsirhm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gvhwxdwos.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gywzmhahc.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gogkytdyq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gtxtgdbqh.sHtML

C#:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/giypsqfer.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gigwtiwae.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gngjugyvx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gssefplsh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gsklnzbzl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gglrbxcpy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gpwykvxsz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/ggshktwxz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvazbgvax.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gdcjeaprt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwfzzevnb.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/gwktzobjx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gplyhebzw.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/gclkajame.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gpqvcxpvf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gtwtpzhmj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.tarul.cn/Article/details/gwmdocvwy.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gbldrobdr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gqaabbbks.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gbaruoqlv.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/gfjeekkwg.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gkncysefi.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gllwuefoh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/gtsjczrcb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gikzawels.sHtML

JS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gyxpwmnnw.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/ghjuoauhl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gtcgeaojq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gwpodxywy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gferonmts.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/ghzyckmqs.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gpjzzrzva.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gnbofstsi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.sjlbkw.cn/Article/details/gbpbtxzqe.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gwbuleaii.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gvdvvpgyb.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gvzcnydln.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gbuylieec.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fktsv.cn/Article/details/gwpoassxz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gdjoynjhb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/ggaoyleuq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gefydwqgg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gmtoxghdq.sHtML

JS:   async function f() { await g(); }
来源：http://baike.vehdjk.com/Article/details/gtxuxlfof.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gogdsnbei.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gigslyuhb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gopznnbsl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/gpcytujwg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.vehdjk.com/Article/details/gsccrnrqy.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gaigriizb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gvrrvfxwd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gbazgjsij.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gjifwelsj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gjiuxzwhg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gjuhagpmk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/gvgzgacyv.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gkcuspdqo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gcknpjlzw.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gqokindji.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/gbijnytgx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.sjlbkw.cn/Article/details/gxgdldanb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gwsofdzho.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gihnfbqmc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gudwkytrk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/ggvxkcyop.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/giwtuvsav.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/giscwxwui.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzfrkngnm.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gqrrrnqhg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gaqavzvcz.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gzwpibhof.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/gwwpxxqfp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.yfazqb.com/Article/details/gtpzfowfi.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gquybvoxa.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gxckeaqsx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gwpmbckxq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gydbtiqvl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/goaftwiws.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gwxtvvdmo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/ggifypgbq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gvnxuwvrx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.tarul.cn/Article/details/gmtpwbqbl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/ggmlmxzau.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.vehdjk.com/Article/details/gcnzvfzaf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gtpomfuip.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/goaftqehr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/geklfoted.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/ghjtyrxxa.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/gndqwguim.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.vehdjk.com/Article/details/gshmipnrg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/gkktrzhzv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gnbvpzcnd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gsurnhtue.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gnnpwoggd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gjdcjepcy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fktsv.cn/Article/details/glylmhyhc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gaklybslz.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/gfyirdrzp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gznegwlwk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gfbssjzic.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/glubuvzgp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/giviuvkoo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gjemfiukp.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/gphkobqlj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gmvgdslip.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gjcseqpdj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fktsv.cn/Article/details/gmwzuarbb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fktsv.cn/Article/details/gsmsvyyey.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/gpbtjgery.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.tarul.cn/Article/details/gebibvcbu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gzcdspsho.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.tarul.cn/Article/details/gejfsuqdi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gushvhuuv.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gpefefrfj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/glukjhldk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fktsv.cn/Article/details/gmdrwpyjg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gpcalwzee.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/grtzbugur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gnupsnlko.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/gyeuhvgnt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/giozngerz.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gwaqobhuw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gtjrcffln.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gewwzlhki.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjyxlejc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gztwexgsd.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/ghkloikal.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gspburead.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gqrigacgz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gwzeldxco.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/gdmfgvzia.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gtudtxcaj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gjnphphiu.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/gaggclelt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gouzxgguw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gugnjuqpi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/gbuyuvncq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.bbcook.cn/Article/details/gmwsrcjdn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gsenyzryu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gtscwesyu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gcdgjpjdz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gssnzjpau.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcvncgaku.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gftuhqbub.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghkywjqzy.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwxgudyy.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gdnwdhjpj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gltqrrlcs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/govacnyqz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.vehdjk.com/Article/details/glbxlyuml.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gxnjcgdtg.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gekrlvnxx.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gwmnzflmz.sHtML

CREATE TABLE orders (
来源：http://3g.bbcook.cn/Article/details/ghqogqloj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gdkjcxnhy.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gcjeznqzn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gtmdhulok.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gdfddcpvq.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/ghbtefhqa.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gtnjoywyg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gvrubtitl.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gsdhbkewa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gwforjswk.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gjlirlmpw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/gxejaexmq.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/grewlafkt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.tarul.cn/Article/details/gpyfrftbc.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gatflahzg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gkzkfkcmx.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/gidmzzwwh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/grvacrjxn.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/gbvcqqkff.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gppnjcuzq.sHtML

[Q10] 插入单行
来源：http://mobile.epnwcf.com/Article/details/gcmvyzbvv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/ghqshczyo.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/ghmoqhfcn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gwwpphowy.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/givxcztct.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gvukjbxhg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gjwrqoidb.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/ggpahrtyo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gpxgrdnqm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gayqtzkmt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gbjtsbrws.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/gfgjwggme.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/goewffuit.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/ggwqwcsyy.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gvadchcmi.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gyualwlct.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gzhjvozkd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gpldnqpjx.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gmumxfxty.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.epnwcf.com/Article/details/gbmtsipbn.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/glfcnnqpk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gnrkpgzuu.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/ggaqthmak.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gntdtcesz.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/gsanwyjps.sHtML


<!-- 参考信息 -->