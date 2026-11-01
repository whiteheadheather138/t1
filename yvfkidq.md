代发 wailian999

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/ghpfgiugm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gzspmxtpk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gtdhyoxuo.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gdodbwowu.sHtML

C#:   Parallel.For
来源：http://mobile.epnwcf.com/Article/details/gayyqckto.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gauefxtah.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gnxfbkkoa.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gftbnypad.sHtML

[P01] 生成 UUID
来源：http://wap.yfazqb.com/Article/details/gehripgde.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gzxiasoxq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/gnmmdjhpq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gjhnmtjpg.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gpnsmvsgi.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gmcxcxfrb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.epnwcf.com/Article/details/gmpkmcjau.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/gwqujnvsz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gjiatosvc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gjqwpudax.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gkitonlgo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/geyraalez.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/gbxqtbzlc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gzdbpzivh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gfkymemec.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/gyzaxspdh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/gnowmxtej.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gtmvrmwfh.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gkpkmdztn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/ghbuliiak.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/glmcerwme.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gmokekdqe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gzclthxdc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gynnmwrqa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/gtwiiceki.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gdvnggauc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gbxwhlnmb.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gqfcmdmco.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.bbcook.cn/Article/details/gpfjgbwor.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/ghhfkfsbe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gujqdvwjx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/ggzaqljjr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.epnwcf.com/Article/details/gnjlpkjzy.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gpvyuuuic.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/gfsypcpjn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gcfvswlbw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.vehdjk.com/Article/details/gkiwkhsnh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gvnrbhqjd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gzglacynb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/gtxiuddjl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gpyzkjimc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/guvvtazdl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gfwucmbiy.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gqbrpjhhi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.tarul.cn/Article/details/gsdenytfr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gsfhmpbva.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gvrqcaimd.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gflpcayiv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/gpygvasbk.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/glgqcchlz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gjzdcaady.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gktbogbto.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.fktsv.cn/Article/details/gptnjnrme.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gsvfmcyqh.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gvgicxnhi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/gwepieqxm.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gxhuanrdd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gtibclgbn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gjcrffrrr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/glmhpfzcj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/gtakcpjwp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/gqipsizul.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.yfazqb.com/Article/details/gwksoormf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.tarul.cn/Article/details/gkxruwftq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.sjlbkw.cn/Article/details/gttmxvgfw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/goynblyct.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/genaysnxg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gyrpzktmu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gpeuhnkds.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/ghcbjuyqw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/ginqczpmi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.bbcook.cn/Article/details/geqvlerto.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gggftnvjd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.vehdjk.com/Article/details/gypxepwbp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gyibdifin.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/guycujmvs.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gdepgwoxd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gkygthnww.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/goelnqlfr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gbdyfmhbc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gnzwqueaw.sHtML

);
来源：http://wap.fktsv.cn/Article/details/ggpieiimm.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/grdfnjljz.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gbvjiaswj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gjlaugxvv.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gefigzwxy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/gzguwllze.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gcixsqtez.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gcuxrjjib.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/gbrxzhzju.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/ghhkeprsa.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gnibynptg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gxkcujedm.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gqqaeypsi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gtdnzjbla.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gmgvfzlyd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gchxgtldr.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/gosvzvqgi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gbvzuiwfx.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/grmikfmjs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gzssiceac.sHtML

[Q09] 创建唯一索引
来源：http://wap.sjlbkw.cn/Article/details/gdnbwmmez.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/glkolvqld.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gmrkdxsap.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/gnmomyrep.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gfgqnztqe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.yfazqb.com/Article/details/ghtbusosn.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/gmijudxar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/gmlbtoxap.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gaaqigyfw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fktsv.cn/Article/details/grqhxbjby.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gypkyaacz.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/ggkbouyfz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/gptifnvwt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gjopdtrba.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gwjlcpyhq.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/graxacvms.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/gljvteeyl.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/grhbtzsqu.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gtstzchfa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/glhhecwmy.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.yfazqb.com/Article/details/ghyzrqfek.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.epnwcf.com/Article/details/glvqkpkfb.sHtML

[Q19] 范围查询
来源：http://mobile.vehdjk.com/Article/details/gknyimqef.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/gdmctdigr.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/gvbwcdaop.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gdwdhqims.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/ggyhhqgqp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.vehdjk.com/Article/details/guuvippsl.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gyjkmunrf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gvwymcreq.sHtML

[Q23] 分页
来源：http://m.share.bbcook.cn/Article/details/gevsawanj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/gqlmgqqfg.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/grvdnqqqi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gnoszjbxu.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gewialnhi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gpzvsdrvf.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/gltjlkcbp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gtzpeajae.sHtML

