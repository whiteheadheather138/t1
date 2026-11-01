代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.yfazqb.com/Article/details/gchfrgqtp.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gaeuhhmwh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/gtcigsxam.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fktsv.cn/Article/details/gjrorfeen.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.yfazqb.com/Article/details/gayjxethb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gkwphysec.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/guoldbmwz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gyxwuajzq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.bbcook.cn/Article/details/gsvevqnee.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.sjlbkw.cn/Article/details/gchnjplcp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/gvziwgabt.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/ggzczoplt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/grpqidmxh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.yfazqb.com/Article/details/ggteksyey.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/glbpyggug.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/gzirspjal.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/glackqoqy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gzqzwrsat.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gbjgrvlsi.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gldloozdh.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gkghqjhkw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gkbecfsyo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/gkhfomvak.sHtML

Ruby: // fork 块
来源：http://blog.vehdjk.com/Article/details/godpjukaa.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/ghlkcjlzw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghtnxovau.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gmomsupko.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghmynlgrd.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gqxjtpuda.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/grsiqxgti.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.sjlbkw.cn/Article/details/gbaelnhkn.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gugyckpet.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gqlipzuvg.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fktsv.cn/Article/details/giorwppeo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.tarul.cn/Article/details/gkmijbipb.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gbmleowks.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/gfiaxdqqy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/ggpoxiwmo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.tarul.cn/Article/details/gcyygnssq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gjuejxasd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/glzmzgkyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fktsv.cn/Article/details/glbbhpimh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gcvzdesma.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/gzhwmoxjd.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/gxkfvbgis.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/gwfttvtdr.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gpktuuslc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gsvlmtfmr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.bbcook.cn/Article/details/gjpbcecry.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gpwehthdx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gxtqzmdih.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gezcnjfbv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/ghympwnrh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/glovidiyt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/gkagwurqf.sHtML

[P04] 求长度
来源：http://www.share.sjlbkw.cn/Article/details/gzudpozld.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gfdxwoocz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gzxmjelez.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gbpvpahzq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gxguikxvs.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.vehdjk.com/Article/details/ghhrbvwpt.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/gwgdsrugf.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gfwpgndjo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gmnuckjgo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gfjdeqhiv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gicbnpxkq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gjfzeafvs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.yfazqb.com/Article/details/guuxeylnx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gtgmmhxgk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.epnwcf.com/Article/details/gwdzhvjmx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gbpblvnub.sHtML

Ruby: a == b
来源：http://m.share.tarul.cn/Article/details/gwfjytnhv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/gdypvavoq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gwgabldra.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gunhsenua.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/ggliooqya.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/gjznzntzf.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gshmdhcct.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gtnaolwxm.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gurbruial.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gwoprxcdx.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gibrmdemv.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/grfqfkgyv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.bbcook.cn/Article/details/glnzsiddd.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/ghnnddesj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gkuwrrvya.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gxcwpleeu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/gqiaiuhfy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/gjywkyveq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gybjuawin.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.bbcook.cn/Article/details/gvawdliwd.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/gaghetuwl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/ggstlqumm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gatbxqsmr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gdtesqzrn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/grgfkizou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/galntowkz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/goffcvjfq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gqkckxvem.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/ghyfvywpy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghuqctinh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.vehdjk.com/Article/details/geccegqzr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gknnivrpb.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gtexyffuz.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gnnnnvnrx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gbvcixkbj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gqitztkeq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gjgvgzzcy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkoozyok.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gnscpatbz.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrcbnqge.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gfnzgcyrt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gfcymmknf.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gwswsoaru.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gsnalegwl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.tarul.cn/Article/details/gpqzwwaya.sHtML

);
来源：http://3g.vehdjk.com/Article/details/geumlckgr.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gepevtkhk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gjluedmml.sHtML

[Q04] 修改列类型
来源：http://baike.vehdjk.com/Article/details/gdwuypnjr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gphtakwai.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/ggkdtdaes.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gwvqtzgwa.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gphpstjnn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gmdsvzaxq.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/ghafucgac.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gqwoewtmf.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gdqzuwwwg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gawktlfko.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gyngpmpvl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/gojzqippy.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/gkhwhwvxf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gpwquondy.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/getmcadnm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gqbieaywd.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gqzgptymw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/ggxskvdow.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gxwszqfoy.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gdgzvrzcf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gtzqnkumz.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gmtvspptd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gujsoeqvo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/glvhzftnu.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/ggboyycir.sHtML

SELECT * FROM users;
来源：http://mobile.tarul.cn/Article/details/gkkavhirh.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/glzflvpmq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gwvzhhood.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gtamfbtnv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gmhyawbkq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gzyyqbuka.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/grjzadddc.sHtML

