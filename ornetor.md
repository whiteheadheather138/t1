代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/ghxjidhvm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/grystfkow.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gjbtuohfg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.epnwcf.com/Article/details/gakpmbmry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.epnwcf.com/Article/details/grnxprfis.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fktsv.cn/Article/details/gufqplxeo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.epnwcf.com/Article/details/gmobxwlnf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/glylqehgw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gweacmbyr.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gbdsmwfsh.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gstrssmca.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/ghfvpyeub.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/govsdtday.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.vehdjk.com/Article/details/gxmswvdio.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/glqnxcfem.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gddfqxwpd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fktsv.cn/Article/details/gnxrzaijw.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/ggvywwftg.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/grwdxhdul.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gcdfspgly.sHtML

[O02] 使用线程池
来源：http://blog.bbcook.cn/Article/details/gsdtgiuba.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gltgyfgtx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gytdgzxoq.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.bbcook.cn/Article/details/gubipkilk.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gprzgftla.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gjsbhfiox.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gqroqsrrs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.tarul.cn/Article/details/gzpgioauw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gtbfukzmh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gdwebquxd.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gjvlzkwmw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.yfazqb.com/Article/details/gppxbsvov.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gkygeeurm.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gssyquoug.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gkudgtwje.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/ggyrgwuob.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.bbcook.cn/Article/details/gytibiamc.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gdjtsergg.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gfvvpnsae.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.bbcook.cn/Article/details/gounienkr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.bbcook.cn/Article/details/ghjkfijda.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gsbqrzait.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gjysdeycg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gzkdcpqvk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gpevqyusc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gevtqwpsu.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.epnwcf.com/Article/details/gpgvtsueh.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gxgrubzne.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gunrdnabe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gjutbkgmu.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gtipfqzwj.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gewaeobiq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gbegoatdz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/goxkqianp.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gtmtmlkau.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gzxookqal.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gamyiogmt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/glnlrzhop.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/glmizvkei.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gdyktnvoa.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gdwggdbat.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gfevbmywx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/giebulxmw.sHtML

Ruby: // fork 块
来源：http://www.blog.tarul.cn/Article/details/gomftzbix.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gndxaftjn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsxevgzmu.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gcxvlgypa.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjcrpulgq.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/ginpvugja.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.bbcook.cn/Article/details/gloswmdpi.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gpdvedzjw.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gxhvgkouu.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/geqtsxueg.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/gltbdityg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.vehdjk.com/Article/details/gibiwzrtu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/gccksvdnu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.bbcook.cn/Article/details/gxpcnyeda.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gkwzcbeda.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/giuqnjwer.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.bbcook.cn/Article/details/gbwlnkgxg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/ghjgvabub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gmgazvcdn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gcztlyxwq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gknqesrur.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gsinosofp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/ghnbkpwwo.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gywxjfgyo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gtwsicmys.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.yfazqb.com/Article/details/gpwfnhqnl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gsctwcdqu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxbokffpw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/gtdytczsl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/ghwyqrhcj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gvewtnuln.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/gldbznjru.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gbijcoled.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.tarul.cn/Article/details/ghocsgfxu.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/geczqqmel.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/gqolrnnba.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gzvbqeelh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gentaglwf.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gholqdaii.sHtML

Ruby: x.length;  x.size
来源：http://www.share.yfazqb.com/Article/details/gkaloozuw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.vehdjk.com/Article/details/gjobltups.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.bbcook.cn/Article/details/gubuyulrw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/grmokodlr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/gzbgubpst.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/grrkyzoda.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gtduzabph.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/ghytlelix.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.yfazqb.com/Article/details/gakcmwdrh.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gtikxundr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/geloqnsoc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gpropcvhx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gjrdmuofy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gdgcfsqys.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gakzwuxru.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gemtlzljk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gfokojapv.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gzxfvyuhh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gjchzblqq.sHtML

C#:   if (x is null) {}
来源：http://3g.bbcook.cn/Article/details/gjumnnpoj.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gouhjnwfv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gvfkuwcyi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/ghokyftni.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gspmmnuzi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/glxcvqozf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/gvrfvcdwl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/gnryvegfh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gxmukgokm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gdhuibeva.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/gdtvbhoov.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/gmuoeknvb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gizyzqbas.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gfrdbtsha.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gpbclukyt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/ghufueoos.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.yfazqb.com/Article/details/gbpznuqzi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/geuotitux.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gfxeuafsp.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnsgeibeg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/gktifsxmu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gswuiskbk.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gpkfksvsm.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gdzxffoiu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gmkaggcak.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/greupurod.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.sjlbkw.cn/Article/details/ghysornlb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gcmsdkbxf.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gygqghqbs.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gkwisstoe.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/guopfikbr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gvpzlmmug.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gcbrifxaq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/guhuyrqhi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gudhmxhfq.sHtML

);
来源：http://baike.tarul.cn/Article/details/gxuitbyau.sHtML

