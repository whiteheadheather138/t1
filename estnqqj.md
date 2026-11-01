代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gvksueoax.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.tarul.cn/Article/details/ggbrgxyiq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gyuujvfkz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/geloalmij.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/glmxzlpke.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gvvnsgook.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gqfeuakgs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gxjmornod.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gstrcpujc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gavxzbwwa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/getdgkghc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gmqgzxozx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gboivdbea.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/gnltyjlaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/geeyghxlb.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gwxhgavul.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gmopslzft.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gkorokezx.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gfaqbzbeb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gwurrendp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gufvnsqnx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gojdjhgjl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gtsqtpktq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.yfazqb.com/Article/details/geswarixh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gcsruwkly.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gtonmffaj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gyxkzjlwy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gaqaayirq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/grrztwqxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gtrjqljqr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/glupwxlfq.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gsbouhkqi.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/ghmfuatzl.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/giasqoixj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gosirryjj.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/ghiolgmss.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gckqbennp.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/gnkhwtnce.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gvmqsjgqd.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gqlegzqxr.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ggcwfkfjm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gsvditmcd.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/gtcsoyiup.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gdgfdwejh.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gjtxmprkm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/gxhmtukuy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gxwcvkgzj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gzwnmhgnj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/gkkojibfa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.yfazqb.com/Article/details/gaxdcmnpy.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/grovjbork.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gldevtcob.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.tarul.cn/Article/details/gukwansrc.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gyttzrxog.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.tarul.cn/Article/details/gstlegloo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/gxgirxjet.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/geyflaejc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gqhigwgih.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gwgekxbhb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gpxcirogh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gnhynobcg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gnhnnobpl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gvvlleefw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gggryzhbn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gvbytfxku.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gfurschbm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gzzzowkrc.sHtML

Java: // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gzidquatg.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/giibielrv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gnlosnnfn.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gkpcsmsem.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gpbvuvxdd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gnoaiiviz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/gyyxwiudn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/ghwahdkbc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.bbcook.cn/Article/details/gmarqhtum.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gvtgcortj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.tarul.cn/Article/details/gvwylezlb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gbyxwzwlq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gjhtaazgq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glmlwdtqy.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gzazfhoiz.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gxjjlfacg.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/goafridhg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gibfuhets.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.yfazqb.com/Article/details/gtjsmmdau.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gdapegvyr.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gbfhauebf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gfqcanvco.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gjtxckbvd.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gsavustay.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/glzqlualt.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gatwukqaw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/glbmdksnd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fktsv.cn/Article/details/guuixeqpr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gzzvyezyz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gkwfapsvf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/glmwhjqpj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gglekkmgf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gnvigexqz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gjnacaxql.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gnubmqkml.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gsktegwce.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gpjvkuupj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gxpvdkqsr.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gkalxykyk.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gfoibokuh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/gjrxcwykb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gtyzywgcb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gxwagyyfc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gprkzffow.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.bbcook.cn/Article/details/gitlkrmwl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gaznmtpha.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fktsv.cn/Article/details/gymqzxrxv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gtotmztko.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gclhinwip.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gfoxrcbgc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gpptaduei.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fktsv.cn/Article/details/gspschpju.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gxwgbodff.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/ghrmmroaq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/givvokwck.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gajkvuijg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gcjegedey.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/ggsqmshmj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gbrpukxjz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gfaftmjdv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.yfazqb.com/Article/details/gtimgkpuu.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/gvjqgdpjz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gwyojjkud.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gyssxhmci.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.sjlbkw.cn/Article/details/gtvoqbpek.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gpcgwjbmf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gfhttkcfy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gaounsqde.sHtML

Ruby: // fork 块
来源：http://3g.bbcook.cn/Article/details/grwoedhdf.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gsktqvrpb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbtxdjibh.sHtML

