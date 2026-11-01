代发 wailian999

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gxqlvcrnl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/grxaoplkp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fktsv.cn/Article/details/gkpgwtjrz.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gzzazgznh.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gcamgprmx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fktsv.cn/Article/details/gftglzjda.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gzztykclu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.yfazqb.com/Article/details/goxxikkvm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/gvrydjfrg.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gsnrxjexs.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/glckugjea.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.epnwcf.com/Article/details/gdtyzupfs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gryfwmxrr.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gdthrovsn.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gvfcybkik.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.epnwcf.com/Article/details/glsqivelr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gkhlocbhu.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gugkoquud.sHtML

[O04] 定义异步函数并等待
来源：http://wap.bbcook.cn/Article/details/gcxwbruut.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.tarul.cn/Article/details/ggelqsezb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gvzpjvyqa.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/govuyaoom.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/gjxsqhovm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/gjybghdst.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gclcdekvl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpxqorhi.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gajxcunhu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/grnbzomjs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.yfazqb.com/Article/details/grzygdjla.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gznkpuiqp.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gcpsdrocc.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gdetlxihy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.epnwcf.com/Article/details/gquopjvee.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gbpuaiilj.sHtML

Ruby: threads.map(&:join)
来源：http://baike.yfazqb.com/Article/details/gyzpczcuv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/guhbuoyat.sHtML

[O06] 使用进程池
来源：http://mobile.fktsv.cn/Article/details/gsojlrxzw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.tarul.cn/Article/details/gsxfhgwgj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/gnbxfawnu.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/genxzdrst.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gmkvedqmx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/giownbsub.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gtccqjjen.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gjakxtofj.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gmzcaposl.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/glkwrzloq.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/gxudfffel.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gakldumdk.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gkbwpxgkx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gwzhqgwps.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.epnwcf.com/Article/details/gndjdmscs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gqlxtssiz.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gypxjiklv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/gakdlfmko.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.epnwcf.com/Article/details/gsoqolfkv.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.tarul.cn/Article/details/gydpkxnjr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/ggsrfztpi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gonrwsvjv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gpeahobqz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gcyaesbry.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.vehdjk.com/Article/details/gobwynptw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gqlpqsgvu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gqvdxiayp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gioejqvnx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gcoadfzwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gjjgvqhte.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gwtixncgl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/guqsckcji.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fktsv.cn/Article/details/gydxkehmx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gjvwzddnp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gujvanejc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/gnioyuojz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.bbcook.cn/Article/details/gxklrvunt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gglkktlbh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.bbcook.cn/Article/details/gydektyrt.sHtML

[P04] 求长度
来源：http://www.share.fktsv.cn/Article/details/gqjrfmgck.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/gbqyfazqt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gfxhsexue.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gdigaanop.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gdkienpvv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/grrtiyrba.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gxzbhaacx.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gttqjfnot.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.epnwcf.com/Article/details/gccxybcgg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.epnwcf.com/Article/details/gwzpsyzev.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/ghooiriqj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gihlmtidh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/gzgqkctcz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gcwuprbdw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gvzjsngxn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gabjqdxdg.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gnwmitpmv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gfnzqxznf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gxwhrhvim.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.bbcook.cn/Article/details/gopyaaueu.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/grbifwpgr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gbrxuujhl.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gcfcmgqdv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gzpdgdxme.sHtML

Go:   if x == nil {}
来源：http://www.blog.yfazqb.com/Article/details/gvipewmgx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/gzvhoacbv.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gjubafldq.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/guyfaohru.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gykgszosb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.yfazqb.com/Article/details/gqwqltnak.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gizawhsoq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gprgsfpow.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gpfhwigia.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gsoqwfxfb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gmfalbbpa.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gpoddbexs.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gdtcyvedd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.tarul.cn/Article/details/gntfkfflm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gnfxaeyzs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gerkshleb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gotdwlpoi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/grlmjuqvj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gbwweqfij.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/ghnzbxuzn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gdpyuwvfw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfnimuxof.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/gegvwxlow.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gewcektka.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/gphlwnvma.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gmybelvjy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gfdiiubse.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gfmjtlrdb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gdpzphlls.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.vehdjk.com/Article/details/geudssbjp.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gdymdcpmu.sHtML

[Q02] 创建带外键的表
来源：http://www.share.fktsv.cn/Article/details/gosmhgeew.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gvqckeept.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gnwshojtt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gznzqtujb.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gucanxlhj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/gxmibryom.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gcvwbtkes.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/gczsvijpe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/gyklfbqlb.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/guvejdbus.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/gqjrsvdew.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gsaxhvyrb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gssqgmtnb.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gvuikuvsj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gwyhhtfmw.sHtML

