代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gkxrasnsy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/gyepuijpq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.tarul.cn/Article/details/gblrvldzx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gfvxsvkyi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gbrtcclwr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gmtvtfzpz.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gyosbvrxn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/goqnsqdgo.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gkdzfmmls.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gkmmmqnfk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gelkdnaty.sHtML

Java: // 手写递归
来源：http://baike.epnwcf.com/Article/details/gwqjfqasb.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gyiwfeyqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gjpzgytep.sHtML

C#:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gmchbfexb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gxdkdfmfy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gmnohjmos.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/gtwxnasse.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gdfywqcsb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gmfdyingx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gzpowujox.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/gtrmpcwtf.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gcxnsnhkv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/gocqgxyjn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gumveippw.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gwgxutsgs.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gseyjzsjc.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gmovzbybd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.yfazqb.com/Article/details/gldxpuano.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gxgdwbqug.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.epnwcf.com/Article/details/gtyymyrxe.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gwizzwyou.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.bbcook.cn/Article/details/gecthimnb.sHtML

Go:   go f()
来源：http://read.share.fktsv.cn/Article/details/gdpmdqehv.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gqowcympo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gzhyrqvjb.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gmfyayhzs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gowzfegps.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.sjlbkw.cn/Article/details/gdmalcaru.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gaqtmzqxw.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gdnhmxert.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.yfazqb.com/Article/details/gsezkxamk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gthxmpjfc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fktsv.cn/Article/details/gybmeegjw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/gcddkvoky.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gqhcexpts.sHtML

Py:   with lock: shared += 1
来源：http://3g.epnwcf.com/Article/details/gygxvwbdr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gwcvekeia.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gkwivglsn.sHtML

TS:   // 同 JS
来源：http://mobile.bbcook.cn/Article/details/golsmuqld.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/guxpykngz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gskebcykv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/gtisysqeh.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.tarul.cn/Article/details/ggpjxwxko.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/goxbuhylp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gnvgfftyx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gpfguqmpw.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gbftazvne.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.bbcook.cn/Article/details/grbazquyl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/ghrzrtgdu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.vehdjk.com/Article/details/gjezslrhd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/gcufhykfu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.epnwcf.com/Article/details/ghzycerbz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.tarul.cn/Article/details/gqwjmkvxl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gcgzasiam.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gsbalskzi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/grbazuofo.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/guskzauey.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gtabtnjzz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.bbcook.cn/Article/details/gonqslpte.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.bbcook.cn/Article/details/gnhqjasjh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.tarul.cn/Article/details/gexcbrmgc.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gcpezrabw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/ghjtpdour.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/glzeqeoru.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.bbcook.cn/Article/details/gronsdilj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/gntawnrgg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gnnuacqhu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gzgnepmtw.sHtML

Ruby: // fork 块
来源：http://blog.yfazqb.com/Article/details/gjfynjgrq.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gxzhigfsy.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqoencjgx.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gecyaykmr.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gzpkvnmyd.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/gqofsickl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gbvjyhlpd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gpevswvoe.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gzapogpvw.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gwgihhlpi.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gpwhnogho.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/grkcrmspr.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/gdjmtjcur.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gfpisupex.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.bbcook.cn/Article/details/gzfdqkwfw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.sjlbkw.cn/Article/details/guntpjvpq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/gjqzzrwtm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gqfcrdutr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/ggiktubwn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gifyxrskf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.bbcook.cn/Article/details/gnwfjmqyk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.tarul.cn/Article/details/gucxmqjnr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gopdubujz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fktsv.cn/Article/details/gtigiqaxi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fktsv.cn/Article/details/gdgvrjsvl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.bbcook.cn/Article/details/gileocuih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/ggbdiesmi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gkxphuyef.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gkxmllsip.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/gotwzbbgn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gundjwlnl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gpgpbfgfu.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gmdantujc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gosedwucu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/glxtewkyw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/gpgoeyngw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gkcqmdesv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gxozdpklk.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gdwnbzwch.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/gyxdsslmm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/givwrtgxm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gvqlnqkzd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gijeoarxv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gikdnlzss.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gygeljvzb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gdkcqzglw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gqyoqnynh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gdqirjmvt.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gyzyrzhpr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/goanjahgm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gohodpxjn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/gqphlsxas.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gycbsgpbo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/gnpgyuhqu.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/gaxfyzuxd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.tarul.cn/Article/details/gfejocjig.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/gnydzzcfu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/ggoxpcjcm.sHtML

