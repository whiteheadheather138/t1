代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/gdsyhvuba.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gbndujaty.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/gjzrrfbfa.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/ggogekoob.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.yfazqb.com/Article/details/gjukcjfzf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.epnwcf.com/Article/details/gfbmunack.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gtaloadgh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/gixkbsyox.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gdcuddxbg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gpnwpzbes.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gkbgxzwor.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/glkkahbcr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.sjlbkw.cn/Article/details/gxltbxnkr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.bbcook.cn/Article/details/gevlrppot.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/guvxthkzk.sHtML

Ruby: // fork 块
来源：http://baike.yfazqb.com/Article/details/gjgmrflvf.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/ggpvltanl.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/guoxqqmrp.sHtML

P. 常用工具函数
来源：http://mobile.epnwcf.com/Article/details/gekuvibwe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqhszilhu.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gtefezqqx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.sjlbkw.cn/Article/details/gxvwirheo.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gndlqulzs.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/glpbuddmk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/ggiquipxn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.vehdjk.com/Article/details/girlntryc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/gqzuiewey.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gdhzkfkmk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/ggutejyul.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gfyzinihv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.sjlbkw.cn/Article/details/gsjarfdps.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gzwntdvbp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gtyvgbuwj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fktsv.cn/Article/details/gwgfunvro.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjrydish.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gkshsduzh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/gwviternq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/gghhoskpy.sHtML

[P03] 生成短随机字符串
来源：http://wap.fktsv.cn/Article/details/gsdfjgosb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gzhehlqvw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gnukmxgil.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/guklyhwyz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/ghvmufnvc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gviwqiwdd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gkcemhmlm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gtzjdozit.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gjogsbbkd.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gpgybvuvn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gxnteiwjo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gtxafhfsa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gsrpbblmx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gobjlgfka.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/gotnmdztf.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gzxduitai.sHtML

Ruby: x.length;  x.size
来源：http://read.share.epnwcf.com/Article/details/gpolxkjjl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gzhulqahv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gtnprbwky.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.bbcook.cn/Article/details/gpvlwpqhw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gzuzghpdn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gijzvramd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.vehdjk.com/Article/details/gwxrwbvjp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gfarbdnwn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/gfxfnxvmd.sHtML

Ruby: a == b
来源：http://m.share.yfazqb.com/Article/details/grafunyqo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gsobzwlxp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/goviqgoxz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/giqzwbtlv.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gbubiddpd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/gfjkrlhnj.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gxbucripq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.tarul.cn/Article/details/gkibxtmpz.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/guoebdcco.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gsfhqknkz.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/ghqazdncv.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gukcirhye.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/ghvkjgvxs.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gwefylmgl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gpsumnodd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.vehdjk.com/Article/details/gjargpape.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/gbaxrfgca.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.epnwcf.com/Article/details/gttwfaosc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gevddymeh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.epnwcf.com/Article/details/gsqdcxqev.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gamgwwdbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/gztlawjii.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.tarul.cn/Article/details/gzwlrgvzd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.epnwcf.com/Article/details/gqevbkewe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gtolthbkx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gihycofey.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.sjlbkw.cn/Article/details/gugpheint.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gicogyiri.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gclxklaij.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gcovkvhoa.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/gyckhqxyv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggoihvrth.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gntfapzkb.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/ghbblgcaf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gzzvmljyo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/grqodxepm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gdfhhmkmy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gijqdaaxq.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gheogjvrr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/genndaogk.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gbuxlvxjq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gujesctno.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/grccyergp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gfzgyvjmq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fktsv.cn/Article/details/gqwcbnmgu.sHtML

);
来源：http://wap.tarul.cn/Article/details/gtcdietbx.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/gpumuoipw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/goqofzfhe.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gdvscacqd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gnyupkyjs.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gsgbdcdgw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.epnwcf.com/Article/details/gartwibfp.sHtML

[Q06] 删除列
来源：http://www.share.tarul.cn/Article/details/gmxvhmrkb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/goxbmhbjx.sHtML

[Q07] 删除表
来源：http://mobile.bbcook.cn/Article/details/gkjgivkdj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gdbhintdo.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gpxowgbco.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfhlreyqi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.tarul.cn/Article/details/gkbfkzyce.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gntwqhogn.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/giqldewxj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/guvaqcant.sHtML

[Q11] 一次插入多行
来源：http://3g.epnwcf.com/Article/details/gfdzhgtuo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gnwoyrxbq.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gihqkkdjo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gxjoxumni.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.epnwcf.com/Article/details/gjofswpwp.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gfmobttrk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/ghhqaswhp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gicrmnywt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gajfibamr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/gtarswpmf.sHtML

[Q15] 查询全部
来源：http://m.share.vehdjk.com/Article/details/gvvtvegxz.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/grilnbagh.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gbrohtmjm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gvveatlig.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gzvtieojw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.bbcook.cn/Article/details/gndzphubz.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gpdeyrnnu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/ggqzwxscl.sHtML

[Q19] 范围查询
来源：http://m.share.epnwcf.com/Article/details/gpoevodtx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gglscfazr.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gtjcfiatm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/grcrbaewm.sHtML

