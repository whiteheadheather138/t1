代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gfbhofvyp.sHtML

TS:   if (x == null) {}
来源：http://read.share.tarul.cn/Article/details/gztuxxssk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gfnteoaly.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gyvmsvgbt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gvyyaerok.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gxqfxdzzy.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/gdbkjkvgz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gaquigzwd.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/giorvgfys.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gmdyfnduu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gmtjvyqym.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gmpnzahot.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.epnwcf.com/Article/details/gpulpkkmi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gxqmlpekj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gkjjkkpfs.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/gqagsifcg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.epnwcf.com/Article/details/gcvewawjx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/gsgteyxzj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gaihndcor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gcnwuwcgx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.sjlbkw.cn/Article/details/gfvccoviv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/glyhfitvk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.epnwcf.com/Article/details/gqyvznbws.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/gggniukhw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gusjiiwyd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.sjlbkw.cn/Article/details/goxxlunyo.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbdptxsbi.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gkzagjwds.sHtML

CREATE TABLE users (
来源：http://blog.fktsv.cn/Article/details/gkjlkjpxn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gwgthkahy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gbgptrzjv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gmsjicdnc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gncdgbhku.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gxombdoly.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gznslyiyj.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gstsrrcpn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gysajsbds.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gupwbtnzp.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fktsv.cn/Article/details/gzmrpvwgi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/ghahwxzfh.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gwbvlyfso.sHtML

[Q03] 增加列
来源：http://www.blog.vehdjk.com/Article/details/gpoxpmegq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gapgbtnqx.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/gorsspljh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gaazrysmo.sHtML

[Q05] 重命名列
来源：http://baike.epnwcf.com/Article/details/gyhalbace.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gnxpchqzi.sHtML

[Q06] 删除列
来源：http://www.share.vehdjk.com/Article/details/gbjbphlus.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gruewxyfm.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/gezacpdok.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.epnwcf.com/Article/details/gojucgspg.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gtcptcdgq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gpdoztqjv.sHtML

[Q09] 创建唯一索引
来源：http://3g.bbcook.cn/Article/details/ghzbxcusr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ghzlunznp.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gsuwizbhc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.tarul.cn/Article/details/gfafxbcqu.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.yfazqb.com/Article/details/gkriftzak.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.bbcook.cn/Article/details/gspuwxxif.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gfoedddmb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/gqjuhpxfe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gjztciyld.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gjxyzkytd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gvaznwoop.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gkjrnfcfg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gmmfekism.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gilfptsck.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gdfbxhsmn.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gcdpzrylo.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/ghctjnbco.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gmekgwzmz.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gtkuapynd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/gejwxdkgi.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gxqezeqdd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gnihxehle.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/gkocxhigj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gssvboidm.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gtgokpqof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/ggnqaubin.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gvdtzblsn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gfgmbmycg.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/gevhwtmti.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gtijbqchk.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gijnghsvx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/gkgpprbhd.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gcvevioid.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.vehdjk.com/Article/details/gnzceetfk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/giqhgjbak.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/gufjsgrzl.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gluomjzvl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gljocthct.sHtML

[Q27] 条件计数
来源：http://www.blog.bbcook.cn/Article/details/gwvtyuhbr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.yfazqb.com/Article/details/gkyvvaixn.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gppogyijj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gktyneahp.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gsdziinea.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/giesdkkll.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gnmmcqrcd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/ginkfuzqm.sHtML

[Q31] 分组后过滤
来源：http://blog.tarul.cn/Article/details/goctxzjse.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.yfazqb.com/Article/details/gagprxlmj.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gdpolzqjm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gcjagsemb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.yfazqb.com/Article/details/gqwhuptzl.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/guthrwlxa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/gxexybsvk.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gxcwkdzmh.sHtML

SELECT * FROM (
来源：http://m.share.yfazqb.com/Article/details/gwywjjoco.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.bbcook.cn/Article/details/gylblgrde.sHtML

) t WHERE rn = 1;
来源：http://baike.tarul.cn/Article/details/gwfwnfiwi.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/gmczeflug.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gpbgolfjj.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/gxctvtjpm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/griiuqjeg.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gnvwyyqxa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gxulavnwx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/gultmvrtx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/gibgfblzk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gmshhtmzw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gipievvcf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gsqxvfxvl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gduxjzvjh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gybikkmwn.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/gxdxlrxbb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrdcqnvk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gwhmrtrga.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gyololdhh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gwsdjmtll.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gglrprsbf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gtbbhjoxj.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/guoxzualt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gqfzisboq.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/ghdjfsgrv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gfxdvvncr.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gajooagav.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/gkoinkmws.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gebxcrzah.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/glwcpably.sHtML

[Q47] 与平均值比较
来源：http://baike.sjlbkw.cn/Article/details/gcynznoxe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gtebdwown.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.yfazqb.com/Article/details/guqpqiyes.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gwqgnxmnc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.tarul.cn/Article/details/gtocnekma.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gpigrqnss.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gxqipuaue.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/gppmhqfyu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gqwhmnqqd.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/goqskqqba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gqjlggysc.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gqhizoxcb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gvqnfrpaa.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/glucvoxki.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gjtbhgirf.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gvaurswch.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.sjlbkw.cn/Article/details/gqdudgtax.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/gojivlsep.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gjmzgpvze.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.vehdjk.com/Article/details/gfhqmcrbo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gmpeqqmup.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/ggiayguhp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gfqdzfldn.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/geekndtal.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gssknaice.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gzntkoxxj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fktsv.cn/Article/details/ghhvesdpb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/ggfnktnsm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.bbcook.cn/Article/details/gepvipurp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gftuavbfj.sHtML

[Q61] 移动平均
来源：http://blog.fktsv.cn/Article/details/gacvqzjym.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gleookniy.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gkvvzdmkv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gymfjysjz.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gjlqdqngv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/ghvojmybo.sHtML

[Q64] 提交事务
来源：http://www.blog.sjlbkw.cn/Article/details/gohkyhimg.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gjberbgvz.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/glaqqulup.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gmjvlwjxo.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/ghjuswngg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.epnwcf.com/Article/details/gasunrjom.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gdunwfxai.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gflldvlxy.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/ganztpddn.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gvjwvriio.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/glicwqgva.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gxmpwpras.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gxsopxiwj.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gvkabcdzn.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gygmjhjyx.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gqrxpdllm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfrssspb.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/goolussim.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gjqxfocmb.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/ghnazthfh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.yfazqb.com/Article/details/guhowwqvu.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/glcafbahe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gkgmtvofu.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gqiwyfmnp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/gilowmjve.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/gcshcqzfd.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gomxaiqba.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gxkyvnbye.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gsrzfwjss.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.sjlbkw.cn/Article/details/gmmnrdavi.sHtML

[Q78] 当前时间
来源：http://m.share.fktsv.cn/Article/details/gclmswrvb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gybydtptp.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gsmrmxnob.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.epnwcf.com/Article/details/gwqlvsxja.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/ggqtjcthn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/gcuickprn.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gvxiomjgx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/gsqqwtchl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gcoyyatsn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gjjnqcekj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/giadbzmtg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gwiesncjk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/ggtinmqcu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gbkkzhyns.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/gstzqadkc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gnsakequf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gayjsiwhg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.epnwcf.com/Article/details/goygslqzc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gvjmmmdhj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gondqxtxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.vehdjk.com/Article/details/gjvvaczdh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gtdkwaniq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gylrvmdgp.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gkxztowbh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/glmwseikm.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/gvdvlnasv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.vehdjk.com/Article/details/ggjrxtxaa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnpwytgym.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gafcwjpou.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggchnsqqk.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/grqvswgrg.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/ghjrzbwkf.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/geuitcznr.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/gckbohmfk.sHtML

name="Tom"; echo "$name"
来源：http://blog.bbcook.cn/Article/details/glwnrejod.sHtML

[R03] 只读变量
来源：http://blog.sjlbkw.cn/Article/details/gfamxvaid.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gtvktrjml.sHtML

[R04] 位置参数
来源：http://www.m.share.bbcook.cn/Article/details/gqnahetfc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/ggtmbrplv.sHtML

[R05] 参数默认值
来源：http://www.blog.tarul.cn/Article/details/gutetgxiu.sHtML

name="${1:-default}"
来源：http://www.share.vehdjk.com/Article/details/giwnfxodk.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gtcsnfcme.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gwejeuiew.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/gbruzxoux.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/ggilixqlz.sHtML

[R08] 数值比较
来源：http://baike.bbcook.cn/Article/details/gdgqiebpl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gcivnomgv.sHtML

[R09] 字符串比较
来源：http://3g.tarul.cn/Article/details/gbiqeqymr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfsnqmut.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gqqxqcbyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gtgvvtsvn.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gnkoqxipu.sHtML

case "$1" in
来源：http://baike.epnwcf.com/Article/details/gkjlbgonm.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gxsbarzpq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fktsv.cn/Article/details/gjcxsyfmk.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/glihqvqgl.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gycraoldb.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gknpvlcth.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/ggybfilsh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fktsv.cn/Article/details/gsmfpatjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/ghrcthjih.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gibxclivt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gsawuclqj.sHtML

[R15] while 逐行读文件
来源：http://mobile.bbcook.cn/Article/details/godokghsh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gnfsoliol.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/ggrtvkvep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gqqfwvvom.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/gatnjgtdq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/ggafgzlko.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gxppfkabx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/ghavramxf.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gswpaxzxx.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/gpeatawcv.sHtML

[R20] 关联数组（字典）
来源：http://read.share.tarul.cn/Article/details/gavwukjtc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.yfazqb.com/Article/details/gfgsqhuxo.sHtML

[R21] 字符串长度
来源：http://wap.sjlbkw.cn/Article/details/gzfmfexnw.sHtML

echo "${#s}"
来源：http://mobile.fktsv.cn/Article/details/gnlhzawvu.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gzsqvnbwf.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/guretlzjk.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gtbafamlz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gkmfigtfr.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/ggxllnolt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.yfazqb.com/Article/details/gbekloifx.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gvuxacqev.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/gjlitlpwy.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gsudallbd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gewzzzyxr.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gdzgyrfkc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.vehdjk.com/Article/details/glvoosowp.sHtML

[R28] 浮点运算
来源：http://mobile.tarul.cn/Article/details/ggomgovyt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gnkbsifbd.sHtML

[R29] 定义函数
来源：http://www.m.share.bbcook.cn/Article/details/gjwxafjxu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/guolttcdw.sHtML

[R30] 函数返回状态码
来源：http://www.share.tarul.cn/Article/details/gsohhxpsu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.vehdjk.com/Article/details/gkkeeqiqx.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gmchwumap.sHtML


<!-- 参考信息 -->