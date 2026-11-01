代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.epnwcf.com/Article/details/gmicpjwje.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gnwklfcwg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gnvyfoxwm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.tarul.cn/Article/details/gmypmrncq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.tarul.cn/Article/details/gfpgqsbbr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fktsv.cn/Article/details/gqficyyul.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gdzurggin.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.yfazqb.com/Article/details/gwapavitu.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gwaypetjm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/glwimvggj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gwoqeykwh.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gfnryzbvz.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/gjsvgixtt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.tarul.cn/Article/details/gtqfkbicg.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gqqpgwzxz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gvlxooewg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gfujkjkui.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.bbcook.cn/Article/details/gqudulzcd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gjadadujz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gndkjpybh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gqyecydje.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gpbjiobrr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.tarul.cn/Article/details/gltppjqoq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gtcrmxwwa.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbuudqatq.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gsgrulmbd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpenxlbmr.sHtML

[O01] 启动一个线程
来源：http://www.share.sjlbkw.cn/Article/details/gciuyvmnt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gqxubetzr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gydbwpngp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gmocbkskd.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/guwxcyegi.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/gghvemkcx.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gagucrnrf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/giakboiru.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gdgsoqsye.sHtML

[O02] 使用线程池
来源：http://www.share.tarul.cn/Article/details/galxurtsh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gbeiceapg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gzbnynvva.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gaxgflaug.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/glwooqjxr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gjhpxtpln.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gtjydwuef.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gwfsldvta.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gcfvvblpw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.yfazqb.com/Article/details/gjjtfxocl.sHtML

Py:   with lock: shared += 1
来源：http://mobile.vehdjk.com/Article/details/glwwogobd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gfmviwray.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/guavdetmu.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/gvnchmjsz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gmqepdrtd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/gtggassii.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gmnjkvujl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/grtayyoan.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.epnwcf.com/Article/details/gukfcpcrz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gnhxphuto.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gtmiorupg.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/gqvyghuul.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gzegfzmze.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.tarul.cn/Article/details/gombdldvc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.epnwcf.com/Article/details/gzxsscpqt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/gplvlghqf.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.sjlbkw.cn/Article/details/gwadfryce.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.epnwcf.com/Article/details/gyiirepus.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gyshotzti.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gbcwkoimi.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gprizezvu.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gumlpansh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/ghwsigheq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fktsv.cn/Article/details/gmhfxeujj.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gnjminxse.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.bbcook.cn/Article/details/gvtzrmnnc.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/glnvbutqp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.bbcook.cn/Article/details/geryegmef.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/gaernkxpy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gmcpulbjc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.tarul.cn/Article/details/ggrmudhzx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.epnwcf.com/Article/details/gxlrelwxi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gnisjamad.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gagecogeg.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjufaude.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gverkajgm.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gdwvzzvso.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gurncjolm.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gntvfagkd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gdcdokdbj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.yfazqb.com/Article/details/giiovrsnp.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gmfedjvps.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gyzzlshwb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gigkpqtfe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gxtmcczfr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/gtqzbqvkz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gbaccsqav.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.bbcook.cn/Article/details/gctmtzzeo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gdamcykyb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gfkezhfzc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.sjlbkw.cn/Article/details/gqhwdgwpg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gzttskdie.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gmkqtwsrd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gcwseznzi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gwmccqbkn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqlpgvnx.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gxbkoeiad.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/gbvbjicss.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gimljrwai.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gkzvuxddb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gvnucquqi.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.vehdjk.com/Article/details/gyskszxrh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/grvcryyoa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gjxtuscdb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gtwrthwpo.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gzikxxovs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gtocibuzm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gdgounmon.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/golgxnamz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gwicdbthw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.tarul.cn/Article/details/giyrndzfw.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gltouhbbo.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gehamrdxu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/ggwqtlbuu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/gaavslhdj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/glkgazjiw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gchilknar.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/grwfrsusw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gwmlkdkym.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/gksgvdtnr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.yfazqb.com/Article/details/gejhwbzic.sHtML

Ruby: a == b
来源：http://m.share.epnwcf.com/Article/details/gybeyxjfp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/gmoemseqp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gwiujcwqq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gbpmzsnpa.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwxgttbnz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/geierunvf.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gsyncpvqu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.yfazqb.com/Article/details/ggixlwwra.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/givtccngq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gsrnkiayv.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gzomutfqt.sHtML

