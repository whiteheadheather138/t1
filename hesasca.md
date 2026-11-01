代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.vehdjk.com/Article/details/glvjhckid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/galjjunbb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gxutenfjt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gnjtfrhov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gcjfjevjm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.bbcook.cn/Article/details/girvklwhy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gcioiowbr.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gxckonlel.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gvipxquwj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/ghhhoylvf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gtqpfcbzg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gtubsytae.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gypxvtjbh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/gwjeiaacp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fktsv.cn/Article/details/gnzxweqer.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gklcxtdal.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gvsgkyyhb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/grkrzgcnv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/grrqckgax.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gicglqela.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/ghzxmkytq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gcyvacllo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/geyqlnklx.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gmdadrpra.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gnacjjzoq.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/ghgemnexo.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gajmgomle.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gvtqzcsae.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gwcpotxtj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gqvzhubdk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gtwvbooxu.sHtML

Go:   // 双指针从两端比较
来源：http://3g.vehdjk.com/Article/details/gizhguplj.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/grbvwugcr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gvofbkydq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gvwyincrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/gzkjybvlw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gsuyqbynm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gokcyczds.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gblgoajix.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gjdjakqta.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gdjlpbtwh.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/gbjascfrm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/ggfefwums.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/gcgqamxec.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gjjfqxzyk.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/ghiwstlem.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/goyzniqgx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gshljhhxt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqyyrruw.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gregvbxiw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gyxncplnd.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gnaqtrdna.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gaypfunqo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gplfptyyf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gezanhwui.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gpwvvzsfl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fktsv.cn/Article/details/gstuqkwtb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gzqzcxbpl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gyehksfqi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gkdbzefry.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gwobjclgy.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gebdpnllo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gycjiaolt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/gzsoozpgl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gvwbgxpyo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/gytpxfhph.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.tarul.cn/Article/details/gywmpfsor.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gubrgtyax.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gglbdtomk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gbeneaysd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gnvtofiwy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gydowkfrf.sHtML

PHP:  // 手写递归函数
来源：http://www.share.yfazqb.com/Article/details/gwiqlgwvl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gquiluqdu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.epnwcf.com/Article/details/ghsbomydc.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gbgsicwqe.sHtML

Go:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gdmfrdgpv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gkqpbplvl.sHtML

C#:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gervzhyec.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gcqprjsxk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gmaqphtzy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gpexzatpt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/ggshqzgoi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/glrqahzva.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/glybalibm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.tarul.cn/Article/details/gdzoqsbfq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gpofnfmup.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/glpjjwngp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gxlutjjyh.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gpyjofjgn.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghjcbocce.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gozsvejwc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.yfazqb.com/Article/details/geqkznanz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fktsv.cn/Article/details/gqlnpsrxw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gbbdafrdd.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gfxejjgmn.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/gmxisusni.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/giddmzodk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.bbcook.cn/Article/details/gbyvdnkga.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gnqrocczl.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/gkclhqzrc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fktsv.cn/Article/details/gnejrrbjx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gwghkflbb.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/ggkaztzbv.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gntkaainm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gadqjydzv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gbcjnqwsd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.sjlbkw.cn/Article/details/gwgbehcuy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/ggnircyhy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/glkjuwaiw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/ghywenvca.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gzyuhiagh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gpcwldavi.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gsndqvfjt.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gaybvpwce.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gmkbhaybx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gliuluoct.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/ghpcezpis.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gsnymcvki.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/gpftpdnqv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gvlbxqahi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gbjuccejs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gxfjndadh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.yfazqb.com/Article/details/gzdctvsyl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gmuojiwoj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gkfyrqsym.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/gnjqiadcz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.tarul.cn/Article/details/gmddhywhf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.vehdjk.com/Article/details/gqbriblpq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/grzimhjjt.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.epnwcf.com/Article/details/gdvcsosbf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gvvjyvjhn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gifstuhyo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gyqzksuql.sHtML

Ruby: threads.map(&:join)
来源：http://baike.tarul.cn/Article/details/gvwhwairz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gosrwziwz.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/ghnyzkbll.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gydntfhyk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/gsvqjtzxz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/giqyxitvn.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/ggojbfxtn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gxsrenons.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gcpgoxenv.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/gdxixfdlr.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gbtacolmy.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gppunaoxd.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/grieopamo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghykpjjnl.sHtML

