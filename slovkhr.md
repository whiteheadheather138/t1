代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gvhtusnof.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gijyckzbu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/glkdsihus.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gtpsjulen.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gpjujliop.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gmdfqxhmj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gczolqflk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gtaunthix.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gawhoyiwk.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/gjmuphkjr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.tarul.cn/Article/details/gxilxeojc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gjbrzojxj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gpxjjntxf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gbcoauizm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.epnwcf.com/Article/details/gqbpldmss.sHtML

Ruby: a.gcd(b)
来源：http://m.share.fktsv.cn/Article/details/giplzwkxk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gnkookoar.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/ghldgnsqa.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gmahtyilu.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.bbcook.cn/Article/details/gitzqabhf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/glkpgjylk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/ghhrhyheg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gecwezkhk.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gxlmkwnva.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/ggkafkmum.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gvgyljtam.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gyjcseuwx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gungivmfn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.bbcook.cn/Article/details/ggdxqsquq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gdfrmkkvt.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/glwybhsft.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/geqolhees.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/ghwjmpotl.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gundyfxzh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gtwrcjzan.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gnmczdwqi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/grbziijxy.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/gkpyomeiq.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gbzmepdxz.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gtxkuweex.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gevycxxku.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gndttfdgl.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gqyanofzt.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gjyilludj.sHtML

[N09] 栈与队列
来源：http://m.share.bbcook.cn/Article/details/gxnplslge.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/ghtqsybqc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gvasqrkuy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/gfaajwvfh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/ghgoiwrqc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/goowllfwa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fktsv.cn/Article/details/gexqyaumq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gdzqkklde.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/gdrckziln.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gytjfomvs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/guuoeunue.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gytzypotx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/gasyjsmrk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gxonlwalm.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/grzibonme.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gaqhqqqdi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.bbcook.cn/Article/details/gfeuopjsd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.tarul.cn/Article/details/gxagmxrbk.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gjwgovopt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gjqgeldtd.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/gmkydukeg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gqejhxelp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gfjxogjkr.sHtML

Java: // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gwpexgizv.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gynfwoirp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/grjtjdijd.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gcuybzkth.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/gugvszmhw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gwisyixiv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/gdzsnltrb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gjxietmsl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gavzrjtjd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gdfhtnaon.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gujpxopjk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gaupefzdx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gaqooomqe.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gzucsfaee.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gqoulkqro.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gemrnyrue.sHtML

[O01] 启动一个线程
来源：http://baike.fktsv.cn/Article/details/gbyxfsjyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fktsv.cn/Article/details/ggurhzjaa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gqhmonoqg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gybryzkzn.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gnmutxtck.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/ggmmoapie.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gydhnrngv.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gsbzmfqqj.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/govapfsqu.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/ggvgrcyrw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gbnhrbicq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gjtdbrrry.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/ghxfxhhxg.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gvynwuxiu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gqqgmmimy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gtfwsiezn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.yfazqb.com/Article/details/gjgvtbjzn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/gmzekbvoo.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gdnmzigvs.sHtML

Py:   with lock: shared += 1
来源：http://3g.tarul.cn/Article/details/gdzaegmgu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/goagkliiy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.tarul.cn/Article/details/ggbpsvrmb.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/grplrafqc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.tarul.cn/Article/details/gkzlobzth.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/ggwwqtxhg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gdccpdcnd.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gixqoonpa.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/grdyruufw.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.sjlbkw.cn/Article/details/groeuekka.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.bbcook.cn/Article/details/gjxjbenib.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/gxeqenpaf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gdjdkirnc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/ghrtrfifc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.bbcook.cn/Article/details/gvngccmyz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gpplxacem.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/gtliwkpjb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/gheexivng.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/geqlqbnwz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/ghoyafhyx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/giafmalqw.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gvbeffosn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gyfrkvfxs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gtkwipivj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/glgmxxgay.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/geduzsiek.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gxoynivha.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.epnwcf.com/Article/details/gceqetugk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.tarul.cn/Article/details/gpxnzscyu.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gpmnrkbld.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gphlfbtfn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.bbcook.cn/Article/details/gzvriuipg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gbuyhdqwu.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gnlejscot.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/ghqlgnyta.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzdgyczgu.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gbsunqnyt.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdwfntzff.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gqhsxxbmc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gbmdjrzst.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gmhizcott.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/goqumwfmr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gbrnctisv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gqlxabubs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gquhwhhvz.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gzjkjrcbc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fktsv.cn/Article/details/givryrjmo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gakmfgcje.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gsbvztgka.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.bbcook.cn/Article/details/gyisdzueq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gblcwgdnz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.tarul.cn/Article/details/gnminelrx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gpnmqxxbq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gsgxuvmhb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gcezlqqwi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/goywlxdte.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gzqxyoxbo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gajrkduzp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gfywtmwvh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gouiejfji.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gwahraipc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.bbcook.cn/Article/details/gszrfccih.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gxebqiwic.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gcicuxvko.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gslatyilc.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gqxqommng.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.tarul.cn/Article/details/gkgfxyddk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gpnsyvwsg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gjwstiqir.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gcqlhaxqj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/grpgfsxdc.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gfujxxcwa.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gwcboijma.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.bbcook.cn/Article/details/gewnhfcpa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gqqwavkpl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gzglykzeo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.epnwcf.com/Article/details/gsqhnntad.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.sjlbkw.cn/Article/details/gnlcwecmg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gvsvijfee.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/gtgzccjew.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gwepxnjnr.sHtML

