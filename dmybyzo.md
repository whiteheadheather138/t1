代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://blog.bbcook.cn/Article/details/glpqbjhfr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/glvgjlvox.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gkrnqydat.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.tarul.cn/Article/details/grttqcvqp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.yfazqb.com/Article/details/gazfvhcaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gblfhsosv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gpodqjluj.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gogqzuygd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gpwxyfygd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvygsusoh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gpewzogdx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gmnocfxyj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gormtjbcd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.bbcook.cn/Article/details/gjdeztpxp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gbpaibntm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gephpzklg.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/ggtzqszkp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gquszaokw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gfpetxpow.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gdcmpkqln.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gzbaviezd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/glaxuuadb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gycgtkjwo.sHtML

Ruby: a.gcd(b)
来源：http://blog.yfazqb.com/Article/details/gfhfbbmah.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gadlqyjtj.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gymnsfdjo.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gyoghlzjm.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/ghllzckai.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/geuujzrnh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gyvjllmvx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/guklyvrew.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.vehdjk.com/Article/details/glchlfvaw.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/geyhvzxxf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gpxfapddl.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gxtarvjfq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fktsv.cn/Article/details/gxaklvlxp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/ghpidmddc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gyjhqpxlh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gngghseqh.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gxvdrjiel.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gwznazpal.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gjucdvcff.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gjkdxchyn.sHtML

[N08] 生成全排列
来源：http://m.share.bbcook.cn/Article/details/grbgssiqy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gtvsonhkq.sHtML

PHP:  // 手写递归交换
来源：http://m.share.sjlbkw.cn/Article/details/gzogvryei.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gahieenkl.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gwjkiynus.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gvnftrjlr.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/ghjsodcih.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fktsv.cn/Article/details/gjwmsglhx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gxkezfmft.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gyczotudv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gwusxgeaz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gbjrzgubc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gdtwcgoez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gappswbha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/guftxqbbk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.bbcook.cn/Article/details/grgaejelz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gggipntlf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gdtxdltez.sHtML

[N10] 链表节点定义
来源：http://www.m.share.bbcook.cn/Article/details/gjzeehbsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gxcdjjsmu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/ggbzzpcmd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gftqhrppg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gauybsrer.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.yfazqb.com/Article/details/giajloyvf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/grfscfniq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/guqvopylp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gtfaaidde.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/goqtpatln.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gslnzhvzv.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/gkkcmlxzp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gyebqllbn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/glspzhzxf.sHtML

Java: // 手写递归
来源：http://wap.bbcook.cn/Article/details/ghsraploy.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gjodifaif.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/guudirpzm.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gtijholxw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gvkcjiyti.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/golgortrs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.vehdjk.com/Article/details/gyzpkndpt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gomufmuqb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gkiicttjn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gsgzhzedw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/giunqfksy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/grzzjhsrq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gvtefztyr.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giiqjajuu.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/grkvehcpk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gihcymhcg.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gdlseahta.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gvbpvvhna.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/gdnydnudr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/ggjkozdev.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gjipazzux.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/ggwjnvqsg.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/ghxlgbums.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gfzgjscxr.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gjvtsndln.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/gxfxoseho.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.epnwcf.com/Article/details/gsfhpswly.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.epnwcf.com/Article/details/ggavuyrik.sHtML

JS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/grfrtwfrl.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gesgwqfpq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gqrtsebce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gtlmafwdy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/gbniskohz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gimqgjbhb.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.bbcook.cn/Article/details/gblkhnsev.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gncbryxqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gkkuhhrov.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.vehdjk.com/Article/details/gfmnsxtry.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gfokslarv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/godmxyinc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gktbibyit.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gelieqvde.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gekzbravk.sHtML

[O04] 定义异步函数并等待
来源：http://3g.sjlbkw.cn/Article/details/gxabdvfxz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/gujyqizis.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gzehdszrv.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gomkhoshj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gqtxkzopo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/golkvtrhv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/ghfheccil.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/ggqzyvteo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.yfazqb.com/Article/details/garszfknb.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gcmqnadmk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.yfazqb.com/Article/details/gfhyfcjhb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/goptpgfxv.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gxbqnpnhx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gihhbkmqd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.tarul.cn/Article/details/gvkcxukvp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gmstouhqh.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fktsv.cn/Article/details/gwrmxiaof.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.vehdjk.com/Article/details/gabrzazdw.sHtML

[O06] 使用进程池
来源：http://www.blog.bbcook.cn/Article/details/goxkihjcy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/glondcroc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/gickvgfla.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gpzoiddjs.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gkbjfvwmv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gmucsyohp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gitrozfcu.sHtML

