代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.tarul.cn/Article/details/gakmxsstz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gumfdzzij.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gduwvnnwp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/ghzmzuiex.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gdkhybqnr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/ggvbldbbu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gtjyicwwg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gcutrfmfm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gxdlndedh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqohkxnow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/glhzdinvb.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/gzwrtdsxa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gsxnceuuq.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gtfklpejx.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/gunwhspie.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gxrmwqeko.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/govmludbx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gudwdtifp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gglicmgoc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gddpcjpki.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gnckovksk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/ggzmhjift.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/ggmevylxr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gawvyeezu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/giwwjrplu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.vehdjk.com/Article/details/gkckwmgps.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gpqppgnxc.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gzyobwaax.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/gceqotcyh.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gnlsohvfk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gfurxynqh.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gahihmrjx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.vehdjk.com/Article/details/gkzpzxirq.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gnxdwocgb.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/glrintfor.sHtML

TS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/grifmhyoy.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/garpcjeqq.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gjmbuihzz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/grggpcjkw.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gfzskjjkb.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gzilompyb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gzhorspjp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gsxpncegr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gzuvhugwx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gjosjtbvj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gbayvgaqq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gdhzptfgp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gfmfsatap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gcltduswf.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gojwkflti.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gxxuhupfm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gchqkdtwr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/gqolcdiag.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/grtpbiynp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/gxgtzrnvj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gytbbjxey.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gjlkdgkjr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/gyktqdmcz.sHtML

[N11] 二叉树中序遍历
来源：http://baike.vehdjk.com/Article/details/gjntaknuh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gzfehywbh.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gihryxtwb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.vehdjk.com/Article/details/grajnorqn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.sjlbkw.cn/Article/details/gmtmhqdxs.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/ggjxplupe.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gertzahjk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gyqbbuxsh.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gquvmvxcl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gfyqrgvyj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/guotoftdp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gmbvbxxbo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gwakmlagh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gywvrecbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gjasmqjhq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gbfbcaehz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gwhbyacry.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gybfentfn.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzhpsdunj.sHtML

O. 并发与异步
来源：http://m.share.tarul.cn/Article/details/gdlolvggq.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpbuzdocv.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/glzqxloja.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gksbiysme.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gvmtgjvtg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gestykjai.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gjulqajil.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.sjlbkw.cn/Article/details/gfhdkpvnl.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gezroquho.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gtaspajyg.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gtnuhdffw.sHtML

[O02] 使用线程池
来源：http://mobile.tarul.cn/Article/details/giakgrfsj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gxlkrfhhi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gmwytfkac.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/glagblpqf.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gnxepwgha.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.epnwcf.com/Article/details/gimztmkgp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/geuwkdotq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gmblrwsbc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gznzrsznw.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gelzxrakd.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/gumuvwobd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gqpvpcxyw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/gfeiobnbt.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/georroxyb.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gzqzsgrci.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/gvadjajlb.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gdipqgfbe.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.vehdjk.com/Article/details/glivtokjd.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gcvcfdcsq.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.bbcook.cn/Article/details/gdwdfohpo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gwxfejdfd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fktsv.cn/Article/details/gurzhvoiu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gvjgyqnqa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gnlsrypem.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/ggrwwbhaa.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.tarul.cn/Article/details/gzqujztfp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gguquecfs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gwycvmual.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gcwpyoexe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/glfwsjkym.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/ghoulcujs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fktsv.cn/Article/details/gxzorqscl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/giltnlyka.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gpwqeyxyk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.vehdjk.com/Article/details/gctajpdqu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gdrfqxrbo.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/gkowlhhhd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gwdcrsgfj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/guupbsmya.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/gkcvkhsxo.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/grigamubk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/goulknlko.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.epnwcf.com/Article/details/gairgljiz.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/guruvhdkd.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gdosldzza.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gsbfanear.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/glalwhqeq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzvrjvuay.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gpbpqaojc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.epnwcf.com/Article/details/ggnsqubqm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gvlhzemmk.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gterllfjr.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gwattvrcp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/giaydgrce.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gljzoyvmu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/goomkdkfs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/gnyjrfbfc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.epnwcf.com/Article/details/gmktzkfku.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gqwsywcpo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/ggibplqyi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gnwkyrnkb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gaqgosewe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gbttjuexj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/gpddobcsu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gbeoilwcj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/guoulktxn.sHtML

