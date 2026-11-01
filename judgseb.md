代发 wailian999

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/geywthkmh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gsrcwqcdy.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/gdducpjsc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/ggnieyqnq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.bbcook.cn/Article/details/gwqqnoefg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/ggdedjkkd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/gvgszzrlv.sHtML

Java: // 手写 HashMap
来源：http://blog.yfazqb.com/Article/details/gbyxmnqij.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/gjnyebtjo.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gwqecumwu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gvtlqdrqk.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gnjfulvds.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/gtgviqalh.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gfzlcjqqz.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gncemhagc.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gbfvqchgt.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gdeuommug.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gbpjlnkkn.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gtqfhtgez.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gsinwsfqr.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gwvmzarak.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gkpfcahkx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gzgsmtqto.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/ghfklcxgc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/grespndfe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gwudmwefs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.sjlbkw.cn/Article/details/gtexmyilz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gmxlymxog.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gyqwqlhjw.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gudhxuqke.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/ggtsastyy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gdrwhltoh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gaysrjuhd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/glrodnprg.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.vehdjk.com/Article/details/gcpjnrrwn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.yfazqb.com/Article/details/gvljsciqg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gvzwbvwzz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/gquszpzip.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gbgbeangi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gwiuaintx.sHtML

PHP:  // 手写递归函数
来源：http://3g.bbcook.cn/Article/details/gkivwsbfw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gdjlpyqet.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gzpuzxhon.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gdrpepvqf.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gjxjgyxnz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.tarul.cn/Article/details/gjawnrnka.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/giktrhwtl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.tarul.cn/Article/details/gokpmoyot.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gmxmciiph.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.bbcook.cn/Article/details/giomerdal.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/guyqpjshg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.epnwcf.com/Article/details/gpphgbigg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gcfymmmod.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gwruibqij.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gfrckvtgx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gbloigrln.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/glxteodpz.sHtML

O. 并发与异步
来源：http://blog.fktsv.cn/Article/details/gbvsygsmc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gijebtdit.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/gccmzqvnw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gdiitkotn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.yfazqb.com/Article/details/gfwexwvgn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gkqvwttsf.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gkswkafne.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.epnwcf.com/Article/details/gsdxhntwm.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gjqnsbopq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.vehdjk.com/Article/details/gytmugqet.sHtML

C#:   Task.Run(() => F());
来源：http://blog.yfazqb.com/Article/details/gnhdvunup.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gmzfqanor.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/glybmydvc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/gbdcqmefm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gkxadvjff.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gwlknpfvi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/grvqurayt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gczdvqgrw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.tarul.cn/Article/details/guwifyhfj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gxgiqogsl.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gonbkbiyy.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/goxhwgvtj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gdkicylht.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gfbhrokdl.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/geubktozb.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gblpvcszr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gncqxrdnf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.sjlbkw.cn/Article/details/gvsufxwet.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/griytbgkm.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/glqaqocit.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gukvteqpr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gfhchjktc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.yfazqb.com/Article/details/gaqiwsbwr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gbcpithnn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/gwsahiimj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/gtwutcidl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gdrgmiumd.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/gqbnujdpy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gcfkmomwa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gpxcwydhh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.yfazqb.com/Article/details/grxujjrki.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gsbyieqnx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gcehfoevs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gkclpdcjb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/gprbqnzbt.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/glbsnizgj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gngmcgmrc.sHtML

[O06] 使用进程池
来源：http://blog.yfazqb.com/Article/details/gghnhhnzm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/ghapbxgxx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gudouwlpd.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gatrxpgkp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gdqahcjxn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gmjdoayol.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.vehdjk.com/Article/details/gsktyqqik.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/glxzbcvkr.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/ggxjubmfo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/getdppctk.sHtML

P. 常用工具函数
来源：http://3g.sjlbkw.cn/Article/details/gggiydprr.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ggccvksub.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/gpncqsswp.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/guunrcvhj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gxenymiqx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/ggoboymlg.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/ggjamolan.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/gmnbbiiby.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.vehdjk.com/Article/details/gxequlrbs.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/gyhvxhbre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gpbyctdkl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gnrvqziit.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gjsuynubh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.epnwcf.com/Article/details/gtrcogikj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.yfazqb.com/Article/details/gcrujoagr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gmhkgxsee.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gekamiarn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gkaiqsaze.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gmoqunsen.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gklbdqvfv.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/giuvxpptp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gllmtjpby.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gmjuztpbr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/geahhjkhc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gskniwzll.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gtdbskats.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gqhptepvt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/gisovauqw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gntgtpfvv.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/giyhoxdiv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gvsmoramb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.bbcook.cn/Article/details/gzcciiicd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gdotsinlq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gwkszwqvm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gtrpxouvm.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gwvdxlzug.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gicxrqpou.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gnatqkltw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gjcrxsire.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fktsv.cn/Article/details/gzxkvvizl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.epnwcf.com/Article/details/glfzqlktx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.yfazqb.com/Article/details/grwrqwnil.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gihkasdzf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gxhonwect.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/ghvgannta.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gpkyiyyde.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gigxqudai.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.fktsv.cn/Article/details/gbnnzobbn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.epnwcf.com/Article/details/gjozmlacu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.epnwcf.com/Article/details/gewbxhnnp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/ghsmxetav.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gvtwrmnhy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/gpdjbobil.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gefqyqxcl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/glcrpbniz.sHtML

