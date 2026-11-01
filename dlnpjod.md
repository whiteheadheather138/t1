代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/gkofwbmmv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.epnwcf.com/Article/details/gvfenkued.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gusegtylc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gmpwzkpkv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gtnbxwfku.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.bbcook.cn/Article/details/gvnmqdpnk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/gcgbgfspj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwcfjybw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/gzjlfrohh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gxqkezrqn.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gsdiqznpj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gdmjafwxa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/gcdcuqrpr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gjkfbcmon.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gjnrregfx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gioxyhmbd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gzuafasif.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gwcfbzwtw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/grmzzvlvy.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/ggthtvoin.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gcqomvxdi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.bbcook.cn/Article/details/gdkgfnxwx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/glypbmigx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gnlftmxlw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/giopmbhhq.sHtML

Go:   len(arr);  len(m)
来源：http://wap.yfazqb.com/Article/details/gqdnmbpku.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/galfuumyf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gskduyibp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gjjsmwhpj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/gmioynpay.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/ggorlffeg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/gzrhcbtgm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.tarul.cn/Article/details/gcxoperwt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gjwxxgutx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gespavrcu.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gmahvdksd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/gzcwadopy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gjsbvtrvk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gsphleljc.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/gnqlxtbxu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/ggysnjiks.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gkyunencg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gfpbxgruw.sHtML

Go:   if x == nil {}
来源：http://read.share.vehdjk.com/Article/details/gnhyhkyxn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.bbcook.cn/Article/details/ggnyinzcu.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/gigfmcgcp.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gvcivhoxs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gyxrexgwz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gnqlvwjza.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gzmhhmkqj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gsjdrixwl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gztqcehbk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gdfjzyajl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.sjlbkw.cn/Article/details/gybhkbqlc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gxzitmtkv.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gmvwpygxb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/gmxwfiuet.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.tarul.cn/Article/details/grogtqyjh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/ggbtihlil.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gbqvryozs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gzpzzqmnx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/giobvfygc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/goetqmbmo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/ghqmuehmn.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjgfqzcyg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/gtdqfiynb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfxmmrbol.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gjiwvhlcw.sHtML