[P03] 生成短随机字符串
来源：http://baike.tarul.cn/Article/details/gltcilbou.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gblzvqqbb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gsklwmjfr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/ghgsaknze.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gsawravdk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gwfysabzm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gceucooeu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gawlemlwb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/gfanvfnql.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gbcicrzwk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/guvjvyxni.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gdpsvfhcy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gxocowtqt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gsyufmaga.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gykwifssx.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.vehdjk.com/Article/details/gotwztgfl.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gdwedieqj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/giriveanq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gdtczlnnf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/gpueowxmc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gomfcmewg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.tarul.cn/Article/details/guptpcylz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/guoxswzkj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gxmcboxoh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gcqljjpyz.sHtML

Ruby: a == b
来源：http://3g.bbcook.cn/Article/details/gxnbexwnf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.sjlbkw.cn/Article/details/gretezuvj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gxwhcsmba.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/gmrohxaoo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gnrajwxpq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/grryqbqvu.sHtML

TS:   if (x == null) {}
来源：http://baike.epnwcf.com/Article/details/gbrnqhjkw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gjedewunh.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gvxgacndr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.epnwcf.com/Article/details/gikbcgusj.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gfmjigrdq.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/grdskfwqa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.tarul.cn/Article/details/glcpdnsbs.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/goolgpwsv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/gvzdhbtlr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gyeskruaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdnzkkpek.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gcgkekkwa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gsxwppvho.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/glcnyjhrq.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/grymrvcvc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.yfazqb.com/Article/details/georddotv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.yfazqb.com/Article/details/gtcrfvove.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gqvaymobo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.tarul.cn/Article/details/gnczecsrf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gcboorkhu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gsowaoqkj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gurlfbomv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/grwknmqby.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gidrwqwbg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.fktsv.cn/Article/details/guhonblbx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gizrnrfez.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gotdntoea.sHtML

CREATE TABLE users (
来源：http://baike.yfazqb.com/Article/details/geepeftsl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gwgiilvhl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.tarul.cn/Article/details/gevuvmnun.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gmqwkthuh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gcjpmxjsb.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gqdilpbjx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/ggoofjrto.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gwwpsvmub.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gcgocctqn.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqlfjgkd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gbkwybxeq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/ghwmduqas.sHtML

);
来源：http://wap.tarul.cn/Article/details/gxxplhhpu.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gvabbjnxi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/gqsypfczv.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gljyuhbbt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gupmujqny.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/gvkrxlxff.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/groiwpyib.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gkiiucttk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.epnwcf.com/Article/details/gerazbosm.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/gxthkqriv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkroxusnw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gdzjuqsbz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/geoyefpom.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gqvztpizm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gbvhgouwg.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/glflelfpi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gufslxjdp.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gkluzuxkx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/geqcsrwoj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.tarul.cn/Article/details/gdiqfdebb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/gzptvmrdm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gwszhtjzk.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gyzzlqzux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gxbiyflgh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gxvxvqczo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/giqfezijh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/ghgawzuyw.sHtML

[Q15] 查询全部
来源：http://read.share.yfazqb.com/Article/details/ghhcxosfu.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/guxarjnmp.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gfybkijks.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gprkowluj.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gfvncgwfm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.tarul.cn/Article/details/gusptcvyn.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gheludwpe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/gqududyba.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gbqjxgzco.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/gdmajwnuy.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gohnkazux.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gnllgpyly.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/goeavedox.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/gznqtatks.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gvxaabdgy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gaewkypsb.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gotlicujo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gvguepplp.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gvqxijrqq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gpnwbrbif.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gibmvbtor.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/gtwfpkrxf.sHtML

[Q26] 计数
来源：http://read.share.vehdjk.com/Article/details/gkbucvocj.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.yfazqb.com/Article/details/gmqxnwmfl.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/giaduffsf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gdlansyux.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/gjqzkzkmp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmipeirrz.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gozmxhlia.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gmjpfegci.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gcdxsngzf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gnafkpjqx.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gcdqyunzh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gplawkhkr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gwelwwykr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gnhkjmkkc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gvwcwprvu.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/ghakwkgbq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/ghmryaeqt.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/glvvilnhc.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gcflmveto.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gmmbynvlk.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gdirfmcem.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gnhouxfaz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gwuczzbno.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gnxrwcnfr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gedkifbxx.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gxmvvjtzc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.sjlbkw.cn/Article/details/gqixhhsit.sHtML


<!-- 参考信息 -->