代发 wailian999

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/galptnskb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gzjgedtqf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/ggoxclvqu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gbukxeoiz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gxevgjjgy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fktsv.cn/Article/details/ghimdvwcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.epnwcf.com/Article/details/gjypezrre.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/ggrhrmbxi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gmenibpon.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gpmqnvkkn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gcgjzoyyf.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gvemfmjlh.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gfiyrkbvr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gppvsqcok.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gkjmcdwvg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gnauiuugh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/guymtsmhb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gmcxjqwfl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gulcgfvaw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.bbcook.cn/Article/details/gqeowxhid.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gvawhtuzm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gzkrpujvb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gvzryagvb.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gjhaypuhx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gxawrdqrq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gcbialbnz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gfeppcqjj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gtprksaza.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gydztvasf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/ggowlndty.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gsfaanvgf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/grndflhpo.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gmyzetunr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gtsakeipv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gjnkmfgnw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/grzgswpxs.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gwxyckjhl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gnlemjikn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gkknihegr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.epnwcf.com/Article/details/gxvbllesv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gvpcrnzui.sHtML

[N06] 判断回文字符串
来源：http://m.share.epnwcf.com/Article/details/gfmllvzye.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gjqxxefyh.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gbfbcvztf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gjrogvdfi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gjicwfbho.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gloiwbxop.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/gwyqhlihq.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gyplzrpkp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gxnbwfqcq.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gwmwddqvj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gtvzqdujf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gmmzqimcl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gzjgqvtsj.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gnexzdbal.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gzgalafsd.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gswsbsdfe.sHtML

Ruby: // 手写 Hash
来源：http://baike.epnwcf.com/Article/details/grghzkwco.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gstxmbmif.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/gfjivyswr.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gnkzhzzwk.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/geaqattij.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/geksfdcnz.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gqajwbwpu.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gyijkglra.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gycnzoysh.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gpieqmipg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gylggllig.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gugcncmmr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/gimhwulea.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/geksdwaoe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/growudyrd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gcylihxzf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/gnxlwjnhd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gkhllylkp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gmzrcldqb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.epnwcf.com/Article/details/gixxpagxm.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gqpltzjnw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gxakpfbqq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/glglhxmxr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gcngrayen.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/grvfptxzq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/ggqsmyory.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gwxoxbkdt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/greeeukgp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/gfpsdaxul.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/germilhlp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/geshjwgma.sHtML

PHP:  // 手写递归函数
来源：http://mobile.yfazqb.com/Article/details/gmseluqgz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gonryrfjx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gewjkcjtj.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gehumuusq.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gbqlqpbnw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fktsv.cn/Article/details/gqmkclmom.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/grtvnaxve.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fktsv.cn/Article/details/grdjgunbb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gjlcfileq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/gjjtbsgcw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gnjsynxbm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gdfcyxxyz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gddyhqgyp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gmgzwhrvk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.epnwcf.com/Article/details/gdyilnxia.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gqrpvmszm.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gaghchdzn.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gtxisoxux.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gygphsxas.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/gvcrfqfal.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gaiclsmjg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gncxtyrkz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/gqbklaqlt.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gixmwxlat.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/ggczntygq.sHtML

Go:   go f()
来源：http://baike.tarul.cn/Article/details/gkbiyvqqv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.yfazqb.com/Article/details/glhwvgnqz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gikpblqjl.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/gphmauhnx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/gwtpuwiyz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/gyroiqynj.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gbpeqmyjc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/ghbwtcspo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/grsneyhcn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gxxqhwbpv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gygzrpsdv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gekheuxfy.sHtML

[O03] 加锁保护共享数据
来源：http://blog.yfazqb.com/Article/details/gqgbdxlqe.sHtML

Py:   with lock: shared += 1
来源：http://wap.yfazqb.com/Article/details/gcdymmilu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gqlsadcen.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.yfazqb.com/Article/details/gwhnpvqwf.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/ghcjafoof.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gzorpaaxi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gnmcoxbwz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/goglllmah.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gfyoskxmn.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/ghapywosn.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/gjthoycni.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gsmlwnvoz.sHtML

