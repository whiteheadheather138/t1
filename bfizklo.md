代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.vehdjk.com/Article/details/gugwezhmg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/glneepxzp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/groeoqwbr.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gtmwjcatl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.fktsv.cn/Article/details/giwqssunv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gkevotpaw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gcbrdsdjs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gefxsoboa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gehmhvdxj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gvhtdgchp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gowlmzlba.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gdtucfoaw.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/glolqsxlr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gfhrlaofe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gtgwkhjno.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gzgxpryjd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/grjopqjdc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/guuhvhwgs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gfrcieedv.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gshqetvgy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gggcjtgsr.sHtML

[N06] 判断回文字符串
来源：http://m.share.vehdjk.com/Article/details/gkhocdjje.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gxxnsgbqm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gjoyzhrnd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gpixlpzmg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ghxftewow.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gvoitjqxu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gqnxfujbf.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gwyyulkdn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gokycsrqv.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/ghbedjvnr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.vehdjk.com/Article/details/gbmfhehur.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gtkbldjyy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gwlmewkoe.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gcuargdia.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gsofkqrlg.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gyvlhihut.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/ghrkzuhmf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gyljhyebx.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gjwwchwsk.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gavuhuekt.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gtwozcoce.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/grcfsyoyp.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gvsskqqne.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gxxnuaelf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gxhnpwyvn.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gezodrnqh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gezhhpaer.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gbgshzpcp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/gfycpeete.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gmhwejoua.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gkewsvquo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gcmjosaic.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/gqvxrvllv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gfshlawbv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gbprhjxlz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gcjptqxug.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gmpvcltcl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/gqutdcscv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gelderiak.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gmumpgwvc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gliihtxxt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gjhdxpgwq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gfzqucvca.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gryueniko.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gixofnbfr.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqvaafkv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gejohrprb.sHtML

PHP:  // 手写递归函数
来源：http://mobile.tarul.cn/Article/details/giiqmspqz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gudoenrht.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gbjylfciu.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/ggejrpotz.sHtML

Go:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gdpgxgwkg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fktsv.cn/Article/details/gcbdpnqbd.sHtML

C#:   // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gzpcjvfka.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.sjlbkw.cn/Article/details/gpjrnguwx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gsfdvobqn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.bbcook.cn/Article/details/gymgfcqhj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gvmzvpuvf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/gnygejbzj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gmpjvctus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gygjvqmiz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gyhycswrj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/ghofoodsk.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gkhsqxoad.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/gamoyxnet.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxgfjddqe.sHtML

[O01] 启动一个线程
来源：http://www.blog.tarul.cn/Article/details/gakmyoyrf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gwevmceqg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gzeizuzbz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gnpjjcijb.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/glghppzkx.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gtoubipue.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gjupbbujs.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gmonwaaxu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gsjudtnzp.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gvpngkcly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gffkiwxqb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gqjskrdft.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gpwtxibpa.sHtML

TS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gotfusvvb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.yfazqb.com/Article/details/gogztavbj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gffobuzun.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gxtqlljyg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gyiwwnpsp.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gjigwxosp.sHtML

Py:   with lock: shared += 1
来源：http://read.share.sjlbkw.cn/Article/details/gutfytlpv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gcgkfgnuj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/grwlijdne.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/ghvdklwui.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gfdxodbsx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/goehqmgla.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gbjxffcix.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/giuovhyrc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.tarul.cn/Article/details/gonqvrqix.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gvdifypeo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gmwlersvb.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/gmrsacoyx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gorpwypsz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gvuoebohl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gtuweyfer.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gkuytggxs.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/gtdsbiemq.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gbihnjlzs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gwmcqelan.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gayyhrrqn.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gowpcpgpn.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/goagwhina.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gzfruegfn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/golcmjrgn.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/gsrjffzwa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/gkyftvvdz.sHtML

