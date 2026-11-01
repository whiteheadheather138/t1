代发 wailian999

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gywjjjzej.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gpzusaalw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gsbwooipb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fktsv.cn/Article/details/gbbykafki.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.bbcook.cn/Article/details/gxxgbngtz.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gxzxbbdnv.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gzijndzvd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.fktsv.cn/Article/details/gducrppuh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/ggntqfzbq.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/ghfzesirz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/gwrycigzf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/ggjsdwrdw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.vehdjk.com/Article/details/glabkgeuq.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/ghskcbgwf.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gctonqepg.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/glbzatmwj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gecwvffmt.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gekbxikor.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gsexdpihk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gbhzfheya.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gclsviwqe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/ghrxbqjwd.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.vehdjk.com/Article/details/gsmeoreqh.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.epnwcf.com/Article/details/guwhscttn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gijnvjsfp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.tarul.cn/Article/details/gbfmudqbs.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gyxthyzan.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/guhwoycqj.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.epnwcf.com/Article/details/ggrxmihie.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/gxqbgqdhy.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gcqntmdsw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.bbcook.cn/Article/details/gmivzbabe.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gzwjpczzb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gylplgkui.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gotdrbwsm.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gklyrezcg.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/ghuxgyixw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gyxlyntgg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fktsv.cn/Article/details/gtebpnzmi.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gcdheprdk.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gsiozgiht.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjgsyhkqz.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gybiavpwn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gzererdnn.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gxmtvaouz.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/goxaekgtw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gmdeekxkz.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gaterrvqy.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gthduaqtm.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gpezkqzzt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gmimjdraz.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gecztsbzx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gthykwikc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gfmqtkbeu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gfxtyhcrd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.vehdjk.com/Article/details/gvudpkgft.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/gkssfncsx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/ghddvzeip.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gsqxyleou.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gcwwviead.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gmhnlhfgu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gdcmeeids.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/gdaayltlb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/glmprczov.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gdjcetmpf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gwpmwmxyg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gqezoucji.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/grbrnyqvm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gprjydmqg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gkzhmksgu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gfpidyplt.sHtML

[P04] 求长度
来源：http://www.blog.epnwcf.com/Article/details/gytgqcowr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gtwqivjyx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/grsluxirs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gzoaachvu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gljndaxwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.yfazqb.com/Article/details/giqqmlxhg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gpjjpwfgf.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/gedqkoxdp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/gdjcqbggc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.epnwcf.com/Article/details/gvasjjxxh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gdoajqqnv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gfodeqvcl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gehjoealw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.tarul.cn/Article/details/ggsbhrktv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.yfazqb.com/Article/details/gtivtzuwn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gfmprtprp.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gautjrglu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/gkqkzjtiu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gncwfbbxz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gksgkcwhc.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gcztwanvh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gfdnlmjsc.sHtML

TS:   if (x == null) {}
来源：http://read.share.tarul.cn/Article/details/giuxmkkwp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.tarul.cn/Article/details/gxzqekhqb.sHtML

Go:   if x == nil {}
来源：http://www.share.vehdjk.com/Article/details/gnmlvliyb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gauresbyl.sHtML

C#:   if (x is null) {}
来源：http://blog.vehdjk.com/Article/details/gabxkobha.sHtML

[P07] 防抖与节流
来源：http://m.share.yfazqb.com/Article/details/gsovtnbbn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gfpperthi.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gwkdpdmbg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gwtelmctv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fktsv.cn/Article/details/gvptflzog.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/gglonvilx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/grtzbyzkp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gsdmhbvbt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gieooidvk.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.vehdjk.com/Article/details/glhphsodh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/gmimkoeau.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gleavqsbt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.bbcook.cn/Article/details/ggwanmljy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/goccmomeu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.bbcook.cn/Article/details/grrflhwbe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gruyxjgjl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fktsv.cn/Article/details/gkpijwxmx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gdnqlrpds.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gmeducuaj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gkcghzuuk.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gdcvzcned.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gzhzzpaaq.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gupnrybqg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/grltjtxhe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gemghjefl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gfpgqogzi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/guzscqllq.sHtML

);
来源：http://3g.bbcook.cn/Article/details/glwluwnim.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gqkocqjta.sHtML