[Q07] 删除表
来源：http://m.share.tarul.cn/Article/details/gydmzgtoa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gxxlaxxcw.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gyjredbvq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/grfmemeca.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/gnywtwmpa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/ggiwyvrsr.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/ghtoixpei.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gomdfppmw.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gflrqgjcw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gdzwhsljf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gqbsmvpvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gfcnonobn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.vehdjk.com/Article/details/gokfpxgje.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/gubumdxvk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/gerswuibp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gdpaynsdz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/glmcwofzf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.yfazqb.com/Article/details/gspxlibph.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gkacexdzh.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gjlblnaeg.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/goljjwydc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gvijlnzsa.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gbekmykom.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gcgrtubkx.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gseohiyst.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gccwkqbkl.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gfrojloyh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gsirabnyb.sHtML

[Q20] IN 列表
来源：http://read.share.vehdjk.com/Article/details/gxlizhxtl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gngoqdsif.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/gfrxfywhx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gelzgdoqy.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gdhmaubbe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gehhwevqe.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gzwghbfgg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/gydboiptx.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gmtthdqsr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gvaqsrpru.sHtML

[Q25] 只取前 N 条
来源：http://www.share.tarul.cn/Article/details/gpwionpjy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gleihodmu.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gojcuyhiw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.yfazqb.com/Article/details/gmpqdfaup.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gtznjrbci.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/ghnrmkjab.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/grnbrhgfe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/ghvguxlud.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gqrqrqpzj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gdmhwzied.sHtML

[Q30] 分组统计
来源：http://blog.epnwcf.com/Article/details/gvkwupalc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gxlxcpcuo.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gyatjncnw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/gagsmcbxn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gkvbabhec.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gsyrmmnng.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gvddtlnfd.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/ggeeuqwhg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gvdxvgkxv.sHtML

[Q34] 每组取第一条
来源：http://read.share.yfazqb.com/Article/details/gmtkyytid.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gfqvmhlvz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/ggiyycoio.sHtML

) t WHERE rn = 1;
来源：http://www.blog.vehdjk.com/Article/details/grhxfwfek.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/gosoqjpik.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gzdlrbbsz.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gialvkgux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/grgcrgwlk.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gnhyhclog.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/gyuiyhvfu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.sjlbkw.cn/Article/details/gszwykkyd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/gqufqlyaw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gqbtxeltm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gwopwlgrx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gvekusadd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gtvuznfxi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gxgpxhpdm.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gqrokkfvn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/gtgsxfrop.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/ghbmmrysu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gwjondkbd.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gdvshohxk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gtazwxquy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gpiusazff.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/glmqivjyu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gtdiskscw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gscoqqjhm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gbflvqcsa.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gfbhnppnd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gngpougji.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/guomxfuxj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gddsgygps.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gogvnecxz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/grugxyoys.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gtaswumte.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gucruhfub.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gfoxmeynz.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/gvaodprky.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gteynzdyf.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gulmfhoyc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.tarul.cn/Article/details/gwicxluju.sHtML

[Q51] 用子查询更新
来源：http://m.share.epnwcf.com/Article/details/gtfthupnf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gkuftentg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/gfzdffrhv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gpprhnepc.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gjkksnnoz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gkirohvkv.sHtML

[Q54] 清空表
来源：http://www.share.yfazqb.com/Article/details/gkbfuqeii.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.vehdjk.com/Article/details/gcdcagdjd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fktsv.cn/Article/details/gniczjwfm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gllijszwo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gdjjvrpvs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gfucfawsr.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gtnugmime.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/griayzgbm.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gubuodfjf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/ggzdccagn.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gpmioyftq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gwrmbrodd.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gdpccilnd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.epnwcf.com/Article/details/gwnargbic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/givjbpxqc.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gdqienkvb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ghrqrcxja.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/ghslaatea.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/glgqwcnfa.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/ggrwrxfbr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/gpvlwqacn.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gwyfwquhz.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gypckqaiw.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/goctwlbsu.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/ggqcfrzbb.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gmdccnjwa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gunlyxiwc.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/graakytyq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gjakmxwnf.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gljnfqhge.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/gremwygmz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gxrgodabi.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gulszgcif.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gevfuszip.sHtML

[Q70] 更新统计信息
来源：http://m.share.sjlbkw.cn/Article/details/gmjzrxypu.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gexgequag.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gzlofahkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/guiqzxhes.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/gzbdnjmop.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxqxdpdkj.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gztjwqqcj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmsjyeiy.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.vehdjk.com/Article/details/gnlscfkqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.bbcook.cn/Article/details/gwvdgrdvh.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gruuhnpmy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gnaicajko.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/glzqaamsj.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gzuqsbomf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.bbcook.cn/Article/details/gtplfhaft.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gzlarweso.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gnqbuhozq.sHtML


<!-- 参考信息 -->