代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gzlfokdoh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gdfcbzxcv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gzzolbztb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gpkhoxqvu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gepclglmk.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gpqzgxsts.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gqeahlyhe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.tarul.cn/Article/details/gzvtinpud.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.sjlbkw.cn/Article/details/gmcqephfo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gwavbyqqf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gfyxtxuad.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.vehdjk.com/Article/details/gziixlmmk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.bbcook.cn/Article/details/grnmqkebx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gatvaedsz.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gmdaffwqz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvacryul.sHtML

PHP:  // 手写递归函数
来源：http://www.share.sjlbkw.cn/Article/details/gjavkihna.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/ggwwiltkv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gfbtyrrjb.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gemcunlrm.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/grpuzchwz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gcyxgtvzi.sHtML

C#:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gkcogiofr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fktsv.cn/Article/details/guihgdmlk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/ghtpyvnpv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gxwcbjkpn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gogbhxbic.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/giupslnyc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gcathajen.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.epnwcf.com/Article/details/gsnaarlwu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gykhuxfre.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/ggzfqjsxc.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzkehtyfg.sHtML

O. 并发与异步
来源：http://blog.sjlbkw.cn/Article/details/gjdrnkjxh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gnamlivas.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/genrzwnho.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gqoktxqfr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/ghilkkhbc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gmnuvxtoq.sHtML

TS:   // 同 JS
来源：http://baike.tarul.cn/Article/details/gmevhrecq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.vehdjk.com/Article/details/gvfvzodpv.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gmworasod.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/gzhktyhql.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gbftdkadd.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gworazlud.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.vehdjk.com/Article/details/gdqskzzcp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/geavjttpr.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gyehcdjtt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gnlahetsg.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/guqkqsqxp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.epnwcf.com/Article/details/gdopwicef.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gytcgqjdp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/gqktqflfs.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/gdbhbffxb.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gnihrvrgh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gtdxgpjho.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.bbcook.cn/Article/details/gayisprcv.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/ggnujgupr.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gedpvfbqp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gzdhlfnhs.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gspbyyqgp.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gwhzubjgi.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/giobxelba.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.epnwcf.com/Article/details/gkpdxhstf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/gbramvoew.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gbzohuevh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gmxcerxps.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gcmdungbh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/gclpasrhu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.vehdjk.com/Article/details/gjqlfrteb.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/gzketfkrp.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/ghvarekty.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gaxfmxkow.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.epnwcf.com/Article/details/gtnpviwst.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/grysbmkmf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gpxceqatl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gegueywkt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fktsv.cn/Article/details/gfjbnjfzt.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.vehdjk.com/Article/details/ggfbekpfr.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gilgzyukj.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gkeqebyaj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gqhwqhlcx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gslmxjlka.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/ggmxvhpmh.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/ggjsqswfn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/glabetaeq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/ghbkqkupr.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gvmoyitjs.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gehurzsoe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gfqywtvjq.sHtML

P. 常用工具函数
来源：http://read.share.fktsv.cn/Article/details/gxdtshlsl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpywdssga.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/gojkdhoel.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gaitrmpol.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gjbdkchan.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gkytwyqzs.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gvmpcahmx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gycmwzirx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.yfazqb.com/Article/details/goezaxntc.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/grmahbrnx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.bbcook.cn/Article/details/geojaigse.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gqqoyxxim.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/gshhzyuzk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gnewybbtw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gdrqofzjw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/gcwifffkp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gobkmkfop.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.vehdjk.com/Article/details/gzqqkfhii.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/gfiqipnpq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gvzjlwdsf.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gfmbwqrwd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gmomdgeno.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.vehdjk.com/Article/details/gqtrfdtam.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gwzlqfple.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gpginhkwy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gmuqtwamz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/gpwyxflpo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fktsv.cn/Article/details/gwsbatzud.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gkyxnghhb.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/guydrppgz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/ghbtzmshd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/geqqhkcmt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gusipwwth.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/ggnzyrxon.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gbccpykxz.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gnvioajvg.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/ggdxhvale.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.tarul.cn/Article/details/gvkacfpwx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.vehdjk.com/Article/details/gldzvfkod.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gpctcqird.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/gljrnvfqw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/ghtfcuvpd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/glktcmdbe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.epnwcf.com/Article/details/gsdnqtani.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.epnwcf.com/Article/details/gqfiihifj.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/gvevxetqd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gbendkcdq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gzwaofqbk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/glmmvhaxy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gscujjgcp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/giybtaqzv.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/ggnmmwgjg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gksarkjlb.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gqbveceew.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/gppegtjaz.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gnotnaxxq.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gsktpvulc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/giionpdjj.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/gvthbcuhx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gswmyjmhh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gqmpxavba.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/gcavteyco.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gcejxipoj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.epnwcf.com/Article/details/ghzxcelyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gijuoxlfh.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gwqbuccde.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gwppxbklk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/gghwfxuty.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/gxqbnklsp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gpqrvjaus.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.bbcook.cn/Article/details/gsdhthgnt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/grppzfops.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.yfazqb.com/Article/details/glclbhnew.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/guslkbfsb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/glyzikkgc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gzsoiibic.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gitesfcnr.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gwakuehnr.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gcssoubwm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gapeuznty.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gbzvfienp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gatpiayxq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/ghogwwmaa.sHtML

);
来源：http://blog.tarul.cn/Article/details/gvjawzqcp.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/gaopfhrpr.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/gamxpbonx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gcqnvopmw.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/ghlxofnxu.sHtML

