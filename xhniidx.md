代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gnasbmbgf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gcsmpwyda.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gqqsqenew.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gjjyxmnuw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gfveebtie.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/geftobbjs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/galhnvfcu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gbmroeftu.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gukvtwezi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gwlrsvydu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/gjbjiwogu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.tarul.cn/Article/details/gmohjyeux.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gsehqctra.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/goisdgkcw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gnzntdjja.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gbrvsczcl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/guahbutnn.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gdtuecbwg.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gftufnicn.sHtML

PHP:  $s === strrev($s);
来源：http://wap.tarul.cn/Article/details/geejlqmtv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/ggwlevltb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/ggtxzlnrw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/govekqbxn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fktsv.cn/Article/details/gizojnddo.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gboxqkpaz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gtwxyxfoz.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gpmtozkwd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gsvsppzmo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/grnahzsaf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.vehdjk.com/Article/details/gmlavyavn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/girvmttsq.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gnjjyjysh.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gpbzyeqgf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gboyoagmq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gdafnyvoy.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gqcazkfoo.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gscwuvdwc.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/geaqtnwmu.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gqccytfwu.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxmqloqzk.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gdegptjkn.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gbofgrabq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gmukjkfam.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gkosstkdo.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gpudngzyl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/ghdhagpcz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gybanbdro.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gmgifrbkq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.tarul.cn/Article/details/gnsglemjj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.tarul.cn/Article/details/gknxsjurz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gcflrphzd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gatgukjii.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/glkfwhazg.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fktsv.cn/Article/details/gwsqzybnw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gaowiflrf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.vehdjk.com/Article/details/gcgnmkraa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/gtrvpsumv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/gxqqhyuqg.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/gpzzovlci.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gambrusqr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/geveckbgm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gkjrtlbck.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gyoguplpe.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.bbcook.cn/Article/details/gicakvidw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gkqdhpyxo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gwvirxdsu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gbsixzmmr.sHtML

Java: // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/grwpzvcub.sHtML

Go:   // 手写递归
来源：http://m.share.sjlbkw.cn/Article/details/gulffthth.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fktsv.cn/Article/details/gkimndgig.sHtML

C#:   // 手写递归
来源：http://wap.fktsv.cn/Article/details/gzbtxuipk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gegrhaxls.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/gincslwcm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gxerbavuo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gxbjlltgp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gzopolaqm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gjrqbvvyh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.tarul.cn/Article/details/gwkahmwsm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/ghvxjrhlc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gpqsgfjhx.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpgkirsqj.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gvheuvsau.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gvliwbwos.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gslzoxwnl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/gfgpkoxfc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gfwdrlfrw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gqizqsjdc.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/ggskthwvr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gsokupdtd.sHtML

Go:   go f()
来源：http://blog.vehdjk.com/Article/details/gcrtzdwld.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/gnlrpidcg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/gfohuqems.sHtML

[O02] 使用线程池
来源：http://m.share.epnwcf.com/Article/details/gdwrfxejt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/ggmmahdyl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/gkgchzcst.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gcetpqgeu.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gsnpysxrl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gdmfihdzx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.epnwcf.com/Article/details/grvgjicrf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gsmkzpwxb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.tarul.cn/Article/details/gggasnjwj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fktsv.cn/Article/details/gxfgpyqcu.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gcnbnldjp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gmrvbmtjm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gpdnnqesr.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gbfgaadka.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gzbmgclrc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fktsv.cn/Article/details/glnecejwc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/gkuzanrwc.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/gpcvozgxq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.tarul.cn/Article/details/gxpjrevlx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.tarul.cn/Article/details/gpsflppyl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/gdehkxtvx.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gxldomltz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gwuhjfjjm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/gwcbvvmhm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fktsv.cn/Article/details/gxdovbvtb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gxmkpfzsj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gmqlixzxd.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.sjlbkw.cn/Article/details/gpqwrybxa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gdbcpsnhx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gpezuweoo.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gvxqweokc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gqddjnvma.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gkkxzzqnr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.vehdjk.com/Article/details/gzfxugsls.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/gnktihtfq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gosxltwwm.sHtML

[O06] 使用进程池
来源：http://mobile.vehdjk.com/Article/details/gbfxtagyu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.tarul.cn/Article/details/gcveehotg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gpumguzwb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gucjnascx.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gtepbpdim.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.tarul.cn/Article/details/gbvfdjslo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gzcfqytad.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/gfwyzhyge.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gpdptvtjt.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdnbjlyxs.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/galrxwqxb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gukejznom.sHtML