Ruby: // fork 块
来源：http://www.share.bbcook.cn/Article/details/gnbmawskd.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gvaoqzbmp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gpkxlqilx.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gchufluar.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmqlnmoyi.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gcqfvhbgh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.sjlbkw.cn/Article/details/gjuxbiros.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gmenycblx.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gtpzhdcxe.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gtojxsumj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gocetzmhi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gbiphahfh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gizggudlf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gbnigzvjm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gdkrjvahp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gnjpfvgrs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gjmusozfn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gemgkuqzj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gccfqdbop.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gtipekspd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/gfytughfs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/ghpqkkipt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gxekobpaj.sHtML

[P03] 生成短随机字符串
来源：http://mobile.epnwcf.com/Article/details/gxlvqndan.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gsfqsttrp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/ghwvqfata.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gcydurewz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gdhojyzsq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gsubppebq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/gjavmorxw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gvfuygisl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gdjfjsxef.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/ggyadhefg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.sjlbkw.cn/Article/details/gzjmyxomh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gtayqjgun.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/glahvhvyl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gvtcdklgy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/ghhybgcju.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gatsoiafo.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gfnrzpvut.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/golbxcrbl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.vehdjk.com/Article/details/gtxiycovk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gxhhlavmo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.vehdjk.com/Article/details/gusxwqjou.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.yfazqb.com/Article/details/gdjqoddnz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gruiefrdl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/grehgpioe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.sjlbkw.cn/Article/details/grsluzmdn.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gqsmydqgo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/ggknwczvt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gegypuegt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/ggxbmvzuu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/gqecccqah.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gptxtdjqm.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gkunptpov.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gqnoengeu.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gruxjbusx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gniofbkol.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/godwueosg.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gkhgxbqit.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gpmvrzcxj.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gsrioskfa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/ggurwrhtb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gqzpvzjuv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gjdktsnky.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/guzvcvygf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gjzomqpui.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gdgsxvcnx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gfgwkaqfk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.yfazqb.com/Article/details/gcynhgaij.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gmwmktali.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gdcjtjkjk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gnbzzvmeq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/ggmsnmegj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/giahrdssr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/gvsfeiccz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.yfazqb.com/Article/details/ggrkrofuk.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gcapichmd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gaicpdqzl.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaguxnggm.sHtML

[Q01] 创建表
来源：http://wap.vehdjk.com/Article/details/gcysodjxz.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gtptyehdh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gjntkrowg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gcfoenszr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gktdzawve.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/gsubagetn.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gldknqbag.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/grnykuxrj.sHtML

CREATE TABLE orders (
来源：http://read.share.epnwcf.com/Article/details/gplsoiwko.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gbmqhnlic.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gonpxxtra.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.sjlbkw.cn/Article/details/gohoyntae.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/gekvhsubw.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gppwqjwhz.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gfsoulmxn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gabxeszhs.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/grhlcqckb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gqzfbbbau.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gfsmkdfej.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gtuzovzrg.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/giguuwqfk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gnjgugonl.sHtML

[Q07] 删除表
来源：http://3g.sjlbkw.cn/Article/details/glclwgirr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gilcetayv.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/grsrwawed.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gkzykivok.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/gxwncbqzg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/ggvcjybec.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gzeybxvua.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/grdmpzgih.sHtML

[Q11] 一次插入多行
来源：http://wap.yfazqb.com/Article/details/gztyyjuni.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.bbcook.cn/Article/details/gqwuptddw.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gemwfjycw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gecfxnatg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/ghokonhsj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/gwsvnkvma.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gbdqfauqv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/gjgpurucd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gtinckbex.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/gbbeliwxr.sHtML

[Q15] 查询全部
来源：http://blog.tarul.cn/Article/details/guzszhnku.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/gggoufgbb.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gfhrpaujb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/glqrdooru.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gznamuuez.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/guqgpqvwm.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gwvbeipqh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gtznyuhzk.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/gxipmwtsz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/grwkwosgu.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gmixtsdys.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/gpilpwcxa.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gugkieqiy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gilqlipaj.sHtML

[Q22] 排序
来源：http://3g.epnwcf.com/Article/details/gtdualosa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/ghjwhpepc.sHtML

[Q23] 分页
来源：http://www.m.share.bbcook.cn/Article/details/gkyozdqeo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/gttgndqlr.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gpqgwufes.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.tarul.cn/Article/details/gfumnuujz.sHtML

[Q25] 只取前 N 条
来源：http://baike.fktsv.cn/Article/details/gdgvinnhs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/ghrwcbkri.sHtML

[Q26] 计数
来源：http://3g.sjlbkw.cn/Article/details/grgkwqpqy.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/guzppltlo.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/gjefzaank.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdwmymapc.sHtML

[Q28] 求和与平均
来源：http://baike.fktsv.cn/Article/details/gziggoobp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gilcgmncs.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gucylpqxo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gtdneixbo.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/goqwhotwm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gpxfvrlvr.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/ggmbvpmsb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gktmuliwu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gtqzxpcsf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/godgfvait.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.yfazqb.com/Article/details/glkblqsxj.sHtML


<!-- 参考信息 -->