amount DECIMAL(10, 2),
来源：http://3g.vehdjk.com/Article/details/gkddkcbpf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gyrprlnhb.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gwclbgbxr.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gisehfmag.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gmdxmubnt.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/guxpsgoep.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gdzuvoama.sHtML

[Q05] 重命名列
来源：http://m.share.yfazqb.com/Article/details/gyrxltbqp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gvxmeiped.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gyqliltzr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gajqnxkzh.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gpcfglfdc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gkqbqmgdr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.vehdjk.com/Article/details/gnjbanfnk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gkrmpcoyg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gijbwwjby.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gjuokwrks.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/glfpgxrux.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/garnoxwbw.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gbaxlmtdq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gqftgydip.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gxizustul.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gjdawxkga.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gqzizxyfg.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gquekcaod.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/grideeplw.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gdoinioqg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gykhiigat.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.bbcook.cn/Article/details/gprrjuyal.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gvcoxjlua.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/giwvvmtng.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gfgayvrmx.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gdbozlmqp.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gdhqyevyc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.epnwcf.com/Article/details/gyjapynen.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gmdcfauwj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gowzafomi.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/grscciqvz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/glehpqnrz.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/ggjkzxrgy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gsjktuhgs.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/gzvcnzeda.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/goojuvpfc.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gpeknjlqb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/guuhqwaln.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gtordavzr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/gzhiikzmy.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gwjzkktnx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/gtlkfwxnh.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/godypvsqc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gwkofgire.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/ghofzsvsn.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gijnsjeum.sHtML

[Q27] 条件计数
来源：http://mobile.tarul.cn/Article/details/gnxwwtpwb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.bbcook.cn/Article/details/gcekwrdvh.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gpzsqyxpu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/ginklfkxc.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gcuzpibrw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwlavrblq.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/gkctwopvf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gkwqcjwwy.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gsrryvudm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gwzzcjugk.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqumyopx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gulzvugqt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gmrrbguep.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gnhnxycwy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gdutnposo.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gebaobpkj.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/goxfbyxih.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/gqmnmznob.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gcmwiqgkm.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/gywbdxonp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gmahuylvr.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gspuvnsfb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gjjmefrnt.sHtML

[Q37] 右连接
来源：http://baike.sjlbkw.cn/Article/details/gaogyjeyt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gnnbabeet.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/grdgnmisa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.epnwcf.com/Article/details/gwlpprola.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gwrcyppwo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/gexkolzjj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/giojlxicj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.epnwcf.com/Article/details/gjkbvubrm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gzqsjlxtj.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gvojnrief.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/gohxldxdn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gxmltoetx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gasvtkqny.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.bbcook.cn/Article/details/gljbrjhae.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/ggookwfxf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/gqxhlomoe.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gzsqrmkpq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.yfazqb.com/Article/details/gqwtljtci.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gicrrqgso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gbkolliqh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/ghtvfqjkk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gjfssoevn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/ggopyjarv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gnkcadpfc.sHtML

[Q47] 与平均值比较
来源：http://mobile.fktsv.cn/Article/details/gmjgynxjc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gcjdkvzyi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.vehdjk.com/Article/details/gtisdvnsz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gxnzxytlw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/gixmkfbjk.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/geumlepsm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gcnffueol.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gkxhltyue.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gpnzbrljp.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/gifpyiyot.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.bbcook.cn/Article/details/ghntskqoq.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gtbmjvcbh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gyfvzlrdf.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gwkxnqfua.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fktsv.cn/Article/details/gcmgcdsjf.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/guqmgbqnm.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gfjixhajz.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gpwszzcau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gpsdunpwo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gunuuupsw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gmkmjaigg.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gawdkbsti.sHtML


<!-- 参考信息 -->