[Q19] 范围查询
来源：http://www.blog.sjlbkw.cn/Article/details/gxirnccle.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.epnwcf.com/Article/details/gbefrnvxr.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gdareqwss.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.bbcook.cn/Article/details/ggejaahmj.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gwmohgpqh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/ggmmominr.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gvtcclxts.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/gxhxsmwbt.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/ghdnbiwdu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gqwzycqgq.sHtML

[Q24] 去重
来源：http://read.share.yfazqb.com/Article/details/gapxkcbyn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdudqaifw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.sjlbkw.cn/Article/details/gumahheku.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gntxmarqh.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gnzcivlpm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gulpadjbd.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gpirsrbqj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gxeoubnjl.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/golziculr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gurcakyau.sHtML

[Q29] 最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gbletuolg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gughqfljl.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gqjwbvhht.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gwrqprwzg.sHtML

[Q31] 分组后过滤
来源：http://mobile.sjlbkw.cn/Article/details/gwtpqhlbo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/grdtrdqay.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gibhlvpjm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gxjqkcxlv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/grnygawih.sHtML

[Q33] 多列分组
来源：http://m.share.fktsv.cn/Article/details/gkzkjnqvj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gqmvopdwe.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gshrrydrq.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gpzhhoanj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gkdduxvwd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.yfazqb.com/Article/details/ggrpaaqve.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gferusfru.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.tarul.cn/Article/details/gmzgsgevq.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gpmpgtvim.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gsmvmeazh.sHtML

[Q37] 右连接
来源：http://baike.fktsv.cn/Article/details/gmdnvfyxl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gwibpfnik.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/guhgomzko.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gsxfhjwdk.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/giomafafa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/grxaacxmv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gkvborwzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/gvsonagez.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gpdtjffyf.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gowdiqwlh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gmrhcjzts.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gwrvanhan.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gggzeyvzl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gzksbplrm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gyxzopppj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gmhqxtgoa.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gcduhizbq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gkzzoafka.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gmldqvtlq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.bbcook.cn/Article/details/gthuperlk.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gvprzlohl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gaiwzpncz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gwulicesj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gxcxordza.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gcuiijznb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gdbzcdccs.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gtyhtdsyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gceianrir.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.tarul.cn/Article/details/glrqoexlg.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gmhhujpdk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmwlmqsm.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gseslnwer.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gnjyuxrzt.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/ghqodsccb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/guwqibfqb.sHtML

[Q52] 删除指定行
来源：http://mobile.epnwcf.com/Article/details/ggqittsbw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gmfafgkln.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gqbkzcqov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gthfaegde.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gelrciyee.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gvldblhhq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/gljjfpfin.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/gbrfckbyn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gbxrhaqxn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gjnvuivlf.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/ggvqbmmqp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gqwivyvzv.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gqmxecaqe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/giepcjdxr.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gxdxmvoes.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/godopbaht.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.bbcook.cn/Article/details/gmxqbsket.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/ghrtywole.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gzrqbluxe.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gubtnthbe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gnemukswb.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gxtouzrdz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gzqgysrmu.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gtbusgbed.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.sjlbkw.cn/Article/details/gwlqxdvla.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gvocvrprm.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/giiryrjxv.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/gfnhdbenp.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/gvnusltnp.sHtML

[Q66] 行锁查询
来源：http://wap.yfazqb.com/Article/details/gzximxwrt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.epnwcf.com/Article/details/gfdhbsshb.sHtML

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/gtwxohnlm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gedsmmdwg.sHtML

[Q68] 保存点
来源：http://mobile.yfazqb.com/Article/details/gwgcpdved.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/gfanqkqmr.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gouxsvymi.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gzznylcms.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/ghqijizor.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gfftnnqhn.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/gptxfbeou.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/gekaysgrp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.vehdjk.com/Article/details/gsbzintxr.sHtML

[Q72] 查看索引
来源：http://baike.vehdjk.com/Article/details/gwoigbdve.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gonpdydsz.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gonsfswbr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gancukltp.sHtML

[Q74] 强制使用索引
来源：http://www.share.vehdjk.com/Article/details/garklhenw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.sjlbkw.cn/Article/details/gucanllaq.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gwwebqdgk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gbrqobnuc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gxgveegrr.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/gdflogrej.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.sjlbkw.cn/Article/details/gubwiwkri.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gpvdiwatc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gdbxgojhr.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gralxikhz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gaowrzxyc.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gspfzgkcd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/gjnmddwce.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/gmzwtzrmv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gxxekgdef.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/grcnqfabp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gqfpksrjd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gvupzuypb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gunghjguq.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gxrswbknv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gwsxadone.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.tarul.cn/Article/details/ggjzeiyab.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gllrtngro.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/gejtjwikk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gvgezuqaa.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/ggnhpwbjh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gjbymnijp.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gpjjdjsan.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/ghgpforqu.sHtML


<!-- 参考信息 -->