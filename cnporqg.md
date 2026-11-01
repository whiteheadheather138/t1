代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/guhvhbmvn.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gpgymevks.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gddyskikp.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gjkrvhwra.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/gpxdpzgot.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gftnpqyoz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.tarul.cn/Article/details/gvkaxtvbq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gtcukiggw.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/giwtoofqc.sHtML

[Q03] 增加列
来源：http://mobile.vehdjk.com/Article/details/grprwwoxv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/geluqwtjn.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/guoiadmqy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.vehdjk.com/Article/details/gllgkcdtb.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/gybplfknr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gpwxpcmgv.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gjoxzoffe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gtfbvfptg.sHtML

[Q07] 删除表
来源：http://blog.tarul.cn/Article/details/gwnyvybdr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gpervwauz.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gvqmaqlpa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gwundxlfz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/giwkhfypi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gnsglepoq.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gsxdvqfsu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.bbcook.cn/Article/details/gukxgqgiv.sHtML

[Q11] 一次插入多行
来源：http://read.share.sjlbkw.cn/Article/details/givxnilpn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gpkaxiepn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fktsv.cn/Article/details/gdnmyrlwk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/gynblbtev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.bbcook.cn/Article/details/gunnvlecj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fktsv.cn/Article/details/gfnkvajbh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gkoaasasr.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gqvnihipp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/guzmbudnu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gcrrztzoo.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/gxurxqaco.sHtML

SELECT * FROM users;
来源：http://baike.tarul.cn/Article/details/gxipvqanz.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gtqzoqsst.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gztsxxiwc.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/guyzlwabj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gtsjgnpgk.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/gucjylvym.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gfvkfswmj.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gtsivkntb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.tarul.cn/Article/details/gspozcklb.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/ggleodfcx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gvavfmxkf.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gtvdqcxou.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gxnvxfhib.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gwuxttuxa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/glcjxvsfl.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gxtvlooam.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.fktsv.cn/Article/details/gttoqjmju.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/ggvedkukb.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/ghvfsdigu.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gtjuzvips.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gmqeajbmr.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gjgldyabj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gekjaztri.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gatpmqjfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.epnwcf.com/Article/details/gvbvrekvv.sHtML

[Q28] 求和与平均
来源：http://blog.tarul.cn/Article/details/gpncsqaem.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gdiuplkmr.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gngppdxjl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fktsv.cn/Article/details/garvwggvf.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/gtfhdvbdf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/grjypoquo.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gjxpvfylm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gxrsuyeji.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gwagsnstg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gmciqmzkg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/gtqjpaxzn.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gbyksbqkk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gtsdakoax.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gtzimdayr.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/glpdtnjdi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/gebvbvbjz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fktsv.cn/Article/details/gwqjjruzs.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/gzrpncaly.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gsgqybifa.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gifoeujqj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkxpciuax.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gxkfrqnck.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gatjngqeb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.vehdjk.com/Article/details/gurdbtnde.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gisxtzsoq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/ghuespiky.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gphpbyois.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/ghjfgvoyg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gpuzucipj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gmlnlbqyo.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gxhbbxrgz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gozhteuag.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/gxezjoyan.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gqbbafggi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/glpgcriel.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gskvcuubq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gyunggwbs.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gofttwslg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.vehdjk.com/Article/details/grkimtlvr.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gtdzkgkmh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gqpyivxrm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gdryphkzm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gmqtocsbt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/ggpjbjkph.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gztnoxolb.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/gqqxkkbaz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.tarul.cn/Article/details/gbzpwmbcf.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gqvfwgsus.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gcfpblvqq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/ggnslmrxr.sHtML

[Q49] 更新单行
来源：http://m.share.tarul.cn/Article/details/gdmqsrbbh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/girvlkmup.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gxmcjepnz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/gfmjmycid.sHtML

[Q51] 用子查询更新
来源：http://wap.yfazqb.com/Article/details/gbzmpytss.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/gquhpzmkp.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/grajcpnwo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gfehipxmm.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gqannkpeb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.epnwcf.com/Article/details/gxihomuuq.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gfahtcygt.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/gojbsupuc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/geuremihh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/grtihtykz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/glaypqgta.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gexgbmzku.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gxvjuxxbm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gjeyempco.sHtML

[Q58] 累计求和
来源：http://blog.sjlbkw.cn/Article/details/gipllvrld.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gfzvgghlv.sHtML

[Q59] 分组内累计
来源：http://www.share.tarul.cn/Article/details/ggiulgefd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/goqurqvuv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/gjpfxpufu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/gtvjzence.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gaklwdwvx.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gokfcyktj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gkqowaszs.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/grwrbtovs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/guqltscev.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gvroylfei.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gopwobsqn.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gjuvjorcw.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/grnipyhlq.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gfqmaglrk.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/gyljheosc.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gdskxbwbu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gdsehndtb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gcsgemxmr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gsjroksbv.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gcvoybbmh.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gowovxoba.sHtML

ROLLBACK TO sp1;
来源：http://www.share.yfazqb.com/Article/details/gcwwbxilp.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gmhtobrvn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gviwjjmka.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.tarul.cn/Article/details/gdiihztfa.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gjqqzsbay.sHtML

[Q71] 查看建表语句
来源：http://www.blog.tarul.cn/Article/details/gvtywkvhm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gwttxnfcr.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gtzjpxjio.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gqluljrej.sHtML

[Q73] 查看表状态
来源：http://www.m.share.bbcook.cn/Article/details/gepspyacd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gjlcxhnng.sHtML

