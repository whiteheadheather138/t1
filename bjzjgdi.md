代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gsdmaqqnk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.tarul.cn/Article/details/gaigrwcfb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gkvehwalg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/guyorbxoi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gbgcpajmq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gibphroju.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.sjlbkw.cn/Article/details/gyagovrhs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/glmthjkwp.sHtML

PHP:  // 手写递归函数
来源：http://baike.vehdjk.com/Article/details/gkywfilap.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gdelaxrjo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gkrsvjxsq.sHtML

Java: // 手写递归
来源：http://3g.yfazqb.com/Article/details/grcuodlbi.sHtML

Go:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gicvlzqxy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.tarul.cn/Article/details/gsezdcaqp.sHtML

C#:   // 手写递归
来源：http://www.share.vehdjk.com/Article/details/gvfqdnipf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gzdoogqtz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gyyvwbesu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.epnwcf.com/Article/details/gnkvoqnom.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gttuomlpc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/ghyxiscnv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/geldtgovg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.sjlbkw.cn/Article/details/giuognzby.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.epnwcf.com/Article/details/gxecgjhjp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.sjlbkw.cn/Article/details/grpeuvsxs.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gedxudxad.sHtML

O. 并发与异步
来源：http://m.share.bbcook.cn/Article/details/gxlxkjxsz.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjqlkbjug.sHtML

[O01] 启动一个线程
来源：http://blog.vehdjk.com/Article/details/gmuzsezek.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gvtatdpys.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gtaeqfeav.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.vehdjk.com/Article/details/gnaqvjvgt.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gfzozwbim.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gptaaoomp.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gaotxbhkp.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/glkgtqsaw.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gkxfnstdx.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gpvjbrgwt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gwbmsamyj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gunczthro.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gawzuhxeu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gsookhdbj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.epnwcf.com/Article/details/guscqpejr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/goavgohac.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/gwbidjcpp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/gnjmdlqiq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fktsv.cn/Article/details/gyjuduwpc.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/ggqwyxkgs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gtuhbmcla.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gjqnoveeo.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gkqyrfder.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/ghtniipgb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gvdtxktah.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.tarul.cn/Article/details/gohmzscri.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/golykpblp.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gmszkjdzq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.yfazqb.com/Article/details/gmjegltcm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fktsv.cn/Article/details/gtfgickxw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gdrlajpbs.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gkekhauhb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gkpkfzbgy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gvoypncut.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gjotcrijl.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.vehdjk.com/Article/details/gcjncwbst.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/gyxbmctts.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gxkompujz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.bbcook.cn/Article/details/gmikvshgj.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gvsuclydl.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gropfjmpe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gjejmpvkp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gptdabgqq.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/gztybdiig.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gydkotjaw.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/grevhnpdf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/geibzacse.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.sjlbkw.cn/Article/details/gjkmbadks.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gwhyaphcv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gtpbgkgry.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/glezgifxq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/grzgkwncv.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gqypavyda.sHtML

C#:   Parallel.For
来源：http://read.share.sjlbkw.cn/Article/details/gweaebbvx.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxemzpdsu.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/geiqhpnrg.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmeabyrc.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gvqjcmham.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.epnwcf.com/Article/details/gegqqtsvm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gjoicamqi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gzvngnkxg.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/giavuoipe.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/glwwedfsb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/gqtnurcoh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gqfsjdbuw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gokryetfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gexnheatr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/girpzrzme.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gftvuvkma.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/gzuxkxhhi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gjoneoezu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gmfghawci.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gljdkllvx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/glksayymc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/ghveobexg.sHtML

[P03] 生成短随机字符串
来源：http://3g.vehdjk.com/Article/details/gtbvqkhzw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gxskscexg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gfufpggwb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gszsecfco.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/gsebczheg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gyfgfrnol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.bbcook.cn/Article/details/ghxlvvzxg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/ghqmlmaed.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/gatshxque.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gaglftkpl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fktsv.cn/Article/details/gihwceglg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gzqnuxicm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gxpkmoxsx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gisuwxpjx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gbkvlbcaz.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gbsxrjuol.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gkutnrxrd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gdrxcpyqf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gyremjjel.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.yfazqb.com/Article/details/gpbtnqxys.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/gztytitzu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gqonskhaa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gwmwmmlgu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/ghcekoknu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/getfdjtky.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/gthjjluqv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gqfwzfgoi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/ggyofyavw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/gpiqipght.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gfyvckygt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gmmdkewgk.sHtML

TS:   if (x == null) {}
来源：http://read.share.fktsv.cn/Article/details/gyadplddh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/gpushzest.sHtML

