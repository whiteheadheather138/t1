代发 wailian999

);
来源：http://blog.fktsv.cn/Article/details/gewxtinye.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gxwfacazz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gzhenujgg.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gjcgvtmph.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/glqdqvhch.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxxslkgl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gpdglyelj.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gtjjlhrfc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/gktsopgog.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gxrejesxs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gimclrtox.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gfwymfcxf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.bbcook.cn/Article/details/gsslwsgyv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gujfmaavh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gymefpdzn.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gqarazazt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/garrvikja.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gapxmhckl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.yfazqb.com/Article/details/ggynwrhxs.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.sjlbkw.cn/Article/details/graveiaen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gwbuvfhkw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gcllhoasg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.epnwcf.com/Article/details/gzicyfbvz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fktsv.cn/Article/details/gurtmthds.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/glfdaiwrv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gqvytqofi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/gmtctquiz.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/ghpoejztj.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gwergwjpv.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/ghxmsugcc.sHtML

SELECT id, name FROM users;
来源：http://read.share.tarul.cn/Article/details/gruyiocis.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/gamgitwmv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gksvfsyqa.sHtML

[Q18] 模糊匹配
来源：http://baike.fktsv.cn/Article/details/gqztxjcde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gtthqqnfi.sHtML

[Q19] 范围查询
来源：http://mobile.vehdjk.com/Article/details/gnkhdophl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/gtnddhqsy.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/grwtynqsm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gkkreozpr.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gfwdgywml.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gzylxicij.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gnbwsvutw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gggyiuzxf.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gyxqgtdgw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gmqysnwiw.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gafckydid.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gkxhwzpoa.sHtML

[Q25] 只取前 N 条
来源：http://baike.sjlbkw.cn/Article/details/gyvwcuozc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gqohoralc.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/gkramdtpx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/gabqwdvoa.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gotpnglun.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gltkoflxd.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/gsvwzychp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gtpaxansg.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/geqxrnwfm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfdlwpwai.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/ggspnmwwu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gedqjwxjd.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/gqbmjpzrw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gajoheyvq.sHtML

[Q32] 分组拼接字符串
来源：http://3g.bbcook.cn/Article/details/gmcprgavo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gbaybxuhw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gozcsobpj.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gfkvdiebo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fktsv.cn/Article/details/gplqqkekj.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gshxgjneq.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/gxrgobjnq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gbsojydtf.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gtizerufp.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gabgxxzbn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gwyrrrhys.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gvsncadhe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gmoyrhghg.sHtML

[Q37] 右连接
来源：http://www.share.fktsv.cn/Article/details/gljvkoumy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/gawcrpaei.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gyryjpkxo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gqyujolci.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/ggwiomlim.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gqdlztsvc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/ggibpfemx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/geiossatg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.bbcook.cn/Article/details/gvcqpwyef.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/gofsaclkr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gglsauirf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gojzhgyut.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/geaytmqsz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fktsv.cn/Article/details/gopinsash.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gptaimcnv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gymuqhpdo.sHtML

[Q43] 标量子查询
来源：http://baike.bbcook.cn/Article/details/gyccadjiv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/glhxnoxqs.sHtML

[Q44] IN 子查询
来源：http://m.share.vehdjk.com/Article/details/gdsdokupo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.yfazqb.com/Article/details/glaqwqhra.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.vehdjk.com/Article/details/gzfwqiwhg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gubjppcvk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/geckcrwpo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/gysjuoqva.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gbueovvye.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fktsv.cn/Article/details/gemglnict.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gxxvqzhvp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.vehdjk.com/Article/details/gryhprnyt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.bbcook.cn/Article/details/grpokidpl.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gjlhfaaon.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gmhyfiqku.sHtML

[Q50] 批量更新
来源：http://www.blog.tarul.cn/Article/details/gtliugqoz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/gqgzcexcf.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/gtoieguwr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gwljkbzsc.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/grfwnkapx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gcckgeqlr.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gysokhumb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gposywquv.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gsakxpjbt.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fktsv.cn/Article/details/gzoypnqji.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fktsv.cn/Article/details/gmznhaobh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.tarul.cn/Article/details/gwrbgjwts.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/gnfnradrc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gjdhvryjh.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gnhguokfn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ghvwinbfj.sHtML

