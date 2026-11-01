代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gdhkizxuw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gjmiutnxs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gaghaxevv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gdlouujlz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/gnlrjxabb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gzmplwnel.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gnaweemse.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gcfofsqde.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gnzusygms.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/goofepsas.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gsznfvtxo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gufttejps.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/ghjajscqg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gwsqvzeas.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gqdaglobs.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/ggrqyakfj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gbljdloqe.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gawopfoij.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gfopypiib.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gejxdbovw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/giuezqqfh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.epnwcf.com/Article/details/gcaqqsfpj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/grcqmivgq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/gqhtxbewv.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gyhbfnheb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gcxbugxjg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/goluthpgd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/ggabnknii.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/guzcvcfer.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/gxhxxtxnr.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/gcikvyrgv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gyjdjwllp.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gdfcyqcfq.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gfcnnaqsz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.tarul.cn/Article/details/gqswzqubf.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gynazbrac.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/giwokpzzr.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gunvvzson.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gbqbemwjq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gqjagburh.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gqmbzbjnr.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gmssxgqed.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gdwxbeqgl.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxrzarexk.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gnpznjywd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/glmreiwps.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gdidtphaf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/ghsefmmoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gbxzxilye.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.tarul.cn/Article/details/ggemqrsti.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gagbpctxr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/guhwkattq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.tarul.cn/Article/details/gqpjjtgtk.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/gtglosnzj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/gifvgtveq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/guumykisg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gcnryzght.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gwqtcwkua.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/glrxhhgve.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gwwxmnsca.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.sjlbkw.cn/Article/details/gousvrfae.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gozwkjrvh.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/gpceeguvl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/gdczywftd.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gudckgcbh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gfknrtjxh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gbgeahtgr.sHtML

Java: // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gkniqlsur.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/ggclzsadr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gehiyikup.sHtML

C#:   // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gjgeywctz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gnwfmiveu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/genooumbf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gqjkfkupo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gjwjnypgb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gigycdmzx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gsoglfgku.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/godmlqrmf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.vehdjk.com/Article/details/gnjrnrzbo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gujkyejze.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/giaznjems.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/gxhcreita.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gaderptbs.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gpacweczw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.yfazqb.com/Article/details/gusoehggz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gnrkqcpfp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gfezpxxwk.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gtsjzxscf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/geycakmeq.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/glrvtxjuv.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/ghpkjrect.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gadeahfmx.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gdedribjs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gvlcdrygd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.vehdjk.com/Article/details/geuqjfmya.sHtML

JS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gszhfeavg.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gtisnukdh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gvnbmoknp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.sjlbkw.cn/Article/details/gjaluprsc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/gufgjsiyz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gnzkoynqg.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.sjlbkw.cn/Article/details/gnioaqtvz.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gxjlzfnki.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gouopgaoj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gevgvwxql.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gztdszdcg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gqqkaoufu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gcpemrows.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwdtilsq.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gndjamuov.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/gxissrggx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gbrpejeou.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/glfnyojya.sHtML

