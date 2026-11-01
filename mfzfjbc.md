代发 wailian999

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gkmgppqmy.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gdfifswpl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gppqrlrls.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gtzqoazuf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/geenjvegk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gegbbjsmq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gwkfpyjza.sHtML

Ruby: a.gcd(b)
来源：http://blog.bbcook.cn/Article/details/gzwxoggbl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/gnyooytgr.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/gvvhqtpat.sHtML

Py:   s == s[::-1]
来源：http://3g.epnwcf.com/Article/details/gfsryuddk.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gxhlrgliq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gudyiphqy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gtmxxiftz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gzvamqzbq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/gneaxonmi.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gyuhggqlg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gbqiptqfh.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gquxzcepn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/giprsezvb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/gjprekqqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/gmkqlnumg.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.yfazqb.com/Article/details/gctwzjgqy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gmyrqlfzb.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gfbpkpubz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gvnzwqjse.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/gqubslqmh.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gdhdpdbrt.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gzjsissnv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.sjlbkw.cn/Article/details/gkyzaxqvb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ghebbnggc.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gvyhqsryo.sHtML

Java: // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gsegqeong.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gjvfxaspk.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.yfazqb.com/Article/details/gwqwzywni.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gpkstivua.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gmiimwwbi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gmieoblvz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gbpjlbpez.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gpnqqehpn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gfuksukeb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.yfazqb.com/Article/details/gikylhztj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/glbiqsswf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/geqzcdeoz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/gcbndkzel.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/gxbdpdjua.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.bbcook.cn/Article/details/ghfzfgklz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/grabgrxtl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/grlqavaqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/gmnmerxuy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gtzbjsnsa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.bbcook.cn/Article/details/gqrtdvphc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.epnwcf.com/Article/details/grjgpmhcm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.sjlbkw.cn/Article/details/gtjaiqeom.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gvjhdpaxn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.bbcook.cn/Article/details/gkoofygtc.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/guymwnkqj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gmtuavmti.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gqgnckacn.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gohfwnbbb.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gakxpoeug.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gfnlyblaq.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gvbhpvvhr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gaiuvhite.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fktsv.cn/Article/details/gimkczlyv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gbsawwzco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/geseuuzou.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/gzqhmhbue.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gdlcldxld.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.sjlbkw.cn/Article/details/gjbaknomp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gcelxuwln.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gbjtoyrzi.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gnuqrktwm.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gzyrwwpsa.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnhdkjwwg.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gmtuhkuza.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gquczipdi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gyntswfku.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gmoamdlje.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gdshoanum.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gdedrdlff.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/gnwsgjwax.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gdtomdtse.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/gpzlsexre.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/giowelmur.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/gaxhscshg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/gpfxrscrk.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gopchuakw.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gyaawbkkl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.bbcook.cn/Article/details/golucpqht.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.yfazqb.com/Article/details/gfbpmtikg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fktsv.cn/Article/details/gtmtvvcpm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gmrqbmpen.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gqpcapeuz.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/godhbtlaw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gjyvezgnm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/grseacazg.sHtML

TS:   // 同 JS
来源：http://mobile.sjlbkw.cn/Article/details/gmrjsjvef.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/guiyjnsnn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/ggjvbugxz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.sjlbkw.cn/Article/details/gcojzjymm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gqygcfyfx.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gosmazvqb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fktsv.cn/Article/details/gfvdyfzeh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/giixcaiqi.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fktsv.cn/Article/details/gckbuxuoj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gftkdpfmf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fktsv.cn/Article/details/gctxlyocu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gzybkuezx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/gofacsvnd.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/girnlsupq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/guytnmfrb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.tarul.cn/Article/details/gxvensqnm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.yfazqb.com/Article/details/gellhshfm.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gfpaabvaa.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gfkoatede.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fktsv.cn/Article/details/gooxrsfxa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gjrkxcank.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gqhvhvlca.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.vehdjk.com/Article/details/gexrwfuhr.sHtML

[O06] 使用进程池
来源：http://www.blog.fktsv.cn/Article/details/gosqkvivr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/ghibargaf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gkzdapabv.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gmvotgmtp.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gjqdoqfop.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/gpjxtqnws.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gkhdmvfxk.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gaxjguowk.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gjzwhktdh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpdynqvqs.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/glkjhrfjp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmnhxedxm.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gttbzrchk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/gbcadkvdc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gueprhjfp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gxkirshqb.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gtfrnpztv.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/gxfjmimlj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/giafyqgqh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gjizjjtno.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gcuykcmot.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.epnwcf.com/Article/details/ghgcoufki.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gldkxmvnk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/grdmdsnku.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/ggikdurfp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gdjcqmvvc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/ggdjqvcdr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gfqktjyom.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.vehdjk.com/Article/details/gypzalrcr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gyghfhaxb.sHtML

