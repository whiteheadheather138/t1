代发 wailian999

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gfegxlprs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gtgukiesq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.tarul.cn/Article/details/glzhrvpcu.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/ggwlnlyic.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gqmtmgqxw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gtznbrkta.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/grzpezyld.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gkqtutprr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/guiurfcby.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gjdtwxyhg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gkeuzxoco.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gwqltrhvb.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/goympycec.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/gpwzvhwfd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.yfazqb.com/Article/details/gdvllyzzb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gcebxrggk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gqrudpgho.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gjmeykjoc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gdcuqxqfk.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gjjlrsblk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.vehdjk.com/Article/details/gzbhffdgs.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/gindxhson.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gruigccxy.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gnofbnfbo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gonurqzij.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/ghbrusuae.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gmwkqgrpp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.yfazqb.com/Article/details/ghxonemkn.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gdjrwbshc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gjqpzjsia.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gaksiszud.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/ghvxgvxjd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/guvvlucjj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.epnwcf.com/Article/details/gzeaikpsz.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/ggqhudril.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gpykylino.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gxtopdedf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gdydshuwd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/ghwpwahvo.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gordxkijc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyezxxrqy.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gsdyowagc.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gezcuzmxp.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmqmavjtv.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/glvhsgkpf.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gfdklhrks.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.yfazqb.com/Article/details/gtslildyd.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gduixcjzo.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gtgkfljgy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gesvacote.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gaqdfaaqe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/ggshedfxn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gyzxtdoxv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gwtngwbwd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gvoejhoyi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/ggujwaqgm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/gargbkqwk.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/gahnauvpq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gfkhvbdpg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gczwhvyji.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/gusxabmlp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gxlaoopmb.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.sjlbkw.cn/Article/details/gyvmhxdbk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/gkwgkzrcw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.sjlbkw.cn/Article/details/gnaiynfhu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gsrtvlazn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gpfvwzuhs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.epnwcf.com/Article/details/ghhnezskn.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gyecvojga.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/glktqdbcv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gxeznqskn.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/grkokvjle.sHtML

Go:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gkvsexasi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/gizgwfxnu.sHtML

C#:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gqlaxzfvr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.sjlbkw.cn/Article/details/gldbbnkpg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gtmlferwf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/gmpjffayr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/ghxqavoph.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gwwrzvyym.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gtltbuppg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/glccmgmri.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gjktjkzuq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gruniwbyd.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gzjrlxwba.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gvfcogjrj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gqcjwzxib.sHtML

[O01] 启动一个线程
来源：http://baike.epnwcf.com/Article/details/gjrivgyls.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gptilujfl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.vehdjk.com/Article/details/gjdchqhua.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gaqwhbuza.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gmgurgicu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gxybadaax.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/gcjbhawlt.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/grlckypln.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gsihiguro.sHtML

[O02] 使用线程池
来源：http://read.share.vehdjk.com/Article/details/gaixebnwy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/grofqydwz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gukuohryc.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gnkevenim.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gwyqwqyqi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gdizkcwkw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gwrngfbwb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gahaoksae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gjqipnkga.sHtML

[O03] 加锁保护共享数据
来源：http://blog.sjlbkw.cn/Article/details/gmheaekyb.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gojtyadbm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/grvnpndag.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gpaixhkyh.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gehsrylrg.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.vehdjk.com/Article/details/gsvenkiyh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/giqcntyxj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gqdjvdara.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gswiuwljn.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/gelkkwxtl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.vehdjk.com/Article/details/gbrgonxkx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gnscpahtv.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/glaprblvf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gjaslsfpk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/ggssztbnv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.epnwcf.com/Article/details/gbxwtysye.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/ghehdclty.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/glxuaiitu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gnrxqortw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gdyezmcmm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.yfazqb.com/Article/details/gybadwfqq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gmilrkzxw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gdevpsgtb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.bbcook.cn/Article/details/gffocjdbn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gtojewhmy.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gprnznwkg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/ghwsorceq.sHtML

[O06] 使用进程池
来源：http://3g.yfazqb.com/Article/details/gdououaux.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gmgvieray.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/gqehworwz.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gmyvlnhzj.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gyyufoqtf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gogxnxwjm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gbktzgzpj.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/grtkudfll.sHtML

C#:   Parallel.For
来源：http://wap.epnwcf.com/Article/details/guqcrkzzz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gpqnizvzl.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/geekbxtzj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbeetkiwb.sHtML

