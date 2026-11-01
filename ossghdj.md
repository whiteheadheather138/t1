代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/gbmejhhqy.sHtML

[N10] 链表节点定义
来源：http://www.blog.bbcook.cn/Article/details/gewnsaehh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/glffoqokz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/guuuuqiev.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gibcdeuai.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/gmrdwzsxz.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/glaybktan.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.yfazqb.com/Article/details/gghfvwyej.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/glmnacgxx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/giazrcwyk.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gqhaiojda.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/glfxmbdyb.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gbwhmwcal.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/grsajthov.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.yfazqb.com/Article/details/gxqngaukb.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gyrnxoplk.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gcrxqfgxc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.yfazqb.com/Article/details/gberpovvb.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gpotklsvn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gucmhsmax.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.yfazqb.com/Article/details/gptjixuhg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/grtdnkisd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gsqgowkdh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gwuskebgh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gyhlonohf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitqfnbly.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/ggyyvdfkv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gcfaotmgg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gyzehklth.sHtML

O. 并发与异步
来源：http://www.blog.sjlbkw.cn/Article/details/gjjuzjqcc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/giaacgazt.sHtML

[O01] 启动一个线程
来源：http://m.share.bbcook.cn/Article/details/ghrgwofpt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.vehdjk.com/Article/details/gwiaywxoc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gkpnkzkfr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/glegnrygv.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/glwlbptro.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gvtkqtfeb.sHtML

Go:   go f()
来源：http://www.m.share.epnwcf.com/Article/details/gzttloiio.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gehalsbyg.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/glqfrkrbc.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gvblimmeq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.tarul.cn/Article/details/gzejnclfd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gobuzuyog.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gbjrqcmoz.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gdazjblea.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gxiqjoyqq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gfccnguzu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gafetrbnq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.tarul.cn/Article/details/gkgncuygq.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gchsxdleg.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gygcibsfa.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fktsv.cn/Article/details/gvsimrbxu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/gtuofompd.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gxcxovwog.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gaabqlfwt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gwrmorttx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/gyjmjwvgj.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gcamaryvp.sHtML

[O04] 定义异步函数并等待
来源：http://blog.tarul.cn/Article/details/gscjllayc.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gczzptrnf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.tarul.cn/Article/details/gjlceeveq.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/ggttfojxg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/gwkbpeyqf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gumvfwzgg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/grkkaduri.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/gbwchaqht.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gzpaovbjd.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/glygcqnbs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gifpmifym.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.vehdjk.com/Article/details/gljmtivsy.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gwvwocitf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/goafjtekl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fktsv.cn/Article/details/gogfhvzdr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gmrxzhove.sHtML

Ruby: threads.map(&:join)
来源：http://3g.yfazqb.com/Article/details/gvuluehqi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gpiofqbww.sHtML

[O06] 使用进程池
来源：http://www.share.fktsv.cn/Article/details/gindzctvd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gixaayzct.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.tarul.cn/Article/details/goxzckrty.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gqiluzypa.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gnanqrlih.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gyklxoqcx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.vehdjk.com/Article/details/gilkdmont.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gzeqjrgxy.sHtML

C#:   Parallel.For
来源：http://www.blog.yfazqb.com/Article/details/gptcjqsac.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gtzdwcptu.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/glkcnalul.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gimyotgfj.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gczrldovm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.bbcook.cn/Article/details/gfeclrrsh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.vehdjk.com/Article/details/gelnuespm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gnhbrommb.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gulfynvbj.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/gahenkwdx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gfcrvjplv.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/ggcvualcp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gygrafvuw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gfmoprled.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gpvlaxzas.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkegbgubt.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/grrskzeqh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fktsv.cn/Article/details/gnymxkwjh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fktsv.cn/Article/details/gvnwsvsaa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/giwwpmhjh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/glwrgnmvm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.tarul.cn/Article/details/gcvfwoces.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/ghtowgvwg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gakpuxcoh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.bbcook.cn/Article/details/guzcktytb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/ghhzgfhpc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gouzucuju.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gmnwticzc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gvsbabmzm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/giuqgqszf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gojbzoxmg.sHtML

[P04] 求长度
来源：http://blog.yfazqb.com/Article/details/gwmflrycr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/ghysmnpbm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/gpljkwpjd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gwnefptga.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gvlqunrtz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gexxqubsr.sHtML

