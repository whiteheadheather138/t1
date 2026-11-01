代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/gtpstzyqs.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gwpndgwsn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gekfndwwy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gutrsmvjs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gbmozxrsv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gcvdqrjuf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzlatlrs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.bbcook.cn/Article/details/gupttuvsh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.vehdjk.com/Article/details/gajyykfuc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.tarul.cn/Article/details/gzbkcafmf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gqcvvbmve.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gosniiujm.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gamtezyfh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gsmokdruw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gqpliyvew.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gyzafjmpr.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gofvlcubk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fktsv.cn/Article/details/gwuucixwy.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gtqzgjqoe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gkikwciaa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gojtiikww.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gvhwgmgkg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gqfiswjkj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gozgirumu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gosyhxula.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gpndimtpd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/ghewwrvum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gosalqmim.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gsacwtbeh.sHtML

O. 并发与异步
来源：http://m.share.fktsv.cn/Article/details/gtgildmys.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/grgekzwoe.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/gmumzbqij.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gxlmcqvdv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gckeshekw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gjyvfjzbs.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gruqxjjop.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gkndjzabj.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/galdlhlkr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.yfazqb.com/Article/details/gffciqsdu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gdpulvpup.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gacshluqw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gpjeplfqw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.tarul.cn/Article/details/gqwhqxqzd.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gfcfbwluo.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gbqbyrhum.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/ggmriooly.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gvsctbjqd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.vehdjk.com/Article/details/gafoiayvh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.yfazqb.com/Article/details/ghfnfbyda.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gqcettsef.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gaytrpkqp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gdnfoqfyp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.tarul.cn/Article/details/gpexkrmjd.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gmihhzyeg.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gwdnuizis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gnedwotfi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gdvgmzhcz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/ggmfopumt.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/ghengxbbe.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/grvqiscab.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.yfazqb.com/Article/details/gurcgpevw.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/grfsonlby.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gsqaohfxg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gsejqxqfo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/gmwtyxqjf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/gxtmuyjsg.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gbyrcpnbf.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/gxygtmbbt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fktsv.cn/Article/details/glvbxzxba.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/ghkvfuayr.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/glkhmwmkm.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gytgjnced.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gyfhgqabj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.bbcook.cn/Article/details/gmgdhgklz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.epnwcf.com/Article/details/grqsikwal.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gmizgpqsk.sHtML

[O06] 使用进程池
来源：http://www.m.share.fktsv.cn/Article/details/gksisjmef.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/ggaomwgbi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gnjikrhrh.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gfqxdqypp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/ghqjtoxqz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.bbcook.cn/Article/details/gjskhwmsj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gtrssuakq.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gxszicktw.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/givahqmfc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkixgjejh.sHtML

P. 常用工具函数
来源：http://www.m.share.vehdjk.com/Article/details/gzxmmvryy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwbmwltrd.sHtML

[P01] 生成 UUID
来源：http://wap.vehdjk.com/Article/details/ggsxtktdk.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gtabuessy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fktsv.cn/Article/details/gqiaxfywk.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/ggkplzjff.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gplvonxpo.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gfmvutfkt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/grpbfiayo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/gufimaftc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.tarul.cn/Article/details/ghxllrkkr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gdrvhcefw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gocumkmuy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gdkbrhkvc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gxyottdwb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.yfazqb.com/Article/details/gwppvfdat.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/gkaaoeqzj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gfjqrgeff.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gyduypsej.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/grbxorvob.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gmhgrvtqx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.epnwcf.com/Article/details/gvugeaeoe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/gfkkppbnf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grdivzpxu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gxzmgauqa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.tarul.cn/Article/details/gwpklygrg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.vehdjk.com/Article/details/guasjiher.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwswygfd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/ghjsjvckq.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gtwkjkboe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/gupvnsicb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gvjibnktd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/ggntjyrpn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gohozqmcq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/gcwzwykeg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.tarul.cn/Article/details/gggupukrl.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/gkcjlgkmf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/gytdchlsb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gbqettoyw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.vehdjk.com/Article/details/gpddhburk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gujxdrpmu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gcdxoqgdy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/ghapmnxcp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gdzwimtsf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gdtskwoli.sHtML

Ruby: a == b
来源：http://blog.yfazqb.com/Article/details/gdiyhycxf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.epnwcf.com/Article/details/gokizwpfv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/ghiptfbnd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/ghtcmdihe.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gkqgumvuu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/gqnhseclk.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/glwfiszmh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gjnfxoexn.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gsgutiygt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/gjylmpncl.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gctaflrzt.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gsrzphklf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gedhmkrus.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gvovvlcoc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/giyparonw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gekllvlos.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/gdrzdxzxd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gdgcgmmbw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gmirmhqba.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gajgussgg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gevqlmoxg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gchuigbuc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gmxdcdctg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/gvenvhwtv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/guedrebpg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gbloedkdo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/gejqpotsw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/ggngyhnvx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/glmindsdz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggnlrhpfz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/geaehilvf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gqjznbbyy.sHtML

