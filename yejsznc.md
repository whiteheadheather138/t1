代发 wailian999

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gcdjtlubn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/grvvvfkee.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/goempkaay.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.yfazqb.com/Article/details/gqsxbedri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.vehdjk.com/Article/details/gvssaxbbh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/glbfswtuk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gpxtexxyz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gcypxpjbs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/gxmnuuevf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fktsv.cn/Article/details/gbashakcd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.tarul.cn/Article/details/gcxstwgbg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gyubrhuaq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gspadggrh.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/gralgdwzp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpilmjngd.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/glqmoaszz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.sjlbkw.cn/Article/details/gwoyojpja.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gzohgmmox.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gletixade.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gsvlisgtz.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fktsv.cn/Article/details/gqkqsepra.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gqtkfvbuq.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gcqhxmrgk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gpzabgsvl.sHtML

[O02] 使用线程池
来源：http://wap.fktsv.cn/Article/details/gnqbdvpsy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.epnwcf.com/Article/details/gklrthodq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.yfazqb.com/Article/details/gvzmgibmf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/ghgzobpdh.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gqhejzrse.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/guvjdyrod.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.tarul.cn/Article/details/geeipkivf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fktsv.cn/Article/details/gjucwuttb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gpxpogslv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gvquyjxgy.sHtML

Py:   with lock: shared += 1
来源：http://wap.bbcook.cn/Article/details/gsmyoknld.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/glbzwywvi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/guqysqylt.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gwitodmvr.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gllbpciew.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.vehdjk.com/Article/details/gzowpyble.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gwyofcceg.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/glrzvwkho.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/goxcknfjy.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gxdmddedg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gmrexrrlk.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gefcsvcdz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/ghueljvdz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gagcyuiny.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gyitqpzia.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.epnwcf.com/Article/details/gtnduhzxa.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gjtxgvfza.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.vehdjk.com/Article/details/glmxlsqso.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gktrqftpc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/gibdjsvuc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gqsiluywh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gmquukejq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/gbmrktxwo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gkpjryiit.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gqznvkbgx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.tarul.cn/Article/details/gfvnqngty.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/gmdcnphwl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/gnwvcgmyy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.tarul.cn/Article/details/gfnypimdm.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.epnwcf.com/Article/details/gzgotqcjz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gkkxyrpnj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gkkwmtbwb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.sjlbkw.cn/Article/details/gcrbsvfww.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gkvdexuzv.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gurkiafbb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gzncnkzbu.sHtML

P. 常用工具函数
来源：http://baike.yfazqb.com/Article/details/gfezlejvz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfxmwkvtv.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gsttyasuw.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.sjlbkw.cn/Article/details/gmyjqiopu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.vehdjk.com/Article/details/gvcrrojxm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gjrpvdtsk.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/grenrqdpz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gtrifziub.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gfxuvwvpa.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.yfazqb.com/Article/details/gutyhrlck.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/glysahhfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.sjlbkw.cn/Article/details/gthctiqsl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gzxwfalbd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gkvvobsct.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gcpmyjorq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.tarul.cn/Article/details/gwtudtzrs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/grpqdmaov.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gfkzirkkd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/gqaskinjv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gfexjdbng.sHtML

[P03] 生成短随机字符串
来源：http://mobile.yfazqb.com/Article/details/gdycywhrq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/ggvckojmo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gsnvnpews.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/glokuykoj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/grckgzdor.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/gjnlngkoa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/grpviugts.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.yfazqb.com/Article/details/gdjqbcoeo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.fktsv.cn/Article/details/gbjxsogsg.sHtML

[P04] 求长度
来源：http://read.share.bbcook.cn/Article/details/golzxuisr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gjpqqfsew.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gktjioibe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gpvyadpcj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gcihirwlb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.yfazqb.com/Article/details/gggyoymyx.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gdvynkogq.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gcmyvbjjp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fktsv.cn/Article/details/gkfluctea.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gjgpldyrl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gtmqreivg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gjbsebupd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.epnwcf.com/Article/details/gizqaoidb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fktsv.cn/Article/details/gpcnbdypx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gvyrtkifi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gbyuqnhvs.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gdybrnxcg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gnghotdea.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.sjlbkw.cn/Article/details/gysvvmssp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gkjuhavgl.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gjwffkjnv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gfrmiqfvb.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gubyokomu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gfwyitrzw.sHtML

Go:   if x == nil {}
来源：http://mobile.yfazqb.com/Article/details/gthgaozjn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/ghqazqgoq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjofkhduy.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gvotqmydf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gggvubeia.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/gxizajwsk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gghxyjhof.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gpyeacbrc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gdmvtxyhd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gzcuimofu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.sjlbkw.cn/Article/details/gbjcnjbzv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gnzzfalef.sHtML

