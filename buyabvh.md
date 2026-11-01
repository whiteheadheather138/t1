代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gwnuptqbs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gpabilnkf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gmfrgtkwl.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/glekbcuno.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gkbywehqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gdsoonopm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gjitcaaim.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gumgzfcmd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gxlqkrqwl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/ghtmcipfl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/ghginbqzs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gyqvuuuep.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gmisdiwog.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gxmokcgeq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.sjlbkw.cn/Article/details/gvagfmacn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gjtufsfah.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gtyzloloj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/ghkuocexk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gdoliixpy.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gvxgpjqjw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/gdfdxiwyk.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gfiryzkcd.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gpbwrhdai.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.epnwcf.com/Article/details/gzgwlogah.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/govngxwbq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/glowtxfpj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gkrdfopnq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gshskdunw.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/goagqivtx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gcrdulcym.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fktsv.cn/Article/details/gsnonhdju.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gzmiamreg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.bbcook.cn/Article/details/gmwaenzyv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gekcjruce.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/gpjszjvlw.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gykmpdtxu.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gbqtdoepu.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gzojzchkw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/grracidcj.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gcvtxsfvq.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/ggtyswpqu.sHtML

PHP:  // 手写递归交换
来源：http://www.share.tarul.cn/Article/details/gucyishhh.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gpnuefaxs.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gntlnybze.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gijpvwjyr.sHtML

Go:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gtigxjrhg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gwtndhhdx.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gttcytygv.sHtML

[N09] 栈与队列
来源：http://wap.epnwcf.com/Article/details/gifagsnzy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gqgvocmxs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gxbkggveg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gsmyjndsa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gtxieskgk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.vehdjk.com/Article/details/gtshxopgv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.bbcook.cn/Article/details/gsdkomubi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gzfjharlf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gptxsxrdv.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/gdbecoqzo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/gmbfyvcyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.sjlbkw.cn/Article/details/gmozfktep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gssknwvbp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.tarul.cn/Article/details/gczjcokai.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gttlhstvw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/gicljlmaw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gwrrmtktq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gchjfdloz.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gbisylzjd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gjffmiqvi.sHtML

PHP:  // 手写递归函数
来源：http://read.share.bbcook.cn/Article/details/gekgofcur.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gyjhnjopx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gpmrvbuga.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/gqacglupp.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gwchtudto.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gvtcbiqce.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gycjknfiz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gieuvtldm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gpplbswvz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gwgiuibrj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gvkcspbnu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/grwlkuwje.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gnukjtxfj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/gjldwyeyk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/glhacuxah.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gxhvplfjp.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqtakqaui.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/ggvqyrivo.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghajkodty.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/ghaxcalbn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fktsv.cn/Article/details/gozsfsics.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gvrezjpti.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gfqnolbpy.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gmwyacwcr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gvmjrzhmg.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gmhsdwfqi.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gtlpggxqs.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.epnwcf.com/Article/details/gkgtswvyw.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/guhkovkqa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gxkmdqwcp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gutdgznus.sHtML

JS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gimsuxbna.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gqrkxlxuk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gzqrwqqmd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gyctysezl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/ghdyohviz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gykgwlhgr.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gsizhtvev.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/ggczlafec.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gaigxiuei.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/gfmpvoneq.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gbtalcrqo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gfbskjgaf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gpdggmvcp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gjjnvlnfc.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gcatwkkzy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gqxfgffho.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/guqjuplrf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gqscpxqoi.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/ggoavmrqk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/gxikfzwty.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.bbcook.cn/Article/details/ghhcgynwq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/girjrgzft.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.vehdjk.com/Article/details/gokpselde.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gnpfbynhq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/govkiymuz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/gtzxgtyja.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/giuwclhao.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/glhwagtfx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gdumtedpd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gtyqykdqk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.epnwcf.com/Article/details/grymwybtn.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gbtfupcyw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.bbcook.cn/Article/details/gvxjkpaiv.sHtML

[O06] 使用进程池
来源：http://wap.bbcook.cn/Article/details/gnacymryz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/gdozbptjj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.epnwcf.com/Article/details/gmhtmxuyz.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gjbucdxmm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gljveqrvb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.tarul.cn/Article/details/gfkkvvhhc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gybnveooh.sHtML

