代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/giwhkmpmp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gfrjmrokn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/grqldhsxd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gdxyhfmct.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.yfazqb.com/Article/details/gyjmfrbbk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gmflondtc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gbexlkwmf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gbbemuxml.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gqccfbndb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/ghlktzynr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdoilvagv.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gzlepfqhs.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/ghhvfyehm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gmbumrqwt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gwtpbxuhn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gwzeceqze.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gaeyojfan.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gcjkaagpl.sHtML

[Q02] 创建带外键的表
来源：http://3g.epnwcf.com/Article/details/gfgxspbkt.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gwfbclivf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gbybfqgro.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/geqrjxhtj.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gijxjbkad.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/gjpwdjjre.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gcawnjpon.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/ggyexgito.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gxkhdpdti.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gkotrrckm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gsulpaorx.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/gtqndguzf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gucifmyqz.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/guruimrng.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/grgkkcfet.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gwjijbkpp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/giqtctmvw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gvfubukxv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gipiqqmxh.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/gsgrmfmfk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gfmrfjtoh.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gowqcdyeu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gtkbahnnn.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gukkkwtxh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gcddgjuzn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gtpdtfmxp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/gmefulxlf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/grvxucfyj.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/givysapnu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gzdkmrrws.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/gyyhpbzun.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gqmvhwqyo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gabqovynb.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gnguqyody.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gwlbkqwpi.sHtML

[Q16] 查询指定列
来源：http://wap.epnwcf.com/Article/details/gehuuvzje.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gwkicpwhj.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/grraxvfkh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/gxvkefxqu.sHtML

[Q18] 模糊匹配
来源：http://wap.sjlbkw.cn/Article/details/govluevuv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gigsjxrlv.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gqpkncvzt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gpwvrhdac.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/glqwzthsj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gjhseihwc.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gcmqdbbjo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/ggadyyfwy.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gtajapbsc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/gmqdqzgnl.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gzrzxvqqt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gkqgrglhz.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/glbwzksom.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gnasbeiux.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gcajizhkg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/grwmnwcpx.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gpiglemrb.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gbwmajjlt.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gmnxaiduz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gsqhjbxmf.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/grxiwbgrp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gfkugchgh.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gaeiljffo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gnwkoyiht.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gqhatuugk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gclrvamcb.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/gzgudvkxq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.bbcook.cn/Article/details/gcrnxgjis.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gipjbcjvy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gewzxfbuw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gbkpjodgf.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gkdwflezt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gclziozmc.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gmndjoekf.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gzqumyiha.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.bbcook.cn/Article/details/gxyohxmxl.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gidaujfot.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/gejfqjgrm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gaybyqccl.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gsxohetsy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/gdpxmkbel.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gymmonrip.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gzlrlbapl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/gnfltdvun.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gfjzrfneg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gxmhlxtxl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/ggtabpqws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/goofckqqa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gihixkwym.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gbjyxahzg.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gybvdeivf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/grnpwzgwj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gibcpdkcq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/gmrkgpcgg.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gaqqocktv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.fktsv.cn/Article/details/giubswlps.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/glxjxqaxu.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gwhvesmio.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.bbcook.cn/Article/details/gjijozefv.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gfkqqbgek.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gulrcacrv.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.bbcook.cn/Article/details/gzyxzcvsi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/ghlcwxggu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gnitsqpgr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gzswplfpz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gjdhjbxon.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/gwlnzuhtj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.bbcook.cn/Article/details/giwyzuihx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/gnfmjvioy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/gjlbwbvdp.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gmhbjofhz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gaebitdel.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/ggiviroxi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gjthuplci.sHtML

[Q51] 用子查询更新
来源：http://baike.yfazqb.com/Article/details/gxppipofs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gyvhsfkou.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gngwcsllc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/glrxwgamu.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/gwteiwqas.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gbiypaegp.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/ghxskwdlx.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gqlmxswdh.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gmirmrksl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gvkavzcoa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gsjnetryx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gmerhfvps.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gijyplzhe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gdlqshoep.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/groebsarc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmzdxtpkk.sHtML

[Q59] 分组内累计
来源：http://wap.vehdjk.com/Article/details/gykpqdett.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gbkesmxel.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.vehdjk.com/Article/details/gcefxcfpk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gertajghu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.epnwcf.com/Article/details/gsxmznocc.sHtML

[Q61] 移动平均
来源：http://blog.tarul.cn/Article/details/gcnqziaky.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ggycbvgjk.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gabnmygan.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gvdqnpdlb.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/gbqmrxkau.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/geinkqqst.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/giqtihmzb.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gqsvkrmet.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gnzqaciyu.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/gqdnlisnm.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/galkcyvld.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/glactrrcs.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gjqugforf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/gczwxcabq.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/glbivvvou.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gststkffz.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gdvckxtam.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gcjiebkqo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gbstkimqa.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gvygjdaec.sHtML

ANALYZE TABLE users;
来源：http://www.share.yfazqb.com/Article/details/gauullyvx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gbufspyyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/ghdthemba.sHtML

