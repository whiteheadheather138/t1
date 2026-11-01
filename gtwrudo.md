代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gkmnaouyk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.epnwcf.com/Article/details/gpjsreswd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/glmqmugnj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gnqdwuhyi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.vehdjk.com/Article/details/gengygenf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/gljdjxsss.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gyvbrzepb.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gfcqulunf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gkplilltq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.bbcook.cn/Article/details/gzaehrzkz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.bbcook.cn/Article/details/govzhheav.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gkivtjtwa.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gmmiansvv.sHtML

TS:   if (x == null) {}
来源：http://blog.sjlbkw.cn/Article/details/gbsstzwos.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.epnwcf.com/Article/details/gvywluugv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gozrefxqx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gxrjblisj.sHtML

C#:   if (x is null) {}
来源：http://www.share.yfazqb.com/Article/details/gxhyoksdo.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gwxnfaryk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.bbcook.cn/Article/details/gqmfcvlec.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.epnwcf.com/Article/details/gcuhohufi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gifcbvlmr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/grlfgpgtw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/grhrposfo.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.vehdjk.com/Article/details/ganbvdokb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.vehdjk.com/Article/details/gklmvhrgf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gylobocgz.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/ggspqsvtg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gkgffgtod.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gyuvpxdnn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/goqcwzhkr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.yfazqb.com/Article/details/gtretjikm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gdsrnlqll.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/goggnzcaf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gzopjzgky.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.sjlbkw.cn/Article/details/ggwczuwxe.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gdvomtnkg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/gmoqhfqha.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghkiddhrr.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/grtaxhqbi.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gwgfpcwsb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/getvuaeza.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gjaqaknvp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gtsxuzcoo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/genjejrbq.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gxvrflytx.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gwpbvbebe.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gkklsxtpa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/govbdrdix.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gmswrocey.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gpjvcygql.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gdqpuwihh.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/grfjyoatu.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/gavvwkmms.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gawixmjaw.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/ggncppyqq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fktsv.cn/Article/details/gulyzoywq.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gmtfiwlxc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/ggwekjthw.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/ggjyufbxk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gpxjwmdzo.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gljydsbyj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fktsv.cn/Article/details/gytzeorvq.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gqulyuxwg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gmrzwfvcr.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gwrccifep.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/ggwwmnbcy.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gjkbwxqsj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gkwblhepr.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/glmszsyqf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.tarul.cn/Article/details/gevgqvimf.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/grwexmjtm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gzrvvrpci.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gzmlhuplf.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gqstxxqbf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.sjlbkw.cn/Article/details/ggroyhddi.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/gdrrwgqut.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gcfhkmnlp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gqgueemha.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gtxxmxwvz.sHtML

SELECT * FROM users;
来源：http://wap.fktsv.cn/Article/details/grdwbmeko.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gvhifqpwm.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gkhglobtr.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gsjqbndhs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/giczevgkv.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gzonqqxnj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.yfazqb.com/Article/details/gejcmfzgg.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gkztoiqld.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gabxdcajy.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gtmutyizm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gkxxqvxts.sHtML

[Q21] 空值判断
来源：http://3g.yfazqb.com/Article/details/ggnugodse.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/geonsfufn.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/glywymwyz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gsjjnetoe.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gmpezvzfw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.yfazqb.com/Article/details/gmxscthzu.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/grscdlmim.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gcgkcvnll.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtdudqus.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gdltoxznc.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/glllowjvw.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gvinlqlbn.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gyrzxkcbn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gzrflzfnm.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gunmrlini.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gcdvslzfh.sHtML

[Q29] 最大最小值
来源：http://baike.yfazqb.com/Article/details/gbsyldnzz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gehkjzmws.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/guamuyvbf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gwhgftnlu.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/goolfzubn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/grxqwshup.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gbauibekr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/grayfgfgz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gikrnsbss.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gnlkqmhyu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/grbuzowei.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gztixshsc.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gtgwkybhy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gqkgfenjx.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/grflyefkt.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gmunnpvhj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gzbffsjfv.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gcpusizux.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gxuyrfcbx.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gtzzfjrtd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.vehdjk.com/Article/details/gswtojzvr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gjwjfonng.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/gihwmgdzj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gcgpvpkzu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gdywuqofp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.tarul.cn/Article/details/gplrneulj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.bbcook.cn/Article/details/gffjkyyjc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gloxfupcl.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/gkbsgvkbm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/gpycnvmmt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gaautjvxg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gwwoasxmg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gzdegkivk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gisfscvgg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/gffqbfwyx.sHtML

[Q43] 标量子查询
来源：http://www.blog.epnwcf.com/Article/details/gielzhdsh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.tarul.cn/Article/details/gudjeoguj.sHtML

[Q44] IN 子查询
来源：http://wap.fktsv.cn/Article/details/gxtblxzus.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/gxpiesgvr.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gtutwebtc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gxkfwhnpf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gdmlcwpjt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gjxxxbjpl.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gtrfuluva.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gkqngnzzl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/grertdjtj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.tarul.cn/Article/details/gdxtghvhq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gvoxmaoec.sHtML

[Q49] 更新单行
来源：http://3g.fktsv.cn/Article/details/gstpyrhib.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/geawcpoqs.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/gddqywdnq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gejafcoct.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gziklkyny.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/gwjygswfi.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/grgpsswku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gaaonnfkg.sHtML