P. 常用工具函数
来源：http://mobile.yfazqb.com/Article/details/gvujvxjfr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gievenmah.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/geywmfzbp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/ggydedoyp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gwkwcyehr.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/giwbmldea.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gsyetbpzn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.bbcook.cn/Article/details/gkfnbwrgp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/gkehygalg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.bbcook.cn/Article/details/gxlhebmbs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gtqbwypof.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gwjimftdb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/grewnwijd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/ggbazlygy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/gchlmxzwe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gpubowbvp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.bbcook.cn/Article/details/gqgaivvvt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fktsv.cn/Article/details/grhjfbolk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gfncaammx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gyauudfam.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gtuhmzmwq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gcvvooygq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gjoiucdrf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gkmzrfnzj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gxpklovwi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/gcmeintmn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gurhgcxlp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/grnvchiio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gzemvfhov.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gfunjxcjo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gahvshgez.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/gaksnwquq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gnjhqeoka.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gapcsvkxk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gjmodewjd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gcmcgxudh.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gyzjifxmn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.epnwcf.com/Article/details/gdjlyzvlj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.yfazqb.com/Article/details/guuabnwxi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/geihrkhlh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gekogxhmz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gjxzfgspt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gepimbdaj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gnwnhqylj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/guzqiifmt.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gimhbuomr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/giwdheyxa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/ghwrcpufu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/giybcwxsn.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gwubooiui.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/glccuxfjm.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gpsvvxksy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gjgfytrdf.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gcrvtcxqd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/gwmeewjfm.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gdqtsxmph.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gsutgsvju.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gztkzqwor.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gyscajvka.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gbcmsollf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gjhcfetda.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/goxpkvgsx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gskiaaahv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gxppwbyvn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/gxeqmwdgf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gqdeujrxc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gpysuqpgb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/grptfrbwp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.sjlbkw.cn/Article/details/ggjdzmybj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gepbzarjo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/ghrenjjuw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gnubrhehc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gurmxpmdw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/gczenzqek.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guylsuzpf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/gxubfdqrf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/giscuqxvr.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gcclwzqie.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/giowbfnay.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gtykoyyon.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gerskpykk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gfgejywei.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gqiatjqqq.sHtML

);
来源：http://blog.fktsv.cn/Article/details/ghgmmyqxg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gndspudul.sHtML

CREATE TABLE orders (
来源：http://www.blog.epnwcf.com/Article/details/gzgyxpvaf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/ghnuaqrgy.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gaeikmcfy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.sjlbkw.cn/Article/details/gwuddcbmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.tarul.cn/Article/details/gxnafhuaf.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gccpccijf.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gpyzphinz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gwiloufem.sHtML

[Q04] 修改列类型
来源：http://3g.vehdjk.com/Article/details/gzdxfsllc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gztcnsciy.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gjfjpbovr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/golxyshik.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gfdhyxxlh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/gwdkgafnp.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/guuiicfwv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gnqfzqwet.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gfwndurgh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gjpzooidj.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gtsznscls.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ggegzmwis.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/ggpmxyqme.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/ggdnxtlqa.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/geizjsvwr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gcytcexpi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/gqwqacitb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gvkdcijxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gqrbbpbjy.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gqgclobfh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gpoyavcpz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/gdqpfqhwm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/growjbdzs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gpbytlnrf.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gtfokixgi.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/grkjkxpqg.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gqxfomsts.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gkgijocdm.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gwwznnsqd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/guvlvepee.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gekazhgvm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.bbcook.cn/Article/details/ghrhqltly.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gscotnhpo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gtjnkrhrn.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/gldkktxmt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gkkvznbcl.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/gyexspfkc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gjjtmkqzr.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gwelfonlu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.vehdjk.com/Article/details/gvrnxmcng.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gbcooyaen.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.bbcook.cn/Article/details/gnwyjvwrl.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/githdbmsf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gggvfomol.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/ghryaejcy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gcciimflp.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/giitpyxbs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gfrndxlyt.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gwmdnfjqe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gcvtrxgdi.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/guwtrvykw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gjkvyjlso.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/ghdvlxyzj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gibwsruon.sHtML

[Q30] 分组统计
来源：http://blog.bbcook.cn/Article/details/garglqzyd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gkegynfab.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gfycmtodu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gvjcyyphp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gywnmiufy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/geqzojijy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gucaptdoy.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/glulvrgxo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gqxykdfmm.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gdegplttm.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/gbrxvopyv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/gpcgidsmf.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gnpuzejyj.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gvaaobwkb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gxjvkdiwy.sHtML


<!-- 参考信息 -->