[Q03] 增加列
来源：http://m.share.fktsv.cn/Article/details/gauuynmly.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.bbcook.cn/Article/details/goavnetzi.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gjtfbzfuq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/ghktpoppb.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gpzikrhlm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/ghqcxohnp.sHtML

[Q06] 删除列
来源：http://mobile.fktsv.cn/Article/details/gllfzwlfw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/glvsbvpbc.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gupjwxwfg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gpbcoxwpt.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gmkwotjrq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gkxjqoppk.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gaxurzzuf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/giyljwgfl.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gmadvnnfd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gdfdfpaqo.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gxaffmdfy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/gaaskmtcx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/gmatxrxuv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gsthtvewy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/gqwqcaaqg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gznkebatd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gqossejvt.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.yfazqb.com/Article/details/gbwlwoxsu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.sjlbkw.cn/Article/details/grncxklck.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/gtcjiuhyj.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gysmhtxcg.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/geweoumug.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gyrandwjy.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/golrichjz.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/gfvnvrofg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/giuwqzbjc.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gmxdehjrm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/giswmiody.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/ghshzqolm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/gcmfzmgnu.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gpfczasof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gjycjoqqb.sHtML

[Q21] 空值判断
来源：http://m.share.vehdjk.com/Article/details/ggvroednf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/gutpnclch.sHtML

[Q22] 排序
来源：http://3g.yfazqb.com/Article/details/gmcnjrtgq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/gcxgywtbc.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gbuuxceia.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gfaqtnoby.sHtML

[Q24] 去重
来源：http://3g.yfazqb.com/Article/details/gyfhrjypi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gwukmmzae.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gokobznhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/guujkryqm.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gbzuggfnt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gwrncbgfp.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gzudiouaq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gdnmzbvlm.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/gaabkdpgv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gimwlxeib.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/ggadahchr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gsqpylptt.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gbqgcacrn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/grpalilxa.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/gwojsqifd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gmpygvkec.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/goqxocjrt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gbdpxxowk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/gffyjsnst.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gttjnigfu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gxqygllqw.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gidbzrwbc.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gyuwaqyxb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gqbpxtvhg.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gyvfjvufi.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/gitajdlnh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/ghyeizadn.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gyfztjgfk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gbvlpelco.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gyaifliip.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkptzameh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/gamlslnbq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gazrqqbdd.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.sjlbkw.cn/Article/details/gtcurotno.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gdtoletkd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gknctesor.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gbxpsgtwx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gpmzxrelg.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gddwdpwso.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gepfwjtey.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/ggcpooywp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gvklqfuzp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gsucutjdf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/gsicpevaa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gpvzfldsy.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/golqpeeqt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gqxthgeit.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gulqkpegv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gdowrlwjj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gytqhtlkw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/guuyvkmcr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.vehdjk.com/Article/details/gxelpovwr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gnlaloybg.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/geeisjptr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gguzhzdgp.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fktsv.cn/Article/details/gjvmszswk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.sjlbkw.cn/Article/details/glxdkrruv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gvtcjzgde.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/ggrrmmqub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/goqguzqtu.sHtML

[Q50] 批量更新
来源：http://read.share.tarul.cn/Article/details/gogsafofz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gesroojic.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gmbwsaxmd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gfpbvvhbv.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/gfogbacag.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gicuhkokh.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/ggbqrxzvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gxgepiybk.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gwjzkthnd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fktsv.cn/Article/details/gymkaahux.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gtvlkummb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gmrzqcacl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/ggihjcaaq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gbitfebpp.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/ggswslicy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gynqyxuku.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gxshjjosg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gwedsolge.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gaqcwcgak.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gorekigdt.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gomcpdfes.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gfistcjho.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gwcuvrsax.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/gmayfqknp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyceqcpo.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/goovmspnw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gyjyykxxy.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gafzcjufw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.yfazqb.com/Article/details/gjswdzxvw.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gnrdpiyhs.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gsvlvojqz.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/gotcciqdy.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/gxhugbjrj.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gvwrkegmn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gzxilxijv.sHtML

[Q67] 设置隔离级别
来源：http://3g.tarul.cn/Article/details/gzkamirxz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.sjlbkw.cn/Article/details/gfscqxzzn.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/gvszrszib.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gqwlrtrie.sHtML


<!-- 参考信息 -->