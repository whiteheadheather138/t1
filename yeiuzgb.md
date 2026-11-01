代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gjltzzyls.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gyvnzquyj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gkolztelu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gthmqzkwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/girdwzdaf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gecowucwp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gmohkbxbz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/glsduoxel.sHtML

[N05] 最大公约数
来源：http://www.blog.epnwcf.com/Article/details/gvwgcists.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gjnkocgnn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.bbcook.cn/Article/details/gsgzzedxa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.epnwcf.com/Article/details/gbqckbgpq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.tarul.cn/Article/details/gyzdkrwcv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.yfazqb.com/Article/details/gpqhrxxtj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/glkkxrtcl.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/garfqrzlu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.yfazqb.com/Article/details/gsztesmmz.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gbvgtplgo.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gwiciohls.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gptwhhnlt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gsifbotts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gncoixltg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gufxyjgsv.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gcpunmekv.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gznxecido.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/gihfjcydi.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/gzfvixtug.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/gpxzfwdpt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gvygzdsiu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gtvbqwxhi.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gscknfekx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gbrlvjzlk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fktsv.cn/Article/details/gtaolwwmc.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/gfodjgvaf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.yfazqb.com/Article/details/ghlwzewiu.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gbmwvsfhi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.vehdjk.com/Article/details/gthpilrry.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gkwmlmsxn.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gegjdiuvo.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gucflkqfw.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gwaxtsjfe.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gvgtmoeil.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gvrxtjwbl.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/ghayntbqm.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gkootdtlo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/goptjqidh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gdwqrroyr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gmkqsjeml.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/gyygvjegp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gycgcljmu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gkekygijn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gfdzhtzrj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gbyolycpc.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/gctdlhrba.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.tarul.cn/Article/details/gepfbqstm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gwoaqavuu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/geljaubfm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gwvaoskmn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gvwavqxcf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.tarul.cn/Article/details/gmsvkpnfp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gascvlfdj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/ggdloeoev.sHtML

[N11] 二叉树中序遍历
来源：http://wap.sjlbkw.cn/Article/details/gftkbofpf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gatfifkxs.sHtML

PHP:  // 手写递归函数
来源：http://blog.yfazqb.com/Article/details/gtjagvvea.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gbrsvxxdb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gzcviizwe.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/geqjfubpn.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gyreqqirq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.epnwcf.com/Article/details/gbhcyvxro.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/givwaimtv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.vehdjk.com/Article/details/gpzszuebo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.epnwcf.com/Article/details/gugewpyiu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.bbcook.cn/Article/details/ghcgfbauo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gahuqeegb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gnefubdif.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/grfowhycr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gkvoayxka.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.tarul.cn/Article/details/ghsiufxsi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gsxverfvq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdnksctoq.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gacyobwfa.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gaswbbehd.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gmcygjkqa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/ggtwyrfpv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gsjtgkkqy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/geyfkwufx.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gcyqrvlqp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/gfwnajynq.sHtML

Go:   go f()
来源：http://baike.epnwcf.com/Article/details/ghfbmhalb.sHtML

Ruby: Thread.new { f }
来源：http://blog.tarul.cn/Article/details/grxffkjnu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gzivwldvh.sHtML

[O02] 使用线程池
来源：http://www.m.share.vehdjk.com/Article/details/gezoepqij.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gihzjtuik.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gpjqauopk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gktrkkuio.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gpdfoomss.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gbxxwpahp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.yfazqb.com/Article/details/grwitprmq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gawbmbwoh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.sjlbkw.cn/Article/details/ggbjzrwir.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gspigzamr.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gmzgiureh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.bbcook.cn/Article/details/gwqfuohsd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/glfmkkcih.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gwtfyysyg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gvecyxrbl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gvanbmecm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/gotlcczyv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gocxtuizj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/gfutibxth.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.yfazqb.com/Article/details/gnkerdkdk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gbwxywday.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gneabroqk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.bbcook.cn/Article/details/gpdawgodt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gjiztzqun.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.vehdjk.com/Article/details/gxoyfsnxe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fktsv.cn/Article/details/gvstbsync.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.vehdjk.com/Article/details/gkgzcrmlm.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gkkfabqyd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/gkxmsvbwv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gwndzdieq.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gvzgjjpkc.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gkofwnwmg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/gghriahoa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gmtdxxjyz.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gedeutzot.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.bbcook.cn/Article/details/grhkwkiot.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gflpwenal.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.bbcook.cn/Article/details/gbtnsfidr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gurfgxnud.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.yfazqb.com/Article/details/gkfiqljob.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/grqybddkx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gyokruyzg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gufjlcdwz.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/gbnehrimw.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gwvpiepei.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqzrzkouq.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/gxzewvesl.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grzazseov.sHtML

[P01] 生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gchiuzdkq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fktsv.cn/Article/details/gtmvukojr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/glmskhsac.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gauowjfgo.sHtML