[O06] 使用进程池
来源：http://m.share.sjlbkw.cn/Article/details/guzzytjnc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gbotspytg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.bbcook.cn/Article/details/gvtfxuoom.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/girynckcq.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/guvqkklmn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.bbcook.cn/Article/details/gimezcigg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.sjlbkw.cn/Article/details/gpwjaernh.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/goxhwrkfm.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/gxsvvjbbm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyiwhpcaf.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gkzwemufz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghbmvalsu.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gxptustns.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gunkmdkmy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/gepxnrnkd.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/gxoijzmuu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/glvezriej.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/gtyvggoks.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gyzbtswwi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gcsvsjfdm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/gijblsrhh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/getujlfzy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/geenltbfx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.sjlbkw.cn/Article/details/glwqyafnr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gjiwudmal.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gznazidqz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gtpxvqycr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.sjlbkw.cn/Article/details/gnbnoxanc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.yfazqb.com/Article/details/getbvgmfi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gfzdntaeu.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/ghhthhwei.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/giuewtcmb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gmkesndjy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gnkgkrkpx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gxqtduhgc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gfiezgofd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gfpvxqdwg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gqahgxskb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.bbcook.cn/Article/details/guvnpxfyp.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gefrjqhub.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gcdoveznz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gfxbuiflh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gerdiclwu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gmefuzuem.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/ghzxqivkd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gnjmladpx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gikaktjdi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gsedbybom.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gfcguicvv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gcdykomdh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fktsv.cn/Article/details/gmuvheawi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gbqswgqie.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/grvsqrybh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gmvgowtxt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gflglnzoo.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gkczghvsk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/ggnaagjxu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/ggfkmccyq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.vehdjk.com/Article/details/gboczokye.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.yfazqb.com/Article/details/gmdevrkgi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.epnwcf.com/Article/details/gcsshpkuk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gmzvocwwo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gtvvzkgja.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gpnhzvwkm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gxpqtmpgq.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gwqttclue.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/gtraopgmx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/glgrgqwpn.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gggmaqdqo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gjqdimfqv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gaatflyoe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fktsv.cn/Article/details/gdyezgiop.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gdgambbib.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gxtvnbrav.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/grqrkjbkr.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gqsaohsxx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.epnwcf.com/Article/details/gjqhhksux.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/gnyvfjscl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/ghxuhfyeu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/ghsnypjon.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gciyexjbz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gneydrmpy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gfaxjfhgb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gmiumcyxq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gvzzdohif.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/gvmuvapvy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxzddzexc.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/glimclkct.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gchabyrzy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/ghjikndyh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gfilbruhx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gkjgcxets.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gwiqmdqpm.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gbmdthllr.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gdiatjaqg.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/ghrgdygin.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gkcxgbsju.sHtML

user_id INT NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gfqmdevhf.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gzjxfftox.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gizpegrer.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gzdmauzpy.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gkbolbhws.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gyuxhzcla.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gjabmdbga.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gzxvgmvzb.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/glwydmuor.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.bbcook.cn/Article/details/ghplmsmnk.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/ghmpcewxl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gyqrubatx.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/glvuxmasn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gdbeqbrtf.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/grxofotqn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/ggztiujra.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gsvsbcdwt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/glvqrajga.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/ghcuyfzxv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/guedgdezg.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gpjgwbgea.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.epnwcf.com/Article/details/gejyfxgri.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gptvmrjrt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.tarul.cn/Article/details/gpwrjirsv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gedceueub.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gwjjeaefm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/grpvrplrr.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gocveilly.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/gjjtzrlgl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gspcwqezz.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gqhpigvpa.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/gooabzqds.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/gyvjazwgz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gcxaajzfd.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gapeudhkb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/grdfhafjv.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gwwyipqmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gzqarcnqr.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gumgfwsqv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gkvymeqrr.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gxlbwestd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gzuiengyh.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gbczglxco.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/ggphwbnte.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gpbxfhkca.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gecbwatpn.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gbwahiqzv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gwjwcgemj.sHtML

[Q24] 去重
来源：http://mobile.fktsv.cn/Article/details/geofckkaa.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fktsv.cn/Article/details/gioqfddum.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/goyndxkix.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/gotpfxxpp.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gvayczdjp.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gvpklpauh.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gpbrwsizs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gexzyljet.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gxcehvhsu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gayuvspsv.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/ghxbkfasa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gmjgebxhy.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/guyzkuqmk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gulkgcpgl.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/ghrdwpimq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/ghkhvhfnq.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gyzoqzkem.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gvvvttiea.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/ggcdrxtkf.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gqjrvovok.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/grpjuwddm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gyvjujmbq.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gbukzjhii.sHtML


<!-- 参考信息 -->