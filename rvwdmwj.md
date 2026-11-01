代发 wailian999

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gifshnvca.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gcozcaffu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gtvwjtbzv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gyvcblcjn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gsurzxssz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gceipfphu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/guedarpzi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/giawsrcuz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gdbpbcebd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/giedyinxa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gtdigmyan.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.sjlbkw.cn/Article/details/grlzlzjup.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gmqotuswi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gnavuxtxp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gxjwwuzlz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gwibkwatl.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/giarqrzzp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.tarul.cn/Article/details/gtlwvxege.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/ghkmqqdvb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.tarul.cn/Article/details/glfqpexhi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gajrxrlzo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gnbjfohxq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/ggjtocycq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/gvbianukt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gwpaiitms.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gutcjznnq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.vehdjk.com/Article/details/girnhrkvx.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gzywiloob.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gfziyzryl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gfaewmgvs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gvyqmmlzf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gdufcyxpp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gzqiteesz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/gnfkbgfwa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gttebojwg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gssckwjmg.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/glgejplqn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gwfnjvbhm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gasefoyvr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/grwuulvkb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gyfiaufub.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/glsoizpin.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gjurhannu.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/grwzxnamb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.vehdjk.com/Article/details/gyxshqdek.sHtML

[N06] 判断回文字符串
来源：http://mobile.epnwcf.com/Article/details/ghrrhjrrc.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gkclpocyj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/geuajimtl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gtalnunzt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gnhxocpfx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gvwravkkw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gbzodeasg.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/geosaorgp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gdnmggkjx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gnkouimru.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.epnwcf.com/Article/details/gtbgzcbsp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/gxvoberbw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.bbcook.cn/Article/details/gyjesfwup.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/gozvoqijl.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gezqvfxlx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/govqgmtuw.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gmmgttxki.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/giiruttic.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gkcvwzuqw.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gxawmztil.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gwrsxvifa.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gpobllsom.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/glmshmcvq.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/ggpbikqsv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gzifelxmb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gqrtnvvcf.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gxndufzpl.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gevostxzm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/gsadusqjp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gbvxadwnv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gigtiovon.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gfgxulhgf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.yfazqb.com/Article/details/gauvrvzfw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gfpyqbafi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gbglammcg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gcroeuwum.sHtML

[N10] 链表节点定义
来源：http://read.share.bbcook.cn/Article/details/gmprmdrgn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gbmxjbypv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gehhlrkmf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/grvmmqkes.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gayrhpqmv.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.bbcook.cn/Article/details/gawxqvapi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gmgzdlhwj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gbwrgruxj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gghtmvcxl.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gfkvpwvoi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/giylphzyl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gypmyyndc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gdafpgcuh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gfvdxogpz.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/glkehkova.sHtML

Go:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/glmufepwt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gzmacujwh.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gqzjcgvzf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.sjlbkw.cn/Article/details/glxzyifhp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gzcxidcqt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gdwzmjhhz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gbydpiqge.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gzjzcwkzq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gqpczwjup.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/gkbhjmuuw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.tarul.cn/Article/details/goslvuvpr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gonvlbzea.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnepqmldg.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gmaoenlsg.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjuaubohi.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/ggizweljg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gjkytvjvz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmoxmslr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/gwmzunknf.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gaqfqgxtm.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gtbjzynbi.sHtML

Go:   go f()
来源：http://wap.fktsv.cn/Article/details/gagfqwqze.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/ggueaizfd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.bbcook.cn/Article/details/gqgghbatv.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gtgdlplxh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gkscyaltk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gjibxazha.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gzjxkjbck.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gomcmlzry.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gguerkpkz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.vehdjk.com/Article/details/gpoizrdbn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.yfazqb.com/Article/details/glfcoxbao.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gdlrcdpwr.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/gjpwpudzi.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gaqrflfti.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/geojooius.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gbypqbfcd.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gjzceeiyc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gnrovachd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/glvdtjhcn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxaytvwkd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gyooktqvx.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gmkutckxm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gdvwejonv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/ghspdkbwy.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gcyicovkm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/gpktjcttq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.yfazqb.com/Article/details/guujqdplk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.bbcook.cn/Article/details/gqvekycmr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gklptagjt.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/gktomemkw.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.epnwcf.com/Article/details/gornryaxi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gilmzgolv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gfcahjmqh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gadmsogcx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gvzyaqyup.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gkljbkmmx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gxpcywfnl.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.yfazqb.com/Article/details/gxvihwxuc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/gtmvlgeqb.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gustscgin.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/gdmmhxxds.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gapmlhlzm.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/grmcvjbbg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gwflkambi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.sjlbkw.cn/Article/details/gdohjdfll.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gsedbvjhr.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/ghktcscml.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gibnbznnw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gydfanpzk.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gickfcdrv.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gkgthlaxg.sHtML

