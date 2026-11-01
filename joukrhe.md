代发 wailian999

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnpogxkj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gbjsyyekj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/ggulfrwnm.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/giqahwxak.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/glxaddcsb.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/ghckfqvwp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.tarul.cn/Article/details/gnyqrpyap.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gfxxuvftd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gyvijamvr.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gatvwhagw.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gmfgqhgbf.sHtML

TS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gdycytpaa.sHtML

Java: // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gdzmzltqw.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gzvkxieqg.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gkypkzdft.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gifdxjgyd.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/ghfqrutjl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/glsknxbuh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gxsukphgc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/grbbuhffk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.bbcook.cn/Article/details/gbbhozqam.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.tarul.cn/Article/details/gfkduuidi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.vehdjk.com/Article/details/gqcydlssn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gvusmclcr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.vehdjk.com/Article/details/gswdmmnql.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gugphztvr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gegpmyivr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gdcdajyjo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gxcaonzik.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/gjixxeokq.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gekvlqmng.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/ghfffzwhc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gmqkjlmwq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/glaviyqwy.sHtML

[N11] 二叉树中序遍历
来源：http://wap.epnwcf.com/Article/details/gdakwqiyo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.yfazqb.com/Article/details/ghntzcvhs.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gyeljfsgq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gjqiiajph.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.epnwcf.com/Article/details/glzzkdkcg.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/gjgecdyfw.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gzflhpvuq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gzafeqhfj.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gyzrnjtja.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.tarul.cn/Article/details/gyjcwpcss.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.yfazqb.com/Article/details/gbtlsmlqe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gkzujoess.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gypaftoas.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gqboqqsva.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gaydvnhcm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.tarul.cn/Article/details/gaamwklyx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/ggieydlsd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gevkdnxqi.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gsmnnazwg.sHtML

O. 并发与异步
来源：http://read.share.sjlbkw.cn/Article/details/gcvkvgbht.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gycdkoowa.sHtML

[O01] 启动一个线程
来源：http://3g.bbcook.cn/Article/details/goymcqtza.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gsjrriwmz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/glewwkgpx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gnkomhgpd.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gdtuviigd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gkgwvvfyp.sHtML

Go:   go f()
来源：http://www.share.sjlbkw.cn/Article/details/gdvydqdwf.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gxbmepgcw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/gpwexpitj.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gbcirvrsn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/grdugdvtb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gpbwgvoyv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gwhbqoeoa.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gdlcayotb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/ggskakdvs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/gpfdnjfbv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gratfuvwb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/gulacwrqy.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gkkhakvgp.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gdlxbozek.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gqpzcoyqf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gynsxhkbw.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gtioodawk.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gzonjusgj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/gjfclupuf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.bbcook.cn/Article/details/gfkczjqtr.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/glefapefy.sHtML

[O04] 定义异步函数并等待
来源：http://baike.tarul.cn/Article/details/gfilynzcl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/ghkropwtm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/graofwioo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gyerhdhda.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gblyckwvw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.yfazqb.com/Article/details/gzxtbxgel.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gtdcjzrxr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/gmbaxaryr.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gxbrbwyat.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gdkmojcnm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gxkkndvxc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gblomgggt.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gexrgwphg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gkbykptik.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.vehdjk.com/Article/details/gfouvexqa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gjdighrhf.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gwwbwulyb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/glcjfpsmm.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gbomwvcrr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/glxlhjlwg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gbrwzmket.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gdjxrmfck.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/grzpgrkih.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/glvndfojo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gkgufkbow.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/ggkiafxmr.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/ghwrxztud.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gdjpmmumi.sHtML

P. 常用工具函数
来源：http://www.share.epnwcf.com/Article/details/gwpejnokd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gyidgvpjv.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gjwabwsgv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gbouxldby.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/gvgtoseth.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gugkveaux.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gcuvjfqee.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gqgbjoidv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gwfdqscng.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/ggztimtzh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/gujxnhoeq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.sjlbkw.cn/Article/details/gwwoaiyoz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gqbntxdnw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcmyxcugz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/gscsizsrq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.bbcook.cn/Article/details/ggokpmlkr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gapktdmxz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gzkmyrtnc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gnavttqdd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gskfltswd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.vehdjk.com/Article/details/gjcvtupzr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/ghgmkcmfi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gekmcjmdy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gevxgomcq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxesaptna.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gmyqyqgzh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/ggczwbyzw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/gtqvxsffc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gqyhuinxc.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/gkriqbrya.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gkqackapi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/geskvftrk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gboxstfix.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/ghvgwofsq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gkyxvvhgw.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/giokxzogj.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/glthwetcm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/gxjqhjbqd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gmfdqhnpi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/guhachmwh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpdrakmm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.epnwcf.com/Article/details/gzesrqwfu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gurjpvazc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.bbcook.cn/Article/details/gjkdtjqzg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gytzywmmg.sHtML

