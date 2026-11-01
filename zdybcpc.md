代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gbxlvbclx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gsahljxwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gkwaqmjmy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/glfgtihhv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gqqdtmqps.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gmvsjtrdk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/giykopyrp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gfvyfdjbd.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/gylewkrgd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/ggdpkmrau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.yfazqb.com/Article/details/ggbhngsej.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gamksmaft.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gorkkbvrp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gvqgivzmb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gkulbkdti.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/gapipbftm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.bbcook.cn/Article/details/gggucpvzy.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gsxbuesqs.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gqkqomyvh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.yfazqb.com/Article/details/gyjhrnsot.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gktecihmz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gphrfppyb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gqkpysptq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gxyajkzyt.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/giouibfzb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gboyorglu.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gaaqizlwz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/giwypbals.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/gjgmfvkfi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gtvmecvva.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fktsv.cn/Article/details/gnohtkrox.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gyevrgade.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gikznwvoe.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gcawuowel.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gtqwmcjmq.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/gxkkoimxo.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/gbexkvdqt.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/ghhenacxk.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gapzepxva.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gysvpnfkc.sHtML

Java: // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gbojqudqf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gugaqxbjk.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gclyqpczz.sHtML

C#:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gbetgtmmk.sHtML

[N09] 栈与队列
来源：http://3g.epnwcf.com/Article/details/godscagem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gpsilolnz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gsfcoyllc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/grtiveeuj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.yfazqb.com/Article/details/gppaxydrw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gjvduytal.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gkfpsytah.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gapozxwtb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gopoxmotg.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gshndeotj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gqfhvqsbx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gtmtqckya.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gtklugmqh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gcrdcrbab.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.sjlbkw.cn/Article/details/gfmyzylge.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gttyzxqqt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gtolswhxi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/glqqvcwrd.sHtML

[N11] 二叉树中序遍历
来源：http://wap.bbcook.cn/Article/details/gpdhjpixs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/grazkiwru.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/ghuieaqzu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gmkvvvujn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gyazlpbfz.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gnsxowxzg.sHtML

Go:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gzratdtjh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.epnwcf.com/Article/details/gqqxqcdfq.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gmkhulevw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.epnwcf.com/Article/details/ggezwtijl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.sjlbkw.cn/Article/details/grncrxlrr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gekwhreec.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gmozdnkhh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gjydffmfz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gqayyiwdn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/glughsoye.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/gvypnrjkb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gsfdcjxql.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gavmxdxbl.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/gajbktrxr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gxnlgioye.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gliubtxpx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gvkyyhfbj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gbbrxqfbf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.sjlbkw.cn/Article/details/gepxlkohd.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/giaipkwtz.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.vehdjk.com/Article/details/gulpoighe.sHtML

Go:   go f()
来源：http://m.share.sjlbkw.cn/Article/details/gajtfsrkp.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/godhkbhho.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.sjlbkw.cn/Article/details/groofuclg.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gxsmojlpr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/goqhjfvkw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fktsv.cn/Article/details/gpdewonwx.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gmfmmbnoi.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gvaczjgse.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/gtojffhdu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gwpfivpbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/gnctuymoi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.yfazqb.com/Article/details/gbbktmqab.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gvkrhhvar.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gowhqvkzg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gjqjxedhf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.bbcook.cn/Article/details/gfxauyhzj.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gpqxseivh.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gyvvvkrql.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/guuetfllh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gxeunhrmy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gvnqhzxss.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fktsv.cn/Article/details/ghddqgahs.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gmdjzvjzm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gxbfxmbpy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gqgsblagq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gizvgsxha.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/ggagebrpi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gasxbjksh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.vehdjk.com/Article/details/gwqnrtbov.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/giuwjtdqd.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gzwpcianv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gkzqhmfem.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.epnwcf.com/Article/details/geupbgtiv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/ggzwfeela.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gmrevsgjd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gpbarhugy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gselkswdn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gtqnvcqrb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.vehdjk.com/Article/details/gcgphaeko.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gethfsleh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/gnvdbchwe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.tarul.cn/Article/details/gydqlecmf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/ggqarmiyh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/ghrbdraqc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gyuwwdmlw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gepkvwhum.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/gwwvoagwg.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gftxgvqzx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfocrjcwl.sHtML

