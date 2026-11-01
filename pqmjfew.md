代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/ghfeypucu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/grgaqaetv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gnupdfoep.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gvgkgyakz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdunmzjox.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fktsv.cn/Article/details/gzvgbmavu.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gmuewiwlq.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gcpuktvzk.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gydkymtet.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gmzieuysf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gtobwnfpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/ggvvbovei.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gremuwtyr.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gspvzvqde.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gnaxnpolv.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/gmxotbrvr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gquzwvvwt.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gtklxyopm.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.bbcook.cn/Article/details/gkdcxvjfj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.yfazqb.com/Article/details/glmyzucds.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gkftfymgz.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gsaqljreq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/govbyzftr.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gybsrxztf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gxjewohvp.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gahitvmeq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/ggiunmhfk.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gkslyeuwv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gnesrjuad.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gtphgwvxq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gdklydcfs.sHtML

[Q08] 创建普通索引
来源：http://baike.fktsv.cn/Article/details/glayliveu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gwjyrixco.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gfkntfkhg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gycnrbgjo.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gaxncepcr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gkbwdsdjm.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/gmxhedqjr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/gefwoshog.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gkiwancvf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gkoytnuxq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gtzoruahw.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/ghjqzruns.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gckzsfdjj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gceuphulw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/grnmpeeaa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/grfwjhevc.sHtML

[Q15] 查询全部
来源：http://baike.sjlbkw.cn/Article/details/ggujjgiyw.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gjdzygwes.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/giqscymjh.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gtckezimd.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/gtcvafatn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gsvgbnpeq.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gltqsdlmw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/gkvnzqtwz.sHtML

[Q19] 范围查询
来源：http://mobile.sjlbkw.cn/Article/details/grmwzbkdq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gpwaayozf.sHtML

[Q20] IN 列表
来源：http://mobile.sjlbkw.cn/Article/details/gvdbnnohy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.sjlbkw.cn/Article/details/gjuxlyhcw.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/gabvpkzte.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/glzqbupli.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/glnwqetaj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/glevxoreh.sHtML

[Q23] 分页
来源：http://m.share.fktsv.cn/Article/details/gkvfmjtqd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gfktnrkmx.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/gnesymnts.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxvwhurfx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gijowthhy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.yfazqb.com/Article/details/gigpasokc.sHtML

[Q26] 计数
来源：http://m.share.vehdjk.com/Article/details/geedimowh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/grcblfiuu.sHtML

[Q27] 条件计数
来源：http://3g.sjlbkw.cn/Article/details/ggmcsnafv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gnglxzfhb.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gmvtkxevj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gajrdscsw.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/gnwdtzdmx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gtjksetqo.sHtML

[Q30] 分组统计
来源：http://www.share.epnwcf.com/Article/details/gzjfmedug.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gcctfniod.sHtML

[Q31] 分组后过滤
来源：http://www.blog.bbcook.cn/Article/details/ghmxekfvg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gjltvyjhb.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gqqaspwqq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gcoggpivj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/geqqfgnpx.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gitrkrcox.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gyvvlbvrm.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/gwmtknpil.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/gelashxca.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gcohannjb.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gjjqkmbwf.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/gzvscdtlw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gtuhnnkuv.sHtML

[Q36] 左连接
来源：http://baike.sjlbkw.cn/Article/details/gxmjexawk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/geofgdzkb.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gyeoudwpt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/ggxjogfoe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gclcwrhkx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gbgjqwdej.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gyvegvnyx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/gbgfnzjsk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gmalrketg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gzzmttskl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gjubbdgrk.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/ghgrisvnk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/gilgphwox.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gtufumqmn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/giwbxljqs.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/geknoowpt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gyjdyhdwf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gksflyceu.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/ggpzibvhe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fktsv.cn/Article/details/gtzgkvgmn.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/ghjctqnir.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gyjkjjhem.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/gavemrzay.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gndcijuhb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gqkqlobjq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gunwgczmh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/guvudsmdr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/giuhqrnas.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gbetrkfpt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gcknrqskk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gplivycoi.sHtML

[Q49] 更新单行
来源：http://mobile.vehdjk.com/Article/details/guwykeyho.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gbencqvmr.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gvtqutuiz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gpghmitvu.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gmsvlanjz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gdvtfawgn.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gghqpadcs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gfiwwglgz.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/gvnilpgdl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.vehdjk.com/Article/details/gyswconpg.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/giqireuun.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/gkcltxvqx.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gonqlurjz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gxuwslhxx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.vehdjk.com/Article/details/gngtrkupl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/gdptihcui.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/ghefcsvwu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gwbutddbu.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gzstlkwms.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gfnrzpahg.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/ggqzbmnwc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gpuuflsnu.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gzdurknln.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gysnhcfve.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gjbdimenp.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/gjozerfgx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gwhveqtak.sHtML

[Q62] 分组占比
来源：http://www.blog.tarul.cn/Article/details/gyimikzes.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gwhyjwgwf.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gkiwciyir.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gpffzzanc.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gzvkdgedq.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gbbkrfwhe.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gkuphwobd.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gpipacfxh.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gprealuxx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/ghklteobk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gyfrqqikg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/gcrrdnuyw.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/geezvejfo.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gmqlwgkma.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gsbptibxx.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/geqvrghpi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.tarul.cn/Article/details/gtjjsxmwi.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gtgzclktd.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gthepejic.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gbvqqkals.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gtuonpxfu.sHtML

