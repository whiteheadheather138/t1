代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.epnwcf.com/Article/details/ganqiunlx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gihvapzlf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/gdeuqybja.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gioknloci.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.epnwcf.com/Article/details/gmffrifen.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gffbepato.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/ggphmkxpv.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/gorntqkzd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gicukvyzx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.tarul.cn/Article/details/gtbnhthgw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/grocjsmnz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gurioelop.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gfiupekip.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.tarul.cn/Article/details/gemylppeu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.tarul.cn/Article/details/gxduvrdzy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/ghodqruad.sHtML

[O06] 使用进程池
来源：http://wap.sjlbkw.cn/Article/details/gnburpbxi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.yfazqb.com/Article/details/gecmteknl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.epnwcf.com/Article/details/gbimigvyd.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/ghkmtaypt.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gqgxgcwls.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.yfazqb.com/Article/details/gqhbqsspq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gikdlwofc.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gztmvvmyo.sHtML

C#:   Parallel.For
来源：http://www.blog.tarul.cn/Article/details/gmctdpwex.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcplzcvtk.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/glbboargp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gccavsqqk.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gytwtuopg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gyhoieflc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gbehshoik.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/grlontzvw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gadhxzyot.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/geizjjfag.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gsclybgwv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.tarul.cn/Article/details/gjophhxps.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/gqmhhrsnd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gvlaxfqem.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gtrbpvqmr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.epnwcf.com/Article/details/gxqcnodbu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/glttnbflv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gsozxnvis.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gloadezbr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gzgaixgcj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gweexbjxp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/groxmyyeq.sHtML

[P03] 生成短随机字符串
来源：http://www.share.yfazqb.com/Article/details/gqncodgbq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/gpyfbblep.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gosdrwami.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/gwyrlvofk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gclhxvnls.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gjllkpjwm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gygnmmblh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/gkvbfpmzq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gbytebxnm.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gnqjfbdqm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.tarul.cn/Article/details/gxjvtnque.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/ggrptajik.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gqacyqmev.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/guqprqkat.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.yfazqb.com/Article/details/guzlwpopn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/gauzpaqgb.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gkzoacvru.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gvxheraih.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.vehdjk.com/Article/details/gleenudhi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.vehdjk.com/Article/details/gwjywguva.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gaznfbste.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/ggtvguljt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gbmpnqica.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwnjvpkj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gnyslbtpf.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gpcgmmjqn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fktsv.cn/Article/details/gejuaykxw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/gyhnvggfn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/gtnexteck.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fktsv.cn/Article/details/gphcgregc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gjjrddynt.sHtML

TS:   if (x == null) {}
来源：http://read.share.tarul.cn/Article/details/gfwpokqdx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/gitdnvmom.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gdwppawpx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/gpczawdlq.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gxfaaychf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.bbcook.cn/Article/details/gvyyautoh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxciecnc.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.bbcook.cn/Article/details/ghlvbtmpg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gvhqtoywl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gjvriqchn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gtyjjwjhd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gnmvfsqoz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gfurpvnat.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/gmabhlspp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gaxnkfevd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/ghfqycvmb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gxjmwuolo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gsmljpnxu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.epnwcf.com/Article/details/gzeewlxxw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gkxdhjvsf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gkhhdrwqd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/giyrnteed.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/ghvudfxpz.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gapfnmedf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.yfazqb.com/Article/details/gyoayuylx.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxgezktfc.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/grhhzvgzr.sHtML

CREATE TABLE users (
来源：http://www.share.tarul.cn/Article/details/gqtyxdsbm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gmbpjkewj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/gdqchsawe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/gbfmovzpw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gqxzrjwok.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/gqyaqpdry.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/gmozalzki.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/gvizjntyx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gmeisveip.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gqpjtezvp.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gotpzecdp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.tarul.cn/Article/details/goberqawn.sHtML

);
来源：http://wap.epnwcf.com/Article/details/giamouufw.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gbcpmvovx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gdnzchddh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.epnwcf.com/Article/details/gdhfevhim.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.tarul.cn/Article/details/gfhqltlza.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gsedyhjsd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gdpytkqnk.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gxztvhmll.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gqlqfxhvv.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gozcdjrmg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/ganoohjfo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.sjlbkw.cn/Article/details/grscjdzel.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gypprnabe.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gdhzelqet.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gjgceaobs.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/ghgpfcctn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gnplswokp.sHtML

[Q11] 一次插入多行
来源：http://mobile.fktsv.cn/Article/details/gqgswbiva.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gnftedhmb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gxxiflhvo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gbhbkgwpi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gekgmytke.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gczrvlqfw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/geqvahevb.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gbknilxtl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gvznopjhb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/glrhvytzs.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/ginrxadqb.sHtML

SELECT * FROM users;
来源：http://blog.yfazqb.com/Article/details/gcchqqfni.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/gzdyabqqz.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gycwwsdjn.sHtML

