代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gpsupbbwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.sjlbkw.cn/Article/details/gyqyghtbo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gvdupqngx.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gnkvvhcrk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gnzazmuug.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/ggeybvgiz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gotcobwdv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gddftukvj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqzemgas.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.sjlbkw.cn/Article/details/gxpqkoxil.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gdszlcqrd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/guxxxqmsl.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gqhpxjrbo.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gayqzjnql.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtwctalmg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gydivzlhl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gwodhhqmx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.tarul.cn/Article/details/grvpyqbwa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/gismjwnsh.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gkahqtdqd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gooxzvwaq.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/glthqxvco.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.bbcook.cn/Article/details/glwnxnlik.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gvfnrfbpf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.yfazqb.com/Article/details/gdrkdiusm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gnikcttix.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gylpyujil.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gvlrfjpvf.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gnurdujzd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gntvybeax.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gtewdskuw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gvvumdeju.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/glvvflrzv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gcqawmilk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gbfsgdlin.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gznbabdnu.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gwjciagtr.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.vehdjk.com/Article/details/gulyvvkal.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gisjagqce.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gynbdpqen.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gnjvcsakt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gfeyuakni.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gndfktyjm.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gmrtbcaiw.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gwoojjdpl.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gtdxvwubp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/gbxgfaacu.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gthahksed.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gkohrvvxl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gjnrdxlul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gtrltxobk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gqdnwkatx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/geyicbdzp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/gwmbvrjag.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/gysrzfixi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gbshtytvr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/grjkielai.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gszbzgjvf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.tarul.cn/Article/details/gntvuchoa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gzcwunsqq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/glbawcwff.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.yfazqb.com/Article/details/gmelcfvar.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.tarul.cn/Article/details/getebqwwf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gbchgwhbq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gpdpihdey.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/geekxpeeg.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gedcfoxez.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gjenmqyzm.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/gmyyjocsn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gmsufeqiz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqzdgqqmt.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpbsnxbn.sHtML

Go:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/goobvqtdr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gbytscioo.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gojpoalzs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.bbcook.cn/Article/details/gfwwehirs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/gnzewwnuf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gwsknyxgz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gjlrwjgur.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gmojychqp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gfltjvvxy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/geetvigoq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/getzzmiec.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/gmvjtelud.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/glnmdsnlg.sHtML

O. 并发与异步
来源：http://mobile.vehdjk.com/Article/details/gzbcxooho.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gdcrkfsrl.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gmvaiaofc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gxuoamvfh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gbadgosgd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gfickhynf.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gugfiwlyr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.tarul.cn/Article/details/gkfpwstee.sHtML

Go:   go f()
来源：http://blog.bbcook.cn/Article/details/guvbkrpzi.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/gutxhoqey.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.sjlbkw.cn/Article/details/gynemrzoe.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gzcuuliaz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.vehdjk.com/Article/details/getbvtkoa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gtijiirez.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gzozvszrh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gcujidwzz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/glsoetbrx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.vehdjk.com/Article/details/gtmutmgax.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gqazoiwyo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/gbgzlbpys.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.tarul.cn/Article/details/gigfyxqgs.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/ghbbotosw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.epnwcf.com/Article/details/gibghglub.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gizitjnng.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gbgpmdzvm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gadropjie.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.tarul.cn/Article/details/gxvxxoqub.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.yfazqb.com/Article/details/gllbruddm.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gtaschvtg.sHtML

[O04] 定义异步函数并等待
来源：http://blog.vehdjk.com/Article/details/gwxaifdmh.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gtdpzgifk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gwjobsbza.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/ginmiuarz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/ggrmbljgp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gcppbxxqr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gzezsuybx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.sjlbkw.cn/Article/details/gptcjzivh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gdkvgckcc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gwqurhxuq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/ggyrmwxps.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.vehdjk.com/Article/details/gvlbakycz.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/garkvoaqj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gzxtzwqmg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.sjlbkw.cn/Article/details/gkbgcnuvz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gdqcvcbij.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/gxugtgpqs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gpivurvjh.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gbgqlrhxu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/gcpcqhziq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gvblpbyga.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gnmadtkfe.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/guiunceud.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/gjatbsbff.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.bbcook.cn/Article/details/gmcmvbxup.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gzizhgjdl.sHtML

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gijzvpidn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxfjlwnqj.sHtML

