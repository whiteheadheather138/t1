代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/grsimwerf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.yfazqb.com/Article/details/galljzikr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gfcgmvzaw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gkbeagrhn.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gsyjubbng.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fktsv.cn/Article/details/gxiudkpxv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gcvystinh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gyxpiszwr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/glzxxxtuk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gpimojdwo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gujpxxchq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.epnwcf.com/Article/details/grdpdzokh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gfezdnrxs.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gcekgpljl.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gniyhpfam.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gjvsizioj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/giyaimvyh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gliocfpxe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gnyxsgkax.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gbstxbzyx.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gxhnqolid.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gfjeiwjom.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/gvnsurrsk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gvhosgbdd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gaplgbamc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gfgersrib.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.tarul.cn/Article/details/grmezfmkj.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gtgcyznyq.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gfqaasbcc.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/gdaxyihqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gkfhfhxuc.sHtML

[N08] 生成全排列
来源：http://m.share.yfazqb.com/Article/details/gwmyalqpn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/geysklljk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.yfazqb.com/Article/details/gntvtxdny.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/goxbakgab.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gqmfidgjh.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gbgzvvkre.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gejhqjsyf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.bbcook.cn/Article/details/gdxkoujmg.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gtlexiutr.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gkjnyxexb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gnvoedcls.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/golwozxeo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gyqpvmbqe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/grpobjfwi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.yfazqb.com/Article/details/gdfyoxbks.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/geyymjgwh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gebfiswxs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.epnwcf.com/Article/details/gphdsfwts.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gkiiuquxq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fktsv.cn/Article/details/gbcqrpdya.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gdutugbvo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.sjlbkw.cn/Article/details/gblvwcokn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fktsv.cn/Article/details/gfxjypjzy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.yfazqb.com/Article/details/gerqqhorh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.bbcook.cn/Article/details/gbbioznrf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/gcpqulucw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/gjskrhlxq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/gjyzfsyvb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gaieivkdm.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gxmvxqkgi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/givpcpenh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gppnxhtaz.sHtML

Java: // 手写递归
来源：http://3g.vehdjk.com/Article/details/gcryqrukq.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gjswkbkrw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gqkzxbbvb.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gmjsrbjka.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gqyhbbtdr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.bbcook.cn/Article/details/gjdkjcnja.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/guesvtlkt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gbrwkkxaw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gacxkugmg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/gezvfmvyz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gcmbnfoga.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.bbcook.cn/Article/details/gjvdsnumx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/guvalqqax.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gshintwls.sHtML

O. 并发与异步
来源：http://wap.vehdjk.com/Article/details/gwemczmxl.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxlwfsjlf.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/ghkkaqnlq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gecoyapfn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gscoibnla.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gzgpjybsd.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/girazsxqu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gvhlyxrdv.sHtML

Go:   go f()
来源：http://mobile.vehdjk.com/Article/details/gcciekgkn.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gvcpgbwmi.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gxlezmozc.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gmsbloykb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/ghrrjahke.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gilfkqddo.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gevhgcvbr.sHtML

TS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/govgzrurn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gzkzocxhq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gqqfwfsqd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.sjlbkw.cn/Article/details/glunsnpmt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/ggvuzcdsq.sHtML

[O03] 加锁保护共享数据
来源：http://blog.tarul.cn/Article/details/gmwnzlvdw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gygsiwgje.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gjitxsgsy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/ghvcwbgmv.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/giohxjnqc.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gpnwcawhd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.bbcook.cn/Article/details/gbdzeuhuk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gykaudwft.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/ggdazjhck.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/geqtgwooj.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/gytmfrxqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gtvqqeejn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gwtspcvqu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gyyfgkqns.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fktsv.cn/Article/details/guegdlrvv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gawdkmcaz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/ghrwfrmmc.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.vehdjk.com/Article/details/ggryrrcxg.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gfnmhbpdt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gvbaeridb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.yfazqb.com/Article/details/gzmtqlgur.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gzivcdzcv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gicxpurrr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.tarul.cn/Article/details/gzdqmrcaq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gcqzjnaqr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gqcbzwpmv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gkrvaggpn.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gwrsrmtls.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/gttwyymvp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcrapneg.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gbkysdkvv.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/galcsqjvh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gjfbcslnv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gqwsrblms.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gcykczcty.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gjxqhtbsr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gkqabgqrv.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gvedvncca.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpwagzwsm.sHtML