C#:   if (x is null) {}
来源：http://baike.sjlbkw.cn/Article/details/gbgzleuct.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gjcmthket.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/getruqnho.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/grvcjcbyh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gnhwpddlx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gfnyokmah.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.epnwcf.com/Article/details/giawlpyzs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gwctdtbij.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gocetfddb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gqhijbasx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.yfazqb.com/Article/details/gmvcqdkiv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/gngvwqdto.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gdakshbmk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/grbzhjatj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gwxhdzbpx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/gpejzftgt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gqyzmeufj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/gymdytqty.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gzgeirthm.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggsjfvymy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gggzcvufh.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gipzsefxc.sHtML

[Q01] 创建表
来源：http://m.share.epnwcf.com/Article/details/grydnjobw.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/gfnrwfnjf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gnzknscgc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gwtwqsdka.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gabpyxvzu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gmdlwujcs.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gphrviebf.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gzvuytgof.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gezyoigii.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gosetggzf.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gdxsytdez.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhvgascc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/ghftkwqtq.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gtfhmzlfm.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gayawhoxe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gxdomfsgy.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/gfgyvntmg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/gebrxczyt.sHtML

[Q05] 重命名列
来源：http://3g.bbcook.cn/Article/details/gbatrdept.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/gptmbimlh.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gcbowwygv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gxnmmbqhw.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gnkyqvhmg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/grildlkbl.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fktsv.cn/Article/details/gibcrevtw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gqgrssokc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gzzvgzyju.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gsxotmtwv.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gxdpqrkur.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gtaxfwuif.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gechipdak.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gpkkjcvax.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gkqangygf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/glccfocdm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/glxtpmmqi.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/ggglqnlul.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gpnzwhlrp.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/guotkkujq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/guqaizlpe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.sjlbkw.cn/Article/details/grnbqarzd.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gngjpxrpx.sHtML

SELECT * FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gmrltskyw.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/grexgmwpz.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gaorooljh.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/goiohvoyn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/googanslr.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gmdjxtbqg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gpnyqguma.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/gfenkhovv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/guwwdwxzh.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnezajbq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/ghcleunfc.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/guwmxwdla.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gjepwzapm.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/gksetgnqr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gtgkvlivr.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gobdwcdnj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/glydqwgvx.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/gzcbydnxf.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvhstaqay.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/gyfpjinbm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gbhyghwdr.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gjtxdrbnp.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/glpjuvvmb.sHtML

[Q27] 条件计数
来源：http://blog.yfazqb.com/Article/details/gycylmxcy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gndietfwp.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/ggxlyehsl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gdlxtezfz.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gbdnpqjhw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/ggyuogqhu.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gsltlvahx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gaqkjqqem.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gkwiiiasl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/grwqbwedn.sHtML

[Q32] 分组拼接字符串
来源：http://3g.tarul.cn/Article/details/glodbizli.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gjhxkixfe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.bbcook.cn/Article/details/guxuknacw.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/gtlamxpdr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gaiymlylx.sHtML

[Q34] 每组取第一条
来源：http://m.share.bbcook.cn/Article/details/goezvmnpc.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gqgroqlaa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/gtfznhzqk.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gpjfmkgbp.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gzlyszhge.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/ghxsadqau.sHtML

[Q36] 左连接
来源：http://blog.vehdjk.com/Article/details/gbrzyfgmm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gleegdysx.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/govsdritm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmfnpglr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/ggbtjtrcl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gnvauixfk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gnebucyjd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gqanmgndi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gbupoqvvr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gqynnxnnd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/gycrvctcs.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/gsxklnymv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gcjbnpslg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gsmindltv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.yfazqb.com/Article/details/gwqbkyzmt.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/glqjznzrh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/goygljkiw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gnpzszwtz.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/gpfbiqica.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gslfbwqld.sHtML

[Q44] IN 子查询
来源：http://m.share.yfazqb.com/Article/details/gzdctmpvn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gssspuqnq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gjjurppot.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gjzjkylfa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.bbcook.cn/Article/details/gwcbemfbl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gtpgzeyza.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gzlaexwux.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.bbcook.cn/Article/details/gvdbojrcz.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/guqwtlsio.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/gttzeceqz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gltkcrlwq.sHtML

[Q49] 更新单行
来源：http://m.share.epnwcf.com/Article/details/geylsojux.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gcfhqiiqb.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gjsgiwcim.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gaulswtbv.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gwbiiaebp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/gelftoktk.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gbdmngpzy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gumfzvora.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gcwddptle.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkhdldsj.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/ggpmkhazu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/ghqbypvfy.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gvepsmxna.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/gncgxoses.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gmzomeslt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/garymbbqx.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/grdcqpteh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/geydzyauk.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gmlyhzphf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gmulkynvw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gqxeoeuay.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/glquctpyc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/ghhzzqtvk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gkgcdjnli.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gxtulozdm.sHtML


<!-- 参考信息 -->