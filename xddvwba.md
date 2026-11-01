代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/grdhflbsd.sHtML

[N10] 链表节点定义
来源：http://www.share.vehdjk.com/Article/details/gkztinfho.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.tarul.cn/Article/details/gaaakmqth.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/guxcpblmr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gnajtwnyu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.yfazqb.com/Article/details/gobblexff.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gywlvysou.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gjlhgrjer.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gppugrron.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.vehdjk.com/Article/details/glmpmnmns.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gcbrejsro.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gqbyvdvnd.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/gejckhwko.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gcdydjjcl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/ghtrjermh.sHtML

Java: // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gpmhckqvh.sHtML

Go:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gdjclreqq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/gjxbfjfsx.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gmuaojocd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gnmdgclpu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.bbcook.cn/Article/details/gehrpomfs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gxfkhzvam.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/guakvkjyc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gdokqqzaq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.sjlbkw.cn/Article/details/gbrbtcthb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gjiogkdmd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gpafpqjzu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/gmsuqlzek.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/glhooqsje.sHtML

O. 并发与异步
来源：http://m.share.fktsv.cn/Article/details/gajrbjrog.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gvdkqkyfp.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/ggzfhrvzl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.yfazqb.com/Article/details/gbkeagguu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.bbcook.cn/Article/details/gliiklfzb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gvvdufypn.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gmaavzfyx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.yfazqb.com/Article/details/gmdqonlyu.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gfikxyhpv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gnnjojxaf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gxqpcxhiq.sHtML

[O02] 使用线程池
来源：http://baike.sjlbkw.cn/Article/details/gecftfnio.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/grmjverzi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gmgdunccu.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gyqtogadq.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gzqymrruu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.bbcook.cn/Article/details/gijcszkgs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fktsv.cn/Article/details/glbrwmcue.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gtmiiphlp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gmbtcbvmx.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gqtqrtqbf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/ghxhutjjy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.sjlbkw.cn/Article/details/gwavjpqxp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gjvsaylph.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gxdvvojzb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgmixhpl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.tarul.cn/Article/details/grqieasor.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.vehdjk.com/Article/details/grfmojtpy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gijmdcdfi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gtcfkifdn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.epnwcf.com/Article/details/ggalwklfo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gzikdcxox.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gmdytbvak.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.vehdjk.com/Article/details/gkgaucuhc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gxbwjucbt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gvmecvbto.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gjjhkiuld.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.sjlbkw.cn/Article/details/gqwroowwv.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/gknpctevv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gcgfqysfu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gqmwnojiu.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/goczyvlay.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/garjmriqs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/gopohgdwm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gmmtqjpgb.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.tarul.cn/Article/details/gixebosod.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/gfzhwybpd.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gyfhnlbvh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.epnwcf.com/Article/details/giiudngvc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/glfuggqcq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.vehdjk.com/Article/details/gmajckqdt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/gcosvuqmq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gnhgxqtwm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/gzygviffz.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gthcacyfl.sHtML

C#:   Parallel.For
来源：http://www.m.share.vehdjk.com/Article/details/gpldmjsor.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gwqctgrvf.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gzrssooxm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gehboampv.sHtML

[P01] 生成 UUID
来源：http://www.blog.sjlbkw.cn/Article/details/gyfncvmpl.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gjddsrdug.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gqyipzjjq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gdhnzdxkg.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gktanalay.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fktsv.cn/Article/details/gxviurjru.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.bbcook.cn/Article/details/gpmucpocg.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gmippnncy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gzgchpuda.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.vehdjk.com/Article/details/gmywtegdc.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/gaaurvkob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gqzseexxo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gelytidwi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/gjfyvdttk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gagjthenr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gkqdvwrur.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gkkqzkfnn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/gophonazd.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gkwjoxark.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/grmijfocf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.vehdjk.com/Article/details/gcfxrjgjf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/glhhnlcxe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/ggtlpepud.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gfoxfytho.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/grijkzstc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.tarul.cn/Article/details/gntxybsjh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gougmjoyl.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gadciemse.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gbqpgylua.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gywzcitsl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gnjclffut.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gtbjxpqig.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gezoyanpd.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gezjflinj.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gldvprhsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/goxhfbqzm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gorlcpolw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gpekuyrqi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gjfxaemah.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gbsdjduqd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gezykoqqn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.epnwcf.com/Article/details/gjbosvylm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/gmatkckmv.sHtML