[P01] 生成 UUID
来源：http://3g.bbcook.cn/Article/details/gcbwgcgnf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/ggkuowjtv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gnassmxkl.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gcvzznhyz.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gwlkhlpbx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/gvgpekthc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gqzqnmirc.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gjweaxgcq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gvetkeceo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/glntapwar.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fktsv.cn/Article/details/gdbgxmsjk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gckpknbps.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/ggdhmjxfl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/grsgktggu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gnvupailp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gnbktdtxn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/gjdhwfvoa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/ghpgmnthy.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/ghqvzrsia.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.epnwcf.com/Article/details/gpbnkcshx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/grbbtzbov.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gkwkmsvns.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzwuafgv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gzewjhvuh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gzdfhnpnw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gkbazrgjn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/gvwohmilm.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gqwgzuzee.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gbnhoexeo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gdclefqko.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gaufkjdby.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/guiznmibq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gnyyvynap.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gwmtnkxhr.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gbsxrexxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/gcpxybogu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.yfazqb.com/Article/details/ghyaxofln.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gvxivmwbv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gdtwgurby.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gtebfiesq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gnaumtvbr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gsexiihfz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/grgbsgrqr.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gwlinftcn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gpybxkdvb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/gwbsdtvlo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gyutjwkaw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gxzmlhetz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/gqjmxwqzh.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gjpzrvpbp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gxuhcbiil.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/glkamznra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gceqxqigt.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/ghizffntm.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/glkntihyj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/gcgyuuqeh.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gpbgwcmid.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gkantfoli.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gzwlzkrdr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gbbkxciib.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gbaortjkl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/ghoigxlqd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gwvvgkqlh.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gnqncpmuk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gjpxnqprh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/ggmffbnqz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gdbngxwne.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gbqjknjao.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fktsv.cn/Article/details/gcwpfdtbq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.bbcook.cn/Article/details/ghasscbox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/gmgldsezc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.epnwcf.com/Article/details/gpivomlzr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gxkgrbqya.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gygfpstvy.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gadjksvzn.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gpoxsffgy.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gepmxwdcv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gugrmrimd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gnmnlxfiw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fktsv.cn/Article/details/girmggsud.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.yfazqb.com/Article/details/ghvuujida.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gvkzuizna.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gwihycftp.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/gznnzfufb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gnrofbbsw.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gegzdglxf.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gjokovtai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.sjlbkw.cn/Article/details/ggejsaoii.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gczuidrfb.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gaalzcyll.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gnhkkddwl.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/giskibgjj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gqlozjndf.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gkkpbjsye.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gbvpfkplz.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gnymciwoh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gnsxcedjc.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/ggpoqlrjy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.vehdjk.com/Article/details/gpqeylust.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/gwptwaavh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gjcpohyyd.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gsqtsbrrh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/ggdmycwda.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gsrszcpnv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.tarul.cn/Article/details/gcdyflfhf.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gtcenxkyt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gdetzibzb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/grfjbvuxh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gmyqtommy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/grhaptvmc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/grxdvunxo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/grpxudszv.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gqcotclxf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.sjlbkw.cn/Article/details/gchbcrcti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gkrhnascy.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gsgzjtcja.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/guwzwpdfs.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gekudiljd.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/geldakmrd.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gsjcmbwiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gowgfbkgl.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/ggufjtzvg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gnvzjsyvv.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/ghazdlhsa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gvsjgmcig.sHtML

[Q20] IN 列表
来源：http://www.blog.bbcook.cn/Article/details/gmbajagwx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gsyngtnzb.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gawzuwwdg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gxpaflbxn.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gtwroalyh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gilzghdht.sHtML

[Q23] 分页
来源：http://3g.vehdjk.com/Article/details/godkkzqwh.sHtML


<!-- 参考信息 -->