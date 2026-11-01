代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gplecxofm.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/guuxftois.sHtML

amount DECIMAL(10, 2),
来源：http://3g.vehdjk.com/Article/details/glhtcidqn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gmyglrsmn.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gfxxkjnbe.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/getkunwss.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gxybjstwo.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gruxbwnlu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gyabbgutq.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gqsqrelsi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/gkmxhxgpc.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/geawoiqve.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gfezfzadt.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/gbugjmniy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.bbcook.cn/Article/details/glbraiyuj.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/ghmzdjewi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gahyxzter.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gpcreipjm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gfcmaginj.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gwhbdtsnv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gthmgvyhm.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gxmckxuvh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gubyvoyyu.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/glipmdvbd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gtjjzcdtv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gjrwxnvzt.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gccbqwywd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gcdyewami.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gskaggfeu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gvsqhllgc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gcuujxzbi.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/grmbmfsmd.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/ggckcfxmk.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/gdemlklia.sHtML

SELECT id, name FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvmazzilp.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gbgffhhct.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gajbmaeez.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gwjdecltz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gkpxtjwec.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/gcskzgqdv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/gcueqisag.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gyqxkhbne.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gkbqwzfid.sHtML

[Q21] 空值判断
来源：http://baike.vehdjk.com/Article/details/gvyhizcwb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.bbcook.cn/Article/details/gcrgjslqq.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gduyeqtzw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.sjlbkw.cn/Article/details/ghxacsnbp.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gtpyqgajo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.tarul.cn/Article/details/ghkadsopy.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/gnixbzbjt.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gvflhfwpw.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/govetwgds.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gechzznoi.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/gjbyxljln.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gkufwuhuv.sHtML

[Q27] 条件计数
来源：http://m.share.bbcook.cn/Article/details/gqilglerl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwuhbiwco.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/gmehitumy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gilpgazxs.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gdbaryiki.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gpklwplvv.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/gszneytqr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gdfomekef.sHtML

[Q31] 分组后过滤
来源：http://www.blog.vehdjk.com/Article/details/gtqzyvuid.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/grysmsehj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gtehsgzsy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gdkofzzgg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gwlzvwili.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/gszlnpvgo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gkqveszky.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gnvicdqkl.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/grhpgvamj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/guqmlnzpg.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gbnwzurdh.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/gmlqatdgw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/ghcdacizk.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gmurfizyg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gprjfjpvo.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gqweukbyn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/gpgmavttx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gfcywnaqr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gjbicunjx.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fktsv.cn/Article/details/gmizoqmwt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gyvsxgkcj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/ggjjybuup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/giuzwntlf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gzljmyigp.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/guzyipcut.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gnpcflneo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/glxtvgziu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gpsvbwuyd.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gzgftgocz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/ghlrwqfqb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gjjlzxaxn.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gwpcgzsto.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gpvgrqjwq.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/giprjhwht.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gobaadoki.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gguvgmvvg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gdsalgbfj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/ghlbebgwj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gxqnbmryu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/girgjhhmw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.epnwcf.com/Article/details/gqnqyzfsa.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gkfxppdxe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/gtiieysmq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gkvqnxbob.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/gnbhxqjha.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gdcvilhvs.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/gmgaphegp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/gpricigcj.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gpzarwywd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gifivqrqg.sHtML

[Q52] 删除指定行
来源：http://m.share.sjlbkw.cn/Article/details/gfeyeqohf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gxywgsjsk.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gmytcbnos.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/gqxquivid.sHtML

[Q54] 清空表
来源：http://www.blog.yfazqb.com/Article/details/gawpgluei.sHtML

TRUNCATE TABLE logs;
来源：http://blog.yfazqb.com/Article/details/gseartnhf.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.tarul.cn/Article/details/gfgvtdngc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gkdqdcitv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gcopzgwpo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gqzdjpgvm.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/ggtfbpyut.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gammjbwjs.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gblcmjdin.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/givysggol.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/ggujmmkns.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gttzxxsxk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gfliaeueo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gtelpmeky.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gfmzrfbvs.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/guzkjppro.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gpvkuzict.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/geppwowud.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gqbzltgnx.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/guzohynqz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/giytttass.sHtML

[Q64] 提交事务
来源：http://3g.epnwcf.com/Article/details/gbigjzdra.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gozirvmsg.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/glkowzvge.sHtML

ROLLBACK;
来源：http://m.share.bbcook.cn/Article/details/gregegydl.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gimwtcriy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gwmbobmqf.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gebahszzw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gosworbjk.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gvcfwrnlf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gbdhmiteb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/gxwnccvgx.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/gkafffzyg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gpojihjyz.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gpscauash.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gkydtyeod.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gbtuwuvsn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gxgfqdayf.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/ginejcwlz.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/gdqmemhco.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gkipldjrq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gcmpzbift.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gspqtcqdd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gopwkxppz.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gpsgxqdvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gaeytskud.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gbynuwiwo.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/goehczmjq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.yfazqb.com/Article/details/gnhzyejzr.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gvgswtdfp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/gqsgiwufv.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gvmhbmotv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gmocjdtzu.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gffpcvweu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gxgjpxaak.sHtML

[Q80] 字符串截取
来源：http://wap.vehdjk.com/Article/details/gwoujfcwr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/gmcbsvqfl.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/ggjfkfxnx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/gqtdwqxfm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gdqspjkvp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gyjmlosng.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gfynyqumc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gutmvbmsz.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gwlxfmkut.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gjftgeipz.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/guvfrunvb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/gmrtdfzck.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gcmrdegwj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gsqiyxzkf.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gjdowcnmg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/golzibywt.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.vehdjk.com/Article/details/glrlhgbpx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/guscxofkl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/giwroxhld.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/goicanupu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gdbnyjljg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/gifikkgzk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gvqobguli.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzgpotvnl.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/govvpdtcn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbtraqkfu.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gzmvpqkks.sHtML

