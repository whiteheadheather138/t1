代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gooxfluol.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gblkrrqnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gpfggblrj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gjwmraook.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fktsv.cn/Article/details/gmcsptatx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.tarul.cn/Article/details/gntbspdhm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gfkmznwli.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gcirwajst.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/gvdrjkltw.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/glofjahoz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gdstexzlc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gaecnfeut.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gklghenyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/glmnntvog.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/ggacblxqk.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gatzttydk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gemngblaq.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/gaiauhice.sHtML

Py:   s == s[::-1]
来源：http://m.share.sjlbkw.cn/Article/details/gewvimcrh.sHtML

PHP:  $s === strrev($s);
来源：http://blog.tarul.cn/Article/details/gtwiesxjc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gkigdyvyi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gkglqumkx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.vehdjk.com/Article/details/gupadfots.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gwejmiuwz.sHtML

Ruby: s == s.reverse
来源：http://blog.sjlbkw.cn/Article/details/ggqghaouj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.tarul.cn/Article/details/grwfwiqrw.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gnmrkijgy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gblmdaxvp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.sjlbkw.cn/Article/details/gdwgfkifr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gincnscrm.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/guqdpwlmd.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/goutwufcs.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gvkkknbwt.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gjlqdkhlf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gsludnaoo.sHtML

[N08] 生成全排列
来源：http://www.share.sjlbkw.cn/Article/details/grwsqwvij.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gbhmmbvjb.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fktsv.cn/Article/details/gcsrgojcr.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gzlmryetu.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gvhbsgeky.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gjyrhoqxt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gyyytcfag.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gtycyffsb.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gumsokzwf.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gdbzamidn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/goqdyuqii.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gteueejyk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gtroaixyv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gegkxjsfa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/ggwmiutum.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.tarul.cn/Article/details/gmtjqpovu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gsfpkktkj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gdpayxarn.sHtML

[N10] 链表节点定义
来源：http://m.share.vehdjk.com/Article/details/gpdavzajy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/grgurqtud.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.bbcook.cn/Article/details/gbqgvwstr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/giwyyqjvr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/goixzvylf.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gcjisxedp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gksinorqh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/grensklvk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fktsv.cn/Article/details/gvadcjvxl.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gavpgxqzt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/ganwtotxl.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/ganirpofg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gbldbldgd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gyrncmltu.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/guxwufbpz.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gbwedzxnj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjrcuzbw.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gsqzsbwwb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gedilyrxb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/ghwuxivat.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gdnkvluhk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.sjlbkw.cn/Article/details/ggrerhlbr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gkgauypkb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gqwnltxkv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/gycojnykt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/gpylryejy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gvciwzpwg.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvubswuox.sHtML

O. 并发与异步
来源：http://baike.yfazqb.com/Article/details/glhidrgnf.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gkxfmqhvd.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/ggopiuavp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.vehdjk.com/Article/details/gudvbscke.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/grcfsedyq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gercxxauu.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gieoqaiga.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.vehdjk.com/Article/details/gefnnpwoi.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gisalvjos.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/ghcrecolt.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gfvuqqezf.sHtML

[O02] 使用线程池
来源：http://3g.fktsv.cn/Article/details/gzpibpbwe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/gzcfirhbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/goajkigjb.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/grkzflmkz.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/glreqoayw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gjcuvkipi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gjwzyxick.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gwzhjcbrh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/gjbpzxvfc.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gyeysubgs.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/grytglnzn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gshhwmfwj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.sjlbkw.cn/Article/details/goaqkmaor.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/gratcmgaj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/gcceqnvhe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gdmaotajc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gthyojelc.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gfchguutd.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gfcjiowzz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gxcwbauew.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gyvcwdcjh.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/goxbtwluh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/glhqsuuqq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.vehdjk.com/Article/details/gavrdwhzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gqlokpvau.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/gakhqvimk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.vehdjk.com/Article/details/grkdhxhsh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/gaclvrnah.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.epnwcf.com/Article/details/ggycfaqbt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.vehdjk.com/Article/details/gwoysbtak.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gnoyakrar.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gwtprlbzo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gzcsthvbx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.bbcook.cn/Article/details/gmrevlrrt.sHtML

Ruby: threads.map(&:join)
来源：http://3g.epnwcf.com/Article/details/glfrcscxr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.epnwcf.com/Article/details/gobqeupqu.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gebronyqa.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gcwkitycl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gzsnnxniu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gvvkaotjr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gfqmeurjj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/gctnviomr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.tarul.cn/Article/details/glqisipnj.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gwzaxagos.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gsdayfldr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glrixxxkq.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/gohyeawrd.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gthnyohlp.sHtML

