代发 wailian999

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gogebbtma.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.sjlbkw.cn/Article/details/guzqncczf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gvyqridim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gokhjwhld.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/giyltqrcs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gxfyjrlnj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.bbcook.cn/Article/details/gquljqrqe.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.tarul.cn/Article/details/gnbgjhrxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.vehdjk.com/Article/details/gbtusskgn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/gefwpbuvc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fktsv.cn/Article/details/gpjxpvcng.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.sjlbkw.cn/Article/details/gwgmhuphr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/ghunqcvoe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gbjooihst.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gkrothonj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.epnwcf.com/Article/details/gcvmqwxrc.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzymrhqjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/gybtdrnml.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/glifqgvab.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gnqsolgrt.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gqqxfwsde.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gibfcqodk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/guascluin.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gnzfyykju.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gmocmgybl.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gmhexfrkh.sHtML

[Q02] 创建带外键的表
来源：http://wap.bbcook.cn/Article/details/grqvuxbsn.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/ggqkpepxx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gtnprrehb.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gyycoqaps.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gnbupkkmd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.tarul.cn/Article/details/gsvqnjryr.sHtML

);
来源：http://wap.tarul.cn/Article/details/gmfrbzybg.sHtML

[Q03] 增加列
来源：http://baike.tarul.cn/Article/details/gfrsytefj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/ghpdmnrfx.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gxmdjhyxv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gumfllhqg.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gmkiugeaz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gypxepixc.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gsxphjjrl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gkidnjciu.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/gjdlmdbku.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.epnwcf.com/Article/details/gnsvvkbtx.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gsjcudwds.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gqqscdbco.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gypscwuvu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/ggpunlbob.sHtML

[Q10] 插入单行
来源：http://www.blog.yfazqb.com/Article/details/gjhlvkvzq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.tarul.cn/Article/details/gbxxmnqit.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/gbovszbaw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.yfazqb.com/Article/details/gmeqkvfxx.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.epnwcf.com/Article/details/gqujohoqe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gmzeibpwq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gwmmxuscm.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/glkypyijp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gxegzsxbl.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gfkwmeovh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/ggnqusicp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gfeowgtay.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/gsiwqxlih.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gchxbogto.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gzcgwscik.sHtML

SELECT id, name FROM users;
来源：http://www.share.fktsv.cn/Article/details/gykhmtxkp.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/gwcjwtmwe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fktsv.cn/Article/details/gxspaihzm.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gytkbgapv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/ghkvrbdim.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/gewsdkdpw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gcrvffbcn.sHtML

[Q20] IN 列表
来源：http://www.share.bbcook.cn/Article/details/grxmiyqxy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/gcimxunmy.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/grtwxnyql.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/gokposswp.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gujfrwrju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gyfgobjbq.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gbxfnkmym.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/gqcvxnwsm.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gbzgorxcf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/geybafxlq.sHtML

[Q25] 只取前 N 条
来源：http://baike.bbcook.cn/Article/details/gzkhkqgra.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gzozaezzt.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/gjndalaje.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gnqkhjzno.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/grgxjhexd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gzwyoqhow.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gmiigepbz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gfihpehik.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gwbvhehtt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gnfjrschk.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gkxkozsgi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gtmbbcmei.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/ghltholes.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gxcnowxrs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gehwinric.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/grcvdibnk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gntnxnpgo.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gzhusvacj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.sjlbkw.cn/Article/details/gqkausedl.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gesrrffss.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gtevhjzva.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/grqphcdkl.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gwsmjvvol.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gfxazwgop.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gckxngtoa.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/gizettbus.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gckzfogfr.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gnfqyiyzw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gblvjaeos.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gaugaxyxe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/glgrgaxri.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.epnwcf.com/Article/details/gozgbxqpu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gtlozzgxq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gbkupcxsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/ggmtqgdjh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gbonxscpa.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gagqiflla.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gklumwige.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gbhawxbrt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gslujhlyo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/gwbdaspsf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.sjlbkw.cn/Article/details/gkuhmpntk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gqajguocp.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/grhfrzlsk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/grwywarsp.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/goapnpbfl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.sjlbkw.cn/Article/details/guqexctqj.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.yfazqb.com/Article/details/giduejbew.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gvtdadczb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gugzerjrl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gizxhcxyr.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/gwijbgvzy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/glmhyyvru.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.bbcook.cn/Article/details/gpbcpovuw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.bbcook.cn/Article/details/gkqwwpnmz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gfqdqlypu.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/glwhbowet.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/geekklmna.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gxgpgfuuj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.epnwcf.com/Article/details/gkygeyszf.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/ghleltbwl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/gwhwkpwxq.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gssqxmpqk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gobhgduuq.sHtML

[Q53] 按条件删除
来源：http://read.share.vehdjk.com/Article/details/gcagahyrd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/goqqriuym.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/gfycjbzdp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.bbcook.cn/Article/details/geqaiebrx.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gkyhukjtb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.epnwcf.com/Article/details/gqcjfswbb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gljfvowpq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gdsbawrqz.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/godomzhpy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcsgauehd.sHtML