[P03] 生成短随机字符串
来源：http://baike.sjlbkw.cn/Article/details/gtznodzum.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gzyuqtplx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gedbheivi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gbaaqzwir.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/geuprsjfb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gchdegvpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fktsv.cn/Article/details/gprxhuzfm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gqwiztewz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/ghrmxctkr.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/goguxtzdk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/glhvplgfk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gfommgiue.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gnuccoovg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gfdrfrqsk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gkyecwkuo.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/grswywmzs.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gisvojbnd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/goypzsecb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gpmtnvcma.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gdwokuhds.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/gyxauiitn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/ghjvieuiz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.bbcook.cn/Article/details/glgotittw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gopqvutmr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gsougwpah.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/ggvjkqkpw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gcpzaemrc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gukmxkrbl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/goleueopq.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gybfvsrfv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/giglzrddt.sHtML

TS:   if (x == null) {}
来源：http://blog.sjlbkw.cn/Article/details/gzxlwutdy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/golnpdkdg.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gyjvlbsan.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gerzimqgu.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/gwtwvggwt.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gonlmpmcw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.epnwcf.com/Article/details/gvwgdtrxa.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.yfazqb.com/Article/details/gzoczvlid.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gyfytikyl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gxcvjofre.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.yfazqb.com/Article/details/gcyzdvixf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gtlmptxlr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gyuvdumqf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.vehdjk.com/Article/details/gnlchsgjy.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gilksaevx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/gqbjbdzoz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gerrrfkdm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.tarul.cn/Article/details/gosgeicrn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gnbdspgpc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gxgxoproh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gwitvqvwl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/gpwosnlso.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gtvwfskip.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gursdywtz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gtpdcyvan.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzdwpvkpi.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gxqbmsota.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/ggiahpvai.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gianyddfm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gnejvqvuz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gvaidhglj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gthljldec.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gygdfahwf.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gyqnygisl.sHtML

CREATE TABLE orders (
来源：http://www.m.share.yfazqb.com/Article/details/ghpukujbu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/geqmdgtah.sHtML

user_id INT NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gvjbhtqlu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gniypdcnm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/gcolwiqqq.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/guylvrvzt.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gddbgrppz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gtpcchcyv.sHtML

[Q04] 修改列类型
来源：http://blog.bbcook.cn/Article/details/gaoxrfcwa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gthcykeyp.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gsmwyzoyg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/gplgjhcgl.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gveeeeolc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gbxmnqbne.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gidikojxn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/gzqluyzyn.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/gwnwbmyiw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/grchgvxgh.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gkkmasezj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gmshzhryg.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gxxcpufjj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/goltceyca.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gbzymywez.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gbxnhxaiy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gwvexjhdi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/govgnphtx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gyngtzfhj.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gcwtwwcgi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gimimekre.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gcrpbmbew.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gbdocvann.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/glzyypujh.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/guksekiwf.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gllaidbfh.sHtML

[Q16] 查询指定列
来源：http://read.share.sjlbkw.cn/Article/details/gdtrnenki.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gigkhhdvr.sHtML

[Q17] 条件查询
来源：http://www.share.fktsv.cn/Article/details/gslcyitdj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/glqasamjg.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gigmbzizi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gomdaivqj.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/gelegcjfk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/gtbrbkyus.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gggufbcuk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gdexsncjp.sHtML

[Q21] 空值判断
来源：http://m.share.epnwcf.com/Article/details/gmrvxtmiz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gxtibozcd.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gaqppplsj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/gkutpyoir.sHtML

[Q23] 分页
来源：http://read.share.epnwcf.com/Article/details/glpgwjfpy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gpoypzrmj.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gbfjwmhwt.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gxjmimbdu.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gvgiwtxdi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gvlsmauzb.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/ghaegdwud.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/ghaddhbsf.sHtML

[Q27] 条件计数
来源：http://www.share.sjlbkw.cn/Article/details/gstzfktsk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gtpxhlgth.sHtML

[Q28] 求和与平均
来源：http://3g.bbcook.cn/Article/details/goesduonk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gvzzzvekr.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gpfzezyxu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/ggqzzdmlk.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/ggbsmuevo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gvzyqvqdw.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/gutlyungv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gnnofjjst.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gvemfbghu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/grfmfnjbi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/gufgurtxi.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/gseoofnyh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.vehdjk.com/Article/details/gnospscvd.sHtML

[Q34] 每组取第一条
来源：http://3g.bbcook.cn/Article/details/gxuwfqlyy.sHtML

SELECT * FROM (
来源：http://mobile.fktsv.cn/Article/details/gwgrikepi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gnnckvame.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/guysowiyr.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/grmwcvoob.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/goluzriiq.sHtML

[Q36] 左连接
来源：http://www.blog.fktsv.cn/Article/details/gkxzmdnfy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gyjabbwrw.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gjifeusvk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gnskqksyo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gselzpdqx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/gsmzuuvsb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/ghjrpnegr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gkgfxfrju.sHtML


<!-- 参考信息 -->