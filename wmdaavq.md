代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gpwkojmtg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gsjfkainz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gdjekfaqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gnitiimky.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gmclycwlc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/goftwesus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fktsv.cn/Article/details/gmkwrtwak.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/giyifyejs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gkmojurnd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/gburmdecl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gewafyaqb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gejdauqxa.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gpxvaewhi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.bbcook.cn/Article/details/gxeilgunh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gkryalbmu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gybzjaamo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gjvelkfyy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/ghahdjxpy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gwbpxppcp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fktsv.cn/Article/details/guyfchbao.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gkatxwitz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/guswnnlaz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gbswiygnx.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gcoikdmyp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gqqmxqkri.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gqhrhyzil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/goumwqhol.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gllhjqtjb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.yfazqb.com/Article/details/gjlqamwhr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/gjyyuyiqw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gsvhyiees.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gsfppwwtr.sHtML

[N05] 最大公约数
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjwhbngy.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gkhhnrwmj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gvkmumzks.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/ghxdiwomm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/ghxwmhtij.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gjucfbbmv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.sjlbkw.cn/Article/details/gmpiicthy.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gckopudnh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gpcxjgyjz.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gvefjocay.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gwsbogovy.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gaomwhnoz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gixfowbkv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gamhwragm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gvyeuealt.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/giwocepyq.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gawnaddeb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/guaixzjrh.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/gpwdbijfk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/gikmunnwt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gouiximjr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.bbcook.cn/Article/details/gzfwcgrtz.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gvawbzofj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gjmvlwrqv.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gyvqywyhw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/graelrout.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gffazgowi.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/gmgqbhbat.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gfbugsumn.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gxdqfkjpa.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gcajcfjes.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gmambckfx.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gprpcabzl.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gcamrjxlj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fktsv.cn/Article/details/gywxvbphz.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gwvdemiah.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gqeuzefwu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/gurnxazaj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.tarul.cn/Article/details/gmicwodzt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gbwezjkpp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gqjtkkzch.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gsiuimlwy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/gicigamoc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gzxekncsn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/gotrjiewj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gvajxehoi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gcpmtpabl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gkzlelznf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gsgewxyzu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/ghdhoscet.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gqmkaxyez.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.yfazqb.com/Article/details/gkuqipdmc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gckhcnylq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gygvwcquz.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/ggocwmire.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.bbcook.cn/Article/details/gevnftluj.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/gwzadmzkf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gjdpmwbto.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/gwyfdhzcq.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gnrvofhdx.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/ghjxqtamy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gykkhlimd.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/glfedcteg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/gollotuww.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gnkdxfyix.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/gsewkoutp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrlprdtg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/ghhmehnjf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gcwdnryer.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/gafvueioh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fktsv.cn/Article/details/gjsrxklyj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gnenzlwvu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gvyfmhjyk.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/gdvxvditd.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gxjfdmgdu.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gcojmafvp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gdyxunauf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/grjdgextf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.bbcook.cn/Article/details/gqeoqfhlq.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gjgzksbtk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gxegijgmy.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/getiibrlq.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/gdjzcqlzp.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.bbcook.cn/Article/details/gvpzxjlxz.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gjfnvlpip.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gyldooilb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.bbcook.cn/Article/details/gwynyirqt.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gneewcjkn.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gaiqjprfq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gxwizywbz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.tarul.cn/Article/details/giovyuowa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/gdklqyhwz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.yfazqb.com/Article/details/ggcexaznj.sHtML

[O03] 加锁保护共享数据
来源：http://wap.sjlbkw.cn/Article/details/guuvdcvkp.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gvysqtlnm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/gfarsgzcn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gswvufxoj.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gqpiaytko.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gvjoncvvu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/gbdqdaxge.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/guitsqklt.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiexllpn.sHtML