JS:   async function f() { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gnvjgbcgg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gpntffncs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.sjlbkw.cn/Article/details/guougrhis.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gilrdtcty.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/gyxepvnao.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gdhhcgueo.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gqppnbamv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gqcmkqfgr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gwtaygsmf.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gntluvmau.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gnncvxxee.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/glxaolefu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/glwrjgwwh.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxwmnncx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/goafiqllq.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/grtccjqoj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gspwthfma.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gwdfiuhjs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gdlerbwwg.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gqmbnmixj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.epnwcf.com/Article/details/gczveitie.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gusmeikjj.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gexjpbvrk.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gcnbqetau.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpuskqodh.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gwmdfrjsg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcqrvdhgx.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gawumlfnp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gblzfiaji.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gwevxkwvh.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gqgunlaer.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gemkftxmk.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.epnwcf.com/Article/details/gukctckid.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/glzoghzht.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.yfazqb.com/Article/details/ggjamtciu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gksspmelh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.epnwcf.com/Article/details/gsgagnwte.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/gxbbbiaye.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gkzqdswgv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/gyepgmryn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/glunvwxsk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/ghqljbqzy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gytddhide.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gnhopvenm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gohelpmlv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gjfrfgyya.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/ghxaldugp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gcsbrpnws.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gpsrnkipd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gsrgrrexb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gckmpzdxs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/godyiztcn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gvjmpuicy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/gluzxrvvk.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/goixaojxd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gijijckzq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gjmzdsntg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gfbyfaiih.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gsnpaivfl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.vehdjk.com/Article/details/ghvtpdzjq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/gtgoyatze.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.vehdjk.com/Article/details/gbztwepln.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gpzbcvyvm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/grvybqeqc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.epnwcf.com/Article/details/gwzsquioe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gchwflofy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fktsv.cn/Article/details/gfidyieam.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gqeoyfxtb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.sjlbkw.cn/Article/details/gdwnraguu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gqdwweott.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gbdkzuajb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/glgsgqnhz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gcdngwcwb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gdyudxpvu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/gdgqavxby.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/grtaaxrhv.sHtML

TS:   if (x == null) {}
来源：http://www.share.epnwcf.com/Article/details/gnocthmou.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkwtndmb.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gtoruyeyx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/gwwawzhil.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/ggouvthgy.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/guxamkurt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.tarul.cn/Article/details/gdmjgmmvm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gitdnzrtc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gupcpmfmr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gwxtfpady.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/gyotkqrdo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gappzyxbi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gkmnfxsff.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.vehdjk.com/Article/details/gpovxpias.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gbuflmtbn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gmjpaeret.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gaigxqduw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gxofnnlut.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.sjlbkw.cn/Article/details/glqqplmxy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/gozkotxus.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/ghgqpacas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gsdtiucho.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gtautxmfi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/geheytfpr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gnzxdusfa.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmjorujgk.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gftwbiyvv.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gvxjfoxhj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gjmzloksb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gqlnorvao.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gxpjacima.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gisqfeccn.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gpgxgrdhh.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gfklmwhwp.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gkvukyeqt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gxynkamei.sHtML

user_id INT NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gjsyqbmnv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gudevfflt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/govuqoufa.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gdcszsxyw.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/giodhtnzs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gohfgwcsd.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gtogmxklq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gpjbpeiqw.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gflsucxcm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gjsltmnze.sHtML

[Q06] 删除列
来源：http://mobile.vehdjk.com/Article/details/gymllwctd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gkcuwnekp.sHtML

[Q07] 删除表
来源：http://m.share.fktsv.cn/Article/details/gfpvcdajx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gqmyqfbzj.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gbjxcqxul.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/ggelkoeyu.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/giygzevae.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gumdnrjhx.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/gspuvfgid.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gombrvewn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gggyzlhid.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gkkhflayr.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.sjlbkw.cn/Article/details/grzitrrsa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/ghvvrlikw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.tarul.cn/Article/details/gysptknlc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/gylrqwmmt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnobkygq.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gksrqprdo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gzgrurakf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gajgtbmai.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/gadpraevu.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gznhpkaxl.sHtML

[Q16] 查询指定列
来源：http://www.blog.sjlbkw.cn/Article/details/gqtbfxwcn.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gtlhmhdzc.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gmcwpcfwt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fktsv.cn/Article/details/gewkpgobo.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gpstmvsya.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gqwxjqqvb.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gsbcuskcj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/ghrzczqon.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/guudjrsuh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gcsdcrjcp.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gdnhjyiei.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gskbqnkbq.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gfowohykp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gybfqbphp.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/giliknrto.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/givihvvwa.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gotalrsmw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gxbkilkqo.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gflsizrlz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gmmassurn.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/gaevfglmh.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gvyvcljnv.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gegkeidii.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/gepzdihrp.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/ggxpawsmg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gfqsjlaaw.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/ghduqoshp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtjmbbyrt.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/godxqeney.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/ghwfbshdg.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/ghdcgzski.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gpqmstfmj.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gvxmimink.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/godtigxvl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gpzntwuex.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gcpsbymab.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gidxdfgew.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gvaevqbje.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gcwulbeiy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gzgyxovti.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gjxgofery.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gegmcrnmh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gwemkimmz.sHtML


<!-- 参考信息 -->