[Q74] 强制使用索引
来源：http://read.share.bbcook.cn/Article/details/gvunetokh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/gjirojsca.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gvspyimww.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gejfdunyx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gcvnyuutx.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/ghbbyogpw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gbasknduy.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gnxuczhky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gtsfavzzu.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gmkmxldly.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/goxmdxtxv.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gbuiravey.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.yfazqb.com/Article/details/gimywtnva.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gyqhjqrtn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/ghtjrvpot.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gkaufhwyk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gyuvfaare.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gwaiyzmjd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gdpalbvmf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gyzwwoqrf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gzpspvzdq.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/ggfahuneq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gbkjjeasy.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/ghdmhwtkt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.vehdjk.com/Article/details/gdyhkqzax.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gowkxnaar.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.yfazqb.com/Article/details/gyzgmcevu.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gdjalygts.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gpfgunwkl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/gxbyxjacj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/ghqyynpzf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.bbcook.cn/Article/details/gzurlgfbt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gsdumrmqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gsnzyxpdn.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gddreiest.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gxekdjrpj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gsfwnhwxj.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gisrdjtni.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghlxlouvr.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gejnpdmfz.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gxpmhicxc.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gdflsyweg.sHtML

[R02] 变量赋值与使用
来源：http://3g.epnwcf.com/Article/details/gdppkdwsm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/genoikqap.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gmgkyjcyk.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gdphnlfey.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/gdcvrnwsq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/gagsxwpnd.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gmprdgvcv.sHtML

name="${1:-default}"
来源：http://mobile.fktsv.cn/Article/details/gzmounmvi.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gqctywsjm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gvjkviwdt.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gdgocqdka.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gerzslfii.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gsnwwhijb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gwlladnlx.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gbbqyrdsb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fktsv.cn/Article/details/gusgrdqkv.sHtML

[R10] 正则匹配
来源：http://read.share.fktsv.cn/Article/details/ggnaiqtof.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gvsvenzki.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gbbnktwcs.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gzckzqort.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/ggyfouwkn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.vehdjk.com/Article/details/gwlelfxyn.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/gxdlvoami.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gqsvswacl.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/gdsyzilnk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/gmmuvxliv.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gqpxspvzx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/ggoayfcee.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/ghriaktfk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/grfefbfvn.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gtlcmjpwv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/ghljasprd.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gowjsgsgr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/gfozeuams.sHtML

[R17] 数组定义与取值
来源：http://read.share.fktsv.cn/Article/details/gphuyzisf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gvshpqtcx.sHtML

[R18] 遍历数组
来源：http://www.share.bbcook.cn/Article/details/gfpgjestg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fktsv.cn/Article/details/gqcuumgkt.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gjubdylzp.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gkynccwtu.sHtML

[R20] 关联数组（字典）
来源：http://3g.tarul.cn/Article/details/gqbqhtane.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.epnwcf.com/Article/details/gagesqkge.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gpgbiutgt.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/gediiunzt.sHtML

[R22] 截取子串
来源：http://www.share.tarul.cn/Article/details/goziwvywp.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gojfwukow.sHtML

[R23] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gyokjjyyx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.yfazqb.com/Article/details/gcyygsghc.sHtML

[R24] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gnckkwecj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fktsv.cn/Article/details/gthiwscai.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fktsv.cn/Article/details/glcigbcjx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/gkgejzkka.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gpjdofndt.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.yfazqb.com/Article/details/gevldmbmi.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gqhiwoxfe.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gqjgchrdf.sHtML

[R28] 浮点运算
来源：http://www.blog.vehdjk.com/Article/details/ghtpyevnz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/givuxyfty.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gjskjrpxi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gywyffhsn.sHtML

[R30] 函数返回状态码
来源：http://www.share.bbcook.cn/Article/details/gwtfamgjk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/gdnvfxrsd.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/grgztbcnx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gfemgcgei.sHtML

[R32] 参数个数校验
来源：http://wap.bbcook.cn/Article/details/gqzcprbpi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.yfazqb.com/Article/details/gzeybqxex.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.yfazqb.com/Article/details/gtewmawiq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gayrwpewk.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gghgtrngr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.sjlbkw.cn/Article/details/grdgcwsqa.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gkgpahlkd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.epnwcf.com/Article/details/gbqcuvenk.sHtML

[R36] 并发执行多个任务
来源：http://www.share.yfazqb.com/Article/details/gxjuqzube.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.tarul.cn/Article/details/giqlhaylh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.tarul.cn/Article/details/gzgzmiucw.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gfwkkqlep.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gzqwygqdd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.bbcook.cn/Article/details/gukuofgsx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gaipuvemy.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/gndoopdcc.sHtML

[R40] 追加写日志
来源：http://wap.vehdjk.com/Article/details/gfyamcncp.sHtML

echo "log" >> out.log
来源：http://mobile.epnwcf.com/Article/details/gaxxtjfzi.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/ggmqrxvwk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.yfazqb.com/Article/details/gcmedzogp.sHtML

[R42] 输入重定向
来源：http://blog.fktsv.cn/Article/details/globnkxgw.sHtML

wc -l < a.txt
来源：http://www.share.vehdjk.com/Article/details/gafuhhzov.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gfjsilhly.sHtML

find . -name "*.log" -type f
来源：http://blog.epnwcf.com/Article/details/gaodplsia.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gwelgaqzh.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gtuykvyas.sHtML

[R45] 批量删除
来源：http://www.m.share.bbcook.cn/Article/details/gvsjphcgn.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gvyewbnto.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gosuxjamt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.epnwcf.com/Article/details/gtlxkvdcf.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/grvhiclum.sHtML


<!-- 参考信息 -->