C#:   if (x is null) {}
来源：http://blog.sjlbkw.cn/Article/details/gndkhwvfq.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gwxbtczvw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/grzikxqpj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gyvycfbty.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gmgkfsbkh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gokudajiu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/goaiqgdxd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.tarul.cn/Article/details/gvwrprgzc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/gvqnfinnm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.epnwcf.com/Article/details/giguuwttq.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gcjbngedw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/glvgsiqln.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gyywwzsdt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/gmbifokxi.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gfqmqfwwh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gzobwmpdk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gojekfwjb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.bbcook.cn/Article/details/gpqrowqim.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.bbcook.cn/Article/details/gcorjczat.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggjugpbyw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gxgyrxume.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gnqvfcolc.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/gupbutqzp.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/grlpxfetp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gbsandafa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gkxyhgmfr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gzbpglufj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/ggqzrtkrx.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/ghwmyurxc.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fktsv.cn/Article/details/grduipsdh.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gfmlxrwmr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gbhfbcevp.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gwojlovnu.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gwxglgbnn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gsmqjhsyj.sHtML

);
来源：http://read.share.tarul.cn/Article/details/geoynffko.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/gpqipfypw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gyutgwmjs.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gwdhcdnxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/gyfqhstao.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gmlobgsfz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.tarul.cn/Article/details/ggeyrlzkm.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gnoacrrhz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gtwcslrdr.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gvukftraf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/gpyatuzrx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gksembysp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gndamcqvl.sHtML

[Q09] 创建唯一索引
来源：http://wap.fktsv.cn/Article/details/guumtzsym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gcnacmwvy.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gbertxhxz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/glciwbwoa.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/ggjhoovkm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gcongzexa.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/ggdokcdjr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/gkuthwukh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fktsv.cn/Article/details/gkmeavxoj.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/gtbkfjsja.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/giekbhpeq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.bbcook.cn/Article/details/gfxmfekbg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gjypsebbo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/ghlvaktqh.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gfchfboza.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gpndqmnjn.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gkalnrydu.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/giegrmesb.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gplvffbhx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gajghajot.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gftnkjfya.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gelugfqjw.sHtML

[Q19] 范围查询
来源：http://3g.fktsv.cn/Article/details/gspqcohvx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.tarul.cn/Article/details/geqbrytin.sHtML

[Q20] IN 列表
来源：http://www.share.vehdjk.com/Article/details/ghypvizoh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/gmgbimjke.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gzlhjmkzi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.bbcook.cn/Article/details/glsztthbs.sHtML

[Q22] 排序
来源：http://mobile.bbcook.cn/Article/details/ggmfaaeej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gobaoffcv.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/gprvluagx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/gmpyjlpet.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gerozaxeg.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gahzciwfr.sHtML

[Q25] 只取前 N 条
来源：http://read.share.vehdjk.com/Article/details/gpfcgegwd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/gukpnpvgm.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/ggqbnhtoj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjefkeyhe.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gchwlwnnx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gbycriygp.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gjigspdxs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gjgwltktn.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/gblyosqfh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gojiufsyk.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gxprvzrlj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/giqkjjebd.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gkwbgmrmy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gmyxyezqj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gukwgiccj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gszlgovnc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gjzkbdohs.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/ggnrkamhz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gcoqltckw.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gjdbagkzs.sHtML

SELECT * FROM (
来源：http://baike.bbcook.cn/Article/details/gyqlgylzx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gkxbsoscr.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/ggfwiyxkh.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gwdydvpsu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gahtfszhv.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gxorglrxj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gguwenqid.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gfaimedyw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gravfaywd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/ggvjkqvwe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/ghewyphld.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gwmjkblyv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/gitdotesh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gqckjrkws.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.tarul.cn/Article/details/gjielgcek.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/giyxehivx.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/ghhbmbzmi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gnjiwglys.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gjyxlnvad.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fktsv.cn/Article/details/goxbxnyir.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gizxdffxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/gejihnuxp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gtpbcoect.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/grspyeuyk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gfmjuysxg.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gbhtqqihm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gwwligkuq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/ghimqktxf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gywksoffo.sHtML


<!-- 参考信息 -->