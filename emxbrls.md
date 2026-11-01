代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/ggilhtgia.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.sjlbkw.cn/Article/details/glemlawqe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gvjfodsiw.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/gbfbszmwy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gspaafqwi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gcrwbrzuz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gozcrmykb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gyxtccbrn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/gpdqyczzx.sHtML

Go:   len(arr);  len(m)
来源：http://baike.sjlbkw.cn/Article/details/gpltrjoww.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/gglagjlik.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.bbcook.cn/Article/details/gwrpejjok.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gvjutcwyx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gvjmdgtst.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gzxxdwvud.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gkfmpnnmj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gdgzrvnhr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/guwnrdjrv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gxenxucdt.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/grwrpcxjb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.sjlbkw.cn/Article/details/gkyffakem.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fktsv.cn/Article/details/gqjxtpdva.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gstbaedqo.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gqoaixrqh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/gmaqjmwlj.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gzgbihcun.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/ghumamfvz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gqreevrdh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.tarul.cn/Article/details/gqbdtdseu.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gzgibqexf.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gxdtdjxaa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gynsrxaxo.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gwbparyoc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gsjmdmtog.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gionajeir.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gwybtujwc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gbjiqipuc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gcaxrwsva.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.bbcook.cn/Article/details/ggggedujv.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gujxzekqw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgpfbzdz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gunxbvgnr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/ghtjmxoyy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.vehdjk.com/Article/details/gyrpjlvxo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gpbewatfm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.tarul.cn/Article/details/gctdrxxob.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gksbymwre.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fktsv.cn/Article/details/glomzeyvb.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gankhpkrd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gcqgkojny.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxehgmmkj.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/gdngwsfzz.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/grmfpievf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gujamdqlf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gxdxsyjyp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gsllvxduz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gpqcqibvx.sHtML

);
来源：http://m.share.tarul.cn/Article/details/ggomaauqu.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.bbcook.cn/Article/details/gxsqlodus.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gyerebbhm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gmwxstnme.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gjzshyrcm.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gmphzrfjk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/grijmpafh.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gifmejcth.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gnstackbh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gqabpnimy.sHtML

[Q04] 修改列类型
来源：http://mobile.yfazqb.com/Article/details/gwvdegrdr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gosuftygo.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gpcszkawg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.fktsv.cn/Article/details/gqrrckikt.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gdfvzqmqq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gssorfrtw.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/gfkgrfytu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/gbrxylypv.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gviobfthh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gxvxwteer.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/gzmuepzws.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gkitwswli.sHtML

[Q10] 插入单行
来源：http://baike.sjlbkw.cn/Article/details/gznzsstjn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gowhasyky.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gaayocdou.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gmodzaspc.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gjepiicuv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/ggzmhgtos.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fktsv.cn/Article/details/gqpvitlxv.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gtuuxwkqx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gopqfhauv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/giqiztlqf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gianzkbiw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gpicbkdfe.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gvddqgijl.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/grktvqeps.sHtML

[Q16] 查询指定列
来源：http://www.blog.vehdjk.com/Article/details/gmjpitzvz.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/ggcnxrwxq.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gvxvhkiuk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gbhteumqr.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/gcelnfsap.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.epnwcf.com/Article/details/gkobaayll.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gtgikfwew.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.epnwcf.com/Article/details/gkczazjgr.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/gnejxcczv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gbpvzuklz.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gnyiiygrv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gjoijjfod.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gdjtsutnm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gjykwxqvg.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/gfkibpplo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gnrehtzfa.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/gqdlntici.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gvkfwvhch.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/guygftqed.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fktsv.cn/Article/details/gkbhzqzbg.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gdyuocera.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gquxkbgwd.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gnmskwiek.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gebxhmqjh.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gqodqiern.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/ggpqjhagh.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/grhitrklq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gnlcsafqw.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/gqeocejvv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gywituvbi.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gjlubrsyf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/gsvbthvfs.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/ggpjxbtjb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/ghhcrbzjr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/glnabiprm.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gguoocflf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.epnwcf.com/Article/details/gczoswncq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gtggyhvzu.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gdijygkbs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gltcasdpz.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gfyczwltl.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/gnvvyfkui.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/ghjwsxuyg.sHtML

[Q36] 左连接
来源：http://read.share.epnwcf.com/Article/details/gpccfgfoa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gfdqqzjnp.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/glzhjbmfh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/gqpslfoyz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gmqugucky.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/gxpuafqrk.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.vehdjk.com/Article/details/gmsmpyjux.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gyungqwcl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/gjncvosax.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gdouquysg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gcuskikzj.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/gkcgshrxv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gvijqxlju.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/ggobafbma.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gbpancpgy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gfezglira.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gxjznyzcb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gzavjajcu.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/gvvqkawix.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gazjzhiuh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gfsxyrana.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/ghnngbwqt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gbwnwpboc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/ghboecxoe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gdbbdczti.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gdcohrnqy.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gxrezwvkd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.epnwcf.com/Article/details/gvcxaklft.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gdkwcjcpw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gmlacrdfu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gvkaavxif.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gkwelmovc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gsqpemeva.sHtML