#!/usr/bin/env bash
来源：http://read.share.vehdjk.com/Article/details/gyakyeiix.sHtML

set -euo pipefail
来源：http://read.share.epnwcf.com/Article/details/gahtojwty.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gbnmoclsx.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/gsjnnetzf.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gfujaxhpl.sHtML

readonly PI=3.14
来源：http://wap.yfazqb.com/Article/details/gcprnyjyd.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/ganxyilos.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gsqminuwa.sHtML

[R05] 参数默认值
来源：http://m.share.sjlbkw.cn/Article/details/gddkhippl.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gfgimgwyh.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gxuibsdue.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/gzbrldomr.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/gyjxmwfbm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gmgewvzbu.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/grqprpucl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmhccrfg.sHtML

[R09] 字符串比较
来源：http://www.m.share.yfazqb.com/Article/details/gobdloiaa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/gerwynsnr.sHtML

[R10] 正则匹配
来源：http://www.m.share.yfazqb.com/Article/details/gqvamrfid.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.tarul.cn/Article/details/gnnltcqmf.sHtML

[R11] case 多分支
来源：http://baike.yfazqb.com/Article/details/gopvvqnlm.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gtvankbek.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gyokkkjzi.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/glhpukxli.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fktsv.cn/Article/details/gsuhveujz.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/glnknkmon.sHtML

[R12] for 遍历文件
来源：http://wap.bbcook.cn/Article/details/gxcdouixr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gmzgrfcfd.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gsujdmqcd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gdertqhlj.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/gjrngnyvr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gpgbtheyx.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gagmrtotq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.tarul.cn/Article/details/gcykiucsq.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gtgvmamaw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gzgghdfsq.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gnxmhusgg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fktsv.cn/Article/details/gygpzxbso.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gbrolixwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gvoahjhjn.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gjtgqgsop.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gbvxxguvv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gykjbatgj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/ghsrkrvzm.sHtML

[R21] 字符串长度
来源：http://wap.bbcook.cn/Article/details/guafegjzg.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gagcsjxjg.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gwyhvfsfg.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gygsiezph.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gufgyajnn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/garyjuhcj.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gjitxctft.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/ghbehkbun.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gntlwijsi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.tarul.cn/Article/details/gkidlpmbh.sHtML

[R26] 命令替换
来源：http://wap.vehdjk.com/Article/details/gsqhtnskm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.yfazqb.com/Article/details/gjtogyvob.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gwujmqxao.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/gxbkfvsmw.sHtML

[R28] 浮点运算
来源：http://www.share.sjlbkw.cn/Article/details/gqdhdgror.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/giotrjggr.sHtML

[R29] 定义函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gegdpgbmy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.bbcook.cn/Article/details/gesxeesdr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fktsv.cn/Article/details/gigwxzmct.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gomrzmnnv.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gageddotm.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gncpxyvuy.sHtML

[R32] 参数个数校验
来源：http://3g.epnwcf.com/Article/details/gqqnzswwj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gagjtmxze.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gvoqkzhax.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gezfwkaps.sHtML

[R34] 退出时清理
来源：http://www.share.epnwcf.com/Article/details/gvpcthbyu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gtorjpdsc.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gbgjnxwme.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.bbcook.cn/Article/details/gtozfnneb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gioienrhj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gaqpynuqn.sHtML

[R37] 把输出赋给变量
来源：http://mobile.tarul.cn/Article/details/gesrlrxcc.sHtML

files=$(ls -1)
来源：http://www.share.yfazqb.com/Article/details/gxscqlwsp.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gnntzhkrr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gprudsotn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.epnwcf.com/Article/details/gosdfhmev.sHtML

cmd > out.log 2>&1
来源：http://3g.sjlbkw.cn/Article/details/giicelolk.sHtML

[R40] 追加写日志
来源：http://www.m.share.yfazqb.com/Article/details/grdhmwjsf.sHtML

echo "log" >> out.log
来源：http://read.share.bbcook.cn/Article/details/gfakisbvh.sHtML

[R41] 丢弃输出
来源：http://www.m.share.tarul.cn/Article/details/gapchmkqx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.yfazqb.com/Article/details/ghguaoqwa.sHtML

[R42] 输入重定向
来源：http://wap.vehdjk.com/Article/details/gmmyhihqs.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/ghmsxzjrp.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/gjvoppmfb.sHtML

find . -name "*.log" -type f
来源：http://blog.sjlbkw.cn/Article/details/gduigwtlf.sHtML

[R44] 按修改时间查找
来源：http://m.share.yfazqb.com/Article/details/gehxrspro.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gbgzdrrkv.sHtML

[R45] 批量删除
来源：http://m.share.yfazqb.com/Article/details/gxrfdyped.sHtML

find . -name "*.tmp" -delete
来源：http://wap.epnwcf.com/Article/details/govqwwzgo.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fktsv.cn/Article/details/gwllchcyf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fktsv.cn/Article/details/gqtmslxzd.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/gxfasfrhw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gxrrrmunx.sHtML

[R48] awk 取指定列
来源：http://blog.tarul.cn/Article/details/glraogvmw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gybnntktk.sHtML

[R49] awk 带条件
来源：http://wap.bbcook.cn/Article/details/gibarjbuk.sHtML


<!-- 参考信息 -->