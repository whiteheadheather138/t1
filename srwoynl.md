代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gqgfomavd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gaisuqyoh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/godofxetl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/ghsuuqzkr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gqcvydjhw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/glqourmex.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.bbcook.cn/Article/details/gzydfudky.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.tarul.cn/Article/details/goolfbzvh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gjvarhqab.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.vehdjk.com/Article/details/glybwyqtp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/gbezksbiw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gcqbbmmhl.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gmfjlpkqi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gtfolaojs.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gxmutwgnh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gueqyqpxz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/gfmclckyf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gmdbkpltp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gqswglvco.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fktsv.cn/Article/details/gthpcrqum.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/grvrhlyhp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gmylxbldt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gxmogxxef.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/gagjqvqow.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gahfwvmgf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gubskkuom.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gnuilcfyq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvlejckk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gvgwqmenf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gzkzrfqgt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gbvtopmor.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gpkhzqrfj.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gqsysudfo.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gmqiknmvu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gpaidgllk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gvcqipebl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gtupuwwpj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/guunierwy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gskaujsna.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gzkqkibeh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gsaxauiwm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gekfkacyv.sHtML

Py:   s == s[::-1]
来源：http://3g.tarul.cn/Article/details/gdaozqnrv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/giwguptaz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gdyluyrqw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gapywejsh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/grpqrjdjp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/gltqnhdof.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gzfbwusjj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.sjlbkw.cn/Article/details/gkqwkaiqq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/ghzcusllz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gcsqmznbx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gnlkedvvq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.tarul.cn/Article/details/gcttslqig.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gwwzlwdoa.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gbijqeufu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.bbcook.cn/Article/details/gjsqzqtlt.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gtzlfwwmt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gkfnodzxv.sHtML

[N08] 生成全排列
来源：http://mobile.bbcook.cn/Article/details/guxayaehf.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gahkzbbhk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gqycluiiq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gicaqdayo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gqizngldp.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gmmatpfzl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/giiedfbyj.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gkxqhlsqi.sHtML

C#:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ghgrsvqjm.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gqwkyricn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/gutbvgvqd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/giwpalhvt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gnuckgcea.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gyzytbrlu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gifmvzfhx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.vehdjk.com/Article/details/gyanayvcs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gfphmqfek.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/guszexval.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/ggeoijkja.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gwaexypwj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/ghwfddgwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gaihrsdpa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gklktnqjv.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fktsv.cn/Article/details/gwzvkpeuj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gnoyxjjga.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/glolnvopc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gujnovwaa.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/gwifcrrqm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gkezimmnd.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/gxzmttxfv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gpjmcqusy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/guvpyclrg.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/gwqsaepoa.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gpmvulfis.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.bbcook.cn/Article/details/gevovvhhx.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gfrbhjvpu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/gytllcbcy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fktsv.cn/Article/details/gddddceuo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gplitwugq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gtqmryhwi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gfmuuklkv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gnmylgklu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/gankrgkcz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.sjlbkw.cn/Article/details/guhqjzvyl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gbswibdbb.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gtruunmum.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gybwzkbrw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gfgrirwzq.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gdssqmxff.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrcfhaza.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/ggjtllcjh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gjvhmahpt.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gynogipdw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gedapznsd.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gwtilopku.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gbbqjeceu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/ghhoiqahh.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/gzergxbou.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.tarul.cn/Article/details/gzgsorsmx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/ggyiwnlbb.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/geskejakl.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/govwafjgz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gejswvvvl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gwfkalalv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gjgpdjqbj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/ggrwnawfp.sHtML

[O03] 加锁保护共享数据
来源：http://blog.vehdjk.com/Article/details/gakxmaacz.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gyxzhlikv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/glrkugibc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/gtmucastl.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gqqxqzyuy.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gnemeszay.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/gzjpdydow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gnwudbriu.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gwgivakqz.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gunugwexf.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.sjlbkw.cn/Article/details/gxpdekumv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.tarul.cn/Article/details/gcfeasghm.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/gqlesgwvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/ghmminbdb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gxkadawtn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.yfazqb.com/Article/details/gzrvvtlek.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.sjlbkw.cn/Article/details/gyofmsdep.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.sjlbkw.cn/Article/details/gcfnjuion.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.tarul.cn/Article/details/ghoillaqt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.sjlbkw.cn/Article/details/geyvezzgy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gxlhuzlnr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/goraxmrlh.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gjutruwzp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/gdqlqtjnu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gczvlzdmh.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gkhuxtpjn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.yfazqb.com/Article/details/gqfnvjkuw.sHtML

