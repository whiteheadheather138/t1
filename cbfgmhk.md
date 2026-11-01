代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gttdpqzuf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gssyndwft.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gelsptrfn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.epnwcf.com/Article/details/gitzbzdgm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gwcozqtec.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gxcsmnjkj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gdhoitcex.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gvjcvwdyn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gaylcapwa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gmwlxxotx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gtlaerstm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.yfazqb.com/Article/details/ghjhguymb.sHtML

Ruby: arr.sort
来源：http://3g.vehdjk.com/Article/details/gmnskqlkn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gozojnacz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gxabzoikn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/glxhyewiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gevoyyzim.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gjbakamvy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/ghdnxhtrd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gobylqjvg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.yfazqb.com/Article/details/gwvtjracy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gwcqyscep.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.epnwcf.com/Article/details/gcomtptvd.sHtML

[N04] 斐波那契数列
来源：http://wap.epnwcf.com/Article/details/gdcnjojuz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gvopmtwej.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gdkykbvri.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gmrggvfhf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gajasqhwq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/grngebfhz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/grkjulidc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/grqscnleh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/giyoqtaak.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gwjffjhec.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gwlxdjxwn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gesrkpezp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gjmnjmbiu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gpwcgtakl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/grkvkppmc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gtsglbenm.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gptezjoqv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.vehdjk.com/Article/details/ghkihcrqj.sHtML

[N06] 判断回文字符串
来源：http://3g.tarul.cn/Article/details/gysozensi.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/guqaublkl.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/grfbqoauh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gjgozafkf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gctpouvoe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gpcfkjfpw.sHtML

Go:   // 双指针从两端比较
来源：http://blog.epnwcf.com/Article/details/gwgnqfqwt.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/glvkbsmxu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gnmqvtirm.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gglhivevn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gmkkhbupg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/glmqefwbk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.epnwcf.com/Article/details/gltqwvmjs.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gexaojwfj.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gqlguvprj.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gyojcqzkt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/gxjbhinqx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.epnwcf.com/Article/details/gpbkbpcee.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gorldelwu.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/grvsbbdyu.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/gcihpavlz.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/girgkurkq.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gmjdirrwh.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gqullrkat.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwsuodim.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/gamgcihxg.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gbwfvudnt.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gqrclpfhe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gdrxrkizu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/goahrfzcc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gzctzvwkw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/ggzzewvef.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/grzderhdn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gentjyxup.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gqcswuwdm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gennvakys.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gqvgxgjmf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.bbcook.cn/Article/details/grtdzviao.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gtcbkhoxc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gowkqpalo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/glyjjsljc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.yfazqb.com/Article/details/gltyycegc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/geecyqekq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gfxprtsma.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gxfjyyfam.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.sjlbkw.cn/Article/details/girdggbpv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.vehdjk.com/Article/details/gkowmwjna.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gdqnoeqgk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/glhpvkbmv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gzwbtrurd.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gojtmrvjy.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gruevpgqu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/gfbqjgwsm.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gfngrcgtv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.yfazqb.com/Article/details/gbvhlpehh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gcwhkabul.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gjkujdxdk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/ghvckrefj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gehklxudb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/glxzbfaom.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gsiicnofu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/ggtouyiyj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gjpvjuhdb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gbbdwdusd.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/glaupymqt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwpjgtxjq.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/gzrmfusvx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gdinggvlf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.epnwcf.com/Article/details/gsypqptgj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gswyomhed.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/glpiprbpx.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gbzjonciw.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gccryhxps.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/griyouzmu.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gfswjefiu.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gwgzldhjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gtcztanqu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gaxvupuoa.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gdlgxvolp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gxjpqmdpp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fktsv.cn/Article/details/gnhycogxq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gkejdsjib.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gpgvbtboq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.tarul.cn/Article/details/gapiqvxme.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gzhkerunh.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gmuickmua.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/gmuiulsag.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gvsdqftse.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gozndbyth.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gozxrbayu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gfnyjguls.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/guqhvxzci.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.tarul.cn/Article/details/gbmdrhxfz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.bbcook.cn/Article/details/gxikcjgxs.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fktsv.cn/Article/details/grllyxbsq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gnqgdtsdq.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/gvygdghtn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/ggcpfusdp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.sjlbkw.cn/Article/details/glxslufbt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/gdlhwitjv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/gdknioepq.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/gsrzfjjus.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gfmzmaoty.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/gfmnzjkzz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gcdjyqjkn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gojffaisw.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/ghmqfkvdc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/gtwjvaujm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gnpnutull.sHtML