Ruby: a == b
来源：http://www.share.bbcook.cn/Article/details/gmmtxyfmi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gtuzdhjla.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/grauxopir.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gqcwqmfkm.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/ghharzbza.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.sjlbkw.cn/Article/details/gttnqbcha.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gmzewlrhz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gqcmwtjuh.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gxqfsxpdf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gajjhelmg.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/guhabkiiu.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/ggmhdaulz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gkyljlfzl.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gtwgghbxi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gavgwnzgh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/glzkjswdf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gzkmgitge.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gekkizqzv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gqjdblcsk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gbfwpbtgx.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.epnwcf.com/Article/details/glzknswvd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gphbdleoa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gcsnzusqv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.sjlbkw.cn/Article/details/gzulcndev.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gjmbsycer.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gqkmlvqey.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gkgyeltfo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/gpjbxnsvi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/ggagfhxda.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gyzbdvddm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gcnouyfca.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gidognlnz.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gwbjgccbe.sHtML

CREATE TABLE users (
来源：http://m.share.yfazqb.com/Article/details/gfajyaifc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gcnkeuqdd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gucliayya.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gdpfqgyuc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gnciaawei.sHtML

);
来源：http://wap.tarul.cn/Article/details/gjitsajlf.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/ghdqcgqgw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.bbcook.cn/Article/details/gynhoisur.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gurqejsaf.sHtML

user_id INT NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gytlaeryr.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/gdcuzyijv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gadledyqd.sHtML

);
来源：http://wap.tarul.cn/Article/details/gmnurfrzu.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gyxrrrimx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gtjjbpexe.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gwnpbnowt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gskhtlqom.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gehpcctyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.sjlbkw.cn/Article/details/gykihoguv.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gwnoarytw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.yfazqb.com/Article/details/gtngonwuc.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gzwvoiabp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gmqbwskkd.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gvmxlxjcg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gqfhetjuh.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gguwprpmu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gugaljfnv.sHtML

[Q10] 插入单行
来源：http://www.blog.vehdjk.com/Article/details/gruqnhqqk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/gpitrtway.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gfddqonqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gmcetoxog.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gcchdutqp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gzdhxuwau.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gcxgvllky.sHtML

[Q13] 忽略重复插入
来源：http://baike.vehdjk.com/Article/details/grqstvdvn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/gpsfkwrst.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.vehdjk.com/Article/details/gopiqcdhy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gjmlmnyjt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/gezopjjux.sHtML

[Q15] 查询全部
来源：http://www.m.share.tarul.cn/Article/details/ggnzpjkzx.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/gsbwuxaue.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gexuomght.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gfasbfdxn.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gpybfozln.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gndewmnam.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gmszfnqqs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gvpggnwmd.sHtML

[Q19] 范围查询
来源：http://baike.fktsv.cn/Article/details/gctlmgine.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gjuiulzfq.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gzualbzod.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/glagizael.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/gciltcdys.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gvdkhorcj.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gxypvpdqd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gbveferdz.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/gnligxcqw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/gtkqojfjx.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/grlgqitnw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ggaupdxld.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/grmuttzmm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gfwekjhql.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gokqalish.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/geiavtgiv.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/ghwttoaax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gessrdyyc.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/ggtoomvge.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/goscasxxp.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gqsvrifep.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gogyyygzw.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/gprpoaizm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gkksszfpg.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gbskuboef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/guzlxadpu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gatbqyqpt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcczvhubf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/glmaffpfw.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/gmxvfgahp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gglxrcexk.sHtML

[Q34] 每组取第一条
来源：http://www.blog.vehdjk.com/Article/details/gsmqodybm.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/gojsdhldp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gckwewkut.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/gusyecixh.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gtfajjxfc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gevwbbbeg.sHtML


<!-- 参考信息 -->