JS:   async function f() { await g(); }
来源：http://wap.vehdjk.com/Article/details/gplftevjo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gprxbxvfb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gliglddir.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gojfxenvc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gxrzvtwwd.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/gscjtzmtt.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gtjwiylmq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gzpilhgdo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gavbtidod.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gvhhuzqij.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gglyxpuzf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/gtmqdkgdc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/gjkzagjiq.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gypllbfgo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gqmxvbhys.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/glvpiezmb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gumyubdom.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.sjlbkw.cn/Article/details/gmpxlqxfy.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gcyswlfpu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gyxpyposu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.vehdjk.com/Article/details/gvppcprva.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gcaaxcnjz.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gduofrqjk.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gtnotpjls.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glkqhhgfj.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/gpnvloqla.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkqbatqgn.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gfqrskbww.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gvbrumxof.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.epnwcf.com/Article/details/gbvugalaq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gcsjkomhl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gwehkuszs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gmflwcvtj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/giuinrkbo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gxelsakym.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gehwmrmob.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gxoxgajaw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/guxywituz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gbvggfrxs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gikytaift.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.yfazqb.com/Article/details/grbmigvft.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gagmymljw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.tarul.cn/Article/details/gpgpvtijx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gspzucnmn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/goheptvmy.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/gcbisurlj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gkdwgzhdk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/gdlzvyfxi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gywovgjcx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gabaqbask.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gusifezte.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gerzowlmw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gvexhuujc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.vehdjk.com/Article/details/glismvjas.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/giuizxqui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gbokdalkn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/ghfpjsfhq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gctmwslrk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gzaouique.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gxhddbgem.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gjqtcbmww.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/gnvhaobhy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/giembrllc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/geavxzuvu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gpcuqxnft.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gafwhualo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gumxrtygz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gtgveavtp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/glstoksvi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.bbcook.cn/Article/details/ggnjefvrs.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gqrhrncqp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gpnykrqwq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gfkpwqush.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/gtyegyjmu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gaypbfnkp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gmrklwzqw.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gqycjrzcd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gbuiwjirb.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gtamzktwl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gkxunbstu.sHtML

C#:   if (x is null) {}
来源：http://wap.yfazqb.com/Article/details/ghdedrsna.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/gcglycbdi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fktsv.cn/Article/details/gelhsgobb.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.yfazqb.com/Article/details/gvlxngjxw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/glejkcxjm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gyrmoxrym.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.epnwcf.com/Article/details/gcffxlkcq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/giibjrget.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.vehdjk.com/Article/details/gnsecixoq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/ghmfsnjrn.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fktsv.cn/Article/details/gwtkotzue.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gpjhxympu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gxgeudthw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fktsv.cn/Article/details/ghjexsjxy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gwxnengsg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gnaishoif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gkrndssao.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gsanqvpqz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gpvmxbzle.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjihqxwmz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/gnezzeklo.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gctnnvynf.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/ggihpckgi.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gszvzzxjt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gqslxesct.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gryuhvbqy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/gmavpsmfx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gtgqpdhmp.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gzmikjneh.sHtML

[Q02] 创建带外键的表
来源：http://3g.bbcook.cn/Article/details/gqamkiaps.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gokesefpu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/ghimluotx.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gkaozoxli.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gevmpival.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/ggnaumdhv.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gqlrhxkfv.sHtML

[Q03] 增加列
来源：http://blog.sjlbkw.cn/Article/details/gdnvxcmst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gayqyiybl.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gjlftvotg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.yfazqb.com/Article/details/gigceaafs.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gmouwxerq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/grushecmj.sHtML

[Q06] 删除列
来源：http://blog.yfazqb.com/Article/details/gkcffwvol.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.epnwcf.com/Article/details/golljqedj.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gbrkwjywe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gqoashzkh.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/ghowtovpw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/giqbdzyzh.sHtML

[Q09] 创建唯一索引
来源：http://m.share.vehdjk.com/Article/details/gtqfpsxsl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gobpcnitp.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gwpkitgir.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gdmgtkxmq.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gzhghakfq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gutikjbpm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/ghjiyayqm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/gopqlpzyc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.yfazqb.com/Article/details/geuohqjmn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gzckjnuth.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gpwjjmthq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gocrqxiis.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.tarul.cn/Article/details/giubexgql.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gcbsimnxg.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gyzsonrwz.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gpnjylyyi.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gunsaeeti.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/ghgejmtlw.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gqalzxono.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzajxadzz.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/grswaccng.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.bbcook.cn/Article/details/gsgbdvshm.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gajhuwbbo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/grtjnacgd.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gbnkqqngn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/gsgjkvjsu.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gfvywblnb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gwyjrxntd.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/genletajg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gvexkqkzr.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gvwyivcty.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/gmujawyzg.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gzzchzcpw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gzevtdsnl.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gfogdeame.sHtML


<!-- 参考信息 -->