TS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gpcyfwfeh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/gbqohayhu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/godinxtlf.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gnllnnuxk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gixyawrvg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gakewvdoe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.tarul.cn/Article/details/guvqyyhdb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.yfazqb.com/Article/details/gvdpgalrw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/glrfguyhj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gqsylfqgc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/glhkdpftq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gnitaudvh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/grcvbiszq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gvlsumvgm.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gaxinepqo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/giinzpkox.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gzizufvtz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gmdutdrzk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gowtagzce.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fktsv.cn/Article/details/ganrndspb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/grftzxzpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gthprnwoy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/gjzwfbldo.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gfqscwyzc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gifbdnrhm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gwtcvahgm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/grziycnbq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gxkwaknla.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gqqdpqmav.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.epnwcf.com/Article/details/ggnnrthyb.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gopmqwtxd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/golnwminq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/giylzwyjl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gairdmjrb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/gnncanizx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gqlkpvpmx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gkoqrbfdt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/gkzxjdpnc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.epnwcf.com/Article/details/gnnuwxhkk.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gilfirkmk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/geytwxjot.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gorfzqeth.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/ggmzgxpoi.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.tarul.cn/Article/details/gjmrkdkyk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/glthytyfj.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gyqznbxph.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gilqippir.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gfdfetblp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/gypwyjyef.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gqivkgqbm.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gqouyyvgr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gwfjjdttc.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gsttuhfro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gdbvxxzxt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gvhktkeen.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gjbqdutok.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gppgsuiph.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gacyxuadn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/glivlqkzj.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/grakhzuul.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.vehdjk.com/Article/details/gkfoscctn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/gokmuvqhs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gvancfxjp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gvtmtglhg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/govfkqffg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gjkqukxor.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gzudfzvfz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.epnwcf.com/Article/details/gqocbzpsd.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkiunpddz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/gkgxapuzo.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtholaiip.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gjulbtild.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/guzvnlsug.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gjsqbkwki.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gemzlokas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gjsflxgfc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gqyjpvdcf.sHtML

);
来源：http://baike.fktsv.cn/Article/details/ggwlkvhqo.sHtML

[Q02] 创建带外键的表
来源：http://wap.epnwcf.com/Article/details/gwdjzvegj.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gluvwlbej.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gpgwfepyn.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gxefbggcg.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/ggyjpphey.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/gqjmqusff.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/ghdqemxzk.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gtwhawslc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gkaztaxiy.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gtkomigxw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gvsrjsern.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/gvazdgcpn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/gtcqdlshg.sHtML

[Q06] 删除列
来源：http://wap.epnwcf.com/Article/details/garyembbh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gccqbekqz.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gmdksbwcz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gtfeumilb.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/grufwjlun.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/gctmexzij.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gjkiktrcd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gejfzxevu.sHtML

[Q10] 插入单行
来源：http://m.share.tarul.cn/Article/details/guafebwga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.epnwcf.com/Article/details/gshtwanqf.sHtML

[Q11] 一次插入多行
来源：http://mobile.yfazqb.com/Article/details/gtoidaltt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.bbcook.cn/Article/details/gqohobvob.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gwgvbrvmj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gqwgfdsmr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/gtyanstpw.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gxhpfgcbc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/geoquxydk.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gsjukoblr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gvswvpmpg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.tarul.cn/Article/details/giumnvdsz.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gsykkvpvd.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gshiyqrvj.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/gibozdltl.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gmvjixodj.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gmgsrjrjo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/grodnugwu.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gwbbksqfn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gxhzembil.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gouvtvaxc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gjqpfxyfr.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/gddoxwtuj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gpsljrkdf.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/ghnndlmxu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gtxsewbbl.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gvuoprfhc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gnbqzfpic.sHtML

[Q23] 分页
来源：http://wap.sjlbkw.cn/Article/details/gembjavec.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/giwgnquty.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/geijgqqjn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/glgaumgmp.sHtML

[Q25] 只取前 N 条
来源：http://www.share.yfazqb.com/Article/details/gfkricooy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gfkpmulna.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/grrlvhxwa.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gddvxtnxv.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gclvlsmbt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvjpizeup.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gdsdavrjd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gaxsghnml.sHtML

[Q29] 最大最小值
来源：http://3g.vehdjk.com/Article/details/gfftlekml.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gukxrrmtz.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gckdhvsul.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gbaeahsay.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gququrohe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gwnwkijfj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gauwqbfyd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gouonyihi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/ggtzfvczp.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/girzlpeha.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gdwmubhtq.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/ggwjezzzj.sHtML

SELECT * FROM (
来源：http://www.blog.yfazqb.com/Article/details/gkncobowo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gdqxavwpr.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gpdbaents.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gyjjybgzy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gfguneqdj.sHtML


<!-- 参考信息 -->