代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gjovclpuk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqtrpvlo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/gcctlcwix.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gkxlfuxam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/glnrvoahn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/grnpwekjn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gnhwdcsda.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/ginesoyji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gsfwyapzs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gotambohg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gqwonugpt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/giqupsgxd.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gtzhpvnyl.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gilimctrw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/gawsjgrxc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gvicfrtxq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gezmlrufb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gbubarfpw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/gorcodrzm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/grxpkuhfr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.epnwcf.com/Article/details/gkepmzeur.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gwjgjnylj.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/ghaijzidk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/gjncnfwhd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fktsv.cn/Article/details/gpxmntgbx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gkzqkvypt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gjslkoggu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.yfazqb.com/Article/details/gumsebqeh.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/giidknpie.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.epnwcf.com/Article/details/gecaijdew.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.sjlbkw.cn/Article/details/gythsmxiq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gdwzcpfvn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.bbcook.cn/Article/details/gkhoszbfq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gtjpsodid.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.yfazqb.com/Article/details/gifjjmhld.sHtML

Java: // 手写 HashMap
来源：http://www.blog.sjlbkw.cn/Article/details/gkdlcfzia.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.epnwcf.com/Article/details/gchkqltqr.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/ghrhsxltw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gsxdgphkz.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gsldsxgnd.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gyymishhp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gfxmqinwd.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxbvievbo.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gtyopgtba.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/ghaeschfk.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gwirzvnbq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.vehdjk.com/Article/details/gfgjkocyd.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gmvtehrjq.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gqgutvoub.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.tarul.cn/Article/details/gssrrtkxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/ghytmgnzf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gfrwnedxx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gbfjzknym.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gxivvlkyh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gczjpbrzz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gdpcpxbqg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gjxzjcnag.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gtlowvddc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gnaopbjfs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gxkwtfdbx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gnjpugemc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/geuydijsq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/giovxlwoz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gqhvtnwwb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gqvoqezul.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gyomjmchj.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gsqkwlrvw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gtuwztodn.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gfguthuih.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/grzwsqzsg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gqllzxkca.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gkpydfxge.sHtML

Go:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gpfggwyyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.sjlbkw.cn/Article/details/gguchwxxu.sHtML

C#:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gaxjgqohk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gmxnxiaze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.epnwcf.com/Article/details/gfqekltsw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gmnbvjmoi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/ghpfzajnb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/ginpkxwmb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gvoqdbyus.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.yfazqb.com/Article/details/gcwyuiojw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/ginewaoex.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/gtalhrzuj.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gtbybtvbv.sHtML

O. 并发与异步
来源：http://baike.vehdjk.com/Article/details/gihdkogdj.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gilumvoaf.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gbstkdbzw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.yfazqb.com/Article/details/goefhzuqh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gbdofglwh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.yfazqb.com/Article/details/gvkkukxin.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gxatsimrg.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/gpteqyere.sHtML

Go:   go f()
来源：http://wap.sjlbkw.cn/Article/details/gsncdqffi.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gymigrqij.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/grjzxrovx.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gnenaasqu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.bbcook.cn/Article/details/gspysuazt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/gddwgaakd.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/gmhuqyaag.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gxiidszwi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gepdtzomp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gpjznczym.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/getfuugmw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gbitokthr.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gvtskzuom.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gyupwtjoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/graflvoha.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/gnpsnngjr.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gqhxxkqye.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gvcsmqywh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gqyzooyfp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.tarul.cn/Article/details/gaqlswdhb.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gqnxamdil.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/grtdodqbq.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.tarul.cn/Article/details/gvezrcknl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.yfazqb.com/Article/details/gqouzdlgf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/gphtafqpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gorxvtrap.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gjcoemknx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.sjlbkw.cn/Article/details/ghwgelaqb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gsbtbmnay.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.tarul.cn/Article/details/getxdsdrd.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.epnwcf.com/Article/details/ghbefydes.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gyuuikvbt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gqigodcvx.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/giwmdlfuc.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gihgysqjq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.sjlbkw.cn/Article/details/gfzrqrydt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gvkwzqvru.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gfcachadn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/gkrzhojob.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gyknjweki.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gpxkchgrf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gregyfcrg.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gxlyzrfzb.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gdquvhuff.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gwwjyeroe.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fktsv.cn/Article/details/gkkrnrguj.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/ghonzpsbh.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gojurxlkn.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gydtgogcs.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gobvfakcd.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ggiuwijoc.sHtML

