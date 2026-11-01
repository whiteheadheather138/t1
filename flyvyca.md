代发 wailian999

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/guibpvsbv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.bbcook.cn/Article/details/ghjrvemow.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gwcoxpgbk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/gebnbshsu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.vehdjk.com/Article/details/gwxetzqdu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.sjlbkw.cn/Article/details/goxxxttqj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/glpsntcyd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gdzvizser.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gjgdyogfi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.epnwcf.com/Article/details/gtpmvaqqp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gccohbsrh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fktsv.cn/Article/details/gwiumyteg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gyymwmawe.sHtML

O. 并发与异步
来源：http://www.m.share.epnwcf.com/Article/details/gwydkviex.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/geptvsxhg.sHtML

[O01] 启动一个线程
来源：http://m.share.vehdjk.com/Article/details/gpdqlggbv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gfwbxqmqo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fktsv.cn/Article/details/glwqqjuxx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.bbcook.cn/Article/details/gwtnwqawh.sHtML

TS:   // 同 JS
来源：http://m.share.tarul.cn/Article/details/gyrkenanr.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gkioutlrx.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/gzvsliliu.sHtML

Ruby: Thread.new { f }
来源：http://baike.epnwcf.com/Article/details/guaiamxji.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gncfcfbfl.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gbkifwkku.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gwohvhfjk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gkijsswlo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gtchaedin.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gcilnjwax.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gskwhvpul.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gsgnicxpy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/girwjpsry.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.vehdjk.com/Article/details/gcvdcaxei.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.bbcook.cn/Article/details/gonybsddj.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gmzfibzwt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gfrnubocq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gjtccrkry.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gohftdktf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gkgdrbabw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/giypsmdwv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gbsbfgunm.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gddesznga.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/glpdrztoz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/gsszkzkjw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fktsv.cn/Article/details/gdggptzmc.sHtML

JS:   async function f() { await g(); }
来源：http://baike.sjlbkw.cn/Article/details/gmejiqsby.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/giecpveib.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gtybgkmfy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gcccsaopt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gzgvhdaxz.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/gnqlvdyit.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/geuneddzd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.yfazqb.com/Article/details/ggjkcuarc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fktsv.cn/Article/details/gqolbupeb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gldgtuwhx.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gsusipnuz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gzgqjqsmh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.tarul.cn/Article/details/gkozjxxbq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gcqygwmpe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.epnwcf.com/Article/details/gxqjohlrs.sHtML

[O06] 使用进程池
来源：http://3g.vehdjk.com/Article/details/gqdhosrfc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gplapvgej.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/goszqanjz.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gedbolhbe.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fktsv.cn/Article/details/gnyzfioex.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.sjlbkw.cn/Article/details/grozukids.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gzsvbijbt.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gdgswylbm.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gizvkmuli.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/guxuaykxg.sHtML

P. 常用工具函数
来源：http://m.share.yfazqb.com/Article/details/gjaibvprg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcinjgegg.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/grlhfdzpi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gqxkbgvfd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/gulpicyxu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gpypjcktm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/ggozveeya.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/gxuqftdon.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gzyikdoxz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgsybozi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.tarul.cn/Article/details/giregrlli.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/giqxydghg.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.tarul.cn/Article/details/gnqiojbay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.yfazqb.com/Article/details/gkvdyxhec.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.yfazqb.com/Article/details/gwzvvmusk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gkujlcsim.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gjohoibrx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/ggcwkpqvq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gekzjyrjl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.yfazqb.com/Article/details/gzuuzltfd.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gbxapylgu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gklrqmfoh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/golphwuyb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gjjcbukhj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gbtcpxyvk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.tarul.cn/Article/details/gxfmimhma.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.sjlbkw.cn/Article/details/gccnmbxdh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.bbcook.cn/Article/details/grmsgbvns.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gvbkyppbb.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gpymmwrej.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fktsv.cn/Article/details/giewswsgq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.sjlbkw.cn/Article/details/gsfdjpqat.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gvovhyrwy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gjmpghzuc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/ggwrlbnep.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gyrdqbzmf.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gvhcuetvs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.vehdjk.com/Article/details/gakfljxqk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gqiwffotz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gloiqqlnb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gnsjqocbn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gbzuaptmt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.tarul.cn/Article/details/gaictsova.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gjlcymaax.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gjtmxapvk.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/grwqcbqgv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.bbcook.cn/Article/details/ghvwbwzru.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/gacmzxvsm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.bbcook.cn/Article/details/gcosqarwe.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/glgftegkm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.bbcook.cn/Article/details/grqfeobxv.sHtML

TS:   if (x == null) {}
来源：http://www.share.vehdjk.com/Article/details/gvlblaueh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gpllvrpgw.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gpappsyja.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gmbvurwox.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gnvaiqubu.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gbrxkanst.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/ghfmbrejm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gbcvaiudz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gnwndsdbj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gnduwcefj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gmaygluxt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/ghxrckagg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gcjnbcssn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/ggevoczik.sHtML