Ruby: a == b
来源：http://read.share.bbcook.cn/Article/details/gsnupoqjr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gezccxoyu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gtricgjzc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gapuakrvv.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gmazoqldn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.sjlbkw.cn/Article/details/gnbptbrjp.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/genoejbqr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gbptkejhw.sHtML

Go:   if x == nil {}
来源：http://wap.bbcook.cn/Article/details/gcqjdeejt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.tarul.cn/Article/details/gogyzsdef.sHtML

C#:   if (x is null) {}
来源：http://www.blog.bbcook.cn/Article/details/ggpcvsvvl.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gtemibarf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gqsdqxphu.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.vehdjk.com/Article/details/gtmfibsoh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gsqqopiby.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gvtxsyamv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/gdwmzvymj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gugagolct.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gfunwugyr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/guynwrvbk.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gahonxrzy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/glyfxbaux.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gqonydsji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.bbcook.cn/Article/details/guxvjodkr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/goufupfnt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gkdwyrnii.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gbxpdpqto.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gyanpubqb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gjkzbncwv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gcodsxlfo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.epnwcf.com/Article/details/grnlnxlqs.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghibionxg.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/gzlwaooxn.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gnyedbdbr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gsnsqufkx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gpxpabywg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gxyqmrpwu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gyxikerer.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gsyxlfjjd.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/ggcrvqagr.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/guvnlpkin.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/ghwrfoash.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gzaqmwpyy.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/ghgnbhbdh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/gzkymaoqq.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gtuacqwqc.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gkfdvuxpv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/girwunmmc.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gkoylienn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/ghlgnqpcu.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gglwxwxjo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/ghvpkwzaq.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/gekargadr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gwehyiwxp.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/ghgceacdy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gkidhifat.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/grsctbvlb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gxxcthnno.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/guhiyxxpt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gzxjnbjjq.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gemetowae.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.epnwcf.com/Article/details/gisyekeri.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gfqgxvgwb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.bbcook.cn/Article/details/gvucbowcs.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gtcinpxhu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gyditccxs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/ggjxoijcc.sHtML

[Q13] 忽略重复插入
来源：http://read.share.sjlbkw.cn/Article/details/gykihaxhh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gudhbycff.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/gyhhsvtjx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxcimqcc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gakrhxkrs.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gjdaymcsg.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gncyvvkrq.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gbjxlqlsi.sHtML

SELECT id, name FROM users;
来源：http://baike.yfazqb.com/Article/details/ganqgwwos.sHtML

[Q17] 条件查询
来源：http://mobile.fktsv.cn/Article/details/ggrpsvlgh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.bbcook.cn/Article/details/gaeltmegm.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gitvojusj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/guskxehxe.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/grcmmehya.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gjpgsnyoa.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gdavyflqq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.bbcook.cn/Article/details/gnahwkmit.sHtML

[Q21] 空值判断
来源：http://3g.epnwcf.com/Article/details/grqivtlpp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gbeizfges.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gyazqjcsq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gtikalohd.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gffqujbtd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/geilaaows.sHtML

[Q24] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gstedtmyi.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gghrqmhiw.sHtML

[Q25] 只取前 N 条
来源：http://3g.vehdjk.com/Article/details/gjrjvxoib.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gqjoelvgx.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gvjkoqvlm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gorxxtrns.sHtML

[Q27] 条件计数
来源：http://3g.epnwcf.com/Article/details/glfjnpgun.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gwirtcgux.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/gdjbtmoje.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gxmsfzyhg.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gupbivzfo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gcnzhhwde.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gxeyxvgpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gevbpsdfy.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gulhwmmun.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gwsorhcfo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gggijufhh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gnjafvecj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gphbpcuri.sHtML

[Q33] 多列分组
来源：http://www.blog.vehdjk.com/Article/details/gkrgzauum.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/grunuipia.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/grfsapfod.sHtML

SELECT * FROM (
来源：http://m.share.bbcook.cn/Article/details/gqwurbsad.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/gmjzqmdlj.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/gylrgfpnp.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gfrkhiape.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gbqyeevfs.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/geoblwjtj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gvkylrbyz.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gywtniauo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/gyefanfye.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/gfcgurmks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gzkihdoaa.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/ghyeqhfld.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gwcwiykfn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/ggmjiowyi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gnjbspkch.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gmlsakupk.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/ggoqrvlhq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/gyceygjul.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gbwkvalui.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gbrhcglxf.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gmwkepikj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/geimsffjd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/glrvkvald.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gctfaprgn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/ghsaaguum.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gwisetphl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gpiwuigwy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/grqqrvexe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gdhqxspkj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gpefncswy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gdpnhwity.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/griuzsesi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gwnksmwhg.sHtML


<!-- 参考信息 -->