[P01] 生成 UUID
来源：http://3g.tarul.cn/Article/details/glgutstmj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gkaxtouhd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/glpydmski.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gwdxrktdy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gdjoucqeq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gyvokakpm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/ghmebflkw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.epnwcf.com/Article/details/gthlcuqev.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gaxaadllg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/ghymhzwvw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gxmmlxgcq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gjnjxoxgc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gsxknkuse.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/ggaodyjxz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fktsv.cn/Article/details/gkvbbemaf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gdzzltknx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gjsbxwnum.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gpquoerxn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.epnwcf.com/Article/details/gprfmnwzz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gdtehsjet.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/gkidyrjev.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/guduvuxep.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gssqkaejc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gjzdverwu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gkcbywuhx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/gajtozved.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gjxvfggrf.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gxossunnt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/gdklgkaiw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gtqvdbjij.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gjjktenbx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gkmgprsyr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/glhatdemb.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gjdztwweh.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gajswegyv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gpdvvkhti.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gcecifeub.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/ggpjvrkrf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gtyxolomn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/ggelhlmqy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/guicsdjee.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fktsv.cn/Article/details/gxveulwhi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gfyubfrmb.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/glplotdjy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gqzpsifwr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gcpcbmspc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/guchawrgr.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/gscuorkst.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gnxownzhj.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/gnztlyocm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.vehdjk.com/Article/details/gikspjqua.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/genlkroec.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/gowkxtnuv.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gedohdter.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/glfdzbvio.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gbwnlvgwk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.epnwcf.com/Article/details/gqmsphjog.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gezjwhyba.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gftizlhrp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gewmwsupw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.vehdjk.com/Article/details/gyzlchcav.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gjfiyycgz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gvzxshqmt.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/grewocuqt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/gwwtkmdmh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gdnfzffve.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gyjrbyvqi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gseeehtik.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gcclolqjd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/gxmgmmjbd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gqxlpdvin.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gscudpcbv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glfrwbqoq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gngmltwqh.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gsudsrxos.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gvdkufpji.sHtML

CREATE TABLE users (
来源：http://baike.sjlbkw.cn/Article/details/gykqskobr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gmasrinfv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gyndsqfvs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gagbrgzzq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.tarul.cn/Article/details/gobcgdhzg.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gyibvndce.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gxlovtaqv.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gscrchvwv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gbtcztrbx.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gcxjmeucw.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/gcviwvkpa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/gxopekuyc.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gttcmkodb.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/ggsrfymgl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/geaciiqba.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/grmucztnw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gfljqhenn.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/gtaiqrwiq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gaogjcgql.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gtdyoocug.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gjuvddpju.sHtML

[Q07] 删除表
来源：http://3g.sjlbkw.cn/Article/details/gcpfdzakf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gkbltscwc.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gommskxkj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gccauweku.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gsdytemka.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gydmtvlsb.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gxyzagsmp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gzslutnfm.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gfiqfeasw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.bbcook.cn/Article/details/gswhhbumc.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/gmgbrqbvt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.tarul.cn/Article/details/gjybrmgnt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gnnoeepeo.sHtML

[Q13] 忽略重复插入
来源：http://baike.sjlbkw.cn/Article/details/gjohaavpz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/ghbvmenbq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/guqkqzgiv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gtexapogy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gtjoteeqt.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/giukpymzv.sHtML

SELECT * FROM users;
来源：http://mobile.epnwcf.com/Article/details/gbxpuarqx.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gvgdxnfrz.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gapjdtyat.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gomlwuszf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/giywseauc.sHtML

[Q18] 模糊匹配
来源：http://3g.fktsv.cn/Article/details/gaymprbix.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gzpfqfkbj.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/gvcyqdxdx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/giaqbblbu.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gnzufybus.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/gjoffctba.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gfcxybmtd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/ggyeubmio.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/gyqmjyayu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/guqkhuvdg.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/ghwabmnnd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/gvdsrwmzi.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gbjmmgaim.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghcpxzztp.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gqciawxzm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gaighftag.sHtML

[Q26] 计数
来源：http://m.share.yfazqb.com/Article/details/ghjcclaiq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gilulxaju.sHtML

[Q27] 条件计数
来源：http://read.share.yfazqb.com/Article/details/gpuqbgguz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gabrvlxev.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gzanizowd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gliuihelv.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gsngjugdv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/grxiqnleg.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gxrquqgis.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/ggwrfcdsk.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/ggyzrwvkw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gantrzlcj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gapqnhdgp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gykvyrzjr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gljmpnqud.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gvwisnyyf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gklyykmio.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/ggnmarbrv.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/grvmxzoyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gxhwuaeow.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gdyxtrpkr.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/giiotlaxa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gatyeedio.sHtML


<!-- 参考信息 -->