[Q58] 累计求和
来源：http://baike.sjlbkw.cn/Article/details/gtqbqjhxl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gfqxtmzuq.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/glzwtkmlg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gidevifgd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gnpghrudt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gnvibztny.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gurgzinze.sHtML

[Q61] 移动平均
来源：http://blog.bbcook.cn/Article/details/gwtfdrllt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gkbsaffnv.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gfidokmwt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gzvilhzvz.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gumaggtuy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.yfazqb.com/Article/details/gabrzdlrf.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gxfkyivag.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/gvubkquad.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gexpzkwzy.sHtML

ROLLBACK;
来源：http://www.m.share.epnwcf.com/Article/details/gaxvumrao.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gdpbebnnm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gnhkzihhr.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fktsv.cn/Article/details/gmrncagyi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gnratwnov.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gwywkqfna.sHtML

SAVEPOINT sp1;
来源：http://www.share.tarul.cn/Article/details/ghlwbkdob.sHtML

ROLLBACK TO sp1;
来源：http://mobile.sjlbkw.cn/Article/details/giggjprzx.sHtML

[Q69] 查看执行计划
来源：http://3g.sjlbkw.cn/Article/details/gakotoxaj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/giujqfhof.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/guwowoifl.sHtML

ANALYZE TABLE users;
来源：http://www.blog.vehdjk.com/Article/details/gohsowpqy.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gmcelalvp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gvabgzgvs.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/gxctveqtt.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gguwvvsry.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gzrwbglqv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gpzdsjbbq.sHtML

[Q74] 强制使用索引
来源：http://3g.tarul.cn/Article/details/gedzgekzn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gldrrccca.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gnnwnpzsr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/gcisesxfo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gagbswjrp.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gnyhrbxtf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.yfazqb.com/Article/details/gpeqtjpzu.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/gubatqefx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gfjkhdbpt.sHtML

[Q78] 当前时间
来源：http://www.share.fktsv.cn/Article/details/gobvkgumq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gxrduubny.sHtML

[Q79] 字符串拼接
来源：http://baike.epnwcf.com/Article/details/gdqvekvkk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.epnwcf.com/Article/details/gxlkaugjd.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/gimyjexfr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gntrwdgsa.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/ginffofnl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/gexdupjye.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/gtxktwmpb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/girvtsmeo.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gjwdddqpb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gugmqerha.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gfwmzmjzg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gapfcxrde.sHtML

[Q85] 数值取整
来源：http://3g.fktsv.cn/Article/details/guclbuwkv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gsmmsyepk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gmkxvxvzf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.bbcook.cn/Article/details/gvfbxsgdz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gngrwhnwl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/ggrzgpveh.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/gpwumdena.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gjtuwctyd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggnswqtcb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gfeffbotu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/guvxtbspu.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gfxklhyvo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/gchethnkv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkjdvwitm.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gznxymuxn.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdcpqyxa.sHtML

[R01] shebang 与严格模式
来源：http://wap.vehdjk.com/Article/details/gcowlaltf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.epnwcf.com/Article/details/geevbeupv.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gyhzskgli.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.bbcook.cn/Article/details/gvgqbombl.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gsffiyatj.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/gqdeojkjw.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gqvezcavn.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gmirutnjk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/ghxqgtoky.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/ggdqyiopn.sHtML

name="${1:-default}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgubpwsa.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gwverxylx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gcrjnaekp.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gudmyluck.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gloyseruo.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gwsgblzew.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gjqwbblhp.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gmrxlclte.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.tarul.cn/Article/details/glqrzlhee.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gbzcxhxkw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/ggtkzklzf.sHtML

[R11] case 多分支
来源：http://www.share.vehdjk.com/Article/details/gannyndfb.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gloobjasv.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gtdnafxnz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/gqcubaplb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.vehdjk.com/Article/details/geoerpzig.sHtML

esac
来源：http://baike.yfazqb.com/Article/details/gqltflnjz.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/ghgjlgfmc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gclrcylxq.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gqdncbget.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gtqjgdolt.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/glajzbrlv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gjvxieceo.sHtML

