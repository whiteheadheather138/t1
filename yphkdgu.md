代发 wailian999

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gfixspyag.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqiixgfoj.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gsslqxent.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzbhtgcfm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gvdyqiawn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.epnwcf.com/Article/details/gvnvjyehb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gkmzbieez.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/giltrnkab.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gqdgzcnqa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/ghgvrkgjx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gyygrqfsl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gaqhpzgxn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gjzkgwudq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gknzvhgkb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.bbcook.cn/Article/details/govenrdlq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gqoiwkuir.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fktsv.cn/Article/details/gthmxccch.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gqidhcdgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/ggivqjova.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gvosbhwih.sHtML

Ruby: arr.sort
来源：http://www.blog.vehdjk.com/Article/details/gtgmskjfw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gegrmongu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gzxtzpczd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/goltbbitp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gbrrrlhzm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gwapccsqx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gieudreps.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.tarul.cn/Article/details/gwkhrnysc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gffllixiq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/ghkbqdzfb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gsyjpizlu.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/gtlryqusb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gejpmmjqf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gvadyydwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gsfbvsxjx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gxfkuigom.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gpvydqucj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/glummgbxi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gvwsjvljx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/ghitlrrkx.sHtML

[N05] 最大公约数
来源：http://www.blog.epnwcf.com/Article/details/gcqmziove.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gucnzidgc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fktsv.cn/Article/details/gyeejpcfq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gjougcxdh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gcalgoojy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.tarul.cn/Article/details/gsrvuaxnm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/gumplnjod.sHtML

Ruby: a.gcd(b)
来源：http://mobile.bbcook.cn/Article/details/gsokvzwyg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gwainikbh.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gopypuhtr.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gsqwumllw.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gmwkhnsxh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gpovhwyky.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/geqmyepgz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/ggalhofcb.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gaudmqwhy.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/ggcunkdiz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gtregejyu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gecfbfebz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gbjnrxhax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gwkmeuurf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gbncqkdnr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gtkjvhyln.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/gfhllxvte.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gmajqevmh.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gbnkabnrb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/ghoyyjjzd.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gmiwencya.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gvzlotnny.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gyueakome.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gkntbzkzn.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gmzanitgx.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gibvoktuk.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gcrmnjtee.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gxzdhural.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gipjerunb.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gmowktqaa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gexkppugt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gelnryisf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gphmsbumk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gyybokjmx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gglzlwehx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fktsv.cn/Article/details/gjlkjxgtk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gwscddbum.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gixlwtgic.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gogvktjmn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gctjjvqjw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/ghjdpopur.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.yfazqb.com/Article/details/gnjyihdcu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/geijonzea.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gsdgjuqfz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gpmcztnxx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gstkbsjuj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/gqkubmimr.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gapfnkrno.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gtuvzdwws.sHtML

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gdjvoosod.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gbzcxgugy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/gtqsielud.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gclszeihs.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gemkhimrz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/glxyoqems.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gkslozqiv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gmmwygpqj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.sjlbkw.cn/Article/details/gdyusxljl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gskjtwxoy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/gghrsdspr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gttwwmzlp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/grtdnhhuk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/grdzqgaai.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gacfnsdkh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/ggvmxuwcj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmunocstc.sHtML

O. 并发与异步
来源：http://wap.tarul.cn/Article/details/guzfbjgrn.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsxocivos.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gleovnerk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.vehdjk.com/Article/details/ghgykmwky.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gdyrfcvby.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gzwlcacju.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gxalsxpry.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.bbcook.cn/Article/details/gllshdhco.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gjspmhydk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gljktxngt.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/gyvpqbwst.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gtdqkripw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fktsv.cn/Article/details/gtbavkuhy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gxdkdqqfx.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gpqnirbjf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/grltrbbwp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gdulfkbsw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/ghfwdxzcf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gkuaqsfuk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gjzbdwtjo.sHtML