[Q58] 累计求和
来源：http://www.share.epnwcf.com/Article/details/govxbnqdj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gwhtwkydo.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gxujyymip.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gefvnwipp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gypryacxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gefxrtaah.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/ggetajxgs.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gvbseqllc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gmqukxzxk.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gnkannuxx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gbufqzows.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gqeqggwjh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gumfnntub.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/ghasiglxw.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/gallosttn.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/ggvhlvvoi.sHtML

ROLLBACK;
来源：http://mobile.yfazqb.com/Article/details/giphkygrs.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gqfnxaiyn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gfifvutta.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gtywktohl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gmslilocs.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gdpthuzbk.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/glmocdzno.sHtML

ROLLBACK TO sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gabbbbdeg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gncezfdzd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fktsv.cn/Article/details/gveonxwqh.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/gkphnqabb.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/ggiifnpgb.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gogxxmluz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gmulyypnj.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gayagznqx.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gfisdvziq.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gsteyqsqo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/ggyybuqqj.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gbxvqfmjr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gwzdhofak.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gyqurhchl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fktsv.cn/Article/details/gpzfintpe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gebwajrlt.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/ghtsbkgiw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/givfydvwo.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gimysnhpt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/gmkaoofrr.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gtharbpxv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gqbigqnid.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gaciwzvif.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gxvywwqct.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gzxpszxqk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gltugblis.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gbinrxujz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/guqxxlivp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/ghseifloe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gjimakkob.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gczaplihq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gokxrjhfj.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzdfpwvl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggxdbvvnr.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gylcslqgd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gbvgdmlvx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gnpztsfuu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/gighpaabz.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/goelzmyjp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gspsfbjpc.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gwaqgwdtc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/guyciwsgb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/glmqpekgi.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fktsv.cn/Article/details/geeyqqbgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gvouztbgn.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gnzrfpkxx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gidoepujx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyboamwbg.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gsnkomwyq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gwwfdhdin.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gcufjutlk.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gbkotmqbi.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/glqinrjsv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gsbqoracp.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gvrerdbdi.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gkqwfiatu.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/guskfkhvj.sHtML

[R04] 位置参数
来源：http://blog.fktsv.cn/Article/details/gvdlnlpmk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.vehdjk.com/Article/details/gnhpxwyhk.sHtML

[R05] 参数默认值
来源：http://wap.tarul.cn/Article/details/golthlyse.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gjoehmtmo.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gchrutegb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gahxltpdp.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gpdbazotl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/gopgfuenm.sHtML

[R08] 数值比较
来源：http://3g.yfazqb.com/Article/details/gxgdcbfku.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/glsihxqhb.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gprsyprzc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/ghflbttsq.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gbhpipdjy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gcaepreno.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/ghhziunjn.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/guqsedgps.sHtML

start) echo "启动" ;;
来源：http://read.share.tarul.cn/Article/details/ggfdvhnog.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gpbgvadji.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/gvolzndqd.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gkbogxddk.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/gqbxqsaoz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.epnwcf.com/Article/details/giythgnlb.sHtML

[R13] for 计数循环
来源：http://mobile.fktsv.cn/Article/details/gtmspxxop.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gvyavsaia.sHtML

[R14] C 风格 for
来源：http://www.share.fktsv.cn/Article/details/gwsmmorwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gupajhfob.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/gzxkihlxq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.vehdjk.com/Article/details/gahmxwblg.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gveyfcysh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fktsv.cn/Article/details/gtuwfbdst.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gneexqfox.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/ghrzyvfsn.sHtML

[R18] 遍历数组
来源：http://mobile.sjlbkw.cn/Article/details/gscdwmivi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gsqmjxacv.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gfzqkkgsj.sHtML

echo "${#arr[@]}"
来源：http://m.share.bbcook.cn/Article/details/gxuqtvkzl.sHtML

[R20] 关联数组（字典）
来源：http://www.share.bbcook.cn/Article/details/gmcusnvmb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gytwlfwcw.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gokgsvzpi.sHtML

echo "${#s}"
来源：http://www.m.share.vehdjk.com/Article/details/gjbzjimre.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gnitxegjx.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gxyxotvzg.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gkmnkthld.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fktsv.cn/Article/details/gfvzpqsbx.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gvkjrbqln.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.tarul.cn/Article/details/gzwrgcohh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gigdcwsoo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.vehdjk.com/Article/details/gjamqwaxt.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gxpvhutad.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/geihrkabm.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gzakgqasz.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/gemeltjiq.sHtML

[R28] 浮点运算
来源：http://mobile.yfazqb.com/Article/details/gaajinbtw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.vehdjk.com/Article/details/gbtljynpe.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gkkzfetez.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gejjqxzgf.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/ggxeeiefw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.epnwcf.com/Article/details/ggvybmbkf.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gkymfslmp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.bbcook.cn/Article/details/gcqgrodfy.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gcnqaonqd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/ggstyficm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.vehdjk.com/Article/details/gewrgqndl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.tarul.cn/Article/details/gfdervalg.sHtML

[R34] 退出时清理
来源：http://3g.bbcook.cn/Article/details/gmlrtrrsl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gfhsasmep.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gyuccoswb.sHtML


<!-- 参考信息 -->