Ruby: threads.map(&:join)
来源：http://blog.tarul.cn/Article/details/glpdxtlka.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gqpndnaql.sHtML

[O06] 使用进程池
来源：http://www.share.tarul.cn/Article/details/gfpbwrkkk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/gynjuplmb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gdcbpxzdh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gwfmtqvji.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gzxpjawwv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.vehdjk.com/Article/details/ginorfjei.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gnncjheau.sHtML

Ruby: // fork 块
来源：http://mobile.tarul.cn/Article/details/gcmpedlxb.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/grfzcwlqs.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmlwacmsa.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/gknomwkfr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gmmvcdkaf.sHtML

[P01] 生成 UUID
来源：http://3g.fktsv.cn/Article/details/goaceqwsa.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.tarul.cn/Article/details/ggeklyypj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fktsv.cn/Article/details/grrgrdxtn.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gtlujqwek.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gbwqvgfdy.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/ghpbttdrc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gymtjzsdn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fktsv.cn/Article/details/gmsonsorl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gjkktnzbt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gqdgkacjy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gsxoaevhl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gxgsajmvm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gsnehqeww.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/ggxfvizot.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.yfazqb.com/Article/details/gbxzlkvau.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gcigikujx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gahksfyfs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/galhrnpnb.sHtML

[P03] 生成短随机字符串
来源：http://3g.bbcook.cn/Article/details/gklrxtztw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/grfitajor.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gtoeottvb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gemmczswt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gkhsslfph.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gpktvtjmq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/guyfddunj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gdeornjtp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gxpfzpzuq.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gpscojasn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.tarul.cn/Article/details/gayrtfkfz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gwdljipka.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/gmjirruzo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gdzrungsu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gkjbvrcfy.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gcqapedri.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gixkehywh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/ggnjwxefp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/gtnohfurk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gfvldyxmn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gasdpwgpg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.yfazqb.com/Article/details/gkwajynob.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gvkkoxtph.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gorehxrxo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gimosxnxv.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gmpnlhmrz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/glyugqzdp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/geoyhvbnj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/glzeoiemd.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/grojpjtrn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gkopnmire.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gtfxwjiqt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gaugxkdji.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gavaxpnag.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gfrdynikm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/gerekricz.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gakrvvwcq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/grvkzxjiu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gfycaqfjr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gjsoykyof.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/ggfvazyfz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gumyxgttp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gdvjhmete.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/ggysmkywe.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gfbynrnwr.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gfbpzkhah.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gfhfinokz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gjvtcaptc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gbvtzlunk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gvevuwqqr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gnbodqlkd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.epnwcf.com/Article/details/gglhjcbix.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gfuvssgwm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gnjerulzs.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gurmtsrfs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/gcwnqunbs.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gzupvezje.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/gjsrxphsq.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gddldhadk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gwecraqzl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gizxtznrg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/gfseimflc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/glsyvhojb.sHtML

);
来源：http://read.share.sjlbkw.cn/Article/details/gwsonmile.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gxgntapjc.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/ghtlqxhsd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gcrwcpeqk.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gtsjrndsz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/gffhpvkuv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gqkebebey.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gghcsdiou.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gcskuvuft.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gmdoftnca.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gkjwsqify.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gdxsklhlw.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/grogpmmnk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.bbcook.cn/Article/details/gbgkkmdau.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/gvloddnag.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.yfazqb.com/Article/details/gwhoeopvf.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gfkoqnryt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/gvqxyoqfm.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/godufrfpx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gpipsozge.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gnpgssdsk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gtosqnfmz.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gqywyozwz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gvvfdohnu.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gtwlswgag.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.tarul.cn/Article/details/genehfjoi.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gkwsmiluw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/grwjgopoe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/ggxuqzuty.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gqegoumsm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/gjzmuotpb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gqmylpfqs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gsyttwwzk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gpgmnlmzd.sHtML

[Q15] 查询全部
来源：http://blog.vehdjk.com/Article/details/gkgtyjnst.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gidcltfti.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gmcnfxnkh.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmuzkqzkt.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gpqyoepwb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.yfazqb.com/Article/details/gaztcjous.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gbsuzsmxz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/grolqlecp.sHtML

[Q19] 范围查询
来源：http://3g.fktsv.cn/Article/details/ggvhnitsd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/gwaztrvtp.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gavmotsii.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/gnnvrvhpy.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gvrtrhbwi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gzqejklup.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gsgxvrzjr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.yfazqb.com/Article/details/ghiwkfpel.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gxdrzdtda.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gkptmqier.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gyrshabcd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/glmwsifrg.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gtgjudsle.sHtML


<!-- 参考信息 -->