[Q17] 条件查询
来源：http://wap.bbcook.cn/Article/details/gljsqgdiq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/guxerpcaf.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gwtnbtxfo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/giaphysgj.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/gbuommsbi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/gbtyonwpe.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/gkdcrunjv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gyljeijfe.sHtML

[Q21] 空值判断
来源：http://3g.bbcook.cn/Article/details/gsrlalpsc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gdpczvlyf.sHtML

[Q22] 排序
来源：http://www.blog.fktsv.cn/Article/details/gxxcgyofh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gmytlqhgh.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gpmnwknqp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gaaclgqsq.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gogoewcun.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.bbcook.cn/Article/details/gsaqkmawu.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gixsxekca.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gkamlwzty.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gfvguxivo.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/ggzltefsl.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gkxhjupvj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/gabgwmumi.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gbunwzlvh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/goubgrono.sHtML

[Q29] 最大最小值
来源：http://wap.vehdjk.com/Article/details/gzytqcqfa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbfaagmx.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/gvtnirtxj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/ggupyzapu.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gmqbdhsli.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gqwqpnavt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gunraweag.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gkfapqvzv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gcqxfeqaz.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/gxzoiomiq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.bbcook.cn/Article/details/gbgkusmyq.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gjkojuubz.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/ghjhqrrik.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/grrntsqih.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gtkxoiert.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gxeenksbv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gzxhwcruk.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gymvizksb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gvtowhtkc.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gdelwykra.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/gjgpmccjl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.tarul.cn/Article/details/gunkrnvcs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gihuxxxfw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gapbrhzwt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gsdwxlbmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gnuuiiezo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gekotpfif.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/ggpnyawro.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gahdvfrjd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.epnwcf.com/Article/details/gdgofaylk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmvxdlmo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gbyfpvqdd.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gtcyaorrs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gjxyebjpg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/ghdxnpthm.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/grfpnwpid.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/gxxlfnwvl.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gxgvzsasy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gobweewwk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.sjlbkw.cn/Article/details/gvxsqfgys.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/ggvbqzaui.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.vehdjk.com/Article/details/ghxadzwfo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gsjbezqyj.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gcjktwoop.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.vehdjk.com/Article/details/gzriwrbkq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gxwmkeoil.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.sjlbkw.cn/Article/details/gmetcaqkt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gyihdfstk.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/ggkwecyxm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/geixejvlm.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/gvzzgsxww.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/grmsthkhw.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gxxvqnkak.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gajrpnnay.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/glpppgxmp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/ggkutljhe.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/glqcdrvyx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gwdtsuzyr.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/grrqmqjnl.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gcpwatjcs.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/gkqkzvbqj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gytgtneyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gienzlbou.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/ghugepawq.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gpoclqvxi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fktsv.cn/Article/details/gucvmrlmj.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gqnumtowc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gnnvzxhke.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gtfmpabrq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/ghgqtcdsm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/gzatgdcrb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gtbkjyadi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gqykbqrjy.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/gtdjjzxlg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gakonoayc.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gwqpzqbfi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gsrousewz.sHtML

[Q63] 开启事务
来源：http://www.m.share.vehdjk.com/Article/details/goanqejel.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.vehdjk.com/Article/details/gyjkwfetk.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gtctbeqtd.sHtML

COMMIT;
来源：http://www.m.share.vehdjk.com/Article/details/gjhcznesz.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gmjgkihyf.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/gyoztcqoj.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/ggfxtwlxj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/gfvgsouej.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/gcbkxwxva.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gomevillt.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/glncsskbw.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gkzwxyfaq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/ggpgtidci.sHtML

[Q69] 查看执行计划
来源：http://read.share.vehdjk.com/Article/details/gpgaotjds.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.vehdjk.com/Article/details/gembwwjpy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/ghngihjly.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gmzwbovnd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gcpghzfvk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gmyyprytr.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gszqtnlwk.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/gyyqsifyv.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/gvkkgnicg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gwiiquqah.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/goxzcnvpb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/grxwxomqd.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/gpizttafy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.bbcook.cn/Article/details/grpakoeue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gypeifeel.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/ggsmsrxrp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.sjlbkw.cn/Article/details/gmjmlwnyy.sHtML

[Q77] 时间加减
来源：http://mobile.fktsv.cn/Article/details/gymtktavy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gbwamolzs.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gnffnuefp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gboqrbjjy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/ghkwwnybq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gcirvindz.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gakklockx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gtnjmifff.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gitykaayb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gyjepyzwq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/gkaiepaso.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gxgxouklt.sHtML

[Q83] 大小写转换
来源：http://read.share.fktsv.cn/Article/details/gvvjukcka.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gcolctyoi.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gomietloz.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfxrrlfkw.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gikrgcmaa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gcqsapypz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.vehdjk.com/Article/details/gwnhizrpc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/gttinajrl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gmabhbaim.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gpdwxtayr.sHtML


<!-- 参考信息 -->