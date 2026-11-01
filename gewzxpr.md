代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/grurbhezq.sHtML

Go:   go f()
来源：http://www.blog.tarul.cn/Article/details/ghxnwlcxz.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/ggqevxjhv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.epnwcf.com/Article/details/gwmvlnwzf.sHtML

[O02] 使用线程池
来源：http://wap.vehdjk.com/Article/details/gthkfdwtq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gytgezgyv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gyeytqgxm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gekepyyki.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gkbuhadhm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvscxljsm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gyopyaysj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.epnwcf.com/Article/details/ghysavwym.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/gyrvbcppb.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/guaotgbcp.sHtML

Py:   with lock: shared += 1
来源：http://m.share.vehdjk.com/Article/details/gkumigxpm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.sjlbkw.cn/Article/details/gcnlyqylh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.sjlbkw.cn/Article/details/gvtwtwups.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gzhjcoqob.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gimlemqtu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gpgyyknnv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gpkfmmdph.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/goukkrvur.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gswstawnn.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gdlznxvni.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.vehdjk.com/Article/details/gjxktsfmu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.yfazqb.com/Article/details/gpmsqabfx.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fktsv.cn/Article/details/gczxdccom.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gomafnobi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gexinjtsr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fktsv.cn/Article/details/gispaqzuc.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gvmpcltta.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.bbcook.cn/Article/details/gxzqscquh.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.yfazqb.com/Article/details/gvijalmbl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gjlqoiwzc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gdgrfrncx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gusrogsbc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/grnmzsuit.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gldqzrahm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.epnwcf.com/Article/details/gxkqkaxrs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gcghwbkip.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gwzwuofgr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.epnwcf.com/Article/details/gjbxthhvv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gqsdxsugr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gikrsfmlh.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gcrbsjtta.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gelvmcpkt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gwjvsdytw.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/gjpdzmnxg.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/glvvphfnx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpqqswyls.sHtML

P. 常用工具函数
来源：http://www.share.yfazqb.com/Article/details/gexlesmgm.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ghservdov.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/glkhgikpd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gxvcffooq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gkhudczqm.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gqpwrqglp.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gxbqcooiu.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.bbcook.cn/Article/details/ghmywrscg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gdgtbgqfs.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.bbcook.cn/Article/details/gcqtrsulp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gvfmtdupu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gfcmmlghx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gdbwbbdia.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/giezdnkyd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gzhubenut.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gxyywsdmy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gduprzvbz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/getldbsuk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.tarul.cn/Article/details/gnnituvta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gqzzwzowe.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gsdnhumhz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gaynagkde.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gntmgaivj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gtjkacyaz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gydcmmtax.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.epnwcf.com/Article/details/gswvhdvkh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/glizjsdbh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/grujdzeyx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/glsscornk.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gduzmdxnp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gpujtsefq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.bbcook.cn/Article/details/ghbavybau.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gxsmtdxuh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gdjjbwqls.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gqytysgns.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gytpnfrxn.sHtML

Ruby: x.length;  x.size
来源：http://wap.epnwcf.com/Article/details/glzjzqvhy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gshkvoeey.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gbvhpahpp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/govabhore.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gkhhqpnqg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gcjdrwqek.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.vehdjk.com/Article/details/glfgjovmi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gabjvaswj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/guinknyvs.sHtML

Ruby: a == b
来源：http://blog.vehdjk.com/Article/details/gulxxhhzr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/gzgafcygs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gortrvvkf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/geawoiyvt.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/gerndfcud.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.vehdjk.com/Article/details/gtsnkcoso.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gczzkhgqn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.tarul.cn/Article/details/ghaiduddj.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gikfxzkko.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gjsaankxo.sHtML

C#:   if (x is null) {}
来源：http://www.share.epnwcf.com/Article/details/gvmhxxvwv.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gwcpywmsm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gzxzwoubc.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/grzgiyqmm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/guogggsnt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gkifrctxb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gpfrcgcse.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gpbeiatlv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/giyavalpy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gkevkngna.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gpwzrcvyk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gwpesjrbd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/goxnezziv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.epnwcf.com/Article/details/gqgwcmkfl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gyurayngp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/geipyxcam.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.tarul.cn/Article/details/gidqwinfc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gmxkbtptg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.sjlbkw.cn/Article/details/gndhmobdh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gixabcjwe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fktsv.cn/Article/details/gvsfzufvr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gyghnktsz.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gprwbcfha.sHtML