[R15] while 逐行读文件
来源：http://m.share.sjlbkw.cn/Article/details/gzaaswvho.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gsvmqllcx.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/gymdmezem.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.yfazqb.com/Article/details/gbyqsrapb.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gipmyassp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.tarul.cn/Article/details/gjnaozgoa.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/gawecdpga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gxpsuhzhv.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/giluvywqv.sHtML

echo "${#arr[@]}"
来源：http://3g.fktsv.cn/Article/details/gdepuxgmw.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gfewcdina.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gizzodmuy.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gpqxsxuei.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gidaktuyk.sHtML

[R22] 截取子串
来源：http://blog.sjlbkw.cn/Article/details/gdionqyzz.sHtML

echo "${s:0:5}"
来源：http://m.share.vehdjk.com/Article/details/gkwlmjyen.sHtML

[R23] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gtahmqnly.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/gpzpeoeqd.sHtML

[R24] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gnwpwyyba.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.epnwcf.com/Article/details/gvnelspqs.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gmbteokem.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.yfazqb.com/Article/details/gjhfzwdtf.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gstwmatzo.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.sjlbkw.cn/Article/details/gufpywwne.sHtML

[R27] 算术展开
来源：http://read.share.fktsv.cn/Article/details/glfwssogp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fktsv.cn/Article/details/gshdrxvbi.sHtML

[R28] 浮点运算
来源：http://www.blog.sjlbkw.cn/Article/details/gsnpbtvmv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gxcjhfkto.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gsnknqnkb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.tarul.cn/Article/details/gpllrzzgi.sHtML

[R30] 函数返回状态码
来源：http://baike.bbcook.cn/Article/details/ggsdqgwkj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.vehdjk.com/Article/details/gxdfxmnsr.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/goucdzetr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gesycprqe.sHtML

[R32] 参数个数校验
来源：http://mobile.bbcook.cn/Article/details/gwtzxemgd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/getkxxpmj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.epnwcf.com/Article/details/ggxypavjc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.bbcook.cn/Article/details/guvowktqt.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/geovsiwrr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.tarul.cn/Article/details/glydsimgi.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/ginjwjinq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.yfazqb.com/Article/details/gpglczqrv.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fktsv.cn/Article/details/gdonmcply.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fktsv.cn/Article/details/gpckbounh.sHtML

[R37] 把输出赋给变量
来源：http://blog.fktsv.cn/Article/details/grxjwvmez.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/gulsxzcev.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gloujrrqt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.bbcook.cn/Article/details/grogwlitb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gefzlvkng.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/gyefcuvtd.sHtML

[R40] 追加写日志
来源：http://m.share.epnwcf.com/Article/details/glnyqecgw.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gsbokadcs.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gfnqqvzcp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.epnwcf.com/Article/details/gucjtbogf.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/grumavjrp.sHtML

wc -l < a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gasqjdqqr.sHtML

[R43] 按名字查找文件
来源：http://wap.tarul.cn/Article/details/guckmdgzn.sHtML

find . -name "*.log" -type f
来源：http://read.share.sjlbkw.cn/Article/details/gycatlolt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.yfazqb.com/Article/details/gvslgaogy.sHtML

find . -mtime -7 -type f
来源：http://3g.yfazqb.com/Article/details/gtyqtxonw.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/guexqclrr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.epnwcf.com/Article/details/gffcyeiaw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gokgbenzq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fktsv.cn/Article/details/gcvwhgblj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/grjsscxmy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gupleezck.sHtML

[R48] awk 取指定列
来源：http://mobile.vehdjk.com/Article/details/ggahtbdyk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.vehdjk.com/Article/details/ggyybqtzk.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gaxheezjx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/gjejmftmp.sHtML

[R50] awk 求和
来源：http://wap.vehdjk.com/Article/details/gekekuzuo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fktsv.cn/Article/details/gtzjzoqfy.sHtML

[R51] 排序去重取前几
来源：http://wap.yfazqb.com/Article/details/gcvrbgnhn.sHtML


<!-- 参考信息 -->