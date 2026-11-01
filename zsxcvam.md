代发 wailian999

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdnutrdqb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gqfcuvmhh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmwyzsuzx.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/goqffvinv.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gxbxfephr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gtdkklomk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/ghzrninvw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/guvjqtezm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gurrrvmyb.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gsdlbowvx.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gaeutpduy.sHtML

CREATE TABLE orders (
来源：http://www.m.share.fktsv.cn/Article/details/gtsxyshtt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/ghqnowzaz.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gkbnazrse.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fktsv.cn/Article/details/gsxhemsfe.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gxjzizbgq.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gfffebozf.sHtML

[Q03] 增加列
来源：http://3g.vehdjk.com/Article/details/gfgyrocjn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/grwtinfaj.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gsxmizzgv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.sjlbkw.cn/Article/details/gsshokrir.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gqvekrzov.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gjsumffkt.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gwjgyshrq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gonyzxbvn.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gcnaahdoz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gswcfhzon.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gbkywglgs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gnxpkjsll.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gtcilfzmy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gkwtwouac.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/glmzeazbg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/geqvgeyes.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/gxbjatqhe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/gmovgjgxt.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.epnwcf.com/Article/details/gncyaefdi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gpdpxdiyj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gyktxnfhs.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/gmidexjwm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gebhusouy.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gnssrmrlq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/gfdxvgcvw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gnljqzgrb.sHtML

[Q15] 查询全部
来源：http://m.share.epnwcf.com/Article/details/gighnvyig.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gqsdorgyl.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gipbilzro.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gbsokylna.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gchxpzvfp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gdujmyfhm.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gzdchfawc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/gmvvdecst.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gmefutgou.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.yfazqb.com/Article/details/gayeifrjm.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gluochijj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gvjvgvelz.sHtML

[Q21] 空值判断
来源：http://blog.vehdjk.com/Article/details/gfnhpomro.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gakmvbyep.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gecbgvvrb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/gnwwphoxo.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/ggumzfaji.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gpviqsjcg.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/ghjotoytb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gmjgphvuf.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gdmhvuxbv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/gdhhugmmz.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/ggigazpgj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjyzijxhs.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gicuxblyk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gqimpugze.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gntnivnsj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gsgsffsai.sHtML

[Q29] 最大最小值
来源：http://wap.epnwcf.com/Article/details/glwoycvjp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ghdluiusk.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gppmwtirq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gvxbywonr.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gksswzspw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gdggmtafk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fktsv.cn/Article/details/ggvogbedc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gvhtwqkbr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gydfptmvv.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/glfsmajgu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gwxqsgupz.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/ghjsumtck.sHtML

SELECT * FROM (
来源：http://wap.yfazqb.com/Article/details/gbdjzkkdd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gpppljcgq.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gkutfuszi.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/gghtvnicb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gdnzihphm.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gkzcbsilu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gitazqdep.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/grxixcmrb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.vehdjk.com/Article/details/ghkiywmbn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/ghwenozwk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gqyqsykmx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gaiyxemlo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.epnwcf.com/Article/details/gqhdcwjvn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/gpyfgyqca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fktsv.cn/Article/details/ggosadtad.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.sjlbkw.cn/Article/details/gmkiyhrir.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/ggoocbgyk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gdpuvryrp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.bbcook.cn/Article/details/gteuumsbt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gzbeoaeqf.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fktsv.cn/Article/details/gdoxryqry.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gjuksluur.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gbjofefas.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gznmtrjpb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gxvdzarkt.sHtML

[Q44] IN 子查询
来源：http://www.m.share.epnwcf.com/Article/details/ggynuugrc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gxtboepio.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.bbcook.cn/Article/details/gxpnerqcd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gwaberpih.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gibmevalj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gxxbkzjqf.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gplqgtamf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/guvrraaep.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gdqoyiwuq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/gbmdzazgu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gspixgvgx.sHtML

[Q49] 更新单行
来源：http://read.share.bbcook.cn/Article/details/ghmvwabem.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gcvhnyzqp.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/govscqtbd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/geihurbpo.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gyezjwpnr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gbffoeeii.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/goipsibdf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gjxborlxg.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gkwhdlymn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gudcjmjoe.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gwdeiliku.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/gkwcpkekm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/gfkdbnmts.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gyixqxrgk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.bbcook.cn/Article/details/gcqjpitrw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/gbdkpimih.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gkyuvmmvf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gjamvpffn.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gsddkanhl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gjeqlolne.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gnujypgkb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/ggorkovxh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/gdsdmfofl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjblycvi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/getfuqpmj.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gbfzpficr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gmygtjqeq.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gcgffzjce.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gxrcyovni.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/glvztnbmu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gwmjrgzjk.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gtaffyqmd.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gsacdkxll.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/grccaijtd.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gmjywvigk.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gwvzgrhlf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gpeoooxfi.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gptxyfmxx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gocrcgnkb.sHtML

[Q68] 保存点
来源：http://m.share.bbcook.cn/Article/details/gemckfesn.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/ggmbtisgg.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gdcaefffn.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/gyktzepre.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.yfazqb.com/Article/details/gqrxwdsgs.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/gjjzmgppa.sHtML

ANALYZE TABLE users;
来源：http://read.share.yfazqb.com/Article/details/gfxzkdllb.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/gbdpotkin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gquialdjx.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gculyoztu.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggqdzhnyu.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/goyvtwcoa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gsgperbob.sHtML

[Q74] 强制使用索引
来源：http://www.blog.tarul.cn/Article/details/gkmxnerng.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gczkkftoh.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gjnwqwvdr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gabzusnqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/glsdstuuh.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gmrnjyint.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gcpswkccx.sHtML

[Q77] 时间加减
来源：http://mobile.bbcook.cn/Article/details/gvncrzzhy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.tarul.cn/Article/details/gwzizgpty.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gsqopxrie.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gcjquefvp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gmzsrkjey.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/glphlkhzz.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/ggpizizug.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gsetivgsj.sHtML

[Q81] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gymqxrgmm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.vehdjk.com/Article/details/gtpckdypu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/gsqlmnjvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gcfxrhjww.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gjtfzsvjg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gccfoqdrn.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gwtlzzvhk.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gcodjmwew.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gwqovjckt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gbsnrpcyh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gkzjknxaf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/gjwyljmaq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gyqsvdiad.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gsonarino.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/getfwbjxt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gkacdwrve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/goxllyydv.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/gahymfcfw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gwjnltfzg.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gomckbvoy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gxvgcjlbq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gubdeqszu.sHtML

R. Bash 专题
来源：http://www.share.bbcook.cn/Article/details/gquqgggls.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gewuvsogq.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gjxlmwoiz.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/gtijlinaw.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/ggjzswnua.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/grhchhjhf.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gftxngjpo.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gmemwhgst.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gqmimlnyg.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gwpqpbzod.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gqkmhrmuv.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gmnkvztez.sHtML

name="${1:-default}"
来源：http://m.share.vehdjk.com/Article/details/gmvfveoor.sHtML

[R06] 判断命令是否存在
来源：http://www.share.yfazqb.com/Article/details/gyfwtaxqp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gtxgpzsfb.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/geypxkmze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gmroksnfy.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/glecdjlft.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/guknarago.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gypbwjbdo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.yfazqb.com/Article/details/gzwgzjvlc.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gqmbmtfky.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.epnwcf.com/Article/details/gevogqffx.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gaymfrswp.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/ghcgizrkn.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gbpcveepc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.vehdjk.com/Article/details/gdqcfmvnq.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/gfydidyxe.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gmssuoouw.sHtML

[R12] for 遍历文件
来源：http://mobile.epnwcf.com/Article/details/gyhfqwsuy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/grrgrlgwf.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gnspjzjug.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gafmdllve.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gqddzogsr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gvhnllkld.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/gtvyupifi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gwjfiivyj.sHtML

[R16] until 等待条件
来源：http://blog.vehdjk.com/Article/details/greeymtxq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gqypgikkq.sHtML

[R17] 数组定义与取值
来源：http://blog.yfazqb.com/Article/details/gywkqqggn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/grxsxpqtm.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/genbmpzjl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gmkorbdjv.sHtML

[R19] 数组长度
来源：http://blog.fktsv.cn/Article/details/gwsvauyyy.sHtML

echo "${#arr[@]}"
来源：http://baike.yfazqb.com/Article/details/gwgbgbxco.sHtML

[R20] 关联数组（字典）
来源：http://read.share.epnwcf.com/Article/details/gqzmcqzox.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.bbcook.cn/Article/details/gxtplfzdi.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/gumdsiwvp.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gniinubns.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gqjdearhj.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gcwgnvfij.sHtML

[R23] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/glbtgdaus.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gfhuiyvvi.sHtML

[R24] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gccexmmml.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.yfazqb.com/Article/details/gjhwgwbor.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fktsv.cn/Article/details/gnpjukgpi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gquismeqq.sHtML

[R26] 命令替换
来源：http://blog.epnwcf.com/Article/details/gduvupsvi.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.tarul.cn/Article/details/gymafnoyu.sHtML

[R27] 算术展开
来源：http://mobile.epnwcf.com/Article/details/gjihxhhbp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.epnwcf.com/Article/details/ggykthioc.sHtML

[R28] 浮点运算
来源：http://wap.fktsv.cn/Article/details/gfyxpadoy.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gljfnxbvy.sHtML

[R29] 定义函数
来源：http://www.m.share.epnwcf.com/Article/details/gtrnztcnt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.tarul.cn/Article/details/gybdtikjf.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/gjbxitjmd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.epnwcf.com/Article/details/gmevflwdm.sHtML

[R31] 局部变量
来源：http://wap.yfazqb.com/Article/details/gadveljfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gqrlgvimh.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gnfkyfzih.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/gasjyxyxv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/glbnrleay.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gcqgjykkj.sHtML

[R34] 退出时清理
来源：http://baike.bbcook.cn/Article/details/gtnzaxcqu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gfqoevjpg.sHtML

[R35] 后台执行并等待
来源：http://www.share.epnwcf.com/Article/details/gnpsudxmf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gvdamzqea.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.yfazqb.com/Article/details/gnwvgpekb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.vehdjk.com/Article/details/gffgtczyf.sHtML

[R37] 把输出赋给变量
来源：http://mobile.epnwcf.com/Article/details/gfqlqwdmy.sHtML

files=$(ls -1)
来源：http://mobile.yfazqb.com/Article/details/gvbnpketb.sHtML

[R38] 管道串联
来源：http://www.share.epnwcf.com/Article/details/gxvjhlbcr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.yfazqb.com/Article/details/grcntefql.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gstohcgrp.sHtML

cmd > out.log 2>&1
来源：http://mobile.bbcook.cn/Article/details/gemzqonpd.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/gjojjwhys.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gohtuzlch.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gqqtdnblj.sHtML

cmd >/dev/null 2>&1
来源：http://3g.bbcook.cn/Article/details/gcsbufavm.sHtML

[R42] 输入重定向
来源：http://baike.vehdjk.com/Article/details/gziwxqini.sHtML

wc -l < a.txt
来源：http://m.share.epnwcf.com/Article/details/gjkadyisu.sHtML

[R43] 按名字查找文件
来源：http://wap.yfazqb.com/Article/details/gcfgjxwtx.sHtML


<!-- 参考信息 -->