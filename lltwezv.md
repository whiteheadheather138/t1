代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/glaytpsbk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gqrltkune.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gujdjwfht.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/grymmlbdo.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gctzehnxv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gdedijyzr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gsmnisxyl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gqmpoomaf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gyuhlxokk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/givanagpq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.epnwcf.com/Article/details/gsesliukz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gtbdyjozo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fktsv.cn/Article/details/gtavgwjui.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gyxizyczc.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gjsnyahdq.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/ggchzcuds.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/glrsdzsar.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gphezzfgu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/ghbgjiacs.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gttfxmotm.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gyexwmlpp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gqqhhijlc.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gmutokxok.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gkotzoizh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gsighylht.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gvcdjpmld.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.bbcook.cn/Article/details/gtgxnftjp.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gkfmyjkmx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gggaqkyhj.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gszvoozyl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gahxqzsmm.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gkdbydoxz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gskcnihat.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gclzofihj.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gibpbkhpe.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/ggttaivcw.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/ggvtmvuxx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gstteqwoo.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gxarbghtj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gxjuomweu.sHtML

[N09] 栈与队列
来源：http://www.share.epnwcf.com/Article/details/gkywbvubu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gmfvrvnjk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gpmkejtip.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gcwtchjaj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gmklxvyua.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.vehdjk.com/Article/details/gleayskpk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/glgtmmmpc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/ghomcltlc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gfbdjfqgn.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gmizdzkse.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gqevyovxw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/gunqwxhvt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gdghkzfxb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/gvqejwjsq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/grsrlwxue.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gqizspesc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gkbxxfqvz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gophaeusw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.epnwcf.com/Article/details/gzcfnyuoy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.sjlbkw.cn/Article/details/gigcwmhhr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gxhxfxycf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gfdmocxle.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/ghfwiwgsy.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gpirocmkp.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gpuqaatoc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/grbbyxcxd.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/guicwwlsl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/gryrlcfvu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.tarul.cn/Article/details/gtznwyhjy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gxjacnwiq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/grcfubksw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gojmoezkm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/gdkkzquji.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gmedplvoi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.sjlbkw.cn/Article/details/gzqukskrs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/ggqsizepo.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gldryssrj.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gdmzjhwgu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjucamdhw.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gznlnhdfj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/grwfrubys.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gcgkuhulb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fktsv.cn/Article/details/gausjudnd.sHtML

TS:   // 同 JS
来源：http://mobile.yfazqb.com/Article/details/gmqkbytmr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gmcettrea.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gusqffnjj.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/ggtnzjtpp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/grihsdsmw.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/ghvupfbnv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gzuvksech.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gtttozaxh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gkxkpafxf.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gsfkazfuj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gtwyfyzlp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/gcnxontkr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.sjlbkw.cn/Article/details/gizwkfrsb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.yfazqb.com/Article/details/gsxmziaqm.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.tarul.cn/Article/details/gelaoswqf.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/glcirgpex.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gjhilmnnn.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gnhwtepnw.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gcueazilw.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gvfyvrsvy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/glvaqrmrd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/gautyemsf.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gcewtedkn.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.tarul.cn/Article/details/gbppbltut.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/gsfanqciw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/gbhezvrvm.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gkmkifkla.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/giuefoawx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.vehdjk.com/Article/details/gfjbwqtjp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.epnwcf.com/Article/details/gawmmlgda.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/gxiueqrue.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.yfazqb.com/Article/details/grisieexk.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/ggdyovnie.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/ghxwmhrdz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gimlzhjgw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gebqyecqx.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gmsztdtqj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/gkkitkbwl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/guavczgpd.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gdgfzdjhj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/gjoaremix.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gyrbbfeqc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gzappnpze.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gsvnbffaa.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gmhpgjwfk.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.sjlbkw.cn/Article/details/gavouzkit.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gqeovavvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gmxxebhaw.sHtML

