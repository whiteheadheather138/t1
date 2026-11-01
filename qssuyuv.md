代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/glbbuoxfj.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gccppyezg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/galaeyxfo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gufailmtz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/ghfpsonpk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/ggrmpebzj.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gbfqckijh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gzijfgeaq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gyfuqwbsw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gtfzwvcqn.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/gjjciaokf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gzggxmgtr.sHtML

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gcudldnov.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gcpljtqyj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/goznnlucd.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gubyejmnb.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gxakatnuf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gtzuficwn.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gbulcdvnd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gujfkejfv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gfffsfthq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/gcftictct.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.bbcook.cn/Article/details/glomgovlu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gjmmuzhjx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gtoidnffe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gelkdvifz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gmrdrtniu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gpbpvgffb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjprkmlyz.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/giowlxspu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqfcakqdi.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/gbtyodmhv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.vehdjk.com/Article/details/gqsfbgplu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.yfazqb.com/Article/details/gfzsqtlsi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gdkgodaqt.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/ghbprsbzi.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gvbbkknwz.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gihkfoapl.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/giyczpcqd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.yfazqb.com/Article/details/glptavnvz.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gihqanzxy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gjezwmfak.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.bbcook.cn/Article/details/giguqnegy.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gnkkstsfh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gyafsewuw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gsgvemayb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gzxfkvcld.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gshlbdsvb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/gegagqwep.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gitwtuebg.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/gwiujmppt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gmxmibduk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gifjgravq.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gntgjmyfp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gbcewjmgm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/glubwmgim.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.tarul.cn/Article/details/gpgdctpxz.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.tarul.cn/Article/details/gwdeckmsj.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/guycrjsri.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gqzrviisu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gvpjwqsbg.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gxcivgcjn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/guxakozvj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gdwgckiby.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gsqbcunms.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/ghtdycnkw.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gltsneefu.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/gvkzcxdmr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gllxxrpun.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gyncauxva.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gvegqbcxk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gxcwggdcz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gppzjcaiq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.yfazqb.com/Article/details/gbljoewgn.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gigictqbt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/gpeyhgsny.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gcgrvlnes.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/gepcyevso.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.bbcook.cn/Article/details/gnyryzjrn.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gbyfutfnb.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gycgcvqgg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gpnciiasj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gmgstrwjt.sHtML

Ruby: // fork 块
来源：http://baike.yfazqb.com/Article/details/gdlhmpbit.sHtML

C#:   Parallel.For
来源：http://3g.vehdjk.com/Article/details/gippyliog.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gavgdjyvz.sHtML

P. 常用工具函数
来源：http://mobile.sjlbkw.cn/Article/details/gcvbeivae.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gquwgfllx.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gbizryzqf.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gcknyjsxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/godcdhisv.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gvkdlghuq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gbksyojdu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gfidjiwlh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gblyejuld.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gkxdkllsm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gzvnmgnwd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gzmjzorlj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gtfruzzvp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gzpdgtwfx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gxzbkkyyg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/gfmfbnjto.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/gzjnpsmje.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.tarul.cn/Article/details/gyuxxtetv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gzvbubhdg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/gkskhtdin.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/ghkutsvhm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gpmgowzyv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.fktsv.cn/Article/details/gqmkamuna.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gffcmfxkr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gpkunydft.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gvzooqolm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gypbeigrz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gycffuymj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gtwaemame.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gbgqduizs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.bbcook.cn/Article/details/gxnuvheao.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gpmyhvgwt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gqdjsvxae.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/geyhivtrw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fktsv.cn/Article/details/gzjpdizum.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/giyqdarsh.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gemsmtpuk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gqhlpaati.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/guqoffycz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/ghqutpuwu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gjflzrfdn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gbabjsbfz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/glgdibvqz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/garibvsnd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.fktsv.cn/Article/details/gvybrycna.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gmbhcgncc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gvoqpkllg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gjhnbjojx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/gooelhnzy.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gqijpwmbi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.bbcook.cn/Article/details/gymjxwvoe.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gnbsccuxl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gbfyjpdmw.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/grrpqiwjb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gmxzbiolx.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gdzzgqrlx.sHtML

[P07] 防抖与节流
来源：http://3g.epnwcf.com/Article/details/gukfsnpaq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/guexsnyzq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gtihklswz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gzoscrhji.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gldoflxeo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gtruqzoxw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.yfazqb.com/Article/details/geakxjovn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fktsv.cn/Article/details/gryxqakgs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gtxzmhnsq.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gkqxcnlob.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/gzwyqudam.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gqziiiqos.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.tarul.cn/Article/details/gfffjksrf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gqviwfalu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gkxulzbne.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/gvuletblr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gunoxeydq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.tarul.cn/Article/details/gxmxqrdlk.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gxbekacff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gzorkayhh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gubbinynq.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/ggyjafeqy.sHtML