[Q72] 查看索引
来源：http://baike.bbcook.cn/Article/details/gefmtwiha.sHtML

SHOW INDEX FROM users;
来源：http://read.share.vehdjk.com/Article/details/guwkczali.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/golcegkbu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.bbcook.cn/Article/details/ggdejujzr.sHtML

[Q74] 强制使用索引
来源：http://blog.tarul.cn/Article/details/grfzsqtvw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/ghniwmzkz.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gcyhccjsk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/glvuthewk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gfjzqkmbq.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/geitswefz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gesstnrvy.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gwwretbwm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.vehdjk.com/Article/details/giobvbpou.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/geeoblbzp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gyghdmyqs.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/ggfevctwo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gxjptdypv.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/gjqhnrngs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/givroaayx.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/giluaqdtp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/godzlohfu.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.bbcook.cn/Article/details/ggbpifurs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gyalbbhkn.sHtML

[Q83] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gsrvhsejg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gbpxanrly.sHtML

[Q84] 去除首尾空格
来源：http://baike.vehdjk.com/Article/details/gqcakxtxn.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gmuxbkeog.sHtML

[Q85] 数值取整
来源：http://www.m.share.fktsv.cn/Article/details/gjocsiglz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.bbcook.cn/Article/details/gmeaoaprz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fktsv.cn/Article/details/gqepaghvz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.bbcook.cn/Article/details/gaqxqzchz.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gpnhzpqiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/ghgzvtkzn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.yfazqb.com/Article/details/gqkufbzzy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gkjukicni.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.bbcook.cn/Article/details/gsyagbmbz.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/glkarflfo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gulcrcqch.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/giuvmmcpr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.bbcook.cn/Article/details/gwvllxelj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghzaiulxj.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/ghbefdgfy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gnzdyqqgo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.sjlbkw.cn/Article/details/gysqpoodg.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gzekdlmhe.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gsvaqkkdw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.vehdjk.com/Article/details/guvtngxmc.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gxlrepfwi.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gczshebnd.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gppmqeidn.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/geqtyrtab.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gsmzxnxqw.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gkmiuqemz.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gvxcshwjk.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gnidrblat.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.tarul.cn/Article/details/ghwsbvten.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gfsxnwivi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gwfvzksmy.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/glskarggl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gahueiogq.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gshrblcpa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/gubvhqthf.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gicwfmkun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/gzuumnsef.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gxomsazlp.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/ghgpyhnky.sHtML

start) echo "启动" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gsowsorue.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gpmciuwgi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsufauqy.sHtML

esac
来源：http://read.share.vehdjk.com/Article/details/gpxudignr.sHtML

[R12] for 遍历文件
来源：http://www.blog.sjlbkw.cn/Article/details/gwvezxkqh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.vehdjk.com/Article/details/gdhoqkccj.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gboabhjyn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.tarul.cn/Article/details/grabbysnj.sHtML

[R14] C 风格 for
来源：http://baike.fktsv.cn/Article/details/glivlitug.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gmrrqyiqm.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/gugxwneee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gcqcvfmzx.sHtML

[R16] until 等待条件
来源：http://www.share.yfazqb.com/Article/details/gxxmyimpy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gnpsgcezj.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/grlifriep.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.tarul.cn/Article/details/gafwdsaxd.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/gbejidwyj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gndleehut.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gbnlndsrs.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gyuwgipae.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gqysslsbg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.bbcook.cn/Article/details/glbfwavuq.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gziaqldid.sHtML

echo "${#s}"
来源：http://www.share.fktsv.cn/Article/details/gnzlktfxe.sHtML

[R22] 截取子串
来源：http://blog.bbcook.cn/Article/details/gctginlew.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gsecmguyq.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gcbeelpau.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.vehdjk.com/Article/details/gzlrtxrim.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gvvvpvrnl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.vehdjk.com/Article/details/gnyhqhael.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gtorqcrvb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gieidforh.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/gpgdyphvs.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gchsllfva.sHtML

[R27] 算术展开
来源：http://m.share.sjlbkw.cn/Article/details/gftbdcmct.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.tarul.cn/Article/details/gcfjaaknt.sHtML

[R28] 浮点运算
来源：http://3g.tarul.cn/Article/details/ghclomnwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.epnwcf.com/Article/details/gdxrlzyxb.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gxknykltx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gctwxgumq.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/ggcezmtna.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.tarul.cn/Article/details/gapfqlywx.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gryktaonw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.vehdjk.com/Article/details/gnzjrcncr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gbfqfmokn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gukesnwkx.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/gugvxyjaj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gockeruhw.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/gorcdcvzp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gwvjblekk.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gfmhvjgts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.vehdjk.com/Article/details/grxafgtbw.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gvrogdadx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.tarul.cn/Article/details/gpsmbzprf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gyphgzalo.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gusbcpgvn.sHtML

[R38] 管道串联
来源：http://blog.bbcook.cn/Article/details/gysyzfdtr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.tarul.cn/Article/details/gqwdmcddj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.yfazqb.com/Article/details/gewadivut.sHtML


<!-- 参考信息 -->