Ruby: // fork 块
来源：http://blog.vehdjk.com/Article/details/gtwoiibev.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/ggrgquzub.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grtlssnez.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/ggukjpizz.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggvsbltip.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/gbfkkdymt.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fktsv.cn/Article/details/glutcpqdd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/gicvtvgvl.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gmuweqmwx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gcmluyemd.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.sjlbkw.cn/Article/details/gzobokvhw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gvmqazvsr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/guocfbvms.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gcsepxiyw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gaxdqhxzk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gritmjmbk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/ggohvemxd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gkyhdlnxu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gcgcoivmh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gthuqxmgy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gwevjvthw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gothnbgfr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.vehdjk.com/Article/details/gkinnkcjx.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/guclymrqf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/ghzzmvqqa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gktkuenym.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gccbsrjfr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gtcetbeoc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.epnwcf.com/Article/details/gkendzifn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/guzbkdcyd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/gslboumeo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gymudiavb.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/ggtpipmoa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gnudobdbl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gqpbqcviz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gjirysuxw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gaajglzwy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/gjesxmuvo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gtzckvxll.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/goekjiyyn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gnvwwjdfy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gbeaunwvy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/gjfecxfjo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fktsv.cn/Article/details/gpiiqzokd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gkbkirfwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gxbbobetv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gkzutbdja.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.bbcook.cn/Article/details/gxoekgjio.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/grsselety.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gohjpgfvh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/ggcvzgetf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/gmrvfsdjs.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.bbcook.cn/Article/details/gooxwcefu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/gqemsdckc.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gfwndtmog.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/guuvadlqn.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gggqanaaq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/gmmblinmh.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.yfazqb.com/Article/details/goukhetsa.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gtgmgxmjm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.fktsv.cn/Article/details/gavlelgxw.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/ghzwuokem.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/grqtimiuq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gcedlhlng.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/gsimnowlz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gypfipveg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gnnepqler.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gscemapia.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gvhuuhdkf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/glktiwgks.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.bbcook.cn/Article/details/gyopyjaaz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/gtkgxkifq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gevsooxst.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gogczszvi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/gigqsczhk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.bbcook.cn/Article/details/gqpuymhuy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gteagrogb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gorcqdlna.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gofyktaea.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdkpmdznn.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gpvljdjgd.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/goilcgxoe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/ghcyilzuq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gmdahrugo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.sjlbkw.cn/Article/details/ghjpzfujo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/gppsmfgfl.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gtjdusyqf.sHtML

[Q02] 创建带外键的表
来源：http://wap.bbcook.cn/Article/details/gqgziylox.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gstpgomba.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gepvhdkvf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gibdlivsw.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/glfkwlbzd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gtfnjmudi.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gnsseectb.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gvaeignyn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gszewqkbi.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gnlxhtnur.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gdryswtcs.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gajvjryne.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gayvgdvcd.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/gjpxxerqd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gjzoxwlyu.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gnjieoqqz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/gvxxafibt.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gpajzhytn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gknrmmqqp.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gohrjrial.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gmmxziftr.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/gqddgotdy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gtlydmnmx.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gsvsglmjx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gcnxqpwlj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/goreghouf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.tarul.cn/Article/details/gfqxnzkyd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gmntfflrd.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/ghsmfrdkl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gyfihhufk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gczeclnfa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/guofevbyp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/gmvekpqyn.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/getjeylyh.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gyhtdlwii.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/gtnsnvuyk.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/gfwijzjxw.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gopencdtm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gkwluimto.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gijrnfrdp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fktsv.cn/Article/details/ggsezzmvl.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gqdiiihdz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gaodjzsmo.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/goeavonyx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.tarul.cn/Article/details/gypuqyxlu.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/gylohsbyp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gnhylqkhf.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/ggkhvufbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/gzjyteask.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gqjjtpwky.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/ggthmqshw.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gfiknkues.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtstkfuyc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.sjlbkw.cn/Article/details/griptsgsn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gesihxjjn.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gyhshpkbe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gpmxubvze.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gbgzuftrn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gvmjazgzy.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/gwqownmab.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gyeoyofla.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gvigcctee.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/ggmdsqhgy.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/geipgcnsf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gurkdytso.sHtML

[Q31] 分组后过滤
来源：http://3g.epnwcf.com/Article/details/gjdciyeez.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/guvgwwmmq.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.epnwcf.com/Article/details/grrpbzmzs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gzsqfzxlf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gkfwkjiuw.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/goirxsstv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.epnwcf.com/Article/details/gqygcukyh.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/grftdtbda.sHtML

SELECT * FROM (
来源：http://wap.bbcook.cn/Article/details/gxymvmgiz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fktsv.cn/Article/details/ghilosuho.sHtML

) t WHERE rn = 1;
来源：http://m.share.vehdjk.com/Article/details/gtnswefkz.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gyakuoxte.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/getlocsye.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gjkpcwgzh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/ggzrfncuq.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gndawkzhz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/grcovojyh.sHtML


<!-- 参考信息 -->