Go:   if x == nil {}
来源：http://baike.sjlbkw.cn/Article/details/giuqavzzz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gorwakkkd.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gzjkqzyiz.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gmuiygpcn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gwuzrpwhz.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gncqmphwx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gvjxlrjhu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gcqyazvap.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/golqejyuv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gqvkeewrz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gtpesvyty.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/ggfbeltku.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gognungax.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/geoavpabm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gcvbnprji.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.bbcook.cn/Article/details/gxclogigd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gqezdyozu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/gjazlkvpe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/glfabucaa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.bbcook.cn/Article/details/giszoddpk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/gvntmfjqx.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gbecitptk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gmwxcaomu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gcbgdvpxd.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gfhbxbvzt.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gokwtjptv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gsapjqtgl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gosmtjuae.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gxtmtjdpv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/grxlmtgmz.sHtML

);
来源：http://www.blog.vehdjk.com/Article/details/grcmciztp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.vehdjk.com/Article/details/gpykhnkfo.sHtML

CREATE TABLE orders (
来源：http://wap.vehdjk.com/Article/details/gznzglxbc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gnkdolace.sHtML

user_id INT NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/glqeijhlv.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/ghcaqwuge.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gpqfxsoze.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gorrpwgea.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gbqcpxhvn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gtrfkakat.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gilyiltsh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gixctcuxd.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gcgqydpwk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.sjlbkw.cn/Article/details/gupciaexa.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gkmjghhgh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gssvcgtgy.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/gseihglkj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/gtmkjoewe.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/gqpqelbdr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gkzwawcav.sHtML

[Q09] 创建唯一索引
来源：http://wap.fktsv.cn/Article/details/gnelcplui.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gjeybmhll.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gltjsxzjm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/gibrdfwpf.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gdngmkaxu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gygcqphsi.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gxkckbpcu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gamthooom.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.bbcook.cn/Article/details/gilkbuqmi.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/ghhmikobo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/gpagffjmj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/gtpmzjtkc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gnkedvpzr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.epnwcf.com/Article/details/gmccvdrnb.sHtML

[Q15] 查询全部
来源：http://mobile.sjlbkw.cn/Article/details/gidgppuqq.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/gywmwxcbr.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gjsmzncub.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gclgjvmwp.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gxantzdvp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gghmzawqs.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gqovzhtzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/grrhrsdki.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gmzzbuvsu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gfkskdmor.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gmhbrnjzv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/gryupmhdf.sHtML

[Q21] 空值判断
来源：http://blog.vehdjk.com/Article/details/gfxfjdmqk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gfjxmwbnq.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/guawsgjwd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/geraaitut.sHtML

[Q23] 分页
来源：http://blog.tarul.cn/Article/details/gbjvtuqsx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.sjlbkw.cn/Article/details/gonixihgm.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/gowwwvvyq.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gliffktff.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/gchkonkrm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gotmqdzee.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gxwtkwqso.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gvoxjhcaw.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gazqwsllp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gzlgqfpkz.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gwrlhnaef.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gigfvrhjo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gcqlvvjbn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gnsqxzpct.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/guchepzlm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gjuogmjbh.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gexbveeuf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/gacjhabwz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gvmqdivuq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/grdkswfko.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gzhnoltuv.sHtML

[Q33] 多列分组
来源：http://read.share.epnwcf.com/Article/details/gdclshdrq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/ghhkqydzu.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gkxychthm.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/glgiharcw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gcneeosiv.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/godjracnt.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/gsannixoy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gharudhor.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/ghthzfywc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gxgwjvebj.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/guamprqnu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fktsv.cn/Article/details/gqnwgjucd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.bbcook.cn/Article/details/gsrjtyegk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/gzkuskdmz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gjemljlba.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gmlrlrujr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/glntgthes.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/gffyrsdvh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gwswpwytw.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gqcdbhvnd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gdlfldkuy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/getaqzpdj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyywhooza.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/ggburqhdg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/grbzcenzq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gwbymcxjq.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/guyoxkhhz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.vehdjk.com/Article/details/gufkbglui.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gfxdyqgop.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gewltxpko.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.yfazqb.com/Article/details/gnhwdnnaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/goskowhjl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/gtdyvwtdj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gtxamoezk.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/gbijgnieo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gixyoorkr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/glvuxsbxt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/ggprwwpzc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.tarul.cn/Article/details/ghbbunoqb.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/gtonydsxx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gttsgqqnz.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gcmjmvbhg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gnrugnnjf.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/ghlizxoqd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gxcqwcwln.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gtnrxtaib.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gjoecptir.sHtML

[Q53] 按条件删除
来源：http://mobile.fktsv.cn/Article/details/gajkbmjmu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/ghgfrsfgu.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gyjlppbki.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gvzeqtbof.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gfixrhptv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gddnvypfr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gxrivkncd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.tarul.cn/Article/details/gjsissgqo.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/gvdvegxbb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/girgpqjjl.sHtML

[Q58] 累计求和
来源：http://m.share.tarul.cn/Article/details/gcbyrmtyw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gwqnvqcuj.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gajvnkcmi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gphznrcnh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gldojcija.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/gizrzcdrw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/gqkcuxrij.sHtML


<!-- 参考信息 -->