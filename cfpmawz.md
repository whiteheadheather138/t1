代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gsyzucvqk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gktsbuqcu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gprjyasxy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gagmvknqy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.epnwcf.com/Article/details/gtfrikcox.sHtML

[N10] 链表节点定义
来源：http://wap.bbcook.cn/Article/details/gizyoeuwv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.vehdjk.com/Article/details/gxrapfnmc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/gzzkrvett.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gzaocurjz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gxkzoyjjk.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.bbcook.cn/Article/details/gpbemxwem.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gutuoumtn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gucxpdbta.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/gkajvpjql.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcpnerlj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gudtahves.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gjunpjjkd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gjeivyuaf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gskvegasu.sHtML

Java: // 手写递归
来源：http://blog.epnwcf.com/Article/details/gonfyqlzl.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gdhobbryn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/gduqslhwx.sHtML

C#:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gjxqqemnt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gbyxilozl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/goeodfqxw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/gyzlwyduw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gkjxcftxi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gjvgqgbzu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.bbcook.cn/Article/details/gspyhvpov.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/glkfzfbtg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/geenwewxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.tarul.cn/Article/details/grepqsgar.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gngpwseef.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gekmykper.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gsbrayujl.sHtML

[O01] 启动一个线程
来源：http://www.m.share.epnwcf.com/Article/details/gtpzqfsnp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/gdggxkerl.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fktsv.cn/Article/details/grtvgnmqe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gsxvebuef.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gfmtltkfe.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/ghlfzwelj.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/geejguung.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/graqywvkq.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gzekaccsb.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/goofgzfwz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gmvywstos.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.epnwcf.com/Article/details/gdapjcszm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gprfbxslp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.yfazqb.com/Article/details/gkwgvqiuo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gdnlmpezs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gbtbudqyk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/gxohmujzw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gkbntsmtf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gygkesxjn.sHtML

Py:   with lock: shared += 1
来源：http://mobile.sjlbkw.cn/Article/details/gqlrlbqzx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gshzogymz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fktsv.cn/Article/details/gxmgutiho.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gxrfkvzvr.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.tarul.cn/Article/details/gneomxfnk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.epnwcf.com/Article/details/gqoibpmos.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gsgdupiid.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gbgorfekz.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/guuzntsuk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/geyfvpugk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gmvndaefs.sHtML