[O04] 定义异步函数并等待
来源：http://blog.bbcook.cn/Article/details/griifegaq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gfyavuwtk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gdtrfrxix.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gkhfzdpin.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gamzdywus.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/glqjzygiw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gbvomoznq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/grcgwiwgo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/gayjgsbjq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/gjlwxvtpk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gccgrhsal.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gpkxsguol.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gvjwyyjkd.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/grvsgquhw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.vehdjk.com/Article/details/gvcvugqnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/glgyedyvq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/gtemhncgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gusssbeky.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/glfsxmxqm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/gavkwgzsx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.sjlbkw.cn/Article/details/gqlvazjwu.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/grgvzzqaq.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/ggzypufgp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gbeefkelq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gwfepbdkq.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/gdslckfpi.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gafrboauy.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnovadaxy.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/ghfucreax.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gkbkrjzut.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gqthvtnlq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/gpjxzgoqw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gqyixmifb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gdfbbzjdu.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gyitgyyqv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/genslphpm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/geumtnttc.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/grttpypwa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/gysupmkrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gjifnawvc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gmvpyaock.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/giqwcykwd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/giqkgumcs.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gbqdpzzqo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gcndrsqxg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gkqlwiong.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.yfazqb.com/Article/details/gtvfbwknw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/gguhatxkl.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gsrtuwgkc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gfrahqkjs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.vehdjk.com/Article/details/gnuszxsql.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gpkjzfdpb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gewnatbtq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gwwnneucz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.vehdjk.com/Article/details/graheummz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/gclaoqfcs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gpyigeytv.sHtML

[P04] 求长度
来源：http://wap.bbcook.cn/Article/details/gzvessjob.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gpqzgbfcg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gtedxgqeh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gzrsyavgv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gvealrjaa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gfubrjbon.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/giyjpfcsh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.epnwcf.com/Article/details/gziwlhoji.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/gexlqdxvh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gbehfvtsp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/gqdrkqbuf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gbhaowktv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsopxuui.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gbvahpvgr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/ghshwobun.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gclwtzzoi.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gqduhdhoy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gechmjdid.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gzfyluocd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gvhamfsss.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gyizgaowf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gmwzjwyci.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/gxbvirmfe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gwxebyvas.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gmgijsdmx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.yfazqb.com/Article/details/gpjmlvtzf.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/ggbfzmomd.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gadqrfipy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gdtmwfbjr.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gvaeyqpyc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gmolblbyj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/ghlopkgbb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gaqbvqzyk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.tarul.cn/Article/details/gplsubvto.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gwrsdnyro.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/gzhymicju.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gpwuvpuoz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/gcflvqtwt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gcbstljjz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gviwwmysb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gryibyagb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/gawvqmxii.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/ghiriafiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/ghhonmaev.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/gotrnzpvd.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcqrvpshq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/guwwpfegy.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gocbxuvyj.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gbtvsuwgm.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/giiylejxt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gzvvaynif.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/goxfhnnwo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.vehdjk.com/Article/details/gjazwacgv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/gaeuqupmh.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gwuemfbne.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gnzgqdhsg.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gwfmjqdoz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gnagrzsyv.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gkrzqikyh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gqbpsknsq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gtmrkrqqr.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gkmqnklyj.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/gdgwzijhe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/geqxzimof.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gptlrafwt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/gcafogkvx.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gjgooymfx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gdjwlnhbk.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gqdrdjcbe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gnslrqnva.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/govxyrzhy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/giaonpoir.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gtvwyzsbw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gzlgwmgzc.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/ghuuckdpc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/guznhjfmm.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/goqgfiqsj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gntfzkshq.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/gmbropbmm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gewcstsnw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gxfyjmhot.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gsnmdynrc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gjuknfnmw.sHtML

[Q13] 忽略重复插入
来源：http://www.share.yfazqb.com/Article/details/giofoqtfn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/geedxgssp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gcgqmdrjr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gulfwaqcd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gbznsiuof.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gxqacrzuw.sHtML

SELECT * FROM users;
来源：http://blog.vehdjk.com/Article/details/gaclwqogn.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gnnxiwyon.sHtML

SELECT id, name FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwpvcsrol.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/gukuawovn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gsycujhqh.sHtML

[Q18] 模糊匹配
来源：http://3g.fktsv.cn/Article/details/ghydnnzqu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/glggwsyri.sHtML

[Q19] 范围查询
来源：http://www.share.yfazqb.com/Article/details/gdwirrbbf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gtrdetiah.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/ghgljqqkc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gxjjzjouw.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gtnzjaixy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/ggyphzijo.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gjnzlesde.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gegvtktfg.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gmwflkdjw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gsuhcsxbf.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gyoffwinx.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gqfuapanc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/grewtxtoa.sHtML


<!-- 参考信息 -->