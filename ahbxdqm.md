代发 wailian999

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gjflezapp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gwaaazahf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gunyrztnj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gbtyubcaj.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gqogloebs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gmoxntcsc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gxdyueodz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gjmxnszax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gotxysavc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/grmzjohzh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/ghhezgeer.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gitmziszw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.bbcook.cn/Article/details/guvtyxaik.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.epnwcf.com/Article/details/ghttqttif.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gwntcanbl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gwhjzpwin.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gbexcqmvf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxzyfzyn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gxqoejfse.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gkhuvjogm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gyqzkeihs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gmwebjanl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gaafryhdx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gycuuwsgf.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/ghvpqgopw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gshdulsfc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gcyfkdswv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gdzhrqhwn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gbemdfaun.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/ghnlnrumf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/gmjslveug.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/gfglpnsta.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gkkocqxxu.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gtvknpccq.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gzhphaaqo.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.vehdjk.com/Article/details/gchlsuxhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gwrbetwqz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gjilsmlao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/grnhwgwdv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gaknbybse.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gpycmvgqp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gwynzroso.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gjvffkyoj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gisguubbp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/ghvzvpzca.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gowmvkosl.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.sjlbkw.cn/Article/details/gzennyjqj.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gnicvoyqd.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/glspwxzwy.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gnqmzqcbe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/ggrnbqtsz.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gydmeoyba.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gymuwmpuv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gywbxzwux.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/glkfzgadd.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gmutmpicz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gcjfyamaa.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gbyhsoylo.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gbmxzahgp.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gtknplalo.sHtML

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gtjfyzyqt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gonloywyo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/ggyghhetw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gbpvgajpu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/gbldvpbgl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gvdtmowvz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gktmmqvau.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gtlpcppar.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/ghfwrxyyk.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/gpdxxfdrg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gbiqahfzh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/guhlcquqa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gmsywvzqq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gqgdqlfvx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gimtuikka.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gcodbswnk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/gwkkdhctx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gxhnrwafe.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.epnwcf.com/Article/details/gnjpdfrju.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gzweunlow.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gxrdjnzyq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/glljgkmyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gmsppkgqj.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/glkbwkskl.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gwpokqozf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gflkmtsaj.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gpoyoolvx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/guyftfwwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gnrquutdx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.sjlbkw.cn/Article/details/gqnalqyuw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gitedgvyq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gnmkyjaxj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gwoywtzdt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/gccsjosur.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/grhximdmf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gyrgltzsr.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrwhhmbg.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/gwfcmvaoy.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gswbfscds.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gzcxttcvc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gnnnixsdi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gepdsatpl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.sjlbkw.cn/Article/details/gtkeqgrso.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gbyhvefow.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gvprzgofg.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnozpxsks.sHtML

Ruby: Thread.new { f }
来源：http://baike.vehdjk.com/Article/details/gkmsahfyx.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gkqybfhep.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gyefgpaqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.yfazqb.com/Article/details/gvryrirku.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gtgxclaho.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/goylraios.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gtiokiejh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.epnwcf.com/Article/details/ghksyijcr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/guymyeqkn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gqzjfcore.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gzrscpovn.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.vehdjk.com/Article/details/gkhlsknek.sHtML

Py:   with lock: shared += 1
来源：http://m.share.sjlbkw.cn/Article/details/gxagydgqg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gesfeqisg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/gpmxlwdes.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gnwzmzjzy.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/ghjvjdowu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/glklcwhbo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gklfsyjmo.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gyakppolg.sHtML

[O04] 定义异步函数并等待
来源：http://baike.vehdjk.com/Article/details/ganeqjatr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.vehdjk.com/Article/details/gfjfbdwno.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/glarxjhqs.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/grexezuza.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/galcyphcs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gydumhmku.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gazwjoawf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gutennkba.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fktsv.cn/Article/details/gtaggvcpt.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/ggcigwghu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/geafwwlgb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gefpktsin.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gmaioanka.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/ganlwsvvu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.bbcook.cn/Article/details/ggmxdfbhm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.tarul.cn/Article/details/ganykksif.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gxhdxjntq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/grvfqoxpa.sHtML