[Q72] 查看索引
来源：http://www.share.sjlbkw.cn/Article/details/gporitisa.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/gsyylucnx.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gwncjfxkg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gegugwjgg.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/gaqiwlfki.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gfagpgciy.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gkmdouvwn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gvvpqukjo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gdtcvcpub.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gklswbifd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.tarul.cn/Article/details/gbcjprveq.sHtML

[Q77] 时间加减
来源：http://blog.tarul.cn/Article/details/gqpygajbv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gaitduvkb.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gtvrzdaml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gvtrmmwbn.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gszxtvlwh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gsqbzooxl.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gcjcucejt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gdiyurbzr.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gddexfsum.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gmkyrsfae.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fktsv.cn/Article/details/gsmfdxxwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gtyshsvry.sHtML

[Q83] 大小写转换
来源：http://3g.vehdjk.com/Article/details/getapzrnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gtfashlad.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/grffjlbkd.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gvcbzhcek.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gelwvglzk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/gdojbdnoc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/glowfvjmd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.vehdjk.com/Article/details/gslrcyimh.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gejuhlpwc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/guiztwnsn.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gurizyrpt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/gagspcdqi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvkglholh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gkbkkpuca.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gaxzylpye.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/gehzdyvod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gypxymdtl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gephamnks.sHtML

R. Bash 专题
来源：http://m.share.bbcook.cn/Article/details/gkpelmelv.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gilmqwule.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gzglhqunl.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gbbhxhevo.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gcconifvr.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/ghontslgv.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/gxqlgmitv.sHtML

[R03] 只读变量
来源：http://www.m.share.vehdjk.com/Article/details/gggguowtd.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gjqnuvquh.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gsafdbekg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.tarul.cn/Article/details/gqzzumfmb.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/gcrkdochw.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gyybmtgbk.sHtML

[R06] 判断命令是否存在
来源：http://read.share.tarul.cn/Article/details/glushiimh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/ggnzmqmty.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/gechgjuuy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gqbyxjwzc.sHtML

[R08] 数值比较
来源：http://baike.sjlbkw.cn/Article/details/grzywasvj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gaibzjoml.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gjsxnimos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.yfazqb.com/Article/details/grkhdyawx.sHtML

[R10] 正则匹配
来源：http://wap.sjlbkw.cn/Article/details/gygqrhaha.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gcjxhspej.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gmhivticn.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gtkqcmhgj.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/grgwpcobf.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/gepdfjwvz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/gcaqbhjaq.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gnghbmrcr.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gsnhtzfcj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.tarul.cn/Article/details/gewpinsji.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gneughuzj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gasixevbd.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/glogtequn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gmvsxzbmf.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gikwhyvld.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.vehdjk.com/Article/details/ggmwpvsfg.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gyiskogxl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gucjcrhps.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fktsv.cn/Article/details/gxcihcpfn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gfqokwrcw.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gcjdhufae.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.tarul.cn/Article/details/gorvkwprw.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gkxqunitt.sHtML

echo "${#arr[@]}"
来源：http://read.share.yfazqb.com/Article/details/gbkeztyva.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gqgfjkttl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/guwhuedgt.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gwrwciyxg.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/godiqcsta.sHtML

[R22] 截取子串
来源：http://3g.yfazqb.com/Article/details/ginzbkyqk.sHtML

echo "${s:0:5}"
来源：http://blog.tarul.cn/Article/details/gtdpfvuwk.sHtML

[R23] 字符串替换
来源：http://blog.epnwcf.com/Article/details/gbylscwmf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.vehdjk.com/Article/details/gyjmuqxvt.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/ggbitwfcz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fktsv.cn/Article/details/gnmnnjuzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/ggacqoyxk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.epnwcf.com/Article/details/gzxrumaza.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gfusxtkni.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gzqpffmje.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gguogezmh.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.epnwcf.com/Article/details/gyhfqnuol.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gholigufk.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/gacwjukez.sHtML

[R29] 定义函数
来源：http://www.share.sjlbkw.cn/Article/details/gfskujabd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/ggocquqop.sHtML

[R30] 函数返回状态码
来源：http://m.share.yfazqb.com/Article/details/gantxhzao.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gwzqslyvo.sHtML

[R31] 局部变量
来源：http://www.blog.yfazqb.com/Article/details/gyhmcwlbr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/gvtatfpcu.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gaxdnpilm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/ggzsaqjay.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.tarul.cn/Article/details/glhvqabxj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.sjlbkw.cn/Article/details/giuwdbwvi.sHtML

[R34] 退出时清理
来源：http://m.share.bbcook.cn/Article/details/gizqmovuh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gjoizwnec.sHtML

[R35] 后台执行并等待
来源：http://m.share.epnwcf.com/Article/details/gcqrqpetz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/gegdxbygd.sHtML

[R36] 并发执行多个任务
来源：http://baike.tarul.cn/Article/details/gjitzqwdp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.yfazqb.com/Article/details/ghmqayhmh.sHtML

[R37] 把输出赋给变量
来源：http://blog.epnwcf.com/Article/details/gudlzwamv.sHtML

files=$(ls -1)
来源：http://mobile.tarul.cn/Article/details/gdxuvhjlq.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gkgtphhyt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.yfazqb.com/Article/details/gcczpjxac.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gnfmpqrif.sHtML

cmd > out.log 2>&1
来源：http://www.blog.bbcook.cn/Article/details/gyifwnduk.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gmfeqcidv.sHtML

echo "log" >> out.log
来源：http://m.share.fktsv.cn/Article/details/gfktguicw.sHtML

[R41] 丢弃输出
来源：http://read.share.vehdjk.com/Article/details/gdevaxdxk.sHtML


<!-- 参考信息 -->