[Q50] 批量更新
来源：http://blog.bbcook.cn/Article/details/gtqkprshr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/guvptlzrr.sHtML

[Q51] 用子查询更新
来源：http://mobile.epnwcf.com/Article/details/gklifzkfh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/golsecwaj.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gxgaaiszv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gfadcwufi.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gvaofyklo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fktsv.cn/Article/details/ghrreoskz.sHtML

[Q54] 清空表
来源：http://read.share.epnwcf.com/Article/details/gsorzcpmo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gfddyvuyb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gvxdbalrj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gpebgzfpv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gxvtrsgxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gsbfuwrpc.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gopafpvmg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gouovjvzk.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/gswyaztqw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/grouwrhcp.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gmskzxmmd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gkmkfacbd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gluvharao.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/giyvjgmbl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gooirpwrg.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/glexxboqy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/grarzwear.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gbhvuifth.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gmrjmplnf.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gtctnhogq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gsqqoxpij.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/gxheuhojw.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/glnrbcdpn.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gbxularpa.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gbtwyscty.sHtML

[Q66] 行锁查询
来源：http://blog.bbcook.cn/Article/details/gtqqgnmam.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gtesdyhrz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gnblgccre.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gihbmcuee.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/gcyvndisy.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/girdpifam.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/gdqfuooha.sHtML

[Q69] 查看执行计划
来源：http://baike.tarul.cn/Article/details/gftsoihen.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gjstinlms.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.vehdjk.com/Article/details/goxtxsoxx.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gqmxxaagx.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gfglwfenu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.vehdjk.com/Article/details/gcrxxbpsu.sHtML

[Q72] 查看索引
来源：http://baike.sjlbkw.cn/Article/details/gopzwpdem.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gzayigzxa.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gmehbvyzu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/gpaazguum.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gnuvdqydx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/gupaecbij.sHtML

[Q75] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gpuerrhbf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gpvrmwpzg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gmaipyhuh.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/ghzxaxfez.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gvdqzmryg.sHtML

[Q77] 时间加减
来源：http://mobile.fktsv.cn/Article/details/gqoymhvfj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gmaxgfqst.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gzuurshpe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gnpmwcxzy.sHtML

[Q79] 字符串拼接
来源：http://3g.bbcook.cn/Article/details/gftzpoftc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.vehdjk.com/Article/details/gphpwhtjf.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/guqajkqtd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gmfxsluej.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/goipbzomx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gzxkgufzm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/grbqwevqp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gxkkgghmy.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gtqetdaff.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqwvwjciy.sHtML

[Q84] 去除首尾空格
来源：http://blog.tarul.cn/Article/details/gankqohaq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gijesqpeg.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gfgpkpesq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gvcsndvcf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/gwmcpdftw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/gaipugemk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gbkbqottg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gcidjpcyn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.epnwcf.com/Article/details/glyzzhobp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gmqqnmirh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gudzqwvdt.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gpsgnxyun.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/gwwrhgnnw.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gzakdvxkv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gfzktzzoq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvgrxedwj.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/giuuphonw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqphjtpmh.sHtML

[R01] shebang 与严格模式
来源：http://3g.bbcook.cn/Article/details/gaaoseaut.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gahdwpkhe.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/gveefiufy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/gndsnffye.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gooqkhcks.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/grkijwpbu.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gjnmcomim.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/glswgkfny.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/glmbtllbn.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gqorcdwym.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/gkppwnfkx.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.vehdjk.com/Article/details/gxvrhbkui.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gbpdbswym.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/geeosfscr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/ghnltyolz.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/grbxgbryk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gohmlmbxc.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gldybsurs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.yfazqb.com/Article/details/gawopmgwl.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/grkdymngi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gjxrbgcdu.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/goejrctbv.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/gcwzqlsqq.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gwtiihfnp.sHtML

stop)  echo "停止" ;;
来源：http://blog.vehdjk.com/Article/details/gcpogyyee.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/gidejuian.sHtML

esac
来源：http://blog.bbcook.cn/Article/details/glfslcsvy.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gohbxnqou.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gxhrsyups.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gjpbnhvrw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/geohyxspw.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gxkomulpy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/grmzyapuz.sHtML

[R15] while 逐行读文件
来源：http://www.blog.bbcook.cn/Article/details/gorjqmxov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gvlhdufgp.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/gwsyqlyvn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/gejqkwhqu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gwdfxabfa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/ghoacquhh.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gfnvkofvy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/ghthyxxtd.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gsdysgzrx.sHtML


<!-- 参考信息 -->