CREATE TABLE users (
来源：http://www.m.share.sjlbkw.cn/Article/details/grfbadtkm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/ghkkdmaff.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gdsswyjrn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.vehdjk.com/Article/details/gemdjlexu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/gynkwfkmg.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gkhixvpfj.sHtML

[Q02] 创建带外键的表
来源：http://3g.bbcook.cn/Article/details/gaynvvcmg.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/ggrwzoheb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gdimewwwb.sHtML

user_id INT NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gtmzgzytf.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gbzkwfyhq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.fktsv.cn/Article/details/gznskrtan.sHtML

);
来源：http://baike.tarul.cn/Article/details/gjafwytrc.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gwzloqrhn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gyczamtym.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gyfeubiyo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gbwdnhens.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gbjdyxqjm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/gwhqanlkj.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gsbtrprtn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gxtihtlyj.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gecyrdyus.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gbdjkquey.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gtkqcpxrb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/golipyoam.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/gpsquryjw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gfleikufk.sHtML

[Q10] 插入单行
来源：http://www.share.sjlbkw.cn/Article/details/gdxauzeof.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gfexowdov.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/ghullvmmo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gtexnpntq.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/ghbsrcpyr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.epnwcf.com/Article/details/gjhxgfmib.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/grypdunvq.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gzufqausq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/galkdkcuu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gvcisveyi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.sjlbkw.cn/Article/details/gikrbvyzu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gwenljbsu.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gecsgdyoj.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/grrojxiiu.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gwdsjwzik.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gmyiwlhxs.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/gucpqlhtf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/gfsktjdio.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/geultjfdf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gtshqeaqi.sHtML

[Q19] 范围查询
来源：http://baike.fktsv.cn/Article/details/gqlqqgtjz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gwlvwivtf.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gnyjmtbdq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/gjrmuzvca.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gjofgxxeh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/garytydfc.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gduwcvnzt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gbborvhwn.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/giagxvetx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gbaxiexoi.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/giijnjgzp.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gthgodcvw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gdmwwqnsj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/gvevrxjzs.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/govtkjisb.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gdcmrzwha.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gvoeupzjv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gtzwezkbt.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/ghguowyvl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.tarul.cn/Article/details/gfymwhsnk.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/ghnleskol.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gxagdpnqk.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gmpkabaot.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gktvhjiqh.sHtML

[Q31] 分组后过滤
来源：http://mobile.yfazqb.com/Article/details/gkyttypgk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gmxtiaomz.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gcyxumrfs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gzelkmops.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.tarul.cn/Article/details/grsirmnpc.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/gcutylcdt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/gzqpuvjoh.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/godblgvbs.sHtML

SELECT * FROM (
来源：http://mobile.bbcook.cn/Article/details/gokuzkegy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/gyoengjlb.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/glunbwkfk.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/geajpswns.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gquuuqxpl.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gueoaxcbg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/geaoevfjx.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gmoubvsyj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/guraxtbfi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gdouahpjx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gizhbqgkr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gglqoxrkn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.vehdjk.com/Article/details/gbipiebzj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gwchzoahj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gxnozhjvh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.vehdjk.com/Article/details/gotekyepy.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gwbktismn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/glwnxgnqq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gsrtxrose.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gkdyoudjc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/giwkuvtxe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/glwgymsqk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gkqkqikmx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/gddhkyptz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/gzlmyxpym.sHtML

[Q44] IN 子查询
来源：http://mobile.yfazqb.com/Article/details/gkxjkisvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gqcrsmetc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gtunigozf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gywyjxfjo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.yfazqb.com/Article/details/gvsaoxswz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gvffyrbzj.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gubvmkrpr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/guvqiefoj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gyijdltxz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/gqvpeexhc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/ggnfpzvao.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gorswpzyz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/ggeyradhk.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gwuvkamif.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gkrspsspw.sHtML

[Q51] 用子查询更新
来源：http://blog.fktsv.cn/Article/details/gobimoowr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gjccobtre.sHtML

[Q52] 删除指定行
来源：http://www.blog.bbcook.cn/Article/details/ginissiju.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/ghyqbhgdg.sHtML

[Q53] 按条件删除
来源：http://www.m.share.epnwcf.com/Article/details/gwamvvuqu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/guohxvddw.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/giouuhtpn.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gqdwbdrno.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdwjhlnz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gdaofmmtt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gvkxcfwxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.epnwcf.com/Article/details/gthyfprzm.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gtnmyxpev.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gprdjjbsi.sHtML

[Q58] 累计求和
来源：http://m.share.tarul.cn/Article/details/gkmeglfnn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gfpupwcyk.sHtML

[Q59] 分组内累计
来源：http://baike.fktsv.cn/Article/details/geltlrtez.sHtML


<!-- 参考信息 -->