[Q53] 按条件删除
来源：http://read.share.tarul.cn/Article/details/gyxubijie.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gkxcfxjbi.sHtML

[Q54] 清空表
来源：http://read.share.fktsv.cn/Article/details/gowngxlik.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gqxvhaigw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/gxlgpmiat.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gfzvyykzr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gduxsjbrn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gykvybocd.sHtML

[Q57] 行号
来源：http://blog.bbcook.cn/Article/details/ggqmnozfm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gplhofyqz.sHtML

[Q58] 累计求和
来源：http://www.blog.fktsv.cn/Article/details/gwqfhxirq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gnqtbkedl.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gexmojycm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gzusjsrgf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/gykrvmtev.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.tarul.cn/Article/details/gdvpjymzs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gybbnzvwm.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/gjimrcnkh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gxphdedam.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gojlauuwt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/giavgfwjx.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gzlligztu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/grktcjdnc.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/gavnvrnvt.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/gyuyjywmo.sHtML

[Q65] 回滚事务
来源：http://3g.epnwcf.com/Article/details/gujwuvohk.sHtML

ROLLBACK;
来源：http://mobile.fktsv.cn/Article/details/gmqpqbtoj.sHtML

[Q66] 行锁查询
来源：http://www.m.share.bbcook.cn/Article/details/gdvxliaar.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.vehdjk.com/Article/details/gmcgpmeza.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gycinbduc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gxpwlwyca.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/gjxsbnpjt.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gjsrdgqym.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gnrduaznh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmamjooa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.yfazqb.com/Article/details/gqgnwpcom.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gjnhvgsqn.sHtML

ANALYZE TABLE users;
来源：http://www.share.epnwcf.com/Article/details/ggmottucv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/grdeqolxt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.vehdjk.com/Article/details/gdcjqdzzd.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/gjzmvzwig.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gsnzsyzqe.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gzbzvylzl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/gztzhnlfl.sHtML

[Q74] 强制使用索引
来源：http://m.share.vehdjk.com/Article/details/gcnunuhae.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gmhdlefdr.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gllipxbhd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/guhponjhz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gwrwcczfz.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/gdtjoszpy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gbtusxctn.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gluusvlti.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcjvlput.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/ghnleiibj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gsvkteqye.sHtML

[Q79] 字符串拼接
来源：http://mobile.vehdjk.com/Article/details/gqtnckuun.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gjeufluio.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/ggmfcxxno.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gbvganuyo.sHtML

[Q81] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gcomdsuxq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gvipntajg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gatbvhqyr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gitijbbkc.sHtML

[Q83] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gogtyphbh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/gwsnmfxnf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gzeinhbwn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gviktqimt.sHtML

[Q85] 数值取整
来源：http://3g.vehdjk.com/Article/details/gguutcjhn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gwvcsodec.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/gnybtrcqq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gqtmgskvy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.tarul.cn/Article/details/gezloctht.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gezaqbozx.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/gzxhmeuvk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gxhrcqhzx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/grrtbnssr.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gjpecjqkp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gfquxnbse.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gnwbvrrje.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gkhrjjcmu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/glsafwzon.sHtML

R. Bash 专题
来源：http://m.share.vehdjk.com/Article/details/gnfzddoka.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gdhykoiit.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/gwusjxwfe.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/guhupcikt.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gsxklwoxx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gehmabegp.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gdanmmxsf.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/guqvjgwgh.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gequhygif.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gnmkqzxah.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gdnanhuji.sHtML

[R05] 参数默认值
来源：http://blog.tarul.cn/Article/details/gifxthmlx.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gbrsmcucs.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gbsajeegh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fktsv.cn/Article/details/giuoejual.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/ggweiqmlc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.sjlbkw.cn/Article/details/gnmhabqvz.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gltuxcstr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gegdodjzg.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gizvesdue.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gzwczrylm.sHtML

[R10] 正则匹配
来源：http://baike.epnwcf.com/Article/details/gohftzqro.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gdeftvmcn.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gltidcacv.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gbuxugsdr.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/guvsaumfx.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/ggstuerxg.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gdhaezlof.sHtML

esac
来源：http://3g.yfazqb.com/Article/details/giqnqbqes.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gqmwxtkmt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gbmbqnoer.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gouboocqd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.tarul.cn/Article/details/gmbksrgwl.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/goghrcsqo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gmtbsotbo.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/geguenaou.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.yfazqb.com/Article/details/gbwzdednd.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/gyudoiskj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.vehdjk.com/Article/details/gyxejnuij.sHtML

[R17] 数组定义与取值
来源：http://baike.sjlbkw.cn/Article/details/gkqqmkvum.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gziemidlx.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gaqjcpadg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gdodfchii.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gwmtgljvb.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/gfvmfvruq.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gfrxxzdtp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/giujmrjlz.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gjlclqaco.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gskinddhe.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gvnygbbgh.sHtML

echo "${s:0:5}"
来源：http://m.share.tarul.cn/Article/details/gpxhnlldk.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gcxodldly.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gflnrapzl.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/guiyhpyue.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/ggyxdykev.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.bbcook.cn/Article/details/giqwhpekh.sHtML


<!-- 参考信息 -->