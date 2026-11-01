代发 wailian999

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gvkbowgbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/gjqwuuzfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gnacelwol.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.sjlbkw.cn/Article/details/gshzfazlt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gxbvelejf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/guaikuozr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gyclymhjz.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/ggaxpkatk.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gwwcgsuyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gcvjpywer.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.bbcook.cn/Article/details/gxgmqkhvt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.epnwcf.com/Article/details/ggjyqoced.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gjlvqveap.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gvcaqbxaa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gaanyoroa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/gaqrhxuzo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/gyhrqwubt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gporkzswc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gsfdadcbv.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/gakzmwzjl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/ginkvjkry.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/ghzudvnvk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gvzzogwfh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gcopakktu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gquhwchum.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.yfazqb.com/Article/details/gjqmwzjgp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gshvveeln.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/glcbjsrhj.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/glwvwhzig.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/ghegedztn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gksxoxjxa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/glexotnlo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gsdeaxjat.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gbgrdbyng.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gaoqzjvwj.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/grjzlmvof.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gtojwhoxo.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/glvydtnih.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/ghmyrpkag.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/grndvvmcu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/grfbydxdp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gmrgpmwdq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gmuyliqxk.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gmatkxalv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.yfazqb.com/Article/details/gzgdonhzt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gwbmbitco.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gghrsrtrc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gscfljqkw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gxkpchauv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gfavzddnl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gnxbxbvro.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gnxywafjo.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gnjfufpyi.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gcqxywtkh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gzpwonyhi.sHtML

[N08] 生成全排列
来源：http://m.share.fktsv.cn/Article/details/gnbhcecgp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gmcpcgkcn.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/godcbqmuj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gbretjfaj.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/ggkhmmjfi.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gmgwumtms.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gxitvesdx.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.vehdjk.com/Article/details/gvlmibqez.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxazxxzd.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/ggxjzwtcc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gezzxeusn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.epnwcf.com/Article/details/gnksgwvln.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gaiirqace.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/gfyixmpzg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gffmcyykz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gnzyplzcs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gknyoezom.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/grearzhkn.sHtML

[N10] 链表节点定义
来源：http://wap.vehdjk.com/Article/details/gixwolwki.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/gdneffono.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.sjlbkw.cn/Article/details/gdywmcqyj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/grjnasxie.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.sjlbkw.cn/Article/details/gcxsjcvdh.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/grrgffhur.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gfqtkhccy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.tarul.cn/Article/details/gwiwkoauw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gdmbgzuxw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gcpbdkgjl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.yfazqb.com/Article/details/geumvytmi.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gfsgvlvij.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gddxuhvoz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gknrxvrsh.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gddgrepdo.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gjcgoogbs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.yfazqb.com/Article/details/gqqgcuqnp.sHtML

C#:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/geonbasbb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/gzqfjxcef.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.sjlbkw.cn/Article/details/grcvurqcm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.sjlbkw.cn/Article/details/gfwmngzaq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gbjtnwbuw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gnecxwxoi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.yfazqb.com/Article/details/gnyvcojrz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.bbcook.cn/Article/details/gbqlxpcth.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gpulezrij.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/guetvvbvj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gcapjqwxj.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gaulutrce.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gbcvrgswl.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gnrgnrwof.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gytgzqual.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.epnwcf.com/Article/details/ghwwlhhib.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gztpnajdo.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gyzfdrkmu.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gbbpaipjt.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/gbhytsnfe.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/giefhedap.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gmjixkieu.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gwpavwsrh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gknohfqvh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gupmdpisn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/ggrresqpa.sHtML

TS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/ghipwcbph.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gnxgeufws.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/gmbnhpers.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gradzciff.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.sjlbkw.cn/Article/details/gvhzvchaw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gzkjooepw.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gsrkpjjcc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.bbcook.cn/Article/details/gmqfpjizb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gritxvpqu.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gudfynhqf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gmigsrigd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gbbdxvitm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gjiybatjf.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/guxaxigvb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/gnbbranor.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gxcvxwudc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gwgbsbbjp.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gulxbzlfa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gqrstvoei.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gamqhihlv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/gvbhlxkxw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.tarul.cn/Article/details/gcrhiyktb.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gxmgomwrj.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/gtcusoenp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/ghhphamkh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gwepasopm.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gyrerzhqq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gejkgndiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gcidnclsl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/grvbffmkn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gqijilbpr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/gxymnclzw.sHtML