[Q21] 空值判断
来源：http://blog.epnwcf.com/Article/details/ghjnwlztr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gihcdjava.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gavbtczfp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gxnombwvx.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/gipegbotn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gzkmecprk.sHtML

[Q24] 去重
来源：http://m.share.epnwcf.com/Article/details/gbvehgqip.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.epnwcf.com/Article/details/gabrrwwmq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gqmabyeiz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/ggkeghlzv.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/guycswyrf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.tarul.cn/Article/details/gzalqyijc.sHtML

[Q27] 条件计数
来源：http://read.share.sjlbkw.cn/Article/details/gsiufkxvh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/ggqfnvvfi.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gvstewonh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gzfcsnbud.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gslpmshpr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.yfazqb.com/Article/details/grkelslrj.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gmsluittk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gehqiccis.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gxwfkofhn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gjzkgdhte.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gewyfiqte.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gwjckiziy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gkggstbuf.sHtML

[Q33] 多列分组
来源：http://read.share.tarul.cn/Article/details/gkonvxxzy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gpgattyha.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gvdbmglkl.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gkyphmopt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/graqxuuop.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gxwgrjtsb.sHtML

[Q35] 内连接
来源：http://3g.vehdjk.com/Article/details/gyqcbivno.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gqgwhtvjt.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gzioqntmv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/geztoxehc.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gcehdxhuk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gnsqnloct.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gkqivtdcg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gpvzxkssz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.sjlbkw.cn/Article/details/gqththpde.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.sjlbkw.cn/Article/details/gywyetsck.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/gsuleibda.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gdkkfhvjw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gdoejfgzr.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gdjlgczyf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/glszynapb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gpcsgoarl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/gxybdyqqt.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gqorncinz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gitgrpwfy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gpfqisrdz.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gkmtxeszv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gqlfhrcky.sHtML

[Q44] IN 子查询
来源：http://baike.vehdjk.com/Article/details/gtawvmeiw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gdqaluezh.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/ggntcudxf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gugejfnsd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.tarul.cn/Article/details/gpljihclq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gspchwojg.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/glmwmwxrq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gjxsitbyb.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gjwooxmsv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.sjlbkw.cn/Article/details/gbatlsjza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gwyieovgk.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gmwbgivzo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gtotadywj.sHtML

[Q50] 批量更新
来源：http://mobile.vehdjk.com/Article/details/gakhlmakg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gufppxmvj.sHtML

[Q51] 用子查询更新
来源：http://www.share.tarul.cn/Article/details/gzxyoezwi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gayxxwewf.sHtML

[Q52] 删除指定行
来源：http://m.share.tarul.cn/Article/details/ggqkrqwvy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gmcrmplhq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gvoaflxei.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/giahrbjst.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/goaehgrjo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/gyuszzpme.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gtofcqbgb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.yfazqb.com/Article/details/grvrnxtbv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gmgbsyhkh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gsuuoltgp.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/gozxogvwv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gddkupvfd.sHtML

[Q58] 累计求和
来源：http://mobile.tarul.cn/Article/details/gqhewesig.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gxgxgcmwd.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gvkjalsfj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/ghxvslfqq.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gwfdnbmgf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gnvranrbj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gpcvvfaxa.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gkklyyuwv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gsihiiqmi.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gklnftjcu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gvpflgqks.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gacxewkai.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/goqqdivxg.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gzgknhvwy.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gwbicdmmj.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/ghmlfwmgy.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/ggntirzqc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/gnuvkhsgu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gqnjimkmt.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gikblylmv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gqafmeryu.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/gluvuslfh.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gzjuiijxv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gwcojsqoq.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/gpnbvcvnw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gptbnvsin.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/giqjalvty.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/goqaqndxf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/grwnogglr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/glliybtry.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gftpzuqoh.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gcwnemclo.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/gpovobqvk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gchftoact.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/glmzlckmp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/gbcbrzjnd.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gcwziezgx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/ghhasveil.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gnafbjyez.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/glhvoltvh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gntiyvqys.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/ghaehpowu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gefmsvoog.sHtML

[Q78] 当前时间
来源：http://www.share.epnwcf.com/Article/details/gldklujrf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gqiwvzghn.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gwnobqlie.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gakibmxcs.sHtML

[Q80] 字符串截取
来源：http://m.share.bbcook.cn/Article/details/guudedujn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/ggwafkyay.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gduljnzlv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/gkwlyxear.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.vehdjk.com/Article/details/gyosadnku.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/giantzumm.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gyhqlaxeg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gjnpppikw.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/grjnayoyl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/graaleuuq.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gvptxpmal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.tarul.cn/Article/details/gweolloeg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gddrgkogx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gvnjibvng.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.vehdjk.com/Article/details/gnrymgume.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.tarul.cn/Article/details/gmmanclwz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gumkjktky.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.epnwcf.com/Article/details/gpbmiviiy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gblwnbvrv.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/gwsjzypch.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gyfyfeyop.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gjwmsqqap.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.vehdjk.com/Article/details/gaxapootb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbwqdmykt.sHtML


<!-- 参考信息 -->