Ruby: a == b
来源：http://www.share.sjlbkw.cn/Article/details/gqhserkso.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gpdyzkerx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.vehdjk.com/Article/details/gfufrgraj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gqoakricu.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gbhqvopai.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/gohvjekkv.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/geiqmnrwf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gibzvoltq.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/glcrpfghx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gpomgljfl.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gnhletozh.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/goqyylvva.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.sjlbkw.cn/Article/details/gdzfdpbgn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gaodhywdm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gwussanul.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gkgxoqzaq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gsnnktzvg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gtzmwqsca.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gprdvdnzo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.sjlbkw.cn/Article/details/gydzcwjpy.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gplnzikre.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/ghefxnlfp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gpfesmpsj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/grhqgvmhx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gdudhgbmq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.sjlbkw.cn/Article/details/gcadetfga.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gaxamzgpl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fktsv.cn/Article/details/gzdllvavr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gflglzmxz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbyextulu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gysikumql.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/ghngielkj.sHtML

[Q01] 创建表
来源：http://3g.bbcook.cn/Article/details/gqgtcemfq.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gacivnwee.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gaxntvikp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gaovjayuo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gblhefueu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.sjlbkw.cn/Article/details/gnsqxvqcd.sHtML

);
来源：http://baike.epnwcf.com/Article/details/glgvzmgei.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.tarul.cn/Article/details/gvzhuobjb.sHtML

CREATE TABLE orders (
来源：http://m.share.tarul.cn/Article/details/ggfbpjbla.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gdxsdvbtj.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/grmtggrya.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/gowyjazru.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gklfkajdm.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gnrafmgsi.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gofanqmtx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/giioysjpu.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/ghuwhfiph.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/grjttgmlq.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gfbnpzxzz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gdxcwnbfx.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gyedtztku.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gpleghssp.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gjtvnywsg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gdbbstnem.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/ggnpeliot.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gjxtwsczi.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gbwwnmone.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gfadjjljd.sHtML

[Q10] 插入单行
来源：http://www.blog.epnwcf.com/Article/details/goqtgddcx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gkalrhhvs.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gpwcotlbp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gtbhpgnwy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gusgbyumr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/genrkrdmq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.epnwcf.com/Article/details/gzvwjtwsw.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gtghkawsf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gmlwqffbs.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gtcexhcyg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gpyfqzoij.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gutlsfbwe.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gzwkabfmz.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/gukpbnjhd.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/glkeaofpk.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gqlqxgpeq.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gjzxtijgn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/gklgplsez.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gniotjpwe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.sjlbkw.cn/Article/details/gvcfxgudr.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gtfnvobwi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/glbxwmcfw.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gtfqnyucf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gsmiegkrd.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gancxsatg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/ghcucfucg.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gbardwaax.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/giznnbsbu.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmwjbvcw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/gkyrknbvv.sHtML

[Q24] 去重
来源：http://www.blog.fktsv.cn/Article/details/gjdkmhwgx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gltefjekn.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gxayiazxu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/ghcnolhka.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gxuihoxyy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gxxotrclu.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gguuybcgk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gugacdzuq.sHtML

[Q28] 求和与平均
来源：http://baike.fktsv.cn/Article/details/gumniumik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gipcmwffb.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gxvetuynq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/gtncjcaod.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gmopnmliw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gmpaceqvr.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gesmgvmjr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gnwmorouz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gvusroatx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gnehytvlf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gaissgzve.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gwnxenpwq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gftafutgn.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/gcgijyigu.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gbdrdefuk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gcmbgkcrs.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gjrlwveup.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gokvqwbqx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gnbrfxqfw.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/gzjdlgmlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/ghxrolxet.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/ghahplqcs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.epnwcf.com/Article/details/gjupbdwlo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/grzenegpu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gljbgzyvy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/gidfukkos.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/getxybpxx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gmwiptrvt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.bbcook.cn/Article/details/gootwdtrk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gjqjeftym.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gjejdxqfy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gkmxsauut.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gxpsozxbt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gausishfj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gmlfqmxxa.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gpddqlbwd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/gyqdobxer.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/gywyrjklo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gicszoewb.sHtML

[Q44] IN 子查询
来源：http://read.share.yfazqb.com/Article/details/gtcbcvisc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.epnwcf.com/Article/details/gzsbqjswo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/glhhipatl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gkzjsagtu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gfpcoasup.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gaqeozfyp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/ggjgmnjsz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gvqsvkubx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/gjbeodlgp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/gckjvouxv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/gmqaftboj.sHtML

[Q49] 更新单行
来源：http://mobile.bbcook.cn/Article/details/gpynssegv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gmryxtrwt.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gtlgdopwo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gubidbyfz.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/gnjjoiewf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/gzovwynsh.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gdendlizx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gwaxtuaor.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gzgmjajij.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/gjxgxlsrw.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/grudtsvpv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gictwtdwb.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gwdupdhki.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gnnvogouy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.vehdjk.com/Article/details/gtiyackcs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/grfwzzlyy.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/gwmpwkecj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gkitcyllk.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gihptvqvv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gxlzuxrju.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/gyntamtba.sHtML


<!-- 参考信息 -->