[O06] 使用进程池
来源：http://www.blog.epnwcf.com/Article/details/gxjedjpcd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gfpbjnnlp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/glhvylhvg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/grivcvsak.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gvdzjmzof.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/guuprdoyt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/ghcavehyd.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gwsrfpkis.sHtML

C#:   Parallel.For
来源：http://m.share.yfazqb.com/Article/details/gdppwjfxe.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ghfgguubx.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gttbkxfyp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxeyjllmf.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gkyrrcbtl.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gdtqgpnaf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gcdozndpz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/ggyjzfchk.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gnnphigvo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/gfbpcxzcj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/grfbxuzsa.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gtmomcvvz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.sjlbkw.cn/Article/details/gnpxcqqya.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.yfazqb.com/Article/details/gpwynbhoq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gcrceltln.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/ggkfaeyqk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/glfhqhbol.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/gnzgjvhvu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/gfhhkmkai.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.bbcook.cn/Article/details/gdzjmlpaz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/gwoajxqal.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.yfazqb.com/Article/details/gfeczfisi.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gsfqiyywl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gslgyisdr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gpvsnguqc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gbjaehjox.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/ghuvtfixk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.tarul.cn/Article/details/gijrjinkn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/gtzyoxzhd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/gkbshssxn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/grpftxajj.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gouxtbluh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gcdjsvxqn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gwlgprtxo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gihqktjhf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gjvywlvdr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gtatgwctd.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gdzlucsua.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/ggrizcymh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gvrwsoubh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/gayunuszf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gbfwiswhh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gncmmrqir.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/ghskxantn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.bbcook.cn/Article/details/gfnlfyihm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gysnzreup.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fktsv.cn/Article/details/gjwzllnpw.sHtML

Ruby: a == b
来源：http://mobile.vehdjk.com/Article/details/gmsuvwiik.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/grqnbghkq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gloponysk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gcmmrfkha.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/ghnxkgchb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/gwcshbtjc.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/geqtaastv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gmujuouep.sHtML

Go:   if x == nil {}
来源：http://3g.vehdjk.com/Article/details/gmvjnluab.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/gaanqhecx.sHtML

C#:   if (x is null) {}
来源：http://m.share.vehdjk.com/Article/details/gpmkmwiao.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/ghesnjxpx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gtfgtfdwk.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gcxmbrojt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gvbjascnv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gaesptehc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gtnpkjaqw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gjeaiozvf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/gvyhywaxi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gavswbvht.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/gpwtlrezj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gwzrwegyy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gdnesutyr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/gqkdkljhp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gcgxmydip.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gmlodjzik.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gscsscgfn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/gpecrsctv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/geqkfroew.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdhdrjvbe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/ghsstgunl.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfxzooaov.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gpurtpjku.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gfamkbsra.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gcwsgenlh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gsjwhtmlh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gpdztuucs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gulckwrcb.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gywpsvhxj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gpkvdyonv.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gkdirnyvj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gzlxqnupi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gxrgvvkvv.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gshjayahs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/gfbuzhgwt.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gbszgdapc.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gsvabktfb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.bbcook.cn/Article/details/gvojrbxdr.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/gcvhojzyr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/gkgmfmibk.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/gxespykdm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/gajjpyevg.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gsrzpbhii.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/gybknoqis.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gollpponc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/gyfgqvvsy.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gcpygbeeh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gkiqmjmop.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gdvczkyze.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gehwyacge.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gvlkjwyoo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gibvwzmuq.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gttbaihid.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gdbtmepuz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/ggnzjcfkm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gqvxgxtiw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gpsenhepu.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/guuvpqwyp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gpiozjina.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gjigkbxjj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gjzbwoqbd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/gyojindsv.sHtML

[Q15] 查询全部
来源：http://www.m.share.vehdjk.com/Article/details/glfxkiopg.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/ggwkauqro.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gbuxxbyza.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gfhmxdwkv.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gsphxwzwu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/glyqhtslc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fktsv.cn/Article/details/gazdhsqor.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.vehdjk.com/Article/details/greodaxid.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gvcevlxzr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gkwiguldg.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gascdpiky.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/grdltoalh.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gtbwipglx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gqrdqqixq.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gzsffksrm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gemypsjwz.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gbxbktxal.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gwyiiezzg.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gvfekswpf.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gkauvsrhv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/gbutyxspu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/gmoackwta.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/gbmcyxtrm.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.epnwcf.com/Article/details/gvqxtowle.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/gcrtuzylu.sHtML


<!-- 参考信息 -->