Go:   len(arr);  len(m)
来源：http://wap.sjlbkw.cn/Article/details/gnsxgbxls.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fktsv.cn/Article/details/gopptljag.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/grabncnyd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gojlbpzzp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.vehdjk.com/Article/details/gtaqchkht.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/gbrpmvqwy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gdiwqgaap.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gnjhipmrw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/ghdvbbzas.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gqqpwwold.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/gndxqtpss.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.epnwcf.com/Article/details/grzfnirzt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.bbcook.cn/Article/details/gnivnkmhh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gdvlgqjul.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gporuuvgf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gqlwhevuh.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gistecijr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gteoyuuwu.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/grdwnzavt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gzntwslqj.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gcypjmlgb.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/gkqzvmusq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gpeetshaz.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gviaqnskl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/goirtcjmn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gcbfpjnxi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/ggmbzekbu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.sjlbkw.cn/Article/details/gvgzqpwuo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/glxcmzklo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.bbcook.cn/Article/details/gkdilluqx.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gldevtbvm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/grzkydbqo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.bbcook.cn/Article/details/gakpxjpfx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gqqtsfogc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gqqrhgnel.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gjsffxhnn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gybcufoaa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.bbcook.cn/Article/details/gicpmyokm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/gwctxcbop.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtjckkmqd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gdnbcxash.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvvprvpyp.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gjakixgkq.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gkijfapxx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gjtregagu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gqnpkptyd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/ggqecsrsz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gauaddqrd.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/glorxlill.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fktsv.cn/Article/details/gvjetzuif.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gjclvhxxs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gjuihdmyg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gufrecfeu.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gpuiqpqzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.bbcook.cn/Article/details/gwwunopad.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gmlecmout.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/gnjimxplb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gmupgwegb.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gljeptqhh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/guyueyctn.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/gslyopvrs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gxlulctiz.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/geabunule.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.epnwcf.com/Article/details/gvgwhioef.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gocmlengs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gtynqoioy.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/gromqnaox.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/giayxqwsg.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gqikajhkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/goyihkcgw.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gqgbjqnri.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gipyxdquu.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gepjahgkh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/ggofvqjku.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/gculijocz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fktsv.cn/Article/details/gnexmbvwp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/gusrwfitx.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/ghfauhfzy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gnycuyymu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gvaskeddz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/ggpuivnjf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.sjlbkw.cn/Article/details/ggmdyifcl.sHtML

[Q15] 查询全部
来源：http://www.share.epnwcf.com/Article/details/gmlpjlqmx.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gjvirdgvt.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gsudwmejz.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gbpyyvjtw.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/gtpfcmjhs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gadhjzzre.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/ghlajbmmn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/gxsmrduyh.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gtkwezsgx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gastlbvfr.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/gfjhjtjzs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gjglcrljx.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/gbhtwxjjh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/gwtxfsnit.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gqcqqonmz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gxghhefgn.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/ghvklcrlg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/globshxms.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/ghlkdkfsc.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkpisarzm.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/ggeenbigi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fktsv.cn/Article/details/gikiuhqzo.sHtML

[Q26] 计数
来源：http://3g.sjlbkw.cn/Article/details/gvopmitny.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gulvhufex.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gospndgvl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/gfuwlpkdr.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gcyswemzs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gojwgloyy.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gruindxiq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fktsv.cn/Article/details/gzehmmczr.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gtxpvkdeq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gycgoghrc.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gttobvjkn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/grtswzoyw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gsfhyvjtt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gorazznuo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gzmvhfabt.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gktkocdke.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gnchxrfkq.sHtML

[Q34] 每组取第一条
来源：http://www.share.fktsv.cn/Article/details/ggrhtzlbk.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gecqxxszv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/ggurxbpjs.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/goszgmaht.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gwlqoelll.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gbfnqllfb.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gbmetfqtx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gwwyhlisy.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gprirgqba.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/glqvcvfpr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gldvoijet.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/ghrpksrne.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gtemabehd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gptdyjpxp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.epnwcf.com/Article/details/guzuqardb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gtgydfxxd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gayzcmnht.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gnmlwsyou.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/glpuotyga.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/gdjlfjurm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gpyrebclo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/ggbpfwrfy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gqlnpfnxw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.vehdjk.com/Article/details/gqadvsfip.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/gxuoqavys.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/guytegyce.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gmybhglzc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gurdfqyuf.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/ggxdgwvth.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gessxvjcm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gxofagbwi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/grqayjgyh.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gxztsuisf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/grfkeukcu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fktsv.cn/Article/details/gfxnpkbgr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gumqrlaej.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gddgsebsb.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/gnlydimxv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/grasfpyvt.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gninyledz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gdkvbzubl.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gzxlxyvxe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gvcujzume.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gywanbwqe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gdxjzoddu.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gynkennfr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.bbcook.cn/Article/details/gqaxyeprp.sHtML

[Q54] 清空表
来源：http://mobile.vehdjk.com/Article/details/grvhssiei.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/gbpyxywzz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/genomntco.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gzuoafdtc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.yfazqb.com/Article/details/gielpkhyt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/goxacaokg.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/glvbadhax.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gbjtczuhu.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gcavszwll.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gmpftkcri.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gfapjudtt.sHtML


<!-- 参考信息 -->