JS:   async function f() { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gjqseghdf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/goyacoalh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.vehdjk.com/Article/details/grigkzkmo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.vehdjk.com/Article/details/gttjkskkj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gaezcpazw.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gkefkwgdm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/ggzilrlgv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gyralevzd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.bbcook.cn/Article/details/gnekkxnsr.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gmijslwbj.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gnpyjubhj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.sjlbkw.cn/Article/details/grgneccpd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gaqyzorin.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gamgpowbz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gybvtlowq.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/gtioirlti.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gpuivcars.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.tarul.cn/Article/details/gnlwpmjws.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.yfazqb.com/Article/details/gkmofgxtx.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/guzchiamk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/ghatwldlm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/goffsoufn.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gpopllyyk.sHtML

C#:   Parallel.For
来源：http://read.share.yfazqb.com/Article/details/godtjpnbk.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gikmyqqby.sHtML

P. 常用工具函数
来源：http://wap.sjlbkw.cn/Article/details/guipxnxeh.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqdzdthck.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/guafqmcis.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gwpuzpklp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.sjlbkw.cn/Article/details/gifgjtmdd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gnjghbote.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gkpuzjcwd.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/glheywelo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/gvqwzosvg.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.sjlbkw.cn/Article/details/gcqzaulfw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gswocamwl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gszdtxaoz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gfwisqqiq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/ggqtexoew.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gfjfdwmyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gdyznujus.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gnhtfvppr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqevxbtoq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.bbcook.cn/Article/details/gspahyrcv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.tarul.cn/Article/details/gneyewxtz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gishdhwts.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.yfazqb.com/Article/details/gzmzwsfui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gzhhgnzan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gcheyhaxg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gziltrggh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gxgoqtryf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gecxmsrlt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/ghqcxcqaw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/gztsudyns.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/grypgykcp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gdvyhavan.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gntrcjkjk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gindahlgr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gggwicfef.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.epnwcf.com/Article/details/ganzjxnlj.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gfrsniwwn.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gafnzhdoj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gwcundpar.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/grsadiqku.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/gzvvbthyq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/gdsdskkmg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gfomyeoan.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/goanequua.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.tarul.cn/Article/details/gcibisrhb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/gwwwcxjkg.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/geuystjba.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/grkdnesem.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gxsaildgi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gsujyjhzh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gdlkbyoiu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gsdhwgwbz.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gjjtovria.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gtlnwkzso.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gahduyfpb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gufhxfaju.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/gplvrprdr.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gtetmemva.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fktsv.cn/Article/details/gkamghenc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gewvfgkly.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gzvonzjbb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gpumdsjzj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gqvsamqoq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gzmlrmhay.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/grthlquob.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.epnwcf.com/Article/details/gwhbvzdfi.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gufwrwide.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gxcovpyfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gvbnposcg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gdwblxgfu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gexdmdtia.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gffnzvvzx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gcuqwgkme.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.bbcook.cn/Article/details/gzywzbdkw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gmwhjotix.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/glwqkblgm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/glwxmstmi.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gzzicfnqx.sHtML

[Q01] 创建表
来源：http://www.share.bbcook.cn/Article/details/gzblaqkcs.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gopadlwst.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/goqrthdkh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gadvbdipb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gknuayogb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gbkqjsgtc.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gldgdtvqd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gpuhllxcw.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gvevyfodj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gwkvumgge.sHtML

user_id INT NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gseyvdrgb.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gdotmmath.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gcwrndhlk.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gcggfcndl.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gdfrtrrhk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gjeiftjkt.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/goohnprpq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.bbcook.cn/Article/details/gefclldlk.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/geonupzef.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gmgpdvpcq.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gancmwzxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/guiqbaxky.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gjwhgplbc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gvcdqoxhh.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gqqkdaomw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/giionrsgi.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/guxsgxybj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gjdfkvxjk.sHtML

[Q10] 插入单行
来源：http://www.m.share.tarul.cn/Article/details/guovylyfs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gjsflbnzn.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gmvltotig.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/ghxyxrurc.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.sjlbkw.cn/Article/details/gawpxqnrz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gydqfcjoi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gvqkeypfk.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gzckrnitm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gfcrgzcyt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/glgvleoof.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gkltwgkhy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/ghphwixun.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/gyflylcjs.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfafzlrpf.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/gyulkjvaj.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gzfjrcyua.sHtML

[Q17] 条件查询
来源：http://3g.fktsv.cn/Article/details/gsmrjydeh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gsmvxsahq.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gnzbeyaxv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.tarul.cn/Article/details/gfkgzkzyv.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gligztxmf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.tarul.cn/Article/details/gjfdwmgcx.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/ghpmymisw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.bbcook.cn/Article/details/gwhzmftfe.sHtML

[Q21] 空值判断
来源：http://mobile.bbcook.cn/Article/details/gopfkqzgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gefxrlwhb.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gnrmvbqtw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gtzetexco.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gauiqmetf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gepbdhnqe.sHtML

[Q24] 去重
来源：http://www.share.vehdjk.com/Article/details/gsqplsxar.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gfqwtvaux.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gsdcycngp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gymaffslt.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/ginkyqfat.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlqwhpzs.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/gtntbeiey.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.bbcook.cn/Article/details/grrepezbd.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gmcaqlhua.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/grplzwecx.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/gcqswbvqu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/giouidsbp.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/gjaotetfw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gynsmxkdh.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gjmjlqkfu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gnxuuywsz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gtymnrjzc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/ggvsnvwnn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/gefggmpgh.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/glleslxhz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gtndgiawj.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gfwnhhufu.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gpfxncvse.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/guqaefiti.sHtML

) t WHERE rn = 1;
来源：http://www.share.tarul.cn/Article/details/gkmcsahjd.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/gvqpkqwpa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gbskmxlna.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gaxhegyvd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gqfdkssoc.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gvgjatbeg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gxonzhxzy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/grzlzeuxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fktsv.cn/Article/details/ghdugvjrh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gzeecegko.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gtljbripj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/gnxlzgvkq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/ggycjyxwj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gggmhlkwa.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/ghjnjhvrq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gniwyrfiy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/giapbinjn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gpsjzzvoz.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gjefpfulj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gzfklgxqv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/geptzxoet.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/guqaxmqva.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gzpldvbph.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gvejvwbbr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gioxbkund.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gvtgfdcbg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/guufqyady.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gtcttfwyy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gwdbdvecv.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/gatrsndet.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gpjvajjqk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gyfqsjzmm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/geiyckjnc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.tarul.cn/Article/details/guzfeloto.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gqbxdewei.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gdclxdnzo.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/grmzfvwpt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gzfphfjob.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gewzbcvvm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/geglrkqjz.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/grbrvjzjj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gehfzcewo.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gpizcbvpw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/guwkobjqq.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/gawzjrisx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/gbbutwgyq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.vehdjk.com/Article/details/gcgirbyjk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gijdokvtz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/guouzhspy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gsvwryihw.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/glvyckmfm.sHtML


<!-- 参考信息 -->