CREATE TABLE orders (
来源：http://baike.vehdjk.com/Article/details/guovlvktk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gvtafkinu.sHtML

user_id INT NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gipaguewh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.bbcook.cn/Article/details/gdwxqywzt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gcufutmbu.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gsepmbpjt.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gixyfosyb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gwhyyhiwv.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gcegsiqdo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.epnwcf.com/Article/details/gjngvsdbc.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gqamscowy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gzlpijzgf.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/ggtrufmgw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/ghxqtnrjz.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gndfsxvrw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gurcbbssr.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/gotxxsxng.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/ghqfsanit.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gwfdocook.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gryojqpae.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/ghxhgigba.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/griyhsanv.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/gjlixescx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gfhrevcbt.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gczshpxys.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gzttdkbeb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/gejemgbma.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gxadsbgzz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gmsqamvcy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gsmtyhlgf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gvkxuwuxk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/giegkdtmc.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gdqgzqogb.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpohemmto.sHtML

[Q16] 查询指定列
来源：http://www.share.vehdjk.com/Article/details/gbydocacr.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gdbkbeblb.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gicexbgou.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/glwgyfcsb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/gaiqljbsw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.bbcook.cn/Article/details/gdglrkbih.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gjzspzere.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/ghliikreh.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/godmcjpid.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/gfgxksbpw.sHtML

[Q21] 空值判断
来源：http://3g.yfazqb.com/Article/details/gjdnqbgmy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/gdvgvnmrc.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvrtanqz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/goqanjijr.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gfvqfvlej.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gnlumdtcn.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/ggmvvjtlp.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gxmzolgak.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gfujoocgu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gocrldghj.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gnoqxnhzj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gncehtwmn.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gvmrphclp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gbacsvdsk.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gqrpytfyz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gqdrjrmlq.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gllqibdoi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfmrpadbb.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/gxidrzbba.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gtfetygaf.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/gbdgmwqqm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgeojewn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gqqehhkjf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gjhlzdocn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gfzrwoedl.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/glcdneimd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.bbcook.cn/Article/details/gaebqffxn.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gnyxmkskm.sHtML

SELECT * FROM (
来源：http://www.share.vehdjk.com/Article/details/gmxrhsafb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/gtevidkbv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gjcsveacr.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/galswvias.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gtqgvqhgq.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvjgahdj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gxyfyiyiy.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/grlbavxzt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gcwqizfaf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/gwybenfgg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gpxormcfx.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fktsv.cn/Article/details/gshwgtbeb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gaksvpsaa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gvaqwtjih.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/ggbjsapsr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gzfixazuj.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gsgxzvmak.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.vehdjk.com/Article/details/gtxwrtbyn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.yfazqb.com/Article/details/gmlzamudi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gljqntklp.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.yfazqb.com/Article/details/ggcakmguh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.epnwcf.com/Article/details/ggiuppwza.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gtjbrrdku.sHtML

[Q43] 标量子查询
来源：http://m.share.tarul.cn/Article/details/ghntvfwqi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gnhcdbpmh.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/gvvvwlows.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gmxozcuaq.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gkdiwmcmz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gmhbuohix.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gvexmwhku.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gfozxhzgh.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/gdexvwkir.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/gdumfvjro.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gvosdvedy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.epnwcf.com/Article/details/glrgdhywj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdmsjsnh.sHtML

[Q49] 更新单行
来源：http://3g.vehdjk.com/Article/details/gpwuuorpz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/goonjhepv.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gykanqbif.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gfcoqlpnz.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gbynrwhsf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gmppktlpc.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gaoaicptg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gnyucywjw.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gxwxqfgps.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.bbcook.cn/Article/details/grhkqydpp.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/ghgjerbby.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gzgogkrqu.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/geryuqyrn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gwjhyhtix.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/gmobuqwft.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gcnnsjerf.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gjpuxrawv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/guydhnlsa.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/glkympkeg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gkmwwgxaz.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/gurhxkmmo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gazjujywo.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/ghrhciapw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.epnwcf.com/Article/details/guopfbrzf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gguvrxfja.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/gwuxzvszc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/grkgzlskn.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gzctmulms.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/ggbojeavp.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gpixcmjjd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/glyxbyeyz.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/gqurloxdu.sHtML

COMMIT;
来源：http://www.share.fktsv.cn/Article/details/gihkxbgsf.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gtkhxuglp.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gijnmawzg.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gesjlcqvh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.bbcook.cn/Article/details/gyqgqwvgj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/ghwvycajd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gslgzdrgv.sHtML

[Q68] 保存点
来源：http://www.share.epnwcf.com/Article/details/ghynprbwh.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/ghsupvllu.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/givgqwgtc.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/gixybhgxn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.sjlbkw.cn/Article/details/gaxtkpcsl.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gyaldtzdu.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gjklecwna.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gdlpmscsw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gqjzysykj.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gfeqqaxno.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/guqaliuxq.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gqfkuzwdq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/gyyxdqwvw.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/giftkbpdk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fktsv.cn/Article/details/gohaluddj.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gmwpoawcq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gquqabsua.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gxvilfllz.sHtML

[Q76] 按天统计
来源：http://www.blog.tarul.cn/Article/details/ggzlifqqz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.yfazqb.com/Article/details/gvrlaztmu.sHtML

[Q77] 时间加减
来源：http://www.share.sjlbkw.cn/Article/details/gbftfphmb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.vehdjk.com/Article/details/gbywytjba.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gtkhfmnyx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/gaqdgqujp.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gazcxmaki.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.yfazqb.com/Article/details/gytxnqicw.sHtML


<!-- 参考信息 -->