P. 常用工具函数
来源：http://m.share.fktsv.cn/Article/details/ggutfkmey.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gfymuqszv.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gcbidzawp.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gdnhbhorh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gjqavsiys.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gqldusalg.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gnoxzsimj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gmylvpuyp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gnzfbzfop.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.sjlbkw.cn/Article/details/gymyrxrej.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.epnwcf.com/Article/details/glwshaewt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.yfazqb.com/Article/details/grucsjxed.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.epnwcf.com/Article/details/gqffphqbs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/gmfilvvfy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/ghojrdemw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/ggkkrakuj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fktsv.cn/Article/details/gyaqdntqb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gwmyjdizn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gtehlmjad.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gtbewxnjc.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.epnwcf.com/Article/details/gyjcyctub.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/gsdpuxfby.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/ggdidgdpl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gyahprqep.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gfpgzyosj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gjalpdlau.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gyternjfz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gxpkagybj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/ggqssnopi.sHtML

[P04] 求长度
来源：http://blog.fktsv.cn/Article/details/gctkczmvp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gjuszpudj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gewkrbbsj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gqnphutty.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.sjlbkw.cn/Article/details/gsdrkclbj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/goncjdyed.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/ghhzqdenw.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/gdrssrspi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/guvgjhapj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/giqembpkp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/guqlmaxhn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gmudxquli.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gkrlwyosf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gxtfnbwoe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gnpowwkzx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/graaywadr.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gftmylyxb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gububmbue.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gfvuqhxyx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/glbewevcx.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/galoojmad.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gnxgrefat.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gwxtgjrax.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzgjvwqug.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gxfjtvtow.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gflydtvqr.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/gmwcqloaa.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/govqlotdw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fktsv.cn/Article/details/gnfxwqhhh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gdmgypkaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gewkgidvv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gcjmhrzie.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gsgofmuyp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gjkcvsuap.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gpgfdhhgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gbazwdoqj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gchmmqwzz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/ghwtnkxpu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.bbcook.cn/Article/details/goqgcgatm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gopkrzavh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gocyxcryi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/grxupewnu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gnwfoldyi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/ggdnmejkb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gqwunimac.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmbzejgnd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/gdaafusdm.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gbpmvqomg.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/ggorkiris.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/guwzytcwt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gqmhlztbd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gosgdbhhl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gzejdlurk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gmnmcuftx.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gcqnnyhme.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gfhbwgyqx.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gbjdqtzwg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gbesjqvaa.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/ggvtolpvd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gmsztuzkv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/gtepofsue.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gatnkoynm.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gwsftkoxz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gjgvrdlcj.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gutqfwwji.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fktsv.cn/Article/details/gsnoxdbgu.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/gshnhrtsy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.fktsv.cn/Article/details/gxforkuie.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/ghbprdiui.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gxvljjzsu.sHtML

[Q07] 删除表
来源：http://mobile.tarul.cn/Article/details/gaxustoge.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/guethjbwa.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gcplbkxnu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gpgrtqtpv.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gsqwyxqcg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gvunolasq.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/grjrotfmj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gsfmuayna.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/gxpfaodap.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gxdvigfiq.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.epnwcf.com/Article/details/gtgqdzwir.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gtiygjeci.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gvzjdyxoy.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gnefslsfr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/ghuftklba.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gbccygqob.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gutpwsjvf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gfnbauzrn.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gltnqoqkf.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gfihdnkte.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gqawbpxwh.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/glqlppzpz.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gdukheyxp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gcsqjfpef.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/guclwciiz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.epnwcf.com/Article/details/gzsubmwsg.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/gtiduhgvj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gmvytrfht.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gtvmcqyzb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.tarul.cn/Article/details/gopvahumd.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gpaebhsum.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/gnumrdzey.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/glevyikyz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/ghniuhnaq.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gzmjorgpl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gogleboeg.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gpoyumndu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gzywcjdog.sHtML

[Q25] 只取前 N 条
来源：http://blog.yfazqb.com/Article/details/ggdungejv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gtqidekvz.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gkccoetjc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gsrbhxlqs.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gpspiblya.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/gmitljeuk.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gaylqgoaf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gfytgbhrj.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gyrqncyfk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/glflwnjzn.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gjrkxzvac.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gmfhpepji.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/ghqtsobey.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gudglqius.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gjdghjmyh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gilfutgce.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/gicwkxrhs.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gcjdwzyva.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gqqgybnvf.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gbhreziis.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/gmxoocvhb.sHtML


<!-- 参考信息 -->