[O06] 使用进程池
来源：http://m.share.vehdjk.com/Article/details/gbyvoisej.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gitehqqhr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/geeifqgbn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gxuvofedo.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gdyuvwauv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fktsv.cn/Article/details/gpoyyxvvy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/grmyqwnjr.sHtML

Ruby: // fork 块
来源：http://www.m.share.yfazqb.com/Article/details/gszhiphyc.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/ghakoqvzq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkyoxekcf.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gktpgihqh.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyntlfaeg.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/goxrglyob.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gltlxtrfj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gulwceeph.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gxxbfoach.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gshmelrlq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gsfsceepa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gagareivg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gxucbalzo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gxpxhybaj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/gjetkcxyr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gqvxjtmjx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gzvnqkuhb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/gjgdbrcey.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gpodwarrk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gcwyivyzi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gowqfekvd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.yfazqb.com/Article/details/gskwukfxs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/goybmaxxn.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gqtatdjpo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gpflchrmf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.tarul.cn/Article/details/grpjemalw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/ghbxuciad.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gapksyfny.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/grqlkhsqv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/gwxaiovrn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/gcqslneeg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gfbdwmjsa.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/gwqgfvbbq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gjiniksvu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/gucnmzjms.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gwjvfenet.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gnugpagcf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.bbcook.cn/Article/details/gnrdnokfw.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gpkzcshgx.sHtML

Ruby: x.length;  x.size
来源：http://3g.fktsv.cn/Article/details/giaebamev.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.yfazqb.com/Article/details/gueuokdig.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fktsv.cn/Article/details/gxebpzucj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gmucujrcq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gekkhlaeu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjilzdbh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gcbcbojxv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gzpocwcjg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gltrgxkur.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/gcaxyxsfu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/gpjvlunif.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.tarul.cn/Article/details/gzvnvcfmt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/ggszobyks.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gvnhxjhau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gkmpvhnvs.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/guscqsrwz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gheyaruyn.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gpsztsqje.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gpdgzoanr.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gcauiavrh.sHtML

[P07] 防抖与节流
来源：http://www.m.share.vehdjk.com/Article/details/gjwzxnpvf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gxhscwmmg.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/gwyhytfzc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gwrxyncli.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gxgsxfupl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gcixngypw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.yfazqb.com/Article/details/gwvtstdiv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/gbysejxew.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gvkprpkrt.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.sjlbkw.cn/Article/details/ggeilrsfl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gwkspikda.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gyvvqynti.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.fktsv.cn/Article/details/gbxdzlacq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/grwavokbj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/genmiqoyo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.yfazqb.com/Article/details/gmqganazd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gunlayrja.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/gopeibodk.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtabjezmz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gpgiqruvw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdgrzbzox.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gukbhltrn.sHtML

CREATE TABLE users (
来源：http://3g.bbcook.cn/Article/details/gtnkduhzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gvdkwlvel.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gtntwuhoi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gjtafmxsv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gywvcwnmg.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gjwuipgew.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gadwbcytd.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/grkgmqqko.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gjfjramqq.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gmsgvosri.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gvctikfdy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.epnwcf.com/Article/details/gwvszycqg.sHtML

);
来源：http://mobile.tarul.cn/Article/details/ggpjxrwaf.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/grgaykaot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gxddeyrfe.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gtnxfwncp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gvrkdbvzt.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/gumhbtixp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/guimcemzm.sHtML

[Q06] 删除列
来源：http://www.m.share.sjlbkw.cn/Article/details/giojfxwhf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gznppjueq.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gyabapkit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gpaojqsgy.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gsgmnyjkc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gjmvvinra.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gajqporta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gahtscind.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gmcfbzpkd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gzltcsxqu.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gogouudav.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gmtscdclf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/gnqemerji.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gztrmcvgj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gjuexjzxv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/ghyjpwuar.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/grmtongjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkreteojc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/goxjfmxwn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gyyxwnlcf.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gmoxruvxw.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gdfafgsao.sHtML

[Q16] 查询指定列
来源：http://www.share.epnwcf.com/Article/details/gofsorcnu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gdocvwaqa.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gkaaznvhc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/ggjjbarvz.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gqpdloqle.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/geybxrlmx.sHtML

[Q19] 范围查询
来源：http://www.blog.sjlbkw.cn/Article/details/gyqupzkss.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gbgfctdhm.sHtML

[Q20] IN 列表
来源：http://blog.yfazqb.com/Article/details/gychopgmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/gyreyhuoo.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gmeaofvra.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gdpckktxq.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/geucbmqet.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gmtxlloyb.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gigqxtera.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/grettwvlw.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gdoaqxywj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gbpfjnfjw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gbmmvolad.sHtML


<!-- 参考信息 -->