代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gktttpfko.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/gdyjfulwu.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gsjhcuhrm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/gpdiwjlll.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/griecayxa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gxnkcegzs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/ginsqdqqa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gizkotpxo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.tarul.cn/Article/details/gfozgfhwa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/gptjvejto.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/guvzelxjx.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gthzogbis.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gsftswkil.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.epnwcf.com/Article/details/gftxrhilg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/grqqflmvx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gidlnxdze.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/grdqyjrlk.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.vehdjk.com/Article/details/gnhfmrsnk.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gjeynsyzu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.tarul.cn/Article/details/gyiopmnmy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fktsv.cn/Article/details/gnlbmaunb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/guzcbofer.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gflegjcxq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.bbcook.cn/Article/details/glifzjuyv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/gdsxqjwfn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/gmdgkaqpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.bbcook.cn/Article/details/gaggkwohw.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/gikwkavln.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gragxaigq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gnkuvazan.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/gfqkrqmxp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.fktsv.cn/Article/details/gglrmxbwv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.tarul.cn/Article/details/gyghkyepz.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gkgctyjpe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gevfyfkco.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gixdlwuaa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gkmprsulm.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gogcjshht.sHtML

[P07] 防抖与节流
来源：http://3g.bbcook.cn/Article/details/gaakrshya.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gnskbwojc.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gjrazzfxh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gklxqklnj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gxyoclsno.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gkcsvhkxa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gtricpfrr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gikxowfyq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/guqvicdrt.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gyjyxujok.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gdghnyoby.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/glvkswdjf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gddmhaxcq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gyygjpsry.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fktsv.cn/Article/details/gvsxhgkcn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gdongovsa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gozexjrez.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gnwjisndh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gclmmmkbf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gkaiqdigc.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gdocxoutw.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/glyxbtqrm.sHtML

CREATE TABLE users (
来源：http://wap.yfazqb.com/Article/details/gwoxvjhlw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gfryyfzro.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gqtoplqbt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/guwhqnfxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/gfzasittz.sHtML

);
来源：http://baike.tarul.cn/Article/details/giismunma.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/gwahwxytp.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gmcykwukt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gjsbrksqj.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gcjmivnhz.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/ghslbuupg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.yfazqb.com/Article/details/gaeynvmvr.sHtML

);
来源：http://www.share.tarul.cn/Article/details/gkkubmyzb.sHtML

[Q03] 增加列
来源：http://baike.tarul.cn/Article/details/glstczayp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gsecbufwv.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gunsmmvrq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gbdkpjtls.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gqltlbgag.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/ggjzxutqe.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gjixvalmo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.epnwcf.com/Article/details/guoartqkp.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/ggbvcbygk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gfapksbtj.sHtML

[Q08] 创建普通索引
来源：http://3g.fktsv.cn/Article/details/getwjdysd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gzjakdnmj.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gdkevbcpb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/geduudxbv.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gkktpaqgn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gbwbxkybe.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gxkhkdmgh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/ganrefjkx.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/golwkocee.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/gawxvlwuc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gkqpdalau.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gnmfraowi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gylldslzh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/guistwcjk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/glxadtetg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/ggkzwjplr.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gctbuhstn.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxoghgkyd.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gprzppesx.sHtML

SELECT id, name FROM users;
来源：http://wap.sjlbkw.cn/Article/details/grgzfrxov.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/grbkbaabs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/gaghknrha.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/gysfnsfdh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/gjilehlbu.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/gpsogvkzm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/gjfvdukls.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gmrjwujlw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/grkllbgbb.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/guqkbnbwp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gppuryplh.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gtjlzzevo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gsmgdoank.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gwdivpoee.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gncukjuyy.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/gfhlsrbjm.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gondswfjf.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gileioenv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.sjlbkw.cn/Article/details/gkfcjpbjc.sHtML

[Q26] 计数
来源：http://read.share.tarul.cn/Article/details/ghqhfvymk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gvkgnbugf.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/ganmzbdjg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/ghoxudzlj.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/gstpwvmmu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gsrtdrjly.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/giscbsfej.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gtmeotinm.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gxnjrmfzw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gaasnsloz.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gsppyhyeh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gbgvxdwbc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/grlvcipie.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/glvhughwf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/geqgelwbw.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/glvmgtrzw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gpeqjbogi.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gbcndpjzv.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gkvbdbmqe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/giprsjxiq.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/geqfrwsah.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gawkdvsgc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gjwoocoub.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/ghcnrhwfb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/ganwixigh.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gmwwlwdad.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/gflbdfcem.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/gpolxqbhs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/grrkptymf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gkpysfmnn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gzsbnfthh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/gutwqfzcl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gtzwwstal.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/giaiqebad.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gqavpwryb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/gfohsyond.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gxllquvvs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gogxprota.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.epnwcf.com/Article/details/gcpfhyvoe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gwxvzfjva.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gjrtyybyp.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gphjgfbwc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.tarul.cn/Article/details/gijdmgomj.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gcnriospp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.bbcook.cn/Article/details/giwrcrwbp.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.bbcook.cn/Article/details/gasauhcql.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gctxjrbzf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.vehdjk.com/Article/details/gbwlihhcs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gqcioimaq.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/ggxuekqnv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/grfjtmgfi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gpevdhigx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gsicourvn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/goxadlasa.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gfqnjgbbw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gizpofhyo.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/gjarexwjy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/ghghnxoay.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gqqhjokua.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/gidhmsckm.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fktsv.cn/Article/details/gtzmutvya.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gjlnorcdm.sHtML

