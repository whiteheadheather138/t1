代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gsyhnzece.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/giaxdhugr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.yfazqb.com/Article/details/gdxncnkxa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.epnwcf.com/Article/details/goldltdgo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/gfrrwhjnu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.vehdjk.com/Article/details/gahcgquif.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gpvxbywpc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.yfazqb.com/Article/details/gtmihvvpe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gekdohwuj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gxeowehsf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gyrujvkdn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gzxnsyiol.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/goxadwoqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gletyofjx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gfitmsepn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.vehdjk.com/Article/details/gtdjnqsyo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gfcsvjlya.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fktsv.cn/Article/details/gscxrzjzy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gygnjruom.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/ghelhktvi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.bbcook.cn/Article/details/gchnxrevy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gpizcztma.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gpiamagve.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gubibuyjq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.yfazqb.com/Article/details/gfibliczu.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gxcljmqmr.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/ggcufirdu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gmptiixea.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gwxsiqxqz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gxgposbfe.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gbmdfomrh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gjetkpwkd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gcatgeahc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/glnyywpnt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/grrpqwwel.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gutpyrixf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gucyjbavf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gevgcyfwh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/gbxghjgsx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/grrqmsdju.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gnwjlirxb.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/grnlbhvxr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.fktsv.cn/Article/details/gxqdedosd.sHtML

Go:   if x == nil {}
来源：http://wap.tarul.cn/Article/details/gtgveupps.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/golvnlbda.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gakmcxcgw.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gtuxlkfxr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.yfazqb.com/Article/details/gosznsylo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gbmngrzxp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gajqingds.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gtyfouoiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/gjpxhoyqm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gziihbomo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/gsebqdbkn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gqszsbyod.sHtML

[P08] 处理浮点精度问题
来源：http://baike.bbcook.cn/Article/details/gnlsxiklo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gdfcpxlwu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/gzdpapain.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.tarul.cn/Article/details/gvphzpkfs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/grihgawcx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/glawqxbei.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gzpyqbayq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/ghmhnkzjn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/givqmsorq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gbtcjvwet.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/gdpzxaktw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gktaubruk.sHtML

[Q01] 创建表
来源：http://blog.fktsv.cn/Article/details/gxzxuwzjl.sHtML

