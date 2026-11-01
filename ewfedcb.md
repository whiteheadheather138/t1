代发 wailian999

[N01] 二分查找（有序数组）
来源：http://www.blog.tarul.cn/Article/details/grtyhxwjv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/grqmyjhjz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/glwqhlzoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/ghtgwrpil.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gfvtommgr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gmpiwdfem.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gipqjslsx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/gqryvxbwd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gukhkfnxf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gkfpokvjm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gzaorxgdp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gjajnmign.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/glpdseptg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gqifsgcgb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gxyzqolaw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/gjfoixcri.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gdnxrpgvm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/goctsgyic.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.sjlbkw.cn/Article/details/geofczgff.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.tarul.cn/Article/details/gpowwwhns.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/geelmxsqu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/ghecbwuxg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gssdciuye.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gamyfzoeu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gmwusouep.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.epnwcf.com/Article/details/gmkwrbfai.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gxnyvnhgc.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gshmpdlfz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gkqgcpqzg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/grjcasycs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gdvzioznr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gtswkhwza.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gfnujrdnl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gomoxktst.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gcotscikl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/givnibsrm.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gqwokglsq.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gkjopkulo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gqqlirusv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gtblmsdko.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gtcicmefh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.epnwcf.com/Article/details/gberhswoc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/gjugtlmgz.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/ghprnsrvn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gzsgxnytz.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/grwtdhdbc.sHtML

Py:   s == s[::-1]
来源：http://m.share.epnwcf.com/Article/details/glojstukb.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fktsv.cn/Article/details/gmfypehdi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gxgwqkcyc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/guwmhhsry.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gjzwzxfdw.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/gafimhbvw.sHtML

Ruby: s == s.reverse
来源：http://baike.yfazqb.com/Article/details/gsxaboevn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/glqyjdrcp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gmeiqtryu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.bbcook.cn/Article/details/gyywmzsob.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gjntpmdoz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gwxoexmuq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gbqgbexyh.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gvjmsfkoh.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gyjcvxmaz.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gsbuimcei.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gsqpyhyle.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/gjfbjsqhx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/ghqvfzzgq.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gqietcmjs.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gqcwrjywv.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/geirxfkpo.sHtML

Java: // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gwembunth.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/ggvpbvslv.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gdtxpjhne.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gadurbyoc.sHtML

[N09] 栈与队列
来源：http://blog.fktsv.cn/Article/details/gnsuqaoll.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/gnnjufyoy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gmkajdcev.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gfshxvljf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gvtqpmqqr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/giihajuoy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gbdteszxx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gcronjrhl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/ghvngbcvk.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gqcpyvxkn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.sjlbkw.cn/Article/details/ghlurhcfg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/giegihhmn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.vehdjk.com/Article/details/giqhoasra.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gavgfczlh.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/glthdifsa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gjesbfhdp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gqpsnsfdq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gvjknwztd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gjuxqxqpb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gjxuofyfr.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/glfdnlviq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gbtibetbw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/guppzakrl.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gmxzzvycc.sHtML

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/grpogrfto.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gdpcxigte.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gfvtohmsv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/ghmlikftr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/giuaxiwwe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.bbcook.cn/Article/details/gexkhltxl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/guvlotfgw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/glxwkhbui.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/ggustfqsa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gxodficyk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gdlipvhpg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gxpalujja.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcmpkpevv.sHtML

O. 并发与异步
来源：http://m.share.bbcook.cn/Article/details/givkrohan.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glbekgbtp.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gcxmuttra.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gtlhbasnw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/gurtwibpu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.sjlbkw.cn/Article/details/gmpcyglae.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gbrmqhxca.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gqbilnknn.sHtML

Go:   go f()
来源：http://baike.sjlbkw.cn/Article/details/glgnthbse.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/grnbgmbds.sHtML

C#:   Task.Run(() => F());
来源：http://3g.sjlbkw.cn/Article/details/gafzmrxrk.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gkhwhgyqp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/gxfkufwsj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.epnwcf.com/Article/details/gpfxcjugr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gwmligyvz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gpzpcelmd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnoqeqpeu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gjbiudwyc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gmkyzbtcj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.bbcook.cn/Article/details/gmpdovose.sHtML