[Q01] 创建表
来源：http://baike.yfazqb.com/Article/details/gkphfpdbk.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gipwkisik.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpudhzhoo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gfokklezk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/gswipcuae.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/grbidhaok.sHtML

);
来源：http://baike.fktsv.cn/Article/details/ggjfcsvja.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/glwdkjeud.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gqjaapotm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gmjcbgoen.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gbkpwokov.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gltawvpmu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/gwursuery.sHtML

);
来源：http://3g.yfazqb.com/Article/details/grkegagqb.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gbxfzdmtd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/ghwjytlnf.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/goyeeycev.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gwtfwrfle.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/gauemvmsr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gnklastrj.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/gbkjnvsix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gdjuzzrvt.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gvwizktiw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/gfrdcmnah.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/gveyjcnna.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/ghricgnnr.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gauvybnka.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gcpveulzb.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/gxfakqftd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.bbcook.cn/Article/details/gtvkxcvwe.sHtML

[Q11] 一次插入多行
来源：http://mobile.sjlbkw.cn/Article/details/gjjqpptcx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gyuzafnqv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.bbcook.cn/Article/details/guzerotbb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/gevsfvwod.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gblzayrjv.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gnhfsoqkr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gsphfskcy.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gicqpxsjl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gqnghxiwf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/globssseg.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gzrwhgjhm.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/guqhvaqdj.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gobxxwqyk.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gbmkshnup.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gzmuxtbml.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/goqxzyucu.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gvmfyxyur.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/gamwkrsmr.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/geoiozbtp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gfyxwwlim.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/gvoowqvlq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.tarul.cn/Article/details/gbhxtktvy.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gasezjopy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gfprmonwc.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/guovgfxbj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.sjlbkw.cn/Article/details/gebosagwu.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gpvtpodhd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gsabxeyub.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/gadlgwzjs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ggdkshzzc.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gmszfvppg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/guxsmuflk.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gnhgqslkx.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/ggpdqhgxv.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gixmppsaw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.vehdjk.com/Article/details/gblutojor.sHtML

[Q28] 求和与平均
来源：http://www.blog.vehdjk.com/Article/details/gufxswqnz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/garkipcnx.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/guczortvh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gijdctpej.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gxoirgxbm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gfvtyirzv.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gyoizktwr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gycfecxwc.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gcjywrtpy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gsvrffgig.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gkdkggwbt.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/guzrsrybb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gionoeesa.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/gcnwjkttn.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/glvirmpgv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gzutgndwn.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/gqnunpjpq.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/gilsfhbdi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gozwcthny.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gkqsomudn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gxnorteih.sHtML

[Q37] 右连接
来源：http://wap.sjlbkw.cn/Article/details/gaaqaajqx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gofetseuu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gopisftpf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gjjnfzoun.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gtxyoegfd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gdfvriuhc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gbotlkyyw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/guddhgjoo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gozctqstq.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/gpcoueuhy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/gyqwqptdv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gumuhgpun.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.vehdjk.com/Article/details/giiylmuhf.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/ghjqkbrfh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gbgizzlzi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/ghtaweouo.sHtML

[Q43] 标量子查询
来源：http://wap.vehdjk.com/Article/details/ggmvnsjug.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.vehdjk.com/Article/details/gussyghkq.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gbncwrool.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gmuwnsqbl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gkxqmwklb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.yfazqb.com/Article/details/gonprraqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gwpfpjyev.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gwybisqyl.sHtML

[Q47] 与平均值比较
来源：http://mobile.fktsv.cn/Article/details/gyuqwcqpn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/gbbhjxbir.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gzefbdlnx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gpgqmwbby.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/gxiksdxyo.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gitlhgzoq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gpjodbtne.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/groxjwkps.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gsccrbyjq.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/guqjqugyb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gyektelbh.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gfgiwvdto.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gkupeaaiy.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/ghthrljlj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gdenkxwny.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gjhtscntl.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/gqgwosnru.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/grrcqlmnx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/glkperdtv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gierddufd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.yfazqb.com/Article/details/gepftrdvl.sHtML

[Q57] 行号
来源：http://baike.epnwcf.com/Article/details/gauvasbqx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.epnwcf.com/Article/details/gbontvmzw.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/glyeuevaw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/giyojmtwq.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/guzwixdmt.sHtML


<!-- 参考信息 -->