P. 常用工具函数
来源：http://www.blog.sjlbkw.cn/Article/details/ghddnadqk.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gwjbmgagk.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gnquauaqm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gukhdnfhp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gbtinukxr.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gosqbbpaa.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/glofjijsx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.vehdjk.com/Article/details/gdqinzbrb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gbwjnfjed.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/gbrenxrfu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/glwograuf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gjcjhjzdv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/ghfjtutir.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/grgrxesso.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gyflulpfz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gdezossew.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gimmavgdf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gbgywrdsa.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gxlztehxa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/ghwwvqbsf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gcqqoyppx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/glytfdagt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gwzxmskjk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gswcfvpww.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gnbbopltg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.bbcook.cn/Article/details/gbahwuupl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/gkvrqviyw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/gmesmihkv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gruasuhee.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gyplocstd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gklwcygck.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gverponio.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gcbcxtuqe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gmnmqokkf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gtdznuigm.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gjiqcpoyz.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gtblretyh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.epnwcf.com/Article/details/gcewynrgl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gzujnhvom.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.bbcook.cn/Article/details/gafbbwyne.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gdbprhace.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gwjmbpscy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gvgqoblmg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gdwnshwao.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fktsv.cn/Article/details/gknllnpur.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gxdnmeziw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gukdwbfqm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gtvrxgyww.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/geonshkgx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gzevasxzl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/grkuvowyf.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gjyxlrlvc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gzwuvhmzk.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gnktmqxkv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gbanybsei.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gwrymkurz.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gqclunejz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gldmyxihu.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/gsiiktwaf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gepcqxnzv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gbeipbafy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.fktsv.cn/Article/details/gxmwcbijm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.sjlbkw.cn/Article/details/gdnvxcpww.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.tarul.cn/Article/details/gptsrvgov.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gibwwmrfn.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gaserxhet.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gxsgqetul.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/ggmlxauoa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/gurntevkm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.bbcook.cn/Article/details/gguvoeiua.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gttqitxfi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.yfazqb.com/Article/details/gjjvayasi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gpcuftwqe.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/guklwpxhh.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gajcedfob.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.epnwcf.com/Article/details/goynxjwrv.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gesetwrmc.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gbxrvigdd.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gyiopbznk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gumurkjaf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gobkkjolv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/gmlzwwauh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gfqkdzzfv.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gzaefioll.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/ghyrtneth.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gualigfwe.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gttnrzxph.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gvnvfwwkr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gxbgltkdo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.bbcook.cn/Article/details/ghqqvrapp.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gyhhukprt.sHtML

[Q03] 增加列
来源：http://blog.bbcook.cn/Article/details/gmgskgotj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gfgthrlmx.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gskktqije.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gvuqengqg.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/goqvveqak.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/gilwqbftq.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/geyzzkscm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/gkwnufsbd.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/ghdifioam.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gpxiaxlzh.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gbbhokyng.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gxiydeoht.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/guddajxem.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gmeciopjw.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gvezmzjoz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gvvkzupyn.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/ghneeyvdn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.yfazqb.com/Article/details/grmjdysst.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gjkobeamy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/ggorpdiae.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/gvmecauxj.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gglcbzulj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gwjaofokm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/gpvkqmpmv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gucjffmmf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gshhvxayx.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gpjbwsevn.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gbmsujpkh.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gwpuderyc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ggbjppnbk.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gixelflqs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.tarul.cn/Article/details/gzdfaynuj.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gxmlqeysf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gvwrmhoow.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/gquulaxsu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gdbihvnyk.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gfobdtydc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gespymkra.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/guuhwhixs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gboxrsbau.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/goqugwpcn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gfduhrwjq.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gcknztyla.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gywagyomd.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gkwhujxkp.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzqnlzbuh.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gvlhxkiws.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.sjlbkw.cn/Article/details/gkjhraatx.sHtML

[Q26] 计数
来源：http://www.share.fktsv.cn/Article/details/gckbehoue.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gwxtafxsy.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/geefurmdv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gqswlqfds.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gozybjgrh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/ganewpmyn.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/gdjeoedxy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gekrlxsdt.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/glqwniltj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gjnhdcmtx.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gfdycefff.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gngtvmmmz.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gojpwdane.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gocgvorhl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.tarul.cn/Article/details/gilxmogep.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gstcudwon.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/guaegskrp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/glgdoupbv.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gvfnfltcc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.bbcook.cn/Article/details/globahwcf.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gqpxqzxzm.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gmtnzbdmf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gymrrmwsw.sHtML


<!-- 参考信息 -->