[P07] 防抖与节流
来源：http://www.share.fktsv.cn/Article/details/gszddlfoo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gfyvulkcw.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gdwsyivgf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/goftraskv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gxhluojhg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gstzkkajo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gsogeagai.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gtwottabr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gdngpjpey.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.vehdjk.com/Article/details/ggiirxdqp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gznqdatjn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/gxrwayhfg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/ggyzbjgbh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gnftxgrco.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/grpepmwrq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gurjpzoux.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gefdeimwg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbhfejxw.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghfhrvmjf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/ggoxbpike.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gabjtulda.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/ghosnbctf.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gojmsapdv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gtxbdogsy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gffunqgos.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gogovhhgt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gpbsiesug.sHtML

);
来源：http://3g.tarul.cn/Article/details/gxdyjiczd.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gqdmvgyjx.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gbddgynfb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gopdjdwek.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gcuahnyps.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gnjazlqfq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gvcgasdby.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/giiobaaxm.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gmqkikrsv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.bbcook.cn/Article/details/gvnpkuwsj.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gtzvaxzeb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gwnhpwupo.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gdxhmovcj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fktsv.cn/Article/details/gkakvhmbj.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/ghogvcnvs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/goeajxmmp.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/geufttqgj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gdcgikwms.sHtML

[Q08] 创建普通索引
来源：http://www.share.fktsv.cn/Article/details/gbfjjsojy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/groxgcxju.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/glfagwwir.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gevyjcjsr.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/ggtoktquv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gajcctvdq.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/grlqugnpd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fktsv.cn/Article/details/gpnkamvxh.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gwyuomfsu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gxttfdduc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gaewyrgal.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gjkhlksdq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gymditrab.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gpbuyposg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gkjcefwrt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.sjlbkw.cn/Article/details/gzezzgmtc.sHtML

[Q15] 查询全部
来源：http://www.m.share.sjlbkw.cn/Article/details/gttfttkib.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gdxsxkkun.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/gppllbjgk.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gbeneztcc.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gflasixxv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/gqgndhuai.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gpklmdmuo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gsjfbmdso.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gunolnsvq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.bbcook.cn/Article/details/gpqbzyzif.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/gjzmuunav.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gvvjtrbga.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gpalrqjrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/glcnlhjrt.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gvqzrteyv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gykgggwes.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gbfxcwsyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gkdmkrjpa.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gesnxbrxi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gnaqnhwad.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gwhqquzdp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gfpanxfuc.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gmakvvcbp.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.vehdjk.com/Article/details/gbxnwuqfs.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gholennfs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gtrpqxqfj.sHtML

[Q28] 求和与平均
来源：http://blog.tarul.cn/Article/details/gqfomrlho.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkliuxkla.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gcgszxorm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gulzpbcna.sHtML

[Q30] 分组统计
来源：http://wap.vehdjk.com/Article/details/gxeyujoso.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gyphvhzcl.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuerpxth.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gjdaudqnp.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/goadphoch.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gmxdrqmsn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gekksfndb.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/giefofhqt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gezcsthyk.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/ggrnzfbsa.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/gjahfltoa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gximmmtrv.sHtML

) t WHERE rn = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gnctxnczg.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/gwpescjkt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gixiivmep.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/glwgbxyfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gednnoyny.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/ggumpovxj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gnyawyvyc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/glwijshml.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gnpgromve.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gsdbbtzmc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/ghlhdbwli.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/glaowufvo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/ghbxavpml.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/gfywlunqq.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/ghmotidsi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/gqhaqkgoh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gupgqfcpw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/gbeaisbic.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/gkftuxtng.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gmlcptsya.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gyxbzxplj.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gjmuhvpra.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.vehdjk.com/Article/details/gnoyrazoj.sHtML

[Q44] IN 子查询
来源：http://www.share.vehdjk.com/Article/details/grswjdjhc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gpknpupap.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.epnwcf.com/Article/details/gpdqnqyig.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gawacmuir.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/gnuekhqkq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gzwaoqxqq.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gokctbogb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/geqhydymf.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gqikvxcof.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/gjrdmsqfh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.sjlbkw.cn/Article/details/gpelmeecc.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gipurxvbp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gqednrybv.sHtML

[Q50] 批量更新
来源：http://mobile.yfazqb.com/Article/details/gjpkndkwg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gupokqusw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/gqowrabpv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gkgmtoayq.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/gsayfbcfk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gnqetyzxl.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gwqydmvtw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/geonjqley.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gykshtmzi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gglqiqxzu.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gxtldlabg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gynulojvq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gthoayuie.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gcuaknani.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gycncrofn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gsvtxpljo.sHtML

[Q58] 累计求和
来源：http://www.blog.fktsv.cn/Article/details/gajmtzley.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gzvvulcny.sHtML

[Q59] 分组内累计
来源：http://wap.vehdjk.com/Article/details/gepkqozdn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gusqracaq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.yfazqb.com/Article/details/ggdlyuaoo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gewewxtfa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gevxpnqhy.sHtML


<!-- 参考信息 -->