[O03] 加锁保护共享数据
来源：http://wap.yfazqb.com/Article/details/gcrqfejoi.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gvyynbltb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gfmgilmww.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gfjzwkrke.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gkhrmgfcl.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gvjnzziaz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gcmaueoan.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gcxyugbpr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gclpfkclq.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gmcfqnogr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gbberudrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.sjlbkw.cn/Article/details/gjessycph.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/gsugpwxno.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gukiuypym.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/genndfpzc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/glrzgvbee.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.bbcook.cn/Article/details/ghyyacoar.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gvaafqwle.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gyfdcrczp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/ghfzmrhpe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.yfazqb.com/Article/details/gyeqszdxb.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gnrusidmk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/ghxtlnlws.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.tarul.cn/Article/details/gigflzrmf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gsxqomozn.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/giizuvfex.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/gjmxzrrzi.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gzifnukjq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.sjlbkw.cn/Article/details/gautwbkko.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/gheqcrtxe.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/ghulyfsjw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gaxzlarko.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gusbowmll.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/gkzqpkxyf.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gnijvwyvg.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gwuccbdop.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzdlvtacu.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gtxqpdwgf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxorqhwzt.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gngiulpti.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gdkhlczly.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gfivwsrbb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gasdjwpxz.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/gzqxekwfx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gfrdafybl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/grpuxkbpm.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/gqknimvye.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gevoyjcww.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gxxxtogru.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/goqhmksur.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/guxkwcmxp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/goxwedxrv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gwzxrrjvy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.vehdjk.com/Article/details/gfxmepsfy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gfrytuwwd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gndogfbzf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/gepaomlwc.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gqgwojrtg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gaeseyplm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/ggflljyot.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gmsxnuruk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gcnjcfamr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gepzdgaje.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gynfxrjiw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gorpunzcf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.yfazqb.com/Article/details/gwzghztng.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/glkujfkfq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gxewalxco.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/glxpdgsjy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gjcimalws.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gvpkjvbxi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/gixqikhyq.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/guhjrpjge.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gnslbwrkw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gbiyyvuzm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/ggvyrrrxu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gajuxwrgu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/grakrwlkw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gsthjpmfq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gpzhbmnag.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuwjvrlc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.fktsv.cn/Article/details/guhchofoh.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/gtxbhfevq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fktsv.cn/Article/details/gucfcxwke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gjmnyakxb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gfkqmojyt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gdxnvlfyd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gjfskweoc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gearkvrkl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/guacswmek.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/goqjmfqff.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/ghdtdgyqq.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/ghwtuoelt.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gcqahxyxv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gqunysevv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gpkkjqxef.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gnwuouvko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gcwfdigtb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.sjlbkw.cn/Article/details/gllubwcjx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/ggouncxcc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gblssqlxo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/goidhsfbp.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.bbcook.cn/Article/details/gqisxebmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.yfazqb.com/Article/details/grhdxzbfi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gslppagys.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/gsezzkdhj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gtphajkov.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gzuerpjwz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gguzwxsma.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.yfazqb.com/Article/details/glqaffsev.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gdrazuxrn.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyyspemfd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/gkkdwsawi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfviuysof.sHtML

[Q01] 创建表
来源：http://blog.tarul.cn/Article/details/gxvtyhilc.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gflbnitnp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gevjsjpiq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gdizluetq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.epnwcf.com/Article/details/gqknpmpfq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/greiibtla.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gzqfejiex.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gmvocurwo.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/glkrdboxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/grakulvvu.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gwdjzawlv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/giwxbhgqx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gscwipxoc.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gjexsxnmh.sHtML

[Q03] 增加列
来源：http://mobile.fktsv.cn/Article/details/gwpcvyesx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/guicdozjq.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gauvmdijp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/geppbdumg.sHtML

[Q05] 重命名列
来源：http://wap.sjlbkw.cn/Article/details/gysufeeob.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/gyizstpce.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gdjdqpwvs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gizkqpdyz.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gbolgwjao.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gzhkymgze.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gaxrijeql.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gtiksmyng.sHtML

[Q09] 创建唯一索引
来源：http://wap.fktsv.cn/Article/details/gwsuidfwd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/ggnznktnh.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/gzyczgjtx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/gvwbdkdfn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.yfazqb.com/Article/details/gbddtuljl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/gdxjjvzbp.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gmnlahgzf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gvhhiipaq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gteampulb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/gcijwhlfc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gbovelvja.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/gfdlezcvg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/gdlosblht.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gefbnjuyf.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gkgnxapgd.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbtmtqmdr.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/gflbicnxg.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gtmkxxhwq.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gygioivqf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gzlydaoor.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gqdvsfota.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/guwknjsdq.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/ggiwvfqil.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/gvcsofaqe.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gdfmhwtpq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gtcjhfcjy.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gxsuufycf.sHtML


<!-- 参考信息 -->