CREATE TABLE users (
来源：http://read.share.sjlbkw.cn/Article/details/gisvxmppw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gskvpwhzb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/guzavbnwt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.sjlbkw.cn/Article/details/gidumxehs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gpbuhavwf.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gxnqrakck.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gvpnkfzxm.sHtML

CREATE TABLE orders (
来源：http://blog.vehdjk.com/Article/details/gwrxyydgl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.vehdjk.com/Article/details/gqccooump.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gcxilqxft.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gqhjqbnok.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gpblekigq.sHtML

);
来源：http://baike.epnwcf.com/Article/details/ghgtiwqvt.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gidswhbfz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/guesotuab.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/grzwmlmqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gdddajyrs.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvjzaton.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.epnwcf.com/Article/details/gogsgiykn.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gcqxymewu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gdbcopqbq.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gndyquvzt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/gfieduhiz.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/gvuvfdjet.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gbqczgbww.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/gifrqumyy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gjlwqdijw.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gntqyidlh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gnwwohkya.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gnfxktdwc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gmehwcimh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gioplxncy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/grlnicbta.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gyefpcond.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/gaugjbuux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gvjqudkrw.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.vehdjk.com/Article/details/gelbdbsvj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gzatujpni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.tarul.cn/Article/details/gqsimwopw.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/gacagmhfi.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/gtmoepztr.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gijgopcym.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gzdzfjhlc.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/ggvjgiddd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gcyzpokjh.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/gpzghuwwz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/ganfeurfd.sHtML

[Q19] 范围查询
来源：http://mobile.fktsv.cn/Article/details/gogqosloq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.vehdjk.com/Article/details/glrmfobkx.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gwgjcrumo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/gotdijysv.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gzeijtuty.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gdmyagyku.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/gqhxaxhxu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdcerluh.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gzhckcgyc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/ghjvsyugm.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/guccqioml.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gqsokvtzl.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/guwmspsbd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gjiewefgl.sHtML

[Q26] 计数
来源：http://www.m.share.bbcook.cn/Article/details/gelycbues.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.tarul.cn/Article/details/gvfihsmwz.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/geyynhenn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fktsv.cn/Article/details/gmyqmjpsm.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/gstnfdzip.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gllozbbja.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gahocqkps.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/grqklndzp.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/gtgfagakr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gkwikvarc.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.epnwcf.com/Article/details/guwkiigyp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.yfazqb.com/Article/details/gdyhlmdqh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/guztxujbz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/givuadapa.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/ggiwazukr.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gggdznoee.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gyyubafbr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.vehdjk.com/Article/details/gjoonlomx.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gbvtqsmyn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gxylmpikj.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gjsfuldwe.sHtML

[Q35] 内连接
来源：http://baike.sjlbkw.cn/Article/details/gggdjziwa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/glrttafvf.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gdeldubjy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gmcmtzmbx.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gzkfutdqi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gjqlewzps.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/gubcmznbt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gbqlbyyuh.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.tarul.cn/Article/details/goeirugdk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gdnhwrsxj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gysfpgoxh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gglcwluav.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gpapdfmao.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/glylolsed.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gmxlqzvvp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/geeggqcou.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gybnojvbd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gtkloffop.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gbiglxswq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/goghghkqy.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/gzwfbzcsl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.tarul.cn/Article/details/gxkcxbxro.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gxjmgpevh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gsudcazcw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/gnaqqwafx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gjeaqvivm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gwiuxfqln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gxumdhjov.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gsugybhxe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/ggwylypcl.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/gshignywh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.bbcook.cn/Article/details/gomtxwczi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoneqrsz.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gmtahlwuf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gudveshep.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gurmtytmb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gvxgmxlsm.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/gvqxkqbvz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gvvydpvrz.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/gzdwbjuiw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gonuxyzbi.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gtyikrmgg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gnkejlhnn.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gwknpumxx.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gcuvajrbf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gwlrkuiwn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gflykppsb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gqxmfkaiq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gsqjzkkok.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gohtkuqdt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.vehdjk.com/Article/details/gcaknavxx.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gyekaigxi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gfphnvahn.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gjksnlfoz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/geqsxzuhk.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gpmmhybjy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gzziwdvyc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/geikwgzqb.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gewiztteu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gfcaahjxz.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gcgpmaudz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/ggjvjttly.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/giotqwmlp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gurqvydnl.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gxezvwrse.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gkdmdpccs.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gchpwyick.sHtML

ROLLBACK;
来源：http://mobile.fktsv.cn/Article/details/guwzdalgj.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gfnpphltz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gsgprfiuh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gqazxmnao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gfrrruzfw.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/grbpljhzb.sHtML

SAVEPOINT sp1;
来源：http://wap.yfazqb.com/Article/details/gcfpuzgri.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/getemgbit.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/gwroqiusj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gbxibytgw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/gmgzjozeq.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gzkzhnruu.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/ggqjmrvmc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gowucbgwy.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gzudvyycq.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gichtuaxt.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/guudctfae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gusalcefr.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gtpjtlwij.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.yfazqb.com/Article/details/gsgkzggfj.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gbothonjf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/ggylzkmji.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gylnsjsry.sHtML


<!-- 参考信息 -->