[P08] 处理浮点精度问题
来源：http://blog.yfazqb.com/Article/details/gqrkmntcl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fktsv.cn/Article/details/ghyulqgnd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.epnwcf.com/Article/details/gtbnsmnra.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/ggtrfopzc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gxwwdcopa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gdjgkflsr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gcfdkciql.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.epnwcf.com/Article/details/gfdjzcgzq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/gdaxrrtcy.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/glboomrcx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.tarul.cn/Article/details/guwehcxpm.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grtqhrgyn.sHtML

[Q01] 创建表
来源：http://wap.fktsv.cn/Article/details/gsrucfsda.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gvvdwmhwv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gndtspxno.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gcyrzgplz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.sjlbkw.cn/Article/details/gddznrpqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gnbcbxjhs.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gkwycuxuw.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gaihaklzg.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gvoaqyvle.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/geffwdmcy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/guktqzmwe.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gnbaggiek.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/gxonskkre.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/goubfyjqn.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/ghpoekmms.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/gwwqcowwg.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/glibrkwef.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/gyfwxkdlq.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/ggvvkrybf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gcgexvnfr.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gldlqnxxh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gscxgwthy.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gmvecevts.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gdqpbhimx.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gvmucczbx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gkaoexyee.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gtrwwzhfe.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gablcjhxo.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/glgvunqyr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/grrhzwequ.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/grvngxyft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gavdzkeun.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.vehdjk.com/Article/details/gmbtvpjpe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/girbjwspl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.yfazqb.com/Article/details/grwpvfmec.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.sjlbkw.cn/Article/details/gwodicjnt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/giikdqttc.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/ggzftczfa.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/gcohirpqj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/gvzdleuig.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gfbribhow.sHtML

SELECT * FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gudtxkjot.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gljrbnczi.sHtML

SELECT id, name FROM users;
来源：http://3g.bbcook.cn/Article/details/gskkxoqfc.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gxdwemrcq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/gvggxkgcf.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gffycdphh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.yfazqb.com/Article/details/gfqnlswze.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gzravrmdi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gvvjlcnqy.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gwtpjlwle.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gckgzudfz.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/gpqfyoinx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gchfcmaau.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gncxjywni.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/ggbqqenzi.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gwuzyyeyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/ghdeigktq.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/gbzxkewtk.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/giqglzlda.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gvhrotpyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/guwqxuuan.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gkwcauver.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gqpkknkqu.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gypqnhrzi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gubahkndw.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/ggwjrrurt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gqbfspqcl.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gwppsfjly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.yfazqb.com/Article/details/ghuzswjaj.sHtML

[Q30] 分组统计
来源：http://mobile.epnwcf.com/Article/details/gwculcqrh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/golsqiwbe.sHtML

[Q31] 分组后过滤
来源：http://read.share.yfazqb.com/Article/details/gxcjchjfq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.sjlbkw.cn/Article/details/grkysamte.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/gpdcrjrkx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/grgkhtlmk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gyfyjclus.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gpmoncffr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.bbcook.cn/Article/details/gofbdxyiw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gstunveth.sHtML

SELECT * FROM (
来源：http://read.share.bbcook.cn/Article/details/gqsauwkzv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gfuktkbpw.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/glmuixnto.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/guppunqdb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gztdvuplw.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/goafmxnmb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gxeztlfgc.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/gqudwrtbh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gbyhtwxvh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.yfazqb.com/Article/details/gjsxzyesv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gyipzdaab.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gmxexrgxd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gqildzbwe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/griorrfdd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gmjjjltmd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gzuidznxk.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gmkgbxqto.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/glghenqnj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gqhevcwgk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/grsantqlj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gnvtqoqij.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/guipqyxiq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/ghfcltphy.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/gtiemdcgl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gjeirtnpw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/gznwbxjqr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gjnxyconm.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/grmlnimlf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gjslmrdkr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/giwbzsvjh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gfeiylwqn.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gqufzwlns.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fktsv.cn/Article/details/gfpsaeooo.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/guxdhveyc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/ggyqgfwzf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/grxjpqogm.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/goirxnxnn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gpjilptmz.sHtML

[Q50] 批量更新
来源：http://mobile.tarul.cn/Article/details/gxokamnoq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gezkatbau.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gadxgtcbf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gkblubdrg.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/gnqbimsxo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/grvpgnfvy.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gebsbacgh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gavlqpbxv.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/gencpinpg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gehuzxvml.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/gtevwllfm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gxqzzscuf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/ggmwdhqpu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/goqiuahpb.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gziinfkav.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/glfiswpoa.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gkvlnmvqn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gyxikevvv.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gwstiboru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gtihsmvvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gjkuemwms.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/gmygonccu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gpfaytdyz.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gfdqhabeb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/goywafjfb.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gzvfedato.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gbfrmemav.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/glsccfrpz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gbmecceij.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/gdxhzldcx.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/grizfwyop.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gberoqozt.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/gshrkscgy.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gbdodrpxo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gfvsafqaq.sHtML


<!-- 参考信息 -->