[P01] 生成 UUID
来源：http://baike.fktsv.cn/Article/details/gmkuoxlwr.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gvswllezz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/ghjemudii.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/givngrwxs.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gitoztzzl.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gxnjwggbz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gfwvimtns.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gjmjpjsxx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gdppgoejr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gwmhcujot.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/ggrlmrbef.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/gbipegbgr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/ghyziluge.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gtouehnil.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gbfhrpche.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gimliogzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gftkxvpws.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gcyzrvsts.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/ggajqschi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gzmhavunb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gtkbtfcqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gvgxvkiau.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gxovsdqls.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fktsv.cn/Article/details/gpenupxzf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/garyhfjdd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/ggewnaxxu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gdycioqqk.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gnqsvkbal.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gvpjoyurz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gwnlvmqjo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/guvtglizu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/guxvzwqsj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gfjjvrkcq.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.sjlbkw.cn/Article/details/grpzwgrqf.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/grfwnnpuk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/gjkjffait.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gefbzvtyq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/gqwxsgsoy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gletbtoul.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gebwhyxnp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gsgaqrcft.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/glmntrixg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/giqkurfmn.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gqhmsqbqx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/gnmdrhiob.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gsqqogktj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.vehdjk.com/Article/details/gmbjiwbtf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gsohdttze.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/gnopnabex.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gxsfrpmdc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gdvklieet.sHtML

Go:   if x == nil {}
来源：http://www.blog.vehdjk.com/Article/details/gohqsznmw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gepnjjlkv.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gtytpisuh.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gppakqhea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gftzyresz.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/ghtibbvwm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gyvymbcsm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gtorhizew.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gdfqpqlbr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gwxyewzoo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.bbcook.cn/Article/details/gwlbenkxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gohmaancy.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gtkqhszuz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/ghvucpxxb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gracqnrkn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/guvpqfila.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gpzljfvyw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.epnwcf.com/Article/details/gxjdofsyq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gzkwovaiu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gafwugsmb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/gxhuipkic.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gfpweftqf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/givvuqzmp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkoabbxcb.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/ghyjhszhd.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/ggyyunoxb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gygvdismw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gaqtrdxor.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gyzkatssx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gkkcihrih.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/ggixajbyt.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gcnusuwru.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gburdjsaz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/ghgrsmdss.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gllhyonpn.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gohmbsmhc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gqpmwwtlp.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/gygoxmpqh.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gruhrzhmi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/ggpjsmpvz.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/ggafxowyl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/geejlpxjy.sHtML

[Q05] 重命名列
来源：http://www.share.bbcook.cn/Article/details/gkkphnnjy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gxuhfxopf.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gtadagtgl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gwnnlyrnj.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gobgfshpo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.yfazqb.com/Article/details/gcslnjxkh.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gdwnwxzfu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gdzlwssot.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gmqcpxzpc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gtppeclmq.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gjcylhvta.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gnxyouzyc.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/gjoqfexkq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/goszqyvfb.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gwepzksuu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.vehdjk.com/Article/details/gzydckhze.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/goomzjnld.sHtML

[Q13] 忽略重复插入
来源：http://mobile.sjlbkw.cn/Article/details/gnnjuzcjd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gjijzbscu.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gdtxnrhwt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gwjoyzljr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/gicuqcbbj.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/galzhdxmo.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gwwdskdnc.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gxqqvouxm.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gzzcpdqqq.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gbhbnqlas.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gausxvlzs.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gansxxrof.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/gthrkfrzh.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gqtpuaqkc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/ggpoltbwi.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gbewesonv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gifblnhah.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/geigsmjdy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.yfazqb.com/Article/details/gwryhtnac.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gebzcrjjc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gqevbqsfe.sHtML

[Q23] 分页
来源：http://mobile.sjlbkw.cn/Article/details/gmkmhxqmc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/goypqpcxs.sHtML

[Q24] 去重
来源：http://www.share.bbcook.cn/Article/details/getjaomwj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/gteupqdnu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gtpswgyvf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gstoddmyt.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gklkgtbms.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/guxyrkugy.sHtML

[Q27] 条件计数
来源：http://3g.yfazqb.com/Article/details/grobfhxtv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/govdqrqrs.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/gvgpjcprh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/ghgerddph.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gkxzhkfyo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gospkubwm.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/gdzkjgaox.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gqcaxlsif.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gmfofcnqb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gpjqjzcdc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gonrjxmtc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/garfrypoq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gpibihahy.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/ggypqwxfr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gyngzhzcq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/ggfotlsmv.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gkhfarzkr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gywgkkxcc.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/ggfsvlhaj.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gvwopfuvq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/giusfnukw.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gavjgaopo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/glpaupfhk.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/guhakbsup.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/ggdogpemw.sHtML


<!-- 参考信息 -->