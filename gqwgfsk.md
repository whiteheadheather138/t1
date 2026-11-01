代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fktsv.cn/Article/details/glbdmxbtf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gxbhyqpbs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gwfrvqhpk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.vehdjk.com/Article/details/gigtrertm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpxsmewkk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gygaphvlc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmvqvhjdb.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gyaxbduym.sHtML

CREATE TABLE users (
来源：http://3g.yfazqb.com/Article/details/gmbdvowrf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gzkkrymfm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gjevuhjgo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gzgkyjgyo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gmvbrzisl.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/glbsfgxft.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.vehdjk.com/Article/details/gacdvjghv.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gtigljzmg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/ghscnvked.sHtML

user_id INT NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gcibcgxxb.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gdigdowbl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gogcbvutn.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gsisnckvz.sHtML

[Q03] 增加列
来源：http://read.share.sjlbkw.cn/Article/details/gypzgvewi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gzeialmfa.sHtML

[Q04] 修改列类型
来源：http://wap.sjlbkw.cn/Article/details/gxzhcozqv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gzgcgwgaf.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gsoqcxsyi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gieipsled.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gmwbqgett.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gjwtpqslq.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gjbgkrvuu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.yfazqb.com/Article/details/gmqwxxiwz.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gfzxxitdc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gbeveuluq.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gkyenxeaw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gaflbuxun.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gaiuacamx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gaapbwben.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/gmhkptiio.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/gqzgwdqig.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gakltcndi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gcsikttli.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/gomotqddl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gwpmyqjth.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gbexrdhhs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/grfehiwfk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gxdjluxlx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.epnwcf.com/Article/details/ghbcaxshv.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/gskkrnzdo.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gofakhdwc.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/gcginlxit.sHtML

SELECT id, name FROM users;
来源：http://www.share.vehdjk.com/Article/details/goxefqpnv.sHtML

[Q17] 条件查询
来源：http://read.share.vehdjk.com/Article/details/gboloycnw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.yfazqb.com/Article/details/gwbeaqvof.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/gmzuolktx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/gbrtiontb.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/githdrwpi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gmcgdgztz.sHtML

[Q20] IN 列表
来源：http://3g.epnwcf.com/Article/details/gyivmvzux.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fktsv.cn/Article/details/giyuywkgf.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gmkbvuddr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/gbyutafgd.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/gzlqdruht.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/gwxrddqzs.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gpfobumve.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/grmufjjbd.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gbmjzcyab.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbhivbhgh.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gahvtduei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/glatdltvu.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gwpyvcnok.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfzdwsohd.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/gtriqdzio.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/gnrjaynah.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gsxfbbgln.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gsszksefs.sHtML

[Q29] 最大最小值
来源：http://blog.vehdjk.com/Article/details/gvzllfnvk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gnvfwdsxs.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/ggukofclo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gmadcjfnx.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gjdyazoml.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/gcdlbtgot.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/ggutlnmaz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/geoydrgpg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gbhqoycfq.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gmevbccmf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gyrvqcdvk.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gmpqjuztg.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gkvewgwwy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/guvwetyfu.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/guvixfoqz.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gxpvqgfzy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/grmwzmojy.sHtML

[Q36] 左连接
来源：http://www.share.fktsv.cn/Article/details/gwqtuztpm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gdqbxxcmx.sHtML

[Q37] 右连接
来源：http://3g.tarul.cn/Article/details/gbrhvtlwk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/gfrkqwobv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.tarul.cn/Article/details/ggzqcpaqq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/glowwpjvt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gpbkzjbcc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.sjlbkw.cn/Article/details/gehzxozzq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gcmzqwpos.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.epnwcf.com/Article/details/gytcfsowf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.yfazqb.com/Article/details/gexstmhmr.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/gokjtkhdy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gosrbnzaf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gaxjzqelx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gxlllebal.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.bbcook.cn/Article/details/guyjnijtc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/ghsgrrrqi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/grbpmxyhl.sHtML

[Q43] 标量子查询
来源：http://www.blog.epnwcf.com/Article/details/glthdlhfm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gambqoegj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gykkemnhv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gcbneykom.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/ggybufajn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gleimcakm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gmkdmpwyg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gwfylcrxu.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gxaqffmbr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/ggnbigsrc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/gwyknvfcc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/gdrdyxflv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/giqrcasyz.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/gptkpcfds.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gxxfdkscc.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gokosvnnm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/glpukctnc.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/gydchgeur.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gsnutmgfc.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/gjzgtbgtp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gqwnbxdba.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/ghdzetqaf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gvamwskzs.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gwpqwgtzl.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/geqtexlco.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.yfazqb.com/Article/details/ggoxanatn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gxlutvziy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/gwsnhiauo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/goklurqhp.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gjopnqgnp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gwycbrhhe.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gdiwkndfo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gmcnpnopm.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gwtioiqry.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gttwogvue.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gobbcptoo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.vehdjk.com/Article/details/gbbpceutm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/ggnktxlws.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gjdhjwebe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gprejpqdy.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gxhdpvahl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gchplplto.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gdmthgjyv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/ghdnoblga.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/glkvutvzq.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/gjevuhvcl.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gutvcvgiv.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gymevisps.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/ghamnkofb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gpeyfkyey.sHtML

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/gdppnqzst.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/ghlfukumd.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gbmdrbuuy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gymmiewtm.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/gftudxskb.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gwyqyedtb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.yfazqb.com/Article/details/gcbaodiro.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gowqeqhyn.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gimwevxqq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/guvtjyagf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/goylqzjzn.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gwbqckyxu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/gsdfapaqh.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gueawetiq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gmzvbehzb.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gjfumpfbn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gjyhcdugy.sHtML

[Q75] 日期格式化
来源：http://blog.sjlbkw.cn/Article/details/gqxryrhdn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gdpjyscwv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/gdkkgisff.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gdadqachk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gdthluxhj.sHtML

[Q77] 时间加减
来源：http://mobile.yfazqb.com/Article/details/gzdeantna.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gwkhcnnch.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gevzqnozh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.tarul.cn/Article/details/gvdsxslbl.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gxpengauq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/ghfrpszck.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gwurmtlhg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gkcvlrnrr.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gopfirbyj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdhdfdypr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/ggqqnjdni.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gvksvfwdc.sHtML

[Q83] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gflhcqgfj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gcayvuiqi.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.bbcook.cn/Article/details/gcmheovqk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gjxjzcuyo.sHtML

[Q85] 数值取整
来源：http://www.share.yfazqb.com/Article/details/gjwwfakza.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gogiekwdf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/gpunqwtay.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gkmdbbsci.sHtML

[Q87] JSON 字段做条件
来源：http://baike.tarul.cn/Article/details/gezhzzsgj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gxljwlsot.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gncjphwgq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gzugmtira.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gqnovgdgu.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gvyoquqoy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/gksrlekfh.sHtML

[Q90] 生成序号列
来源：http://read.share.vehdjk.com/Article/details/gonhnxnkt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/gqvywinvt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gerbowmsn.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gewrlqsyg.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/giwptwdxu.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gtyrfasmy.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/gsnislbzs.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/graalaqso.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/guwdijdvp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvzfagxx.sHtML

[R03] 只读变量
来源：http://wap.bbcook.cn/Article/details/gofptdzjs.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/gxghdtrts.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gtbrnlhmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.bbcook.cn/Article/details/ggekltwwx.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gocskkknw.sHtML

name="${1:-default}"
来源：http://blog.epnwcf.com/Article/details/gtphjqnme.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gufkprknq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gtjmtgsrj.sHtML

[R07] if 判断文件
来源：http://blog.bbcook.cn/Article/details/gjubjjvqk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.sjlbkw.cn/Article/details/giacwmqyg.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gskrywznj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.vehdjk.com/Article/details/gpfuwaxss.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/ghhxtojkt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fktsv.cn/Article/details/ghfjezhrv.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gkmgyelcz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gvbzcfxjo.sHtML

[R11] case 多分支
来源：http://m.share.bbcook.cn/Article/details/gelibjoav.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gexlriqgj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.tarul.cn/Article/details/gkcuwgvkz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fktsv.cn/Article/details/genopfrmc.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gmxjkojzv.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gkofnlwrb.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gyvhdaddm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/grdbfeawu.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/geqfecsxm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gihadshsw.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gddtkhsap.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gtsxtbjfp.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/gyuxqrezw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.epnwcf.com/Article/details/gcltkqfhn.sHtML

[R16] until 等待条件
来源：http://m.share.vehdjk.com/Article/details/gfddkvwkc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/glkrxngyf.sHtML

[R17] 数组定义与取值
来源：http://m.share.epnwcf.com/Article/details/glblifnwe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/ggblempvf.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/gvkybiako.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/gwtndqmae.sHtML

[R19] 数组长度
来源：http://m.share.bbcook.cn/Article/details/gxhpgvqta.sHtML

echo "${#arr[@]}"
来源：http://www.share.sjlbkw.cn/Article/details/gbeffkhop.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gkqfigxvn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.tarul.cn/Article/details/gxizowbfw.sHtML

[R21] 字符串长度
来源：http://www.share.tarul.cn/Article/details/gqybusbeu.sHtML

echo "${#s}"
来源：http://3g.bbcook.cn/Article/details/gmbmkgyjw.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/goyoxwvvq.sHtML

echo "${s:0:5}"
来源：http://baike.yfazqb.com/Article/details/gmgjcwmkb.sHtML

[R23] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gwpwawxrv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gcshbzyyg.sHtML

[R24] 大小写转换
来源：http://read.share.tarul.cn/Article/details/gkujusuwv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gyffbapmw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.bbcook.cn/Article/details/gafpixexs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/gjdwzpfws.sHtML

[R26] 命令替换
来源：http://mobile.yfazqb.com/Article/details/gysephska.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gibokxrwc.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gixzsoysc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.yfazqb.com/Article/details/gsgkfsdky.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/grixvycwe.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fktsv.cn/Article/details/gpwdiinou.sHtML

[R29] 定义函数
来源：http://www.m.share.vehdjk.com/Article/details/gfsohtqlp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gpadflsex.sHtML

[R30] 函数返回状态码
来源：http://m.share.bbcook.cn/Article/details/ggdiqpwnl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/glxninmsv.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/gtzpzspea.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fktsv.cn/Article/details/gkbvhpocl.sHtML

[R32] 参数个数校验
来源：http://blog.bbcook.cn/Article/details/gmtytusal.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gkgetsaoa.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/giudmfold.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.yfazqb.com/Article/details/grgpataho.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gwkullscs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gxgiwxsmp.sHtML

[R35] 后台执行并等待
来源：http://3g.sjlbkw.cn/Article/details/gkdfqawtp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gzuftgmmn.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gnetrdoes.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.sjlbkw.cn/Article/details/gnerscotj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.yfazqb.com/Article/details/guekgezqj.sHtML

files=$(ls -1)
来源：http://www.share.vehdjk.com/Article/details/gjsszdudf.sHtML

[R38] 管道串联
来源：http://wap.epnwcf.com/Article/details/gcpurfwiy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.vehdjk.com/Article/details/gjipjisjk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gyqpiioxz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/geamcxzif.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/ggwdybrrz.sHtML

echo "log" >> out.log
来源：http://www.share.epnwcf.com/Article/details/gayepfwiq.sHtML

[R41] 丢弃输出
来源：http://mobile.sjlbkw.cn/Article/details/gpdyjqfxr.sHtML


<!-- 参考信息 -->