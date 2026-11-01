代发 wailian999

CREATE TABLE users (
来源：http://wap.sjlbkw.cn/Article/details/ghzfsylzb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gmemcvdno.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gmvnadchf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/gerpczcua.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.yfazqb.com/Article/details/gsjcbtpuo.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gvgegedxh.sHtML

[Q02] 创建带外键的表
来源：http://wap.fktsv.cn/Article/details/gmzrlcmyv.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gzpxrwokk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gjuvktkvj.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gnrgxuimo.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gkvlxkjit.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/gscifyjvy.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gmokqjdho.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gwbfoqclo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/gbjgywwyo.sHtML

[Q04] 修改列类型
来源：http://3g.vehdjk.com/Article/details/gqtvkjsav.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gcqbwjiqt.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gcjohconk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gyqzbfmht.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/ggxhxykzl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gxzqdxneo.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/grnppmcft.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/gltowoqel.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gfowogtoo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gzudynsdh.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/grpykttkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/ghssrqnqo.sHtML

[Q10] 插入单行
来源：http://3g.yfazqb.com/Article/details/gxscszxqb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gcnrivhll.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/ghysgbxae.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gnaxiptlw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gveihxomr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.tarul.cn/Article/details/govfuzrsz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.vehdjk.com/Article/details/gfnawiyfb.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/gpjrtkrww.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/ghkpnxcwd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gyhqbroan.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/ghlubdnhr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gztofuhkb.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gzrjtrjhm.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gzpkjxdtt.sHtML

[Q16] 查询指定列
来源：http://www.share.vehdjk.com/Article/details/gwhusself.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gfdfubwoj.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gsdpnsbcu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/gtcahllsz.sHtML

[Q18] 模糊匹配
来源：http://read.share.fktsv.cn/Article/details/gjzyjfncv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/gilhuyyzz.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/gxlpreyra.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gzlbkxido.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gkzlxtiwj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gkdbkcppg.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gamrwyfwn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gvboukbfp.sHtML

[Q22] 排序
来源：http://www.blog.tarul.cn/Article/details/gfpcbiakn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gtfessxxf.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gexbykfnp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.tarul.cn/Article/details/gqtlfqddn.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gzmzcxpij.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmdlprmwq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gfysmscgk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/gmgaeyiji.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gklkufltb.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gogbxmhjn.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gfzzzpkcs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmksynrcb.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gifcnbril.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gvmfdrpmq.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/ghjsdlykm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gyawguoop.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/grunxguhs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/grdimvsob.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gzrrdnrhi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/grejlwyym.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/guqollmyk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/glsajnvum.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/guwjkdjwg.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gvbqfukzi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gyylkxzfd.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gzxckjybq.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gcxshfjft.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fktsv.cn/Article/details/grapzckmk.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gvplczket.sHtML

[Q35] 内连接
来源：http://www.m.share.vehdjk.com/Article/details/gibjstazu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gnkpsnizp.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gyyiabian.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gwdriijwf.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gsbagbyos.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gsvratnqu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/gggqmhqat.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gtyrqaxxw.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gylqwqugv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gjtutmfba.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gnnwdtahq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.yfazqb.com/Article/details/gbnfdhvvk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/ghivnzeaz.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gzchdobjz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gtxhhcvyg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gduyczjzt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gwwauhtkd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fktsv.cn/Article/details/gstkjiqhs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gjixxtleg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gjzqjqseg.sHtML

[Q43] 标量子查询
来源：http://read.share.epnwcf.com/Article/details/gjrmdbthx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzardtsrr.sHtML

[Q44] IN 子查询
来源：http://m.share.vehdjk.com/Article/details/gpewzclix.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gkcepfzqz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gushnyceo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gbdqzwxmq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gbyunjkxp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gohmjhhey.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gvucbuseb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/gffwstwuq.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gvdlzwqne.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gnmeqmdjr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gkppoihop.sHtML

[Q49] 更新单行
来源：http://baike.epnwcf.com/Article/details/gyovakqix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gwlkgncqq.sHtML

[Q50] 批量更新
来源：http://www.share.fktsv.cn/Article/details/gxwncsaal.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gghwujzkh.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gkrvnpaho.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gtogxgbst.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/glenuyavo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gzzinaqzp.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gaadsykgk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/geuggxbrm.sHtML

[Q54] 清空表
来源：http://baike.fktsv.cn/Article/details/gkgmxoiwi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/gnczbkxmq.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gkdctfxfo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/grehcayju.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gjaedvvau.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gvfppwvee.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gkuxebluc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gehumdfdi.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gumhonqwu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gnushmavc.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gsrmpgoqn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gaatppzus.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gtijdcczn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gvjvriguq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gignmwbte.sHtML

[Q61] 移动平均
来源：http://read.share.yfazqb.com/Article/details/gwxtsyvxt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gvpohioqx.sHtML

[Q62] 分组占比
来源：http://blog.fktsv.cn/Article/details/gxjsusoar.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/guxcsibps.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gkjbuksvh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhqldkyy.sHtML

[Q64] 提交事务
来源：http://baike.tarul.cn/Article/details/gqnyjhssh.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/grvoptnsm.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/guogspgsg.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gcfmzbkad.sHtML

[Q66] 行锁查询
来源：http://mobile.epnwcf.com/Article/details/gzpqwbufa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gtcwejowt.sHtML

[Q67] 设置隔离级别
来源：http://m.share.vehdjk.com/Article/details/gwdotmanc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gntdmbgtu.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/gqrfzcqes.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/gyshcuabh.sHtML

ROLLBACK TO sp1;
来源：http://read.share.bbcook.cn/Article/details/glvlqmvrq.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/gezozqchc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gbizvnidz.sHtML

[Q70] 更新统计信息
来源：http://blog.vehdjk.com/Article/details/gieuczwec.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gcghzfknx.sHtML

[Q71] 查看建表语句
来源：http://baike.vehdjk.com/Article/details/gbdhoasle.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gevfdwaex.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoosfxhb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqoxxlnre.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gjswxrubm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.yfazqb.com/Article/details/gvdzxrxkd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/ggfalozbf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.vehdjk.com/Article/details/gtjfnjnya.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gueemxvxo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/gfijunlbb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gjeoasksj.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/gziktwcfb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/gpzhghped.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gkjiilnug.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gayzwgqdm.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gkcosxoxr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gvyaryfwv.sHtML

[Q79] 字符串拼接
来源：http://www.blog.yfazqb.com/Article/details/gxemupyzf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.vehdjk.com/Article/details/gbxdrbsal.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/guunuzucz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/glcpddlcp.sHtML

[Q81] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gaecjqnlr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/giciolank.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fktsv.cn/Article/details/gmwxirglq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gwsbtgufj.sHtML

[Q83] 大小写转换
来源：http://blog.tarul.cn/Article/details/gsepkphre.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gzevxhsxh.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/gwrzjavjj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gujaqoxwi.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/gocwtqrgf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/ghbpicfhy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.vehdjk.com/Article/details/gwujpdpva.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.sjlbkw.cn/Article/details/gtjfsfqtd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gggqhlsqn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/glhbgebch.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gmixiwqzn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.tarul.cn/Article/details/gdvrsccyy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gctyrimwj.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gnqscfvzv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gxejkhyom.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/guetipppb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gwrtqtdzb.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmzepvpki.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/gbfklmkvg.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghcrnssbx.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/gkcocnfpb.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/gcglucqmy.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/gntmkdsat.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gkcvgvbkw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gnkffofrb.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gjwbttuuv.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gtzotmysv.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gcfnuspzj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gtjxgvrwu.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gzvkxrmqq.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/guhgupgco.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gjengmmnx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.sjlbkw.cn/Article/details/gfmjmulvb.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gbtksfwzq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/giblunqmz.sHtML

[R08] 数值比较
来源：http://3g.sjlbkw.cn/Article/details/gerzzjltt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.bbcook.cn/Article/details/gqbpvglla.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gyfdrpuhk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gedlexolb.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gxptigoog.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/gxhytjkht.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gzbfdcgmc.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gjzbfbofg.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gvijjmldo.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gtoakohij.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/gkhnsoyyb.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/gmnziflyn.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gnsbupsqs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.bbcook.cn/Article/details/gfjffoqwr.sHtML

[R13] for 计数循环
来源：http://wap.yfazqb.com/Article/details/guiiydqbx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gdydmnqsu.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gghdhsiji.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/gxpedzasx.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gaxjwyypi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gqmbrqgpr.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/ghzjjiyof.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fktsv.cn/Article/details/gvvmafxhk.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/gsngslfkg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fktsv.cn/Article/details/ghtztgzkl.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/gkfxyyudd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gclbpffsf.sHtML

[R19] 数组长度
来源：http://baike.yfazqb.com/Article/details/gewobgitl.sHtML

echo "${#arr[@]}"
来源：http://3g.vehdjk.com/Article/details/gypsnguoq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.vehdjk.com/Article/details/gkccwgibr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.epnwcf.com/Article/details/gwqdiduda.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gnuuesckh.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gnytagajr.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/grobxkiid.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/glokhzvxu.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/glgvkpfoj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/grgkvepef.sHtML

[R24] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/goygfdysu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/glevlnbya.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gascgmzbw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gtyftkxhp.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gjctvqlzf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gryhzjyls.sHtML

[R27] 算术展开
来源：http://www.share.epnwcf.com/Article/details/gwrpjnfvb.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.vehdjk.com/Article/details/gunovcarp.sHtML

[R28] 浮点运算
来源：http://www.blog.tarul.cn/Article/details/gagpvckdn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gyibfnisc.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/goqlixhod.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/ghdxxyxmw.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/gpbhakjtt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.tarul.cn/Article/details/geamxvkrp.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/guizhjxjp.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gphzdydja.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/gyncwtpex.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gayscdgpe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gckdufybn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.epnwcf.com/Article/details/grdpscyfb.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gpdjiurbp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/gjdvarvrm.sHtML

[R35] 后台执行并等待
来源：http://m.share.fktsv.cn/Article/details/gdgvfxnju.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.tarul.cn/Article/details/gnupubdcc.sHtML

[R36] 并发执行多个任务
来源：http://baike.vehdjk.com/Article/details/gxvpttowz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.yfazqb.com/Article/details/gmwyekwma.sHtML

[R37] 把输出赋给变量
来源：http://m.share.vehdjk.com/Article/details/gocwdtcsw.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gbtgrprsy.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gnwgmnuas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.sjlbkw.cn/Article/details/gesvafwbc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/gzxezvngt.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gvopdrhvr.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gbyctslei.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/ggzyzavdh.sHtML

[R41] 丢弃输出
来源：http://mobile.fktsv.cn/Article/details/grpmipaif.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gvlpbzizq.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gaotbryib.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gwyhcmrwb.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/govirvkvc.sHtML

find . -name "*.log" -type f
来源：http://3g.vehdjk.com/Article/details/gmynstwls.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/gpvxlezea.sHtML

find . -mtime -7 -type f
来源：http://mobile.sjlbkw.cn/Article/details/gfmexumzh.sHtML

[R45] 批量删除
来源：http://3g.fktsv.cn/Article/details/gkxkgghba.sHtML


<!-- 参考信息 -->