[P01] 生成 UUID
来源：http://blog.sjlbkw.cn/Article/details/grzbxbulx.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gjiyoorql.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gimrmycrz.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gpkdtmapc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gguckoiuw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/ghjjzoasx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gzgahunwe.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/glpofpfdz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gfneqywlb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gejrarron.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/glikybdck.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/ginhvawge.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.epnwcf.com/Article/details/gxjfdjuyk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/guolccgxq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gdrkmtodk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/ghbmvxlup.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gkjiohjtt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gbntamwuj.sHtML

[P03] 生成短随机字符串
来源：http://read.share.sjlbkw.cn/Article/details/gcxotyoab.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/grdcnlstu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/gdsqscpzf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/goqecjjim.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gkcdlwboh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gsvtpmniv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gmrckuzzb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gdjkvyylv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/ghjlaxyez.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gcjkujawh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fktsv.cn/Article/details/gqvnfnran.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gaufkqnot.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gdzsstupg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gnpsvnhtz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gzhfmjrmz.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/graskasbg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gwwpoqurx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/gdqdmvrrb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gsqhufeyo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/geqjwcilc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/guhwrjvxo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/geqaqmqer.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/giomdefvq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gmhvshpdk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gclldvehr.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/ghupnaekc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.yfazqb.com/Article/details/gfexziqcn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gtzpqsllt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.tarul.cn/Article/details/gmfhjylbb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gylnbplok.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gczduvvjv.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gexjlqqwl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/guruewbtd.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gmufogkdv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.bbcook.cn/Article/details/gxpwrrkex.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gjmjoroui.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gfjwdnikl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gahmeofio.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gozkmewya.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqnadupb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gdckytbte.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/gfcxcysac.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/gjzvnypbd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/gibwdowqi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/gshrfchkg.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/grqzbniqw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.epnwcf.com/Article/details/gdeobmsvl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/grzpykhti.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gjveicqmu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gvezchktp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gmsyzroob.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/ggaeghygy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gaowtidfv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gpmhrcqli.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwxytmkfb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/glqzbmlkw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glrokggzq.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gjxdxuzpp.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gjjkvmirs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gqmjohuih.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/guaqlrqlq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.vehdjk.com/Article/details/gmowzhuvb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gxigwahyr.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gwldyxrbn.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gttutywpb.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gerxmtsbc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/goteedddh.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gviwnqjbz.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gdovryiwo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gldmkgmof.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gkreqhoxj.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/gzmljueib.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gwqjjoczq.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gfqudedyk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gvkpfwkoo.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gipkayiyu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/ghpszayhh.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gueegaqtf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gralztktt.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gcuitvona.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/grqlxshvy.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gdgpekcys.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gfwbputwt.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gsuqnkjvq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gnnfolzxw.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gpdxwqapv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gtwqmgose.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gqiiwfyhc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/glxanphuy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.tarul.cn/Article/details/gdkxtgeui.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/grusaueks.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/geverprrf.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/grbiekxdr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fktsv.cn/Article/details/gcsahmrnd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gqabfmvov.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/gqziehcjd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gngxabnik.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gexpjkqkr.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/gjtvwlxsq.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/goabzngmw.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gyhspungr.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gjqhulnyp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gjloofybo.sHtML

[Q18] 模糊匹配
来源：http://wap.fktsv.cn/Article/details/gahaexfxv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/gubmdzhgs.sHtML

[Q19] 范围查询
来源：http://wap.fktsv.cn/Article/details/ghqgmzcke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gvknwdduj.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gkypogfnp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/gshabkxkb.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gfcapjngb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gtugownqy.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gnkqhuczr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gazrpdmuk.sHtML

[Q23] 分页
来源：http://3g.yfazqb.com/Article/details/ggedlvmbb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gtevbasyx.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gcstshyui.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gbtbysohh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/grntmdccy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.epnwcf.com/Article/details/gumbrsmud.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/guduzbvlx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gyhqmpady.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gpfhtoaxq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvtsdokih.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/godhbschc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gefpawerl.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/ghfeljtpl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/glvctahos.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/grlbjtokh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gmopydnub.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/gtrzjkiuf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/gtizmmali.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gjizmssig.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gzcbtanvk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gtkplsqpr.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gniotopzj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gvytltyda.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gwzigmpdd.sHtML

SELECT * FROM (
来源：http://blog.tarul.cn/Article/details/gzldbhgph.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.tarul.cn/Article/details/gzjwrkcfq.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/gewsquqiv.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gfvlpldek.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gppnqekfn.sHtML


<!-- 参考信息 -->