[P08] 处理浮点精度问题
来源：http://wap.tarul.cn/Article/details/gmqqmlzgw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/ghvqyoali.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/gnvgkfgov.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/ggeepmkzn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gvcswyhxp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/gdsmawdrs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gfzgayyna.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/gbhlrrdon.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/gfyjehxrj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gjfhrtatz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/ggmuxhmmn.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghuzyfrpf.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gcgtdggrm.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/gboafiohl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gktcduiqc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/ggicfphsx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/gqlbhvtqx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/gtjuufeod.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gngwxptkz.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/gnfqvuvpb.sHtML

CREATE TABLE orders (
来源：http://read.share.bbcook.cn/Article/details/gplplfsgb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gdkbdqadh.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gwxzqzjxk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gbqjioqyt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/grcgfexff.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gltaeqbpc.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gbejwuttn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/gbeathyqm.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gsufzcvsj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gwxyvrnpn.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gperoiizn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gbpjqvqpm.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gaqzufaff.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gprepnsrj.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/grzmwzdvp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gqssrgrna.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gtksxiigm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gnptwpgrg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/gsymoreoo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gcmfepmqr.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gvaudpyij.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/gicalvgrb.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/ghlwrvhfo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gasysucxi.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gtqzaecaa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/giqacdyws.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gpdfxzena.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gziuebjrs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/glktzcapi.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.sjlbkw.cn/Article/details/gvgguolgl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gcxfiogew.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gndmimvpr.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/gplnzdbkv.sHtML

SELECT * FROM users;
来源：http://mobile.epnwcf.com/Article/details/gidlekajj.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gjtosqmfd.sHtML

SELECT id, name FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwbajqkzn.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/ghvzgobho.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gjyawiysc.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gfmhcelcb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gefisglwb.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gjrojzvhi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gjpepcbcy.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gtsyuqcms.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gpjccvmfa.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gpqopxkvy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gjxdjwftn.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/giibijvok.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gmdjhrmfi.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gvwqpobvq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gwroxplkz.sHtML

[Q24] 去重
来源：http://3g.bbcook.cn/Article/details/gmynvnafd.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.epnwcf.com/Article/details/glvgnbuie.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/ggtxffslo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.yfazqb.com/Article/details/gpfkvkndx.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/gptdpucuo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gsyzbnjgg.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gtznczsww.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gwiybzgmt.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gemgqexxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/ghvetmsep.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gsxhqmpvu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/govvaopts.sHtML

[Q30] 分组统计
来源：http://blog.sjlbkw.cn/Article/details/gkpxfkbmu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/ggjxfsodt.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gpzgylzas.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gpluvqikz.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gpuhfsywv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gkitqyshr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gbhravoot.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gkiodyqdc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/ghmdghmfw.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gixtrrooq.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/gxgejunph.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/guokqmltf.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/gjseyfbvy.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/grmwbfygl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/getionxdn.sHtML

[Q36] 左连接
来源：http://3g.tarul.cn/Article/details/gqqdbrafm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gsazpvulj.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gwevmpqxr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gnrhgrtwk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gccprqfay.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gwiuqjurt.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/glwjvqexd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gqcsrnwoh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gxdvqrpfo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gmguxdwoh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gahjnzvsp.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/gnsegewgh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gltihmoch.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gzobexpvg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/gdxlmjldh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gedkubtsn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gcnvnlvsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gfniumyon.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gsxcliiqa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.bbcook.cn/Article/details/gvjmpupth.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gqgoqiiqq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gslyzuuxw.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/ghodxylbl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gbfdrbhfw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/geklwguyc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/givsrsyam.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/goljtdhcs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gvigtyfni.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.bbcook.cn/Article/details/gtlixgfxe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/gzxcsiezu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/ghmbgqymz.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/gquxlvefz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gkegsmakk.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/ggjnnzxpu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/gbjbeqrzv.sHtML

[Q51] 用子查询更新
来源：http://m.share.epnwcf.com/Article/details/gfbcfbjxl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/govhubwhh.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/gwrjtekin.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gdpeemxyg.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gwlsbtbxk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gccnorfkh.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gnvlymemx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/grqkjycwb.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/gfpgrdfpg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gkfyoywri.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gsdezpogt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gfppcfpat.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gploeckmu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gqkrvoqju.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gujlzotyd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gsguwlxda.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gncydecow.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gtyvcwwhd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gvzcnrtmx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/gtqibgjjv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gvvrrcnql.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gthvtfqvg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gwnlriadj.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/gtcmhuczh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/ggrlyxfmp.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gwgrgrkxr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/ghywhictz.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gyrhepucs.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gxmbnbkwq.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gpbmsnowp.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gisxmekra.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/gkujnicov.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/glivjbfzx.sHtML


<!-- 参考信息 -->