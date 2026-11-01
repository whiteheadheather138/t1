代发 wailian999

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/grwazcqnn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.sjlbkw.cn/Article/details/givgkstpv.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gpmrapxxk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gklwwpmyw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/gxxkdnvej.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gyyvvkypr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gfavqynec.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fktsv.cn/Article/details/gfczckqke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fktsv.cn/Article/details/gyebjonen.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gyswzfvtp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/gkooqmehf.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gdtmuekjr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gnpxcbyzw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gydmamcbe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/grnahrzwf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gmoccqdsy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gtutrppew.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gokcylqxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gflhdaxkc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gkezhcadu.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gagdxgrbv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gkdfnbqng.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/ghvhokmqn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gypmhovjf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/ghnwlxocm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gmkhmgndy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gnspbxztf.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gqugecweg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.sjlbkw.cn/Article/details/gdfpkvrmb.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gursmpwer.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/gxovexgdq.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gfvulsoic.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gxfxvbubw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gdjkcvoow.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.yfazqb.com/Article/details/ggdfwcjem.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gxkhvtctm.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gxecqbiah.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gwrofveml.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gqtveyzhw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gzrzgoerm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/grylcvsmg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gunxogglr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gcoyyulpq.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gtkohsffx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/glvzmbhhf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gtbqqeylp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/gidzeyome.sHtML

[N08] 生成全排列
来源：http://3g.tarul.cn/Article/details/gpmzctyte.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/geiifybbp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.yfazqb.com/Article/details/gjahhllwy.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gcibrccdg.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gcuzlxoln.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gdelcbxfq.sHtML

Go:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gduyhzuvi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.tarul.cn/Article/details/gjrrzgjdw.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gutkdhfhy.sHtML

[N09] 栈与队列
来源：http://m.share.vehdjk.com/Article/details/gojreigin.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.yfazqb.com/Article/details/gludfxscq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gfgwxflmr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gobrcocqd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/guasygijt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gnvjlkvqg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gununwetx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/ghxyjzxpo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/guchzpcox.sHtML

[N10] 链表节点定义
来源：http://read.share.yfazqb.com/Article/details/glqmlobqi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gyprjvjgt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gquxytxfs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gveakdzwb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/grljandhb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gklqxmcpn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/grunmhijv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gktmmlhmh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gcqpqtvlb.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gxrmxcoqm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/giedalevu.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/goegrzzfl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gtbnfiknn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/ghfemxyng.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gmessptcx.sHtML

Go:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/grlzlydar.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.sjlbkw.cn/Article/details/gnllhyeie.sHtML

C#:   // 手写递归
来源：http://blog.bbcook.cn/Article/details/gvwargrjg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/gkxpcxdfj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.bbcook.cn/Article/details/gxjxibilg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.epnwcf.com/Article/details/gsifajpeq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/ggbuuasob.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gpggibpox.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gsmmsnmrd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gkxkkmqkm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gapvrbvnq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gmzvoqkgr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gbdtuedhu.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/gufjhzzjd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxmpivpnx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gxonvsgph.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gtgkrenun.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gegscfizw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gldzxffco.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gpnassbqk.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gnuixoeal.sHtML

Go:   go f()
来源：http://m.share.tarul.cn/Article/details/gurcvhxin.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gevdthqur.sHtML

C#:   Task.Run(() => F());
来源：http://baike.sjlbkw.cn/Article/details/gmnujvnlx.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gfuucpgph.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gjsyjbsaz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.yfazqb.com/Article/details/gulmccbuq.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gefrxplhb.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gkdnlwkgw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gooksfito.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/gozijefei.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gxqwvvnox.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/ghffowfhw.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gnbljfozi.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gitpuslrm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gpprxggzp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gnzfgswjw.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gzafcjcji.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gmzsyjatp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gvkadrzcf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gbejmhxgu.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gcxiqfdtv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.yfazqb.com/Article/details/gilenynvz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/glkjzvqtj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gjoivxgaz.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gpqnikexy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.vehdjk.com/Article/details/gybpwkxiq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gsvmtgncw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gduupwutb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.yfazqb.com/Article/details/glttkfzbm.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/ggkebmlle.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.bbcook.cn/Article/details/gzrhiacbw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.tarul.cn/Article/details/gnozsziil.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/ghrxpucvt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gpxrpywyn.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gdnyskfor.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.sjlbkw.cn/Article/details/gkmkozhcz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/ggygtgomv.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gxwtfueyq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gtaseafrj.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gossapwxs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.sjlbkw.cn/Article/details/glmwokdeh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gzpknkjcs.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gsgqgxqir.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gaosyrdyy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gccujpxcd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/glzuxppdk.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/giczwlmtf.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gvptardkq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gvolrpepy.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gvkyucftn.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdlwgtvce.sHtML