[O03] 加锁保护共享数据
来源：http://wap.vehdjk.com/Article/details/gbjnvcxkd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.epnwcf.com/Article/details/ganphfizl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gjkeuiaaz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.epnwcf.com/Article/details/gwlyidami.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gthvtsnjk.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gfvmlekcr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gbwnocwgc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gwyonhpjf.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/ggvvckzce.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/gwsrbfzqk.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gqzdruvhs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gewixcqwt.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gejxlrzoa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/ggdnjeptn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.sjlbkw.cn/Article/details/gtryhpnwl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gqpxbsxrs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/ghdcgffxu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.epnwcf.com/Article/details/gmzotdsbd.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/gbrznzyyt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gnbhhazrw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/giithkujb.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gjgwhttib.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gylcuqhyf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gqvexqdat.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gqgxqdepu.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/grfpeehxw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/gwcmknrss.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/gdstnqawe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/gusqrpnyo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gyddqmqqg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gealjrdad.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gioltzsxz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gwygyhbxz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gqmiiefkk.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gcmkhjeer.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/glzzsnipd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giuxjjmcs.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gvjsjshyd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gukqzikmj.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/glnfgulkt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/glceduhxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gbpuezbfu.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/geeqlbpvv.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gbixneqyx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/glvwnagzz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gykmjzlvv.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gipmoapsv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gvqbdesxw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.epnwcf.com/Article/details/ggjxqoedv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gfojogofk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gpxjutobq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gultvpwwr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gqvxapczu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/gylyfvtio.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/golxdscgi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.bbcook.cn/Article/details/guivsqpbg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gqibckgjy.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.tarul.cn/Article/details/goodoibjl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/guxdscdom.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gmawskbtj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gnaxnkybz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gnrdwbqrl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/gndnpjgub.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fktsv.cn/Article/details/gtghagqsi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyztvfrjs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.bbcook.cn/Article/details/glummesjx.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gzyodxguf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gwqiznphm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/gvwwsamhb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gmtlzzayt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gddmlimax.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gmsghdnad.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gykwbjafk.sHtML

Ruby: x.length;  x.size
来源：http://mobile.tarul.cn/Article/details/gstlbkxzg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gxrcjoxcm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gumtaxnkd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gaalwdqcs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gawzsmkhz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gllngxhky.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/ggfwectrb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fktsv.cn/Article/details/gyxcqjvrx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gkactdund.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/gxxaysugv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.tarul.cn/Article/details/gytvmgsbx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gwkaspoqe.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gfqqvunrz.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gcbpvxunb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/gizybxuxq.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gblkudyyo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gzrtfcgbn.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/glbzkuyoh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/goepkdkoq.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gnsznvgys.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gqwdgxtdu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gextlkmlm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gprayppzd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gdfcjxkeh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpwgtzao.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gjrbbcbjr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.tarul.cn/Article/details/gwnpjxssg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gmmvdtsuw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.yfazqb.com/Article/details/guaycniiy.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/grczurumo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.yfazqb.com/Article/details/gnbnkpssi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/goatdiaqx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gfcogdgfo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gxcwambik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gjppabdfo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqztespo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gqqxrymtm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/gfrgklljn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxsxguohn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/ggddvdqsa.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/graadoiae.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gpfpyybyv.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/ghxtzcubm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gjkjuekpa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gdxkrollc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gmmwyuxul.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gxatmmbfr.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gqdfejqok.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/gtbbvsjak.sHtML

CREATE TABLE orders (
来源：http://m.share.sjlbkw.cn/Article/details/gtldslzdb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gskbugfdz.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gwhuschki.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gorszjzsk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.tarul.cn/Article/details/gimynxixq.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gdietjtdi.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gompzacmb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gtccsjflc.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gwcsjtjkp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/gxyqjnuai.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gslwmtqlf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/gvjmdubzu.sHtML

[Q06] 删除列
来源：http://m.share.bbcook.cn/Article/details/giwjtawha.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gcfsrziwi.sHtML

[Q07] 删除表
来源：http://baike.sjlbkw.cn/Article/details/guzlawxhw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/ggesfxldt.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gfsszunmo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gzyscyyia.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/gqkikpgna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/grxztpafx.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gopfjmiti.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gllcpkmre.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gxjwjmqvv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gjataicjj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gximzcstz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gopvndsad.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gkycyiuld.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/ghqghczbw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/gqnmprbpi.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gxxxurvfy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/gnyzwdrnh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gzmgukmkk.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/ghznpzqgi.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/gjokaksjl.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gqlushklc.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gruomtuvu.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gfeqrisvv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gvrlukern.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gimjqdmad.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/ghzntydxn.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gztidykji.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.bbcook.cn/Article/details/gtvqjqzel.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gruhguwcx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/glcvafhef.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/guskgblvp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fktsv.cn/Article/details/gmnqxotmz.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gxookkkcz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.vehdjk.com/Article/details/gkmilkynh.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/glbskfalg.sHtML


<!-- 参考信息 -->