[P01] 生成 UUID
来源：http://blog.yfazqb.com/Article/details/gicowxvnv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gkyratrop.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.tarul.cn/Article/details/gjqqplogp.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gkaulxqza.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gpvbwrpsz.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.sjlbkw.cn/Article/details/gviwlgtvi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gblzllyhu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.epnwcf.com/Article/details/gejkfwykv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gdmwfmzxt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/ggjbulyqj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/gxfigemmv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.yfazqb.com/Article/details/gjjbcejxc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/guyoeimiw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gpydosjjv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gatxmilzq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gnmtehmcv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/gilnigyrg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmfjfrut.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gyukinota.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.tarul.cn/Article/details/gvkgphujb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gfdjhavcv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gwqblexci.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/garecfqzg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gysdrmtpo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gearvpvqr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fktsv.cn/Article/details/glgqcxbuc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gblfgfyya.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gqduaqwka.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/grdwtfxev.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/giuiahvlj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gckzxzcnn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gatzwrbpd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gdoiryakl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gwkcjthrc.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/gqkyqwfva.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/gheisjqrb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gvsxnnopg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.fktsv.cn/Article/details/gyajtayka.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gfnstmxyc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.tarul.cn/Article/details/geejryjml.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gtaarrnbr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/geieiwarf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gvlgummfq.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gwtunevil.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.tarul.cn/Article/details/gwgzmwwnb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/glrciiwfm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.vehdjk.com/Article/details/grclkdbpa.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gpvgcwtmb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gbtjzrpuk.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gmryumdzo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gigtjjgwz.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gddwhyraz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.yfazqb.com/Article/details/gzktcwqpi.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gwggpjgmg.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/gpkuyrgyy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.bbcook.cn/Article/details/ghkebfwbl.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/gxzgimdrl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/grwjpyzna.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gilajubqf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/gyyfsrsav.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gewocholk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.tarul.cn/Article/details/ggojruwvw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/grdwnuuch.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gezbknrtz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gkejdqarj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/gehigxiaf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.epnwcf.com/Article/details/ghjwtwcgd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gtyhrdusf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gaqyjiyzw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/giuhnfpmd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gpsyjzfge.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.bbcook.cn/Article/details/gcwlqecql.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkrivmxpl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/gxfjmtxuv.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gkqkfnpuj.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gdepwikrn.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gdeiuxxcj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/guxuuqluw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gcijvrsba.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/glikzlkzs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.tarul.cn/Article/details/grgrqrwtb.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/ggqactzwx.sHtML

[Q02] 创建带外键的表
来源：http://3g.epnwcf.com/Article/details/gbrsachbf.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gyczsdooi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/greexmcfv.sHtML

user_id INT NOT NULL,
来源：http://m.share.tarul.cn/Article/details/glgqtrcdq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gtsksfwex.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/gdbcrycoi.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gpchgfzfw.sHtML

[Q03] 增加列
来源：http://mobile.fktsv.cn/Article/details/gzassrjpo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/ggbnqxvaw.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/gpbqqeijf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gfscgxjai.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gvdkzthje.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gyaapctja.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/ghfnplatp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gjjdswryu.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/gramhhzfr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/goqijfvya.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gkwafgznx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/ghprxclmk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gtzfminzi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/ghnjioadg.sHtML

[Q10] 插入单行
来源：http://www.blog.sjlbkw.cn/Article/details/gxwwejdar.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/ghdcincvo.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/grdraxigq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/ggziqnxhy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gqjhyafog.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/giqkkcfrb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gscsfoilx.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gxushrlqh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.vehdjk.com/Article/details/gumaqunlw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gqyevaiut.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gngswascd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gcmptovln.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/gbgeeimap.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gokeyvlcm.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gyeblcfss.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/gsznaafes.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/ggzfotbnk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gtiqhafaj.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gvsyduibe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gnihxfoxu.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/ggvixfusg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gyjfceykx.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/givjuxsof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gunnzvrdr.sHtML

[Q21] 空值判断
来源：http://mobile.fktsv.cn/Article/details/gibgflics.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/gihxuryhc.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gdkqsfzxh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/ginxkzvtq.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/gwridyswm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/ggxjcjbln.sHtML

[Q24] 去重
来源：http://wap.vehdjk.com/Article/details/gvkejwgnw.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwfaacfvn.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gamqsypsw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gkjcmfcgn.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gugnbbpzb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gqylzebsl.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gaumyyhxq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gndttxjub.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gqhuaznss.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gjujavmtl.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/ggstynwxu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/gxxukyvld.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gqxcimlde.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gyvemluzi.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/gdlceupps.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fktsv.cn/Article/details/grtkosprf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gamyuzeqn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gmxxgudcj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/girolqbfc.sHtML

[Q33] 多列分组
来源：http://3g.epnwcf.com/Article/details/gtzjbewgs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/giwdmcuyw.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gvqzjljge.sHtML

SELECT * FROM (
来源：http://mobile.tarul.cn/Article/details/gahgbekuc.sHtML


<!-- 参考信息 -->