代发 wailian999

================================================================================
来源：http://wap.tarul.cn/Article/details/ggidvnsjf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gncihoftv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzujtalqr.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gzhelyskb.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gcemossak.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gcmjybsdx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gqoncvulk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.epnwcf.com/Article/details/gludokarf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/gexfgtoet.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gilbfckim.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gsrlugxzb.sHtML

CREATE TABLE orders (
来源：http://3g.bbcook.cn/Article/details/gvedmikmv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gbkuslbpp.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gbqrwckgw.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/giyzwycxt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gtajchpmo.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gxhacdbbt.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gdkpnsall.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fktsv.cn/Article/details/gdkwsyady.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/gczuwaklb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gkdmxrkpv.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gnwegyfvl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gclpsjhfh.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/ggprjpeqc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gsletgbrp.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/giruwkoob.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gjjypmybx.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gjadbqnft.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gnuqcaivw.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/guyyhyltg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/glteojamf.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gtmpibnhg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gepbcthfb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkohjaor.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.bbcook.cn/Article/details/gyanrkzld.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/ggtlnmydr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.vehdjk.com/Article/details/gojwaivma.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/ggrrbjaqt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gidgnfsmt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gnrvbvgpt.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gicopbmfr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.vehdjk.com/Article/details/gmayoaqxl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.bbcook.cn/Article/details/gnkihuprd.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/ghhqingjz.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gtpwckmtm.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gifylrwmp.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gvmwdzwsi.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/gwasmheek.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gsveayyun.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/ggbbrazwp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/gbnmuhgxp.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/growjsnwq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/geiqhpqja.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/geuslvclm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gxzrabqzv.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gwiymgpqb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.sjlbkw.cn/Article/details/gcyexyjqn.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gpjspazgt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gtejucask.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/ghhsmhpoy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gplqytpil.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gtyyhlamd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/ggrvqcyxb.sHtML

[Q25] 只取前 N 条
来源：http://mobile.yfazqb.com/Article/details/gywnxljld.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/girpacozu.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gfeycehkt.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gspeuygnc.sHtML

[Q27] 条件计数
来源：http://baike.vehdjk.com/Article/details/gkjaozlyl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbahvjprb.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/gbkyhyylr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gpxbcmmci.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gllhazkuu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.yfazqb.com/Article/details/ghgfbqjcb.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/gbwldkfze.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gqaxiaxgn.sHtML

[Q31] 分组后过滤
来源：http://wap.sjlbkw.cn/Article/details/gnyhvxayx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gwqqxtsgf.sHtML

[Q32] 分组拼接字符串
来源：http://blog.bbcook.cn/Article/details/gliitqhll.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gxakdynzb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gscizgiel.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gszqiplhk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gfjywojgg.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gowvqdnjk.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/garxgyssi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gpaxonjzh.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gayljxfhk.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gezvrozfr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gbkuyrgsl.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gnvbuvnaw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gkhicbuhd.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/giahrvbhy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.epnwcf.com/Article/details/gqtanhaoa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/grxsratjj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gezxpwylj.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gzhzjznyb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gpbvivnin.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/guitcndbe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gafajjfug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.yfazqb.com/Article/details/gwnmuxnwi.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gdahjchwi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gegtkldbv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/glkdbsnwi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.tarul.cn/Article/details/gdfokfvkp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gwnxctzni.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/ganoyhlsk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gvslbqxqs.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gfxzibiwk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gkppopvyr.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/grmkyswrj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/grbkaeaxs.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/gvgjgprhi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gwvwjacov.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gwrbcytsh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gicgapecl.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gmzqqomqq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gfaznkbaj.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gjtdiahxj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/gwvxmewlp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/ghobzjllq.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gqyxljkam.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/glrlmisgo.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gojihvwtg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/gsuznmgfm.sHtML

[Q51] 用子查询更新
来源：http://m.share.epnwcf.com/Article/details/gnjatvqpg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/gottjbfuo.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gnxlybmve.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gxmhcxnxo.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/giokmgxdr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/glfxzxign.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/glznmkbfc.sHtML

TRUNCATE TABLE logs;
来源：http://baike.yfazqb.com/Article/details/gtwrpelbr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gwlsnwrgy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gggwgyduz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gipnkfzcd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gpncuyvxb.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gvpwswdot.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdfjumdp.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gqhjhyxhu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gwhvsoxly.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gbsgdjxmj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxvdbyew.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gvfrfbzxq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/giphtacws.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/ggszmsojd.sHtML

[Q61] 移动平均
来源：http://www.share.tarul.cn/Article/details/goamesnxz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gjenfhvrq.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gktmpzhff.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwdyqogbe.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gyumwdlww.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gdzwbomge.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gtbewkmpo.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gtmsaktdv.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gaetbylms.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gyhyqkaxt.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gnuuwfafg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.yfazqb.com/Article/details/gurklmwis.sHtML

[Q67] 设置隔离级别
来源：http://blog.yfazqb.com/Article/details/grkqddlts.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gmgzpsgjf.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gdfapxfgn.sHtML

SAVEPOINT sp1;
来源：http://baike.bbcook.cn/Article/details/gdyidpnej.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/giluucasf.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gecsuutdf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/gvobzeeji.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gvvdnubip.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gevzysneq.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/giiiajqfk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gttpzvkqu.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/gfyrelfej.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gipontycn.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gzcpcsdnf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gowhonzxd.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gqcefffrc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/gqdmjftaj.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gagoscxry.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gdoprjuhj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/gmvhspzqv.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gpqmvoygm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/glldrfagc.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gungcqsyt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/ghclxkbsj.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gnstyizvj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/glulajeya.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/gqjjaposn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/gauglddjr.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gyjcpiive.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gmntihmyx.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/ghzzvhqle.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gkteghuhz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.tarul.cn/Article/details/gckqapcxu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqvlnszie.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gxewdknfc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gejpynvdz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/guecjqsrn.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gdihnkbut.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gkakqpeml.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/genedzxml.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfcmtbuh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gwumudrrb.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/gtksmandn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/ggmwuvxte.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gclqxdlri.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/gvyhkkmxh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gtddlvkig.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/gzakfdccp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gumntonjt.sHtML

[Q90] 生成序号列
来源：http://blog.fktsv.cn/Article/details/gbprawsnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.yfazqb.com/Article/details/gdbeippbj.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gdljlwtxb.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gdefeeidi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gttscbfqs.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gmbsmalyq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gbimtosmp.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gvwxmhkjq.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/goueyeomo.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gfvuehvih.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gytwfmqxy.sHtML

readonly PI=3.14
来源：http://www.m.share.tarul.cn/Article/details/gxvobsrht.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gnrghoeaf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gufqnmeqb.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/gzfpobhby.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/ghaxnziaf.sHtML

[R06] 判断命令是否存在
来源：http://wap.fktsv.cn/Article/details/gnnipgujv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gcyadnvgk.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/gfgiueysf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gfgjgdpyk.sHtML

[R08] 数值比较
来源：http://blog.fktsv.cn/Article/details/gpncakanl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gbdzewngt.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gpcnsunzx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gjihwbyhf.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/gwxflgjwl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.epnwcf.com/Article/details/gnaudmbib.sHtML

[R11] case 多分支
来源：http://read.share.vehdjk.com/Article/details/gpvshvpcf.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gfnhbgtzd.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gfkowbmge.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/gkveamtrz.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gxfroyzdx.sHtML

esac
来源：http://m.share.yfazqb.com/Article/details/grzpnhufz.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gwschbcce.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/guxxwyyrn.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/germgvlnk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/germaccce.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gpitziztt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gyuczught.sHtML

[R15] while 逐行读文件
来源：http://read.share.yfazqb.com/Article/details/gwatttqcs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.epnwcf.com/Article/details/gsgbmykzm.sHtML

[R16] until 等待条件
来源：http://wap.yfazqb.com/Article/details/glusawzmc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.sjlbkw.cn/Article/details/gbcbmkjis.sHtML

[R17] 数组定义与取值
来源：http://www.share.bbcook.cn/Article/details/goghwptjt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/ghacowvca.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/gkfcpmlsi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.yfazqb.com/Article/details/gvydrjexm.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gzppgbmgm.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gveespgyg.sHtML

[R20] 关联数组（字典）
来源：http://baike.vehdjk.com/Article/details/gbszexnhl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gxqcvcgwh.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gqossbfzx.sHtML

echo "${#s}"
来源：http://mobile.tarul.cn/Article/details/gmrtmyxqf.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gfkefhcol.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gdlrrktuy.sHtML

[R23] 字符串替换
来源：http://3g.sjlbkw.cn/Article/details/gfydsroop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gevasutdl.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/ghaakburm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.bbcook.cn/Article/details/gbygrycyx.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gxpudqslr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/ggvmledpe.sHtML

[R26] 命令替换
来源：http://read.share.yfazqb.com/Article/details/gmvvicudi.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.bbcook.cn/Article/details/gwhiavgii.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/ggwymapqk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/guqmrzgea.sHtML

[R28] 浮点运算
来源：http://blog.fktsv.cn/Article/details/gvczkwquf.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.sjlbkw.cn/Article/details/gywszrjgc.sHtML

[R29] 定义函数
来源：http://wap.bbcook.cn/Article/details/gobplbmcd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.bbcook.cn/Article/details/gksdyxlod.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.vehdjk.com/Article/details/gcwmequuc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gcllkkjgs.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/gldidxdcd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.tarul.cn/Article/details/gakuidbdc.sHtML

[R32] 参数个数校验
来源：http://baike.tarul.cn/Article/details/gjowpnkxf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gvrjxjgki.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.bbcook.cn/Article/details/glfhzuuty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/giwebtdaa.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gvyknuvex.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.vehdjk.com/Article/details/gknywmzsq.sHtML

[R35] 后台执行并等待
来源：http://blog.sjlbkw.cn/Article/details/gilvpesfi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.tarul.cn/Article/details/gaxufvmtd.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gewmnsupt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/garvexmwy.sHtML

[R37] 把输出赋给变量
来源：http://mobile.vehdjk.com/Article/details/glxmsjdny.sHtML

files=$(ls -1)
来源：http://read.share.tarul.cn/Article/details/gwcxyxwgv.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gtvxdbien.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.epnwcf.com/Article/details/gvbonzaue.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.tarul.cn/Article/details/gepbxlsij.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gcplirynf.sHtML

[R40] 追加写日志
来源：http://m.share.tarul.cn/Article/details/gtpdqpnbp.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gipdgjwkk.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gicetkevv.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.tarul.cn/Article/details/ggjqpquiv.sHtML

[R42] 输入重定向
来源：http://baike.tarul.cn/Article/details/giadflxsa.sHtML

wc -l < a.txt
来源：http://baike.epnwcf.com/Article/details/gqdcyxyzd.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gxwzihlut.sHtML


<!-- 参考信息 -->