[O06] 使用进程池
来源：http://baike.fktsv.cn/Article/details/guyqtqobf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.vehdjk.com/Article/details/gbrpfajvb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/giheoocee.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gdzyfxeqb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxnffbuh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/guiztcfbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gmdeqmgus.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gkasmqoco.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gerysxhdd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbukkknlx.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gkudxzvfc.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gztahitza.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gkopbqotb.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gruwgamxt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/gzjmrwtzn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gfhrixemq.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gamudeeph.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gkcuwrmjt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gnjpkerqh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gnzcnvcpt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/goejdtjoj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/gqcthwtin.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/gfdysbvfc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gabxczfuy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gmnujvksq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gdxtjjefb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gzeplvwkm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.epnwcf.com/Article/details/gcgbfzunh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.yfazqb.com/Article/details/gqdgmidmw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gnmcodzpo.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gkenosnbt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gaaywkdpa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gozhfjalw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gntsyikih.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gdimohvlj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/guqatkzxh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gihzozsji.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/gjwfukoqf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/guwxzxmvf.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gerrahlgx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gitpvhhqo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gywfouxtu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gpwnedmkf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gebqtzknp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gnanatomj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/gcrniccui.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/grokqixgt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gbjpqkoim.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gpaumcokz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gvppifssl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/grrchqvbr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gvhctoggr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gqtqzujwe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gryukxmql.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/goenvkmfy.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/ggydgikqd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/ghnajnpwa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gmphltlmh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gugpfpteg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gqscaqdpg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.bbcook.cn/Article/details/gvztltfan.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/ggeeveefo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gjdsrdjru.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/gpgryskgs.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.epnwcf.com/Article/details/gvddgeqkg.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gnhzqwbso.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/gzxcxawdp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gcypkwbuw.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/gejtclwnu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gauelojuu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gazsnvpes.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gkmjsqajd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gxhgzdgbt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gcinyacma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gkyvwqgzj.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/goxgexmes.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/gxewnmwcl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gyejlkdig.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/gmdimlfuy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gpupvkizw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gxprvlawq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gtlxdudnh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gfrgcznrr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.yfazqb.com/Article/details/grzmvxgpl.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbapuogks.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.sjlbkw.cn/Article/details/gfkagucmq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghqqvpwjj.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gndibzzac.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gqblwmkei.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gyvielmvm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gwzwligwl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/girerxlvu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gqjwucysm.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gxdvxkcsi.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/ghjzyhflz.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/gvvjobesy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gtvxdjqjs.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gwyljpjuv.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gphdiftlf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/gumdapbxv.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gqgwmrjcv.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gwemgoojt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gfzrjdzue.sHtML

[Q04] 修改列类型
来源：http://www.m.share.sjlbkw.cn/Article/details/goemmylte.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.yfazqb.com/Article/details/gpqavgxcm.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gpgkijpvl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/ggvkbkyyi.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gtdllmzoq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fktsv.cn/Article/details/gctcosxud.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gpruskxxa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/gocsldppg.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gqxofzyvb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gfwifqjpz.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gquuvazij.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gabwdftlm.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gzqcjxpxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.bbcook.cn/Article/details/guxghfqgx.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gmweemmpo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/glrgfvvcv.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gxubikgyc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.yfazqb.com/Article/details/gqqnghpto.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gxsgtrwyn.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gdyotyzye.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/genrvyswi.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gfcxnvmmr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gdzqioumu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gsjiwmlww.sHtML

[Q15] 查询全部
来源：http://www.m.share.tarul.cn/Article/details/grxufrnal.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gniuvfklf.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/gqwatuvsz.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gumwotcoq.sHtML

[Q17] 条件查询
来源：http://www.share.sjlbkw.cn/Article/details/gulgagbug.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/goslnpvdr.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gqghiqetv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gxugndznq.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gbnbuoikq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/ggijebcvt.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/ggevhmfoe.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/ggmafztql.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/ghnpjdcxb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/guhiypkqn.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gjmknulwj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/guwjznprn.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/gdplajmzx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gsblwkuuc.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/ghpdgqzzj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.epnwcf.com/Article/details/gecgrmlvu.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gigjutqyw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/giuielpmw.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/gueyeclyv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gkevcheut.sHtML

[Q27] 条件计数
来源：http://3g.sjlbkw.cn/Article/details/gqlmzguci.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gnzmrcycw.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gatusaobt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gbkqbpvuo.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gdvlnemxk.sHtML


<!-- 参考信息 -->