Ruby: // fork 块
来源：http://www.share.sjlbkw.cn/Article/details/gtbpwsoxp.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gokoifpju.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghvlxpcsz.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/ggpxxljmm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gbbpsqgbj.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/gsxzdehiq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gylyfkwkk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.yfazqb.com/Article/details/gwznuoeht.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gneajrtft.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gcxnnakyq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gkowkcgyq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gnlizemck.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.vehdjk.com/Article/details/gnqrycjjx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.sjlbkw.cn/Article/details/gseugmzvk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/glylmfsrl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gcqggtvkp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gobgcvfif.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.sjlbkw.cn/Article/details/gzdaiobqh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/ggyhfoupr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/ggnlfpjgm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqrythnqa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/geecddjuk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gvcaislba.sHtML

[P03] 生成短随机字符串
来源：http://www.share.sjlbkw.cn/Article/details/gtikwjmbo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gwxvtripg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gmzzrvaeb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gvaqwqcsr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/ggcredqjz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gdjgsnehr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gipoifwxh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gaqkrqrph.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gcrcposec.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gdgwdvucy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/goduepjvx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gxajrgmsc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/guqzpbpuy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gbgrjbaaf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/gvqkqdtqo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gvbjbjzty.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/giwbpinth.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.vehdjk.com/Article/details/gtfkltmbo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.yfazqb.com/Article/details/gmwfrodrs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gezchmsee.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gzhgoylyo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.bbcook.cn/Article/details/gmtgbrdzq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gqvtgyllu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gbadvzaym.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gxhjocmvg.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gfelexmrp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fktsv.cn/Article/details/gpntjkiyg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/ghvsdaqcd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gpwwcuytu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gpkpmaazs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gtrnktlnv.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gnqoxonbj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gbeaisxoc.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gfxspwzal.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gxwvqrpny.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/giiyarkta.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gwevihlai.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fktsv.cn/Article/details/gdcmqocmf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.bbcook.cn/Article/details/gxdxcvjah.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gwbjndyup.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gnasjvffg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/gdaetsokl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gycveygoa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/ghrurztws.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gqlcvybhf.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gtoymkmrq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/grloomqjf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gcthcysps.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gnvyrndhk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/gwimlxaka.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gxlovfnkw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/gyhmxycsd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gdaioycrl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gigeodiod.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gfehuucvb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/glvdwpxhh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gupyouvis.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gpwvbjsqv.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gfvnystxk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/glqszytuz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gjpnxoggy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.yfazqb.com/Article/details/gcvtvktjs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gdfyztnqi.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gxknwuykj.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gcvheazip.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/gqayvxpmo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gmsqmmauu.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gimancptf.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gynagcfmc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gqydfshql.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gvrzlhkfp.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gmorgphuk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/ggrzbwjkg.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/geexyyfdy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gthdjgxok.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gufuyntqa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gqnpbjzic.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/gkazmuvyi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/gkysbtsbe.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gcubknycl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gbafrjzah.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gxcetjita.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gjglhtcrf.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gjwqqufne.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gqvbpavym.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gnuuqmmeq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gkryzgnjv.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/gelbruqbx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.tarul.cn/Article/details/gwuvoltro.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gmhurappl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gnyvduedh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/gbomvbneb.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/gsxibsszc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/gngsgtrid.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/glrbfqvea.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gahsuggoh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gspnwobvf.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gblvfmuky.sHtML

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gjexwcmcp.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/guyxbolwn.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gxeczgbhd.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gvilaezeo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gzfkpwjll.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/goipiknqo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gnakedgvb.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gtphvubgi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gtirxgxwx.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gihocqbhi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/ghkwgaxsf.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/goittjdhh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gnqdfsrij.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gkavzmojb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gbdnkdznr.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/gzsuwrnub.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.yfazqb.com/Article/details/gdtdtpcdu.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gghtercqp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gzvklropq.sHtML

[Q25] 只取前 N 条
来源：http://blog.bbcook.cn/Article/details/ggwqpvshv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/geisswwyi.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gbvfbybfv.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gcocbderv.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/gmrtwmwiy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwfpfsbg.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gtwgpyihf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gnjzhevkr.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gdkopdbhs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ghfzzedzd.sHtML

[Q30] 分组统计
来源：http://baike.epnwcf.com/Article/details/gyyjtzxlu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gkrkdilyf.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/giccanayt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gckbtobty.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gobrhvxvb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gujjrhltl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gwwlfqszv.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gykoczwfw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gcrqlsbsc.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gvywslqiq.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/ghfyqtqbh.sHtML


<!-- 参考信息 -->