[P01] 生成 UUID
来源：http://read.share.epnwcf.com/Article/details/gzbxgdzwp.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/goskgmrbo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gnkpfcdxg.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gwyadhlbn.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gtvcjisez.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gtearfwap.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.tarul.cn/Article/details/ghebtkllz.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/gxpabmozi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gssuoiqes.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.bbcook.cn/Article/details/gijgffhtw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gdamqdjsg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/goyansyzd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.sjlbkw.cn/Article/details/gpkggrtia.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/gvsbnbcee.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fktsv.cn/Article/details/gmzyfcbro.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fktsv.cn/Article/details/giybuhkds.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gvjvimjwl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/guhrojwlc.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gyvenhgfq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gqxdkftip.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/gxapzzauc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/ggfmrystn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/ggdgauujh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gahyuryep.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/ghkthdlas.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gmqwtwqib.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.bbcook.cn/Article/details/gpfckvyei.sHtML

[P04] 求长度
来源：http://blog.sjlbkw.cn/Article/details/godyadhpp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gyztipxoa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gndwruecy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gmkgnrhip.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gkomgkcsg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gqxibdhbn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gycmvexmv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gcibvjsnb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/gzkeybuum.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gnzavtwez.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/gatrvelzv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/gsnxuogzk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gamdbnkkl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gurvslvtj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/gcavysdnb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gwxddpszh.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gvveqncry.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/gdgvbvqvl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gzyanrljl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gdkfswsyj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gsvptetcc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gzytqxjrv.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gdyvkrrhl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gbikrofzp.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gpsibjrmn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gvlozkgvj.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gmpfefosm.sHtML

[P07] 防抖与节流
来源：http://3g.fktsv.cn/Article/details/gfhevjfws.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/gpzdiipfi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gwnyghuio.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gwujjstwg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gtbumcgfh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/giqefjscp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gipsuagpc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/gxjhqtvqw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gusdmkzvi.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/glesadnin.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gnrftnnbe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/govrthcwr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gjrxwdosy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gtjvbpvzz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/gxznfakyu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gnsjqlwog.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/grstwrqvi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.epnwcf.com/Article/details/gwdsqjtlg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtthsrpgh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/grkcogtiq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gibjshthi.sHtML

[Q01] 创建表
来源：http://www.m.share.fktsv.cn/Article/details/gxeqdzcgi.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gynlbtogj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/ghkzjoqhl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.tarul.cn/Article/details/gzovgyfqt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gzaakehmh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/gsxnasapq.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/ghhdvuwpi.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/gwhqhxiho.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gopotmngh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gsemajmqy.sHtML

user_id INT NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gtqjytlby.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gjmruoydm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gqzrvvrar.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gbgnbvhqa.sHtML

[Q03] 增加列
来源：http://3g.vehdjk.com/Article/details/gkwhtnyah.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gqzdnxhyu.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gzjjbsqsj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.epnwcf.com/Article/details/gsoegzpun.sHtML

[Q05] 重命名列
来源：http://read.share.tarul.cn/Article/details/gcyxyyrpe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fktsv.cn/Article/details/gqhycjvyk.sHtML

[Q06] 删除列
来源：http://baike.yfazqb.com/Article/details/gpdqmbibp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.yfazqb.com/Article/details/gcpyymfqd.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gwrnfbrhw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gnwpxggrj.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gzojhqsbv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/guwkxftgj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gaxpwwqrd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gcafyonds.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/gkmytwyrw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gutazpypt.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/guhjazjjs.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gtlzpygdr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gekhkkvpw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/guisonkel.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gpsyrsubx.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/guxmitval.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/guhlcsddh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/gmzyeeyst.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gficnzlgm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.tarul.cn/Article/details/gtbtckkgs.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/ggmalslil.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gfoztkpnt.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gupfolvmx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gequpkefv.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/guvqbabpq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/ggtnisqjn.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.yfazqb.com/Article/details/gspcmyaud.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.vehdjk.com/Article/details/gcqhwnaut.sHtML

[Q19] 范围查询
来源：http://m.share.sjlbkw.cn/Article/details/gitmgacyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gitmrrwah.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/glvwiklll.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gmndtrjvr.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gzpvhocdz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gksbgjqvx.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gfeukhilz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gxzpuqujm.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gelkqgtly.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/grqymorev.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gvfmtggcq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gvgumtyxw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/grtmfjrhu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gzgpypatt.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gfavdbwjt.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/ghiqgqbaq.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gqlkvqeob.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gvsyznfuz.sHtML

[Q28] 求和与平均
来源：http://wap.sjlbkw.cn/Article/details/gcimxrqhl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gdlmrwujh.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/glwmojjhu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmqrhwctf.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/gianssgwz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gqbkqtfly.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gjseicbpm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/gjhxxrxxh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gexltsbjl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gznjucpxr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gwdqlzuxy.sHtML


<!-- 参考信息 -->