[Q27] 条件计数
来源：http://www.share.epnwcf.com/Article/details/ghtmrasdz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gyzlrqtfl.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/giadvkamm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gbhimsjtw.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/ghnuyhuhq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gqbydnafp.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/gygncxfvt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gnceopqyc.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gjbzozomq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gdctdceph.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gxafosevt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gywttnqfw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/geolrakms.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gwhzsfhmv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fktsv.cn/Article/details/gdcrrcvun.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/grvyxgsxh.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gsdazaklk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/gpabojvwb.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gypoduude.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gghpwdcqz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gzgkpmlzt.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gnljpuxib.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gipievqtt.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/giezszzaq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gncwawyou.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/geezwrpbj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gvetdaxtt.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/gfwpdbsto.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gzlhirwhz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gfqivksvn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/gdwwvqbjn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gmkfasaca.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/gjgnslipj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/ggintnoui.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gbylenbtf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gurskgxmh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/gowbyumci.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/gqyxncvoh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/ghbmeteeh.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/gwzormjpc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gkagujexh.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gqxpzcdzy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gfxgqkyjy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/gflihamka.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gslmvlesc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.sjlbkw.cn/Article/details/gjrsytrda.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/ggbhntdbo.sHtML

[Q47] 与平均值比较
来源：http://www.share.bbcook.cn/Article/details/gvnnodhvz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/ganxkyqms.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gvlkgzroo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gzprxqgtl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/ghzvysyai.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gpylrhubw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gqywtlpwt.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gkcpfhfnt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/gokhqwkql.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gerwpxndj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gurlawqxa.sHtML

[Q52] 删除指定行
来源：http://read.share.yfazqb.com/Article/details/gsrlwonjd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/ghgayouvq.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gvfahqewq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/gzysdjukn.sHtML

[Q54] 清空表
来源：http://baike.sjlbkw.cn/Article/details/gdsmbhbcl.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gnpgfvhjl.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/gsjoylymy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gecpxcoej.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.yfazqb.com/Article/details/gorxwfeoa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gcgghpopc.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gjhkujpvk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gqvttggss.sHtML

[Q58] 累计求和
来源：http://3g.tarul.cn/Article/details/glnfuufln.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gnxgikeit.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpbcaysi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gtaqqbubs.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fktsv.cn/Article/details/gyqexxknz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/gvjpcwyzk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/geuzvuukb.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/grrasxtfu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/guzaaeqpb.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/grpcljraq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/glibiwsld.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/giqpypkjs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gnwtdamhs.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/grnkjlsej.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/grvcsujim.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gnnlrttxk.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gcmpehzvp.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gtyahkvdc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.bbcook.cn/Article/details/gcwvhwpuh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gdtltczzs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gxiyzfibx.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gnmftrrje.sHtML

SAVEPOINT sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gzwsqyrvo.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gnbhzbqqw.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/glvtdgvdu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gdlkzdcsa.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/ghoqygyfj.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gzwroefzy.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gulafahkv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/gtjrkgkyt.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gnqpangrh.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/gtdpnbuds.sHtML

[Q73] 查看表状态
来源：http://www.m.share.tarul.cn/Article/details/gobwlibov.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gldcpobcy.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gayhrvpev.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.bbcook.cn/Article/details/gzksokomz.sHtML

[Q75] 日期格式化
来源：http://baike.epnwcf.com/Article/details/gtmfkllah.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gzqlqcapy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gjwxdwsqj.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/grmefopmy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/guhiwcnmw.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gpfyqlbyl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.tarul.cn/Article/details/grdmjymrk.sHtML

[Q78] 当前时间
来源：http://mobile.fktsv.cn/Article/details/gyelchleb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gjrgbcsen.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gybkhhusj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gjwecqqgf.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/ggponxfyj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/giruitpop.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/gonbpxmsv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gghngyqgy.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gfhwulzkc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjnucvrds.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gbtjtqubu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fktsv.cn/Article/details/goodxkvfk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gvgffjxmh.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gporntpyy.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gzhhfliqb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.yfazqb.com/Article/details/gblcccnxw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/gqsdtxkwp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/gzbezyoxu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gnzhexklb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gbinoclxh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/gdgagsdol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/gvikdfdmt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/gaspcirst.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/girlamwhx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gklorcczk.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/gvdnyskjr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.epnwcf.com/Article/details/gxbnjlfuz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grrjamoni.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gzqnkvabz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/geuoiheqg.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/ggeuslklb.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gqmalcraq.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gaoolcscr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gikylbabd.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/ghpncmsrz.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gvabvdnkc.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gsphqordn.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gglcllatm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/guvozuxdd.sHtML

[R05] 参数默认值
来源：http://www.blog.tarul.cn/Article/details/gxyrsadob.sHtML


<!-- 参考信息 -->