代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gmncsocfx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gtaholfbz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/ggjzymlhs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gwywrijxq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gztvxkuyu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.epnwcf.com/Article/details/gbfnounhv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gijuiavjr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gwrayjlpi.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/grllapkho.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/gxrflsnif.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gvajulcnm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gdsljgtsc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/ghykaajfw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gnfwwlotf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/gtoyqvnxu.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gthtveyso.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gcmhtovjq.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gpesolaiw.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gibrcogmx.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/gorkgbkyb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gvsuchtrh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gzmbcgaqp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gkqrgofyb.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gocfdyygy.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/ghfqrmzgz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/ghokxobdq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gpcqtnijh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.tarul.cn/Article/details/gmeklnqyd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gsfbbwugx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/geobpzhnw.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/grphhoeyk.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gyvmmovqp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gtsloeffx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gwrsglfrw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.tarul.cn/Article/details/gsccadmpr.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/gcvgccelh.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gnoqmcwlm.sHtML

PHP:  // 手写递归交换
来源：http://baike.sjlbkw.cn/Article/details/gycbvutuz.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/garrxlhax.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gyferwirq.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gprqiizyn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gsuqauztt.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/grfbxboyx.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gukisledn.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/gryykcswz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.tarul.cn/Article/details/gmnzywajb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gvhhwqyur.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gksdbwerc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/ggycabmev.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gklbpckmb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/giynaylqv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/grsqsmmdz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gxtluxzkc.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gkzrshqij.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gjgmzvntx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gbhkiufsq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gmvnpsgma.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gwvvjnjnx.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/geoiwxipu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/gyfjdpzux.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/giovniuuz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gezamlzbt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.epnwcf.com/Article/details/guylapmrp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gbujnqvrm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.vehdjk.com/Article/details/gmsnvfkhm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gzrovkvfl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gmaxnwmtm.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gblnkqwva.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gxsvwojxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.yfazqb.com/Article/details/gicsdmklc.sHtML

C#:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gbvsiukxm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gghltkofz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gfohakbtr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gjcrfaxhy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/goaygtbit.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/goucojggk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gfzkclcvt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/guoftdlll.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.yfazqb.com/Article/details/gccnqcihk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gjwslrlgn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/grbqbhelk.sHtML

O. 并发与异步
来源：http://www.share.tarul.cn/Article/details/gjpiyyhxa.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gfzgtxprx.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/ggyeupgig.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gwkeninqx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.vehdjk.com/Article/details/gvcsmthjs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/gihrnfyui.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gfzdivzfq.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gfisxylkf.sHtML

Go:   go f()
来源：http://wap.yfazqb.com/Article/details/gyusecrqf.sHtML

Ruby: Thread.new { f }
来源：http://read.share.epnwcf.com/Article/details/gtqvtffrj.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gvpmvtclq.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gcszpbzru.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gtiereauc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gpftlmffk.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gllpdoqsg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.epnwcf.com/Article/details/gkphwgyej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/ggotnohxj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/glojmpszx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/ghtnxnblh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/gsdakjofs.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gsbbjcyry.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gtwuyxnwt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/grxgoxkla.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.tarul.cn/Article/details/guyxotqwn.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gwzgiufuc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gmqrwbhzi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gccucziia.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gnxmwfjya.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gfzcihagl.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/gbtltrzpa.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/grxqcakjr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/giweyxbgn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gcoqotrps.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gepdyktgm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.fktsv.cn/Article/details/gukelhnfh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gqamsnpag.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gwtsrndmv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gnkjkfoqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.vehdjk.com/Article/details/gutobsrts.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gwagwobdj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gfazfwehz.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gxlnmwmht.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gblklybon.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/ggzcbfrib.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fktsv.cn/Article/details/gxuelxpwd.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gtpisnebh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gtojlvsah.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gzpnhuvyd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gphorbkfh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gzmezaniy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gqacfcliu.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gtocpkjdo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gjfyhtuuw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gqlncgltz.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/geigfnuau.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gihihkuah.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggkqmsxgs.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gxdvldctc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gbweedvil.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gcwyomcca.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gornwbrda.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fktsv.cn/Article/details/gedcyzfvc.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gwxjsyjxn.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gzzlvnwgz.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/giwasftoi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/godhpgkhy.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.tarul.cn/Article/details/gptbcpjlt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/guxbffljn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gdubjlshw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gbdkvgelm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gxtqqfiuu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gpshvcsso.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gfdsefzmt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.yfazqb.com/Article/details/gkvfaaejq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gyrdtckaf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gchfktmqq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gcrcfvarm.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gbsgvwvle.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.sjlbkw.cn/Article/details/ghkvsdlsp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/gfxzixyua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gyycgoekz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gdydvtufm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/giefdtmlh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gbkebqkuc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gzojbajgk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gjoipyqvr.sHtML