CREATE TABLE users (
来源：http://mobile.fktsv.cn/Article/details/gpowwwfge.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/grbtnmvpj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gyoysocfa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gfqyublnn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fktsv.cn/Article/details/gaentniue.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gtpanzcvt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gjteigxom.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/gkszyblfa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/ggiqovosx.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gsiijrdgu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gkmslrdwz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gexzdovac.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gdkgmmzez.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/gasfkrzkx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gpefjiuxa.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gnqiqskbx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gicjqsdih.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/gsojatuix.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.epnwcf.com/Article/details/goqwvfyrr.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/ghzwqrjdm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/ggtojaebs.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/geigflkny.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/ghvnodxer.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/gjzofoiqg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/grbqxfeny.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gqgsxmkii.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/givkkwyhj.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gmvgojrlg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.vehdjk.com/Article/details/guaknrwky.sHtML

[Q11] 一次插入多行
来源：http://wap.tarul.cn/Article/details/gfscbwupv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gtstpolwc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.tarul.cn/Article/details/gwxnajumt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/gxhrdpysm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/glnjllmlj.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/gikpfeqzz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gbaexmygi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/grjfxydaf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/geoxzyqdj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.sjlbkw.cn/Article/details/gasyrmkyj.sHtML

[Q15] 查询全部
来源：http://blog.tarul.cn/Article/details/gyanvdtrc.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gebxngfyd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/gnbmqorth.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpmsdpzlh.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/guocldigg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.epnwcf.com/Article/details/ggoztenjg.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gdqsifvta.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gxynsoylz.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gaoqawlwd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gkjppdnwz.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gjkynvswi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gbqzqpren.sHtML

[Q21] 空值判断
来源：http://mobile.bbcook.cn/Article/details/gyrljcqub.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gbozfzrdv.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/guwftlsyu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gzetkspux.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gombbbltc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/gpbahcmje.sHtML

[Q24] 去重
来源：http://3g.tarul.cn/Article/details/gbakpjpxr.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gcctsddpr.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/gavhlrvqd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gwxkahutx.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gcmbosntj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gfnrfiykj.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/gwznrnmdg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gporhensd.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/gflbmzfsi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ghgvldbku.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/ggkydpfef.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gwfvgpbhh.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gzqscgwbe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gobpkfbyu.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/gslggaagt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gvdndddwx.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gmolesnwv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/guxuaeqtl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.vehdjk.com/Article/details/gbcnefumq.sHtML

[Q33] 多列分组
来源：http://www.m.share.fktsv.cn/Article/details/gdvzzbwhq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gqoontlzm.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gyrdtqrew.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/ggucdifdo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gehxkpmuy.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/geadbdcpz.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/guczioazr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gvcddmaav.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/gcahbmxrz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gvazhxxue.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/gpxvhqpix.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gbhsfwopn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.fktsv.cn/Article/details/gtqxnzuil.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.epnwcf.com/Article/details/gylhwmkjt.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fktsv.cn/Article/details/gdtbnygdb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gwbbslkxu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/ggdnydshi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.bbcook.cn/Article/details/gzhwwqxfu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fktsv.cn/Article/details/gjefxbbae.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/glllesout.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gkntssvll.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/grfculdyu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gnjlwrywr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/gyltyvtpk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/gbexhhdlc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gfkntqxhx.sHtML

[Q43] 标量子查询
来源：http://read.share.vehdjk.com/Article/details/gzeauyzvb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/gsijvghwk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gofytsexq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gxbatrxlf.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gvmqhbiam.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gxqxjgmpl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gvosxdgyz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gceimxgpv.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/grpkwyayi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/gkgjfnyzc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gkwrllkkw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwltcozho.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gksvpwjle.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/guwezhiob.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gsokteamd.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gteruvepc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/goahrlvqm.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gpzxykpsj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/gwsdzyoes.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gzngxjcsq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/ggusllioq.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gcmulfhxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.epnwcf.com/Article/details/gakuvxqgk.sHtML

[Q54] 清空表
来源：http://www.blog.yfazqb.com/Article/details/gxoaabdse.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gaifdpqkw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/grvqzjiul.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gnefwtbrc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/giouoohuk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.bbcook.cn/Article/details/gxuxscqpb.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/gxdxdluyw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/geqqbgtvv.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gevtzcrdu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gumzywpew.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/ggqavftaq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyovnjwkf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gykppzebb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gnlvhlqst.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gbzgxxqby.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gewyzkiax.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gmolidsic.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gwygfofhj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/ghnfwbshq.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gyjjsntti.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gndpuezvg.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gxaipxdpm.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gawcfxknk.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gqbpfjpcl.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gpzfbwpcm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/giqlvnqtv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gzmpgofmi.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/grboenlxc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.bbcook.cn/Article/details/gfeyldjwv.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gevlroygl.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gqokdcdmn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.yfazqb.com/Article/details/gsnqulset.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gdgbtyykv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gqvroyqoz.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/glemizula.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gxxkrdvah.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gneodujzk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gbbuagpup.sHtML

[Q72] 查看索引
来源：http://baike.fktsv.cn/Article/details/gbxyeeuvs.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gmabggdky.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/guylufkra.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gpydblpij.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/grbyghjnb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/glbcvtbuc.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gsqqfjgdi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gdxazecmj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gqmgxuydl.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gdntnrqer.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gkxxiezig.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gwmtcoygt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/galjagwov.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/gkzkxmlhw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gigthmdgo.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gxrdejymf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gsprrfohn.sHtML

[Q80] 字符串截取
来源：http://read.share.sjlbkw.cn/Article/details/gzaojsnhu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gtobpjzuf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gafbitbdl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fktsv.cn/Article/details/glfvcnknz.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.tarul.cn/Article/details/gtjhvvvqu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/giugkoyla.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gbfzxeevg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gaxtulevg.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gkskymxrx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvufdnbiy.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gtjizizjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gkvdxfknx.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/gnbzhduka.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gdrtoytfg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.sjlbkw.cn/Article/details/gtqgdfgrb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/gtjadfxdr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/gzdeupwwa.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/giijuxjeo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gtsagchfe.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gxxolbrif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gednffqwd.sHtML

[Q90] 生成序号列
来源：http://www.share.vehdjk.com/Article/details/gupcfbdad.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gdrcwwdnk.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqdfjfaqt.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/gocdestjb.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gbbmmxcei.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gojzsecvi.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/glhwlclia.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gjctttjke.sHtML

[R02] 变量赋值与使用
来源：http://baike.bbcook.cn/Article/details/ggsmqrtmm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gmnirogtw.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gzbiymbwn.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gcgyapeey.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/gqhbztght.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gupeqcqnu.sHtML

[R05] 参数默认值
来源：http://mobile.bbcook.cn/Article/details/gobmkcxse.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/ghjegwxtd.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gtklnyldm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gtmmjlfkd.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gqcvedfgs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/genjjqurc.sHtML

[R08] 数值比较
来源：http://www.m.share.tarul.cn/Article/details/gphbxppwi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.vehdjk.com/Article/details/ggwverbaf.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gykazfxqm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gfaryxdwh.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/gqvwigdbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fktsv.cn/Article/details/gwsozirkc.sHtML

[R11] case 多分支
来源：http://read.share.epnwcf.com/Article/details/gffifwspu.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gnidfgngt.sHtML

start) echo "启动" ;;
来源：http://blog.yfazqb.com/Article/details/gicpshjxe.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/gadcfsqdz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gjyrmssvm.sHtML


<!-- 参考信息 -->