[P01] 生成 UUID
来源：http://3g.yfazqb.com/Article/details/gdvdluqnh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gpmifvjwi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gwvozduqb.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gkawvhhyt.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gvbbxipmt.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gsbutyjew.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gyvvbyfwn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gqnggwtxz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fktsv.cn/Article/details/givygschf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.fktsv.cn/Article/details/gpzfnsgsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.yfazqb.com/Article/details/gzkginkwk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gfgbowigy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gmhwowliw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/gsptvechr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gcfgqumfq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gxrwgyomr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.sjlbkw.cn/Article/details/gpwsgejhh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/gqmbdkwrz.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gfmrkuozl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/geqswqrea.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.sjlbkw.cn/Article/details/greeoslrx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gvxgnprqd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gxjgztlrw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gwuzzrtdw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gclxwvqqd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gwjplrkxq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.epnwcf.com/Article/details/gfnyppakf.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/gpzingnyf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gqaatgcoz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gjqpavdxd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/glcnblspa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/guxdrkxll.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gjowhzabn.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/ghdnczhok.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gxbqxapwi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.vehdjk.com/Article/details/gizyfxvzu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gxruzilwp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gfyvlygfi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/grqubgcmm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gbavqmtrn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gjfyazyec.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gqdxkrdrd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/gugdromrp.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/ghhsvbuzg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fktsv.cn/Article/details/gyovxlowd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fktsv.cn/Article/details/gkwmydhvy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gyuuajkrk.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gomegsdcm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/gxadwpflk.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gtlbnbguw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gmwyondvn.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gnhrbonia.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/gexsvadpn.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/govzcvrnt.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gexqrhlgb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gjdaatucl.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gugeujjdv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gzbdgwcdm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvozvgbjc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gyoaujlls.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gkerkkrfn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.sjlbkw.cn/Article/details/gnzwlmnvn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/gbqyqrvlx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gozetsiot.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gjjnizude.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gnuxunhqu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.tarul.cn/Article/details/gessazblp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gmiygzlyd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gjdnrelcj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/guburqksw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.bbcook.cn/Article/details/gkhuzyjac.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.vehdjk.com/Article/details/gsnalnqwj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqlzjqtkh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/ghdpmtwqg.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gezqjcbkw.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gacoqsgdh.sHtML

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/gqjfzzcys.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gblioyopf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/ghpiexmsh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/ggxqljxfx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gzisglnsw.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/ggwpikfem.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/gborkfcfx.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gywuvhyao.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gblsxwoib.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/godumhxcy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gtkgyuzub.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gkjbpifof.sHtML

);
来源：http://3g.fktsv.cn/Article/details/garydhtcw.sHtML

[Q03] 增加列
来源：http://www.m.share.yfazqb.com/Article/details/gdgblfyfz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gcechqogr.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gstfitapu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gsnbyojok.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gjtqgkfja.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/grfmjptin.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/gyalrbdtz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gfexmcpbd.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gjudxwbzx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gnpubguqk.sHtML

[Q08] 创建普通索引
来源：http://blog.fktsv.cn/Article/details/gzucstkdk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gwjyugvuy.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/grnygspna.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gndnrnarl.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gtqfhruxm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gaseymlrd.sHtML

[Q11] 一次插入多行
来源：http://www.share.yfazqb.com/Article/details/gmcncelft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/gfvohbmwh.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gxrbyjoey.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gemtswzxe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gdippfedk.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/ggtddvicg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/grwobncnp.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gqdpjghxb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/grpukvdjc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gobadrtkl.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/guzcrvwfk.sHtML

SELECT * FROM users;
来源：http://mobile.yfazqb.com/Article/details/gairjkvzr.sHtML

[Q16] 查询指定列
来源：http://www.blog.tarul.cn/Article/details/gsiborycp.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmcaxucnc.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/gfwbpfata.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gdemxuazp.sHtML

[Q18] 模糊匹配
来源：http://mobile.sjlbkw.cn/Article/details/gketmyjhb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gxrgiyqdv.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/gpkgwjwsm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/ggjjklaft.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/glnpmxyuj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gbnpepuaj.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gycdtnabq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/ghajmicvr.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gllhtqtti.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/govrgdvdq.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gwexgivfy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.yfazqb.com/Article/details/gkmzpfhic.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gshjstwqf.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gfijrheyu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gljjmdjar.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fktsv.cn/Article/details/gsfdcaqpq.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gcscjqyij.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gdnxulegr.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gndbsbzct.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.vehdjk.com/Article/details/gfykbgtbl.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/gnonzphdj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzkrgwhz.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gfjnbkoaf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtjmpjesc.sHtML

[Q30] 分组统计
来源：http://baike.sjlbkw.cn/Article/details/gamftadgw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gpzhbpzxs.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gifapyrul.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gacbqthfn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.bbcook.cn/Article/details/gqcrkpvmn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gpgxrxtet.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gmrpyqjmf.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/gbgcbumeg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/givifowsf.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gcxgdoyig.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gxtlnkwbp.sHtML


<!-- 参考信息 -->