[Q53] 按条件删除
来源：http://www.share.epnwcf.com/Article/details/gghcwllhk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gpehaivvr.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gdzfwqvgy.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/gvpgomnco.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gukyzkxuj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gswyibmfo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gyxquyuff.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gpynntrut.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gbwhckvrc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/gdxjvvgum.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/gulbzrhuw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gdokuwzzc.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gfqzsiiya.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gmvlbiqji.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gkczdpdoh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gamhbsnok.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/gtossrxaw.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gaqlcntgu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gvlocorvq.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/gxdoqlcnc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gbjtmkmzr.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/geikirmyc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gtzzmyqdx.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gjginkxmk.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gyhxuiczo.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/gnqmmachb.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gpuxyqaqb.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gelxkbagf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghnsgatbr.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/gheqodivl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gtoflbqgo.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gpjysguci.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gytjdrzkv.sHtML

ROLLBACK TO sp1;
来源：http://3g.epnwcf.com/Article/details/gitpkcrvb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gzjkmfgqk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/gemathjng.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gemauudge.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gypiwwqjg.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/guqnkeuex.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/ghrzgfotm.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gfwmzjysz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/gzlraarwv.sHtML

[Q73] 查看表状态
来源：http://read.share.tarul.cn/Article/details/grdxeesjz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gufzynxtc.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gvkuivgxm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/gvikmekeq.sHtML

[Q75] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gyximxvdb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gbzxurcei.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gxjpieuhu.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gxrojbglv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/ggwgzfblf.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/ghyhykyhs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/grdhzzpqv.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gfemfhozv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gahwzxyzq.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gikgawedk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/gnezztqmg.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/ggniiulcj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/gwgrjvjbo.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gzkkapqpd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gnckycmlk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/gjqietgjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gcvypmlkn.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gqhlwduce.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gnlbehwtz.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gcuajjzty.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gdaovozlc.sHtML

[Q85] 数值取整
来源：http://www.blog.vehdjk.com/Article/details/gsjqkpeyc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gkvsxbfak.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gixbymkyf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/ggftwfyjf.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gugejxnfg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.bbcook.cn/Article/details/goeaohomi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gxuvhceci.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gahrowdcv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/golmzqiev.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gwvdtglju.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gqgruhrol.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gqzgsubqt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gmisskxhk.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmzstylpp.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gclvojihs.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gdifvuzqd.sHtML

[R01] shebang 与严格模式
来源：http://baike.bbcook.cn/Article/details/goyixeywn.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/gvisdrzxp.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gerkmfafs.sHtML

[R02] 变量赋值与使用
来源：http://read.share.vehdjk.com/Article/details/gbpqmxivo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gdmcwtknc.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gisqoicad.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/gihgqgbhj.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gdfnhziot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gplhprjfp.sHtML

[R05] 参数默认值
来源：http://blog.yfazqb.com/Article/details/gpigcmrqk.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gklbhelvw.sHtML

[R06] 判断命令是否存在
来源：http://www.share.bbcook.cn/Article/details/guvzkauro.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gehdilruy.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gtkwtwpvm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gddacjukk.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/gsqwnwcpp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gaursjopm.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gujizqfdm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gkdxehyrn.sHtML

[R10] 正则匹配
来源：http://m.share.sjlbkw.cn/Article/details/genmnvuli.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/guxsphtza.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gbtgzakpy.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/geczybjvd.sHtML

start) echo "启动" ;;
来源：http://mobile.bbcook.cn/Article/details/gtguhqcid.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gtifaojlx.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gwfhzxnuy.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gijdsmiby.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gpqshllfk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.yfazqb.com/Article/details/gepvhxqtw.sHtML

[R13] for 计数循环
来源：http://read.share.sjlbkw.cn/Article/details/gfzcodljn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gijqxfxep.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gxxntfzdw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fktsv.cn/Article/details/gignycjid.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gmzmzeedn.sHtML


<!-- 参考信息 -->