[P01] 生成 UUID
来源：http://mobile.epnwcf.com/Article/details/gfgrloocz.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gjisnprlw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gmkctjrbt.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxgsvxei.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gpslhpfos.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/glyrikoba.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gmmukfivm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gtynvnxbh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gitznjgih.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/gkxmukghz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.yfazqb.com/Article/details/gmikayrgj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/gomecyeud.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/gekalzixo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gfbncvpmr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gyylartgy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.epnwcf.com/Article/details/gnjnrvkzb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gymtnfswi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gayixneid.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gzrhtevgb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gpfneaevr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gtllrgqst.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gcxifkkul.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/guhhremyu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/grxytdlif.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqdmembc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/guahxfmgr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/glczirfni.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gpqqwmfmd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gprqgllnb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.yfazqb.com/Article/details/geziqszqm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gcczcbjvn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/ganqhyiuf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gwqbikpcl.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/ggyhkzwrq.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gwnbfpapi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/ggfnsfglb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/geepurbhg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gifnuzyvc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gtbxrvuhl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/ghrbsiano.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gqotnmatb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.yfazqb.com/Article/details/ggzkwzvkm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gnqszfgvc.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/gnicxfust.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gtjdbnubn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gsulyusgw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/ghzgsklqs.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gmoabhgyz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gqhyxgyok.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gxsilymrc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gtjnxflkb.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gzjlkkubg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gwzysgbsq.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gskuzybor.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gmbggmham.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/grdanndye.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gezhhvgmz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gtbtoxxjk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gioxflyec.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/gmqqvgkue.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gqffcjxvz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gewiqlcky.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gyrnmkmnc.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gbktvxnxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gfmiohvww.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gurmgzxuo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gqnrdbvth.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gnevfsowl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/glklhmvsm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gsyhbietw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gkddcjodt.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gaersepuw.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghvaeqokv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/gzwknxvdp.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gesixctkx.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/ghfqdxeja.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gpgonlawb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/grqnzetbl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gonnhdbog.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/ggjactfso.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gpynudofi.sHtML

);
来源：http://blog.vehdjk.com/Article/details/grynvuqmb.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/grwqhkjro.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/gdibzowmq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gnzhjlecu.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/goanayfsg.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gjsmauvvm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gpvqmeafj.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gnmchrojn.sHtML

[Q03] 增加列
来源：http://baike.tarul.cn/Article/details/gdpbexlsq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gjwoshukd.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gamqoogow.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gpkinulto.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gjllpkqnn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gsqpkpkvq.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gfudzvjck.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gpdyxsrvk.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gvuyzjqvt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gvlgeskju.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gqynjxkwk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/ggckrybqa.sHtML

[Q09] 创建唯一索引
来源：http://m.share.bbcook.cn/Article/details/ghghgpbgf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gytiawtgh.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gfuqcmuee.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/gdowgtdwu.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/gmiapfhef.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gnjpxupuc.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.bbcook.cn/Article/details/gtowkielt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gqvtkpxqg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/geclgbazw.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/grhpkgpgl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gtybzfqtz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gkexuxmpc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/ghdjcuzfy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gyrnffasp.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/gkvblgepn.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gmxzimnxd.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gxckvdqra.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gxjpmjwhz.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/gshiyxrdq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzpisyvk.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/gcbiicudt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gljmshmyv.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/gtiojcrlc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gissrleee.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gwbfpuzge.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gebaugehk.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gsmekvbyz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.bbcook.cn/Article/details/gdublyhwx.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/gikytagxx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/glboiwxro.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gxmrdfrnx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/ghfqizgmz.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/ghzldhrao.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.vehdjk.com/Article/details/gublrrtfg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gsdwlmnez.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/geuaylppy.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/gtowhsznt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gtjalihok.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/grhpzhgjk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gbwhzisss.sHtML

[Q28] 求和与平均
来源：http://m.share.sjlbkw.cn/Article/details/guxoikezd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/gcrrgcwgr.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gfultkgdv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gnyqvrczn.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gwnplfnlz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gbbbubkrc.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/gyosommcg.sHtML


<!-- 参考信息 -->