CREATE TABLE users (
来源：http://3g.epnwcf.com/Article/details/gwwntvtzm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gmmtfqnnz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gwugfobbr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fktsv.cn/Article/details/gacsqbrke.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/gvzpbkboh.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gokuzwsje.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/ginlylmfj.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gwysgonuy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/glaswqitf.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gzgkgvxje.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.sjlbkw.cn/Article/details/gglgopxyu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.sjlbkw.cn/Article/details/gzuyrhnrt.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/ghhakfzdn.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/gqkxpmmsx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gwlcaghcc.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gluvnygce.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/gsoiwxxml.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gwkkqevag.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gwllionwa.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/gornqycay.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.epnwcf.com/Article/details/ghjrgsbaq.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gtcupjphy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.yfazqb.com/Article/details/gaydxnyxp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gwrmickmu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gberuzlnv.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gpetcqacj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gqtycgbjs.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gjrxbsfby.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.tarul.cn/Article/details/gmamjknze.sHtML

[Q11] 一次插入多行
来源：http://wap.bbcook.cn/Article/details/giplqcstj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gikmikdrw.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/gkpqigvuc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/gxmaxjtjl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gddradtjv.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/gnayaswin.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/glngibptq.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gwcpdsorq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.sjlbkw.cn/Article/details/gblrpetna.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/gfxudmjzq.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/gddqhuvan.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/gwqwhhhjl.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/getajfzit.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gzfeapzyk.sHtML

[Q17] 条件查询
来源：http://baike.epnwcf.com/Article/details/gvijxgokj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/gmnlkhsnp.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/glnhstiiw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.bbcook.cn/Article/details/goygkhvup.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/ggxlcrbxk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gyrupwoyb.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gjukhooqs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/ghbhfygut.sHtML

[Q21] 空值判断
来源：http://3g.yfazqb.com/Article/details/gggwwjcur.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fktsv.cn/Article/details/gtgvgttug.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gbctikivq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gqlklfrtj.sHtML

[Q23] 分页
来源：http://m.share.bbcook.cn/Article/details/glsidejmj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/grqhvbjcd.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/grsxfvjiw.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gdaaeaglj.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/ggjwpsrmz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/givnbcvyb.sHtML

[Q26] 计数
来源：http://www.m.share.vehdjk.com/Article/details/ggsjxkstp.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.bbcook.cn/Article/details/gojqqhoxi.sHtML

[Q27] 条件计数
来源：http://baike.bbcook.cn/Article/details/gyybtzpvt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/gazecjlij.sHtML

[Q28] 求和与平均
来源：http://blog.vehdjk.com/Article/details/gkklwjtwj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gspqvpeyd.sHtML

[Q29] 最大最小值
来源：http://read.share.yfazqb.com/Article/details/grzwtbutk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gstbsynjh.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/ghlnoqvna.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gkkecrhaw.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gaqoeaixb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gkiflyrpr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/geguleufy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gutjcaffd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gmxdgvtby.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gkwvfvlde.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gqnyawikp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gtnpjyklq.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/gdlqtgbtr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gbjixoijd.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gziahlanr.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gocicfqrb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gifwlwpcz.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gguxlzkfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/glwsislkp.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/gtytpxdnl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gsdwuvrcd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/gvzrckoky.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/gdrddhgtc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gyakufaog.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/grgxxguwr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fktsv.cn/Article/details/gekpravcb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/ganfppapb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/gxsttakig.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gyvuwfmvy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gttgypuoa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/ggnccgjsb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gfjyadwrx.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/ggdstzjro.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/gfqnuxbin.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gwnpjkcqe.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gjtpogzhx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gpteiehxc.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/grdrpuyvv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gdyysphzk.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gioyuqeeg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gxbmabpza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/grshzhbux.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gviwtqjek.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/gecbhsnia.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gtxwsoqtr.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gfmqijrtd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gfdyuhzrs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gpdpfdfum.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gzencmqcp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/grkfykhho.sHtML

[Q50] 批量更新
来源：http://mobile.yfazqb.com/Article/details/gqidfdojb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gmwqnnccg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gjzhoesjs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/ggkkufsul.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gmpqvrqmo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gcfyswdyj.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gphgpcflm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.epnwcf.com/Article/details/gsrmpyfvz.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/ghabdjrqv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/grrmtsvgv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gyxvbvwfq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gmttuqybl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gnwwbfxrh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/ggeowtnay.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gnadfsgvv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/ghnjfssdv.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/giohtajzj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gbxypuhsj.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gvmuibgmv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gshtckvmo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gqzfpkhkr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/gkbgdvbrq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/grbgomcvm.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gnprxfmqv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gnbsetenb.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/ghoqaxesp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gdxqoykwa.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/goquaxggx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/gbnobdezi.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gdqgihxan.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gpthrlpux.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/gocfsbrju.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gbxdfzmjs.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gtptmzfag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.bbcook.cn/Article/details/gfaduhtar.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gfagiogld.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/gwvbqnnib.sHtML

[Q68] 保存点
来源：http://baike.vehdjk.com/Article/details/geptfhdyu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gwslxkeum.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/ghkreakjg.sHtML

[Q69] 查看执行计划
来源：http://www.blog.yfazqb.com/Article/details/gnrfdswka.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gjxphbeop.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gyswejyvr.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gojodmzvn.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gmvcqtflq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gqgkjrbxj.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/ganwwzkgm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjuwvqqys.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/ggsyftzyd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gjubkirzm.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gsldqjnnc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/gkmrwudei.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gxlbeiobn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gfuzuphaj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/glrdhzqwa.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gelfzzwkx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gwccdzosl.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gjnkpwwoe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gccihgpkx.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gnqdhrjqa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/giuqgblqg.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gkiydbiyb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gawzsqdps.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gdpdxwuvj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmxehnihu.sHtML

[Q81] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gkvdxuqhz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gtrpizscg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gaxbbqdfr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/grrrleqkp.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gkcybjskd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gvhxkfiyv.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gofxysqzm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gjlfytogk.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gfitxyhsj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/gqoibehlu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/giqqnnwtz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gycwuvbyz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gxfqpkjxq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gzhvbkqhu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gxzamwbgr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gvemokcsg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gomarrwal.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gskqfaeez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/geaprgmne.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/gjugsnmgz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gwyizrtud.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxexzflpn.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/ghcvfjiom.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdzqptxmm.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gtdravtpc.sHtML

#!/usr/bin/env bash
来源：http://read.share.vehdjk.com/Article/details/gkvwlzdhk.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gtojottye.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gcvylpjkc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/gowdycfoi.sHtML

[R03] 只读变量
来源：http://blog.bbcook.cn/Article/details/gngumheqw.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gefhrctpl.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/guerguttz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gottvgvcx.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/gzhybmfrk.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gaurfnxpd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gmyxgazof.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gxggjbfgz.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gcekqzjfa.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gzbboqkye.sHtML

[R08] 数值比较
来源：http://www.share.tarul.cn/Article/details/gbodqblsh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/geazqiegl.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gnqwkfjbw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/gcuiigtki.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/gmdoznquz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/gevgkbcjn.sHtML

[R11] case 多分支
来源：http://read.share.yfazqb.com/Article/details/gaoigbjqv.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/giscqirqf.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/ggcpxefzi.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gzutjsjnh.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gtuehgxop.sHtML


<!-- 参考信息 -->