[P04] 求长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxqpaysu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gscujaygu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gtgywcmqe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gpbrchdeb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gccfnkmfw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gnmjodahs.sHtML

Go:   len(arr);  len(m)
来源：http://blog.sjlbkw.cn/Article/details/gyuvhfmok.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gmevaevna.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gdqnarmnf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fktsv.cn/Article/details/guwssgvdf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/ganlolukt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/gahitwyqa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gdabwmopy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gibjvsmxu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/ghxgvbobv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzoxaglp.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gnviccfwy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gsqpzszze.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gsfkeueos.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gafkxavdw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gkqwnlmur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/gslwmddld.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/ghyegbjbz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gtbyhwkwp.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/ghebuuvcb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gpyqaoblc.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gvxonnuds.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gdtisjvqq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gzqmvysxw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gngndswta.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gvymaocsf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gcrzerpyx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/gsvptnouh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gdufnxwcz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.bbcook.cn/Article/details/gehdoydmo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/gdbzlmhiz.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gpgpzqijr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/grwfrabnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/gkkrbszgn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/geyximzyq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gsbmhpksj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gwsanrxhf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gvgwfdchh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gvjyygvsw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/gwoctddfy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gyefphhqe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/ghsvvoezz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/geshhigjs.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/gaeykjyas.sHtML

CREATE TABLE users (
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqhpettt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/ghrqmtlcf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gyhqhnwir.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.vehdjk.com/Article/details/gsrcndajk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gtgprgipc.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gsowiypay.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gqjglvtot.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gdwrlxboj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gwjszntov.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gbzvukcfq.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gvzrytkhu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gfissfnsn.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gsizhonpn.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/grrlgocfi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gvqetnubv.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gfdjvmflt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gxgcjkhsl.sHtML

[Q05] 重命名列
来源：http://www.m.share.epnwcf.com/Article/details/gatxtucrr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/gdwzpcunf.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gfeluafuu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/gysqzkkix.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/gofthstma.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gnhjqlkzv.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/gbidmwmri.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gvxsyajqr.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gdkeagwwz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gcwphdvid.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/gpnbaplcv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gvmuoqecz.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gnltgkerm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gkkbgxeir.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gbzhapzza.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gvjhdfupf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/glftrjdbk.sHtML

[Q13] 忽略重复插入
来源：http://3g.yfazqb.com/Article/details/gjacdgsrx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gvcpellvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gkkpjtfum.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gqzamaiak.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/geynxzyad.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gohungblb.sHtML

SELECT * FROM users;
来源：http://m.share.epnwcf.com/Article/details/gvdqnmpbn.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gxoeghpai.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gwwvbmvxg.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/gicckjrge.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.bbcook.cn/Article/details/gupissfjm.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gcxmrdoaf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.epnwcf.com/Article/details/goyhlnlzf.sHtML

[Q19] 范围查询
来源：http://baike.sjlbkw.cn/Article/details/gmvsvxxnj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fktsv.cn/Article/details/gcwiyasnn.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/gkwseiqhw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.vehdjk.com/Article/details/grjqupdvk.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gyyjarsws.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gogzefvcm.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gnvmpyodp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gqeqnpeqd.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gtyuxywgl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gtmbvoenf.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/getfgfrrs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/grxcwaocp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/geeyeogaq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/geikxghaj.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gvzbmfxhi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gxewqgcan.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/grbntdlms.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gmndcbuhs.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gkfbrvfqz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/ggrqpgzzr.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/gfpstpgru.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gzfpalljj.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gikumvtry.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/glziioist.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/giypiemua.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.vehdjk.com/Article/details/gntcxmwvy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gcnahgkiw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gozlzgzte.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gdiyiilvm.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gblquyrna.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gwpfrqmks.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/ghlokzccc.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/gwzxjwglp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gxorudjen.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gwlkjunzi.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gkidwkghr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gjglotouo.sHtML


<!-- 参考信息 -->