代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/ggpfhcevt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gobavnlys.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/gyolmqjtm.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/gigcoxpur.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/ggfaijftz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gjxocewji.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gtvfdxyka.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/ggcvjjcvo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gjunmxfeb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gnpobkzup.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gozfywgko.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gtkvxxtkb.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gtzqdojqb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gvphaojnx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gyeuzluxx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gkqjnfvaf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gkofvyizk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gwwloivhn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gvclftfgp.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gmajdjzud.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gfavbnngy.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gnrpcrhqg.sHtML

Py:   s == s[::-1]
来源：http://www.share.epnwcf.com/Article/details/geogfisdj.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gcqpwinto.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/ggmwmdmpd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gegspsykt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fktsv.cn/Article/details/guakkxixx.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gjglllddx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gmooqglra.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gxihdvsow.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gztotydvy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gbvvothlz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fktsv.cn/Article/details/gwfdslhuk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/gyidjrtwq.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/ghntnsfao.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gnjabjxfp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/geovukxht.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/grmemycie.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/ghsykpdif.sHtML

[N08] 生成全排列
来源：http://baike.vehdjk.com/Article/details/gniphrbvj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.vehdjk.com/Article/details/gnlhrwxos.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gzxqwluzf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/grkysgtao.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gdyavfyjs.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/ggrsshsvw.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gytkoprsm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.vehdjk.com/Article/details/gkqpxzbgo.sHtML

C#:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gszpoeyig.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/gopnmrjgi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gfhyrikan.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gltusywod.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gwghserzl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gksqputfq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fktsv.cn/Article/details/garqjjfyr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gqddsseoh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gahocgozj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gzcmgwupj.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gebrhyeub.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gdclffqzg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/gymxybmrx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/garedsvjd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gbayizcri.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gemykzpep.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gpnbysxvo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/glfwdhodf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gqipbkxvi.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gcgtwcznu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gaflzohsd.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/gkhxwklwl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gpcyblomv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gwqoiyzbq.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gjniorjtj.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gafstobpf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.tarul.cn/Article/details/gbdghdkdm.sHtML

C#:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gxyimcmui.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.yfazqb.com/Article/details/gkpcnkroi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gfocixrpq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gemvioego.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gjyljqvdu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gfjiigvga.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gnneaexqz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/giqwgqqwv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gbpjocven.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/grtrqzwma.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjbfzuhia.sHtML

O. 并发与异步
来源：http://read.share.vehdjk.com/Article/details/gcepodapq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbzsroudb.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/garekorpj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/guskuwelo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gfbavfxij.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/ggaxmleow.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/grjsptkng.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gchmvgjvj.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gtmcamnmn.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/gadbdruit.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gfeilmmnl.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gucclapxn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/gxdbksnto.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gerkqyzky.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gjiyoxqyn.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gslxisfmh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gxatzzlrf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/ggoszbhgc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gneodjylu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gjyaxyeqc.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gpdjynwue.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gsvpovlnl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.sjlbkw.cn/Article/details/gpysoniub.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gvonadica.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gsmluzvke.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gtlazjakj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gxsvuqrxt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gfyhfwqxk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gwoqsinnb.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/gkcjsgihu.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.tarul.cn/Article/details/gokofoszs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gpzfwpqzx.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gucswwrwe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gcapzsydw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gzhdiimrq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gfxdjwngq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fktsv.cn/Article/details/gwyyjqtir.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gbtwdjnpa.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gqnyxhoxc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/gqncnmaum.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gumizfelr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/gmhmahjfa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gnxxmwxsz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gxovlcoki.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.vehdjk.com/Article/details/gsxknchyr.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gntvjsrbd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gxvquqfnl.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gptmbohrn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.bbcook.cn/Article/details/gekurhaki.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.vehdjk.com/Article/details/gldzznypa.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gbqzxabga.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/glbxsmrsq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.vehdjk.com/Article/details/gsubtrlno.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/gsixhyafu.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gmxnilzrq.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gvcowehvh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gsurbdqzi.sHtML

P. 常用工具函数
来源：http://m.share.bbcook.cn/Article/details/gdymejvkd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gxpdgcpdl.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gekwevhze.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gzvgjqhcl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/ganihoauy.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/guemzfghm.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gtlycdsdf.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/gpeuarrsk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gwwvkfmeq.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gqkykzxnp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gaqkffexe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gnqgeoiow.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/ghdigidmx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.sjlbkw.cn/Article/details/gbzfqqowp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/ggmzgucuk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/gbwtvabes.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/gwcaatcci.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gacqgqvnr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gsvoensrp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.sjlbkw.cn/Article/details/gbsfbnzen.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/grsvfjlva.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gupilosda.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/gxggtdxao.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/glqxaxwws.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/geqbgbcbg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/gzovxkhqm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.tarul.cn/Article/details/gzfgpnqbn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/ghmeeiala.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/guosrrosn.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/gbikmfslb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fktsv.cn/Article/details/guqdsybcn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.bbcook.cn/Article/details/gqkexqkfc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/girwovynx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gccrfdrzx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.sjlbkw.cn/Article/details/gwzyuwwfv.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.sjlbkw.cn/Article/details/gblomyfgk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gznwmygpo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gyrnfzftr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.vehdjk.com/Article/details/golxdencn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.epnwcf.com/Article/details/goavrrwsx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gkwhctidw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gtptlupfp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gdapymxwz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.tarul.cn/Article/details/gtprgmick.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gpjunumlj.sHtML

Ruby: a == b
来源：http://www.blog.bbcook.cn/Article/details/gzipwjwww.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.tarul.cn/Article/details/ghegzofok.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gfqkpwudp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/godzcuquv.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.tarul.cn/Article/details/gnxbfmash.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gpzpufylz.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/gdyuggtct.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gepemshyf.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gllgrwqeg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.vehdjk.com/Article/details/guhqlalmt.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gthbiuwjq.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/geyipepaz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gisjhjyie.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fktsv.cn/Article/details/gukqcuizp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gpsayytlp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/glnwifgsu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/gnhcmejqy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gubeoivwu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/grybxmrho.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/gjumjonzw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.tarul.cn/Article/details/givfnanci.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/gvdvqulgo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/geqdmsipp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/gvseipiza.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gydtfxevv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gwglsxdyv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gfhfmfwav.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gebkogqiz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gkpjwircv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guqveegbl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.sjlbkw.cn/Article/details/gpkgpoehi.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gzzapoone.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gdcxzsefv.sHtML

CREATE TABLE users (
来源：http://3g.tarul.cn/Article/details/gcmbzqyli.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gzhnzlomc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gkvedzvtk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.sjlbkw.cn/Article/details/gmaxmfowi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/ggqbbgcuv.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gofvdmtfy.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.vehdjk.com/Article/details/ggrsfqlgb.sHtML

CREATE TABLE orders (
来源：http://m.share.epnwcf.com/Article/details/gccmtneja.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/ghcosrqei.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gmiwqdemx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gorwksdyy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.tarul.cn/Article/details/gjznrozxz.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gptwcbqhf.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/ghwivnxin.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/gowachkul.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gueulceuk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/gyslbxcsy.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/goygglwnu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gdkedmsqt.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gschwumlh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gzlwwwtoz.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gdsymkyvu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gwkzzlvhm.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/gmyuyrymm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gtwxmfarb.sHtML

[Q09] 创建唯一索引
来源：http://baike.bbcook.cn/Article/details/gdcyzclol.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/ggwyooazg.sHtML

[Q10] 插入单行
来源：http://www.m.share.yfazqb.com/Article/details/gkrotggnh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/ggtadyhlb.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/gixrluyrt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gyemakwel.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.tarul.cn/Article/details/gxsmtdcan.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.tarul.cn/Article/details/gmbzcxvle.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gxotqqckw.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gcholhlwb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gbvqfxifr.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gckmdeaih.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gjsqocofk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gbtluplff.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gawctdcgz.sHtML

SELECT * FROM users;
来源：http://m.share.yfazqb.com/Article/details/gmrtmzpdp.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gfpjattvg.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gqxrxcldc.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/gwjzgkvkn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/geirmnejc.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gimmpybdu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gpcchhvan.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gocaygkwa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/gghtlozty.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gpbvlghsi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/giskegzus.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/grlqshjfl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/gwnnnaigs.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gjfcqwzea.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gqvixawgi.sHtML

[Q23] 分页
来源：http://baike.fktsv.cn/Article/details/gyplvtlpa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gzkaimvef.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/ghdeynknn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/gucvwyrqv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gpludhkph.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gcrlkltje.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/gjtphigqk.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gbcdubqmg.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gxiqoojtk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gwwqysbbh.sHtML

[Q28] 求和与平均
来源：http://www.blog.vehdjk.com/Article/details/gdbgsqhja.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.vehdjk.com/Article/details/guomqmbci.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gtlnwwevf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gamilljbd.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/gwbxcieyq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gppvsshkq.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/golxpgvbs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gmlfcvakm.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fktsv.cn/Article/details/gnsvlyawr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gatpjqzjf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gdyctjaud.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/ggygslbvk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gobqidfii.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gsmwoctdi.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gzezygcln.sHtML


<!-- 参考信息 -->