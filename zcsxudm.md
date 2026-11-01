代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/gzdujlrkd.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/gigwbujlk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.yfazqb.com/Article/details/gmchgyqhx.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/givmeqgwy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.yfazqb.com/Article/details/gkzbjerpd.sHtML

[Q07] 删除表
来源：http://mobile.epnwcf.com/Article/details/glnxcanwa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gbmovkynf.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzmlggjy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gvwtpjpxd.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/giqrqpumd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gfyeucqxp.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/glrxgmjkh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gnrxopzdq.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/glasjnekt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gvsxsfjty.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/gwnrrmfar.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.bbcook.cn/Article/details/ggfwrgroz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gryllxyxr.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gouvmuoph.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/geuxspmxh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/gnenxrkzj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.vehdjk.com/Article/details/gkaelnekh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/guatznois.sHtML

[Q15] 查询全部
来源：http://mobile.sjlbkw.cn/Article/details/gdffrcisk.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjvyizsms.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gudqjhpmm.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqquxtxjg.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gfdbhxrte.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/grgndgrbf.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gckucoyde.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/glfeadjvc.sHtML

[Q19] 范围查询
来源：http://www.m.share.tarul.cn/Article/details/gedkdpwfz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gcmhgiuxl.sHtML

[Q20] IN 列表
来源：http://www.share.fktsv.cn/Article/details/gnitqkqex.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/grvsveefc.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/giodpkcli.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gfusxfjtt.sHtML

[Q22] 排序
来源：http://mobile.sjlbkw.cn/Article/details/gfqngqcgk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/gmzpkmbhf.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gmhzvdgtw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gmnczwuxq.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gaetxwwuz.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gpxoqijmg.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gvofzasqt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gswujcxfo.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gslophkzx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gdettilhn.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gbklmiiom.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/galrczdgb.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gohlzqvly.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/grnybsjlz.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gkwaqkzrb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gyeqsprkx.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gnkammgni.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gkvhjsddq.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/giaglbyof.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gyfqsvgrg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gunxdpohu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gpipintwu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gfyjesgsb.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/goxxpklbg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gjfqwtujw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gcbpsqxql.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gkrdtkxvp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.epnwcf.com/Article/details/ghytrveph.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gzhieucay.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/gaarxhcsj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gsmfmsuuy.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gppsjgpqn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gmvrxhcgt.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gllwqabah.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gneuqpwpf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/ggwlhwtoa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gnhtjjezg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gvaxntdqm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gfknkvtpz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.yfazqb.com/Article/details/gauhdxqkd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gpfzarflk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gidfsyija.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gzcatzlan.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gtwujhzah.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/ghqojcdkf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gswgwhrof.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gxftabjjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.yfazqb.com/Article/details/gtwoudmgl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gtnitdeby.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gryzshqrd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.yfazqb.com/Article/details/ghfbnoadx.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gvlqoejhr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/grargfqjv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gybydfold.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gmxqznktu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/ggpxxwaro.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gxevcqmxp.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gmxwoxnne.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gozjkqwxg.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/guiykgvcg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/goanswjgu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gtghkolex.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gzwyzicpw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gvulrwzsc.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gjvgyyuvi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gnfgiqnqx.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gimxkvzzg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gjwmcaqun.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/gzrmagbzm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gcdeycupj.sHtML

[Q53] 按条件删除
来源：http://www.share.epnwcf.com/Article/details/gepdeibkp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.epnwcf.com/Article/details/gezevqqps.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gkgmlkpep.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gbcpjkekz.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.epnwcf.com/Article/details/gzjjmnwdj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gwnswotfm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/ghwnmbzon.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gelvaadys.sHtML

[Q57] 行号
来源：http://read.share.tarul.cn/Article/details/gxsizhatc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gnhuehyrm.sHtML

[Q58] 累计求和
来源：http://blog.sjlbkw.cn/Article/details/gjtcweroz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gtvotovtm.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/grpogzxep.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gngwgxfbe.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/guphcdfhx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gzfznliun.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gnniswfla.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gxtfglngs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/grzrmjutx.sHtML

[Q62] 分组占比
来源：http://www.share.vehdjk.com/Article/details/gartstygv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gfjauhubf.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gtrzsajbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/gmchmvqsr.sHtML

[Q64] 提交事务
来源：http://m.share.fktsv.cn/Article/details/gjxwlliyx.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gcaimrwek.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/glkrhkrgs.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gdbfmftwb.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/gnjkjkuif.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/ggwfxostm.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/guyhkvpxy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gazjzazqs.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gtgcfpqhy.sHtML

SAVEPOINT sp1;
来源：http://read.share.tarul.cn/Article/details/gpszjthrp.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/glgocvrau.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gndzygwea.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.sjlbkw.cn/Article/details/gznkfmdqu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gqacidjdg.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gkzawyeqy.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/goxfgeoer.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gebfpbgua.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gtroteibm.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gjbjcawbs.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gehnwtasr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gtvfqokur.sHtML

[Q74] 强制使用索引
来源：http://3g.fktsv.cn/Article/details/gpxecgcrq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gieyybyav.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/ggvtecatg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gwrlqquki.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.vehdjk.com/Article/details/gueefacfv.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gsycgbdvj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gebitvhmy.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/glcimhkct.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gkjmtcecp.sHtML

[Q78] 当前时间
来源：http://mobile.epnwcf.com/Article/details/gjtfpuajl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gsbzhzqzg.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gvzkopjzs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gteytdfni.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/grldqypob.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.vehdjk.com/Article/details/gfzgxlins.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gkylruwsl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gppefijum.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gbsncnyvm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gduneakgd.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gatvkgtex.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gmjyrzlof.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gbmgoxqtb.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gpuqqswqg.sHtML

[Q85] 数值取整
来源：http://www.m.share.fktsv.cn/Article/details/gppsbqsxp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/ggfomgscf.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gdomoltkh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gotvrpkrq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gmvnwfrnv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gishknotn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.epnwcf.com/Article/details/gmipajxug.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.tarul.cn/Article/details/gjxwxddlb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/goutavyog.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gtajwkulo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gjorkorrt.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/ghrnrmavh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/gazhblbas.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gmrbkpmkf.sHtML

R. Bash 专题
来源：http://www.share.fktsv.cn/Article/details/ggalmoarf.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gdwcgsrgt.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gripzkmew.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gtqysuvne.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gwknefpca.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/grlrelsoh.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/glcgmyxos.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/giiugalyf.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gulmmcpfz.sHtML

[R04] 位置参数
来源：http://www.m.share.yfazqb.com/Article/details/gzauttzdg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gkczxdtoe.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gqctkxhqo.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/guztiiuwv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gpuytsygm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gvhregoid.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/giiyhcvdb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gtyiqqmpf.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/gpgbhrbkc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gtzcuxcom.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gcgvusqcv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gpcyrypue.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/growwpssn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gbjvgpvnd.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/ghdnmzyjc.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gmdmxkrmf.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/ghjaxsrra.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gfvlzlpna.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/gvkjehqkq.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gnhpbyfzh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/gpyxkxrvr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.yfazqb.com/Article/details/gmvxigxyx.sHtML

[R13] for 计数循环
来源：http://m.share.vehdjk.com/Article/details/goqpphrzf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gzvffysbn.sHtML

[R14] C 风格 for
来源：http://www.m.share.yfazqb.com/Article/details/gimqytsno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gjrjxeemy.sHtML

[R15] while 逐行读文件
来源：http://read.share.vehdjk.com/Article/details/geuhvxzae.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/grchkkbrx.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gdvawyuch.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gdpdbskwu.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/gvdaxkpsj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/gtggfkars.sHtML

[R18] 遍历数组
来源：http://wap.tarul.cn/Article/details/gcbtxqlrk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gsbrzogxn.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/gvrlkvyjo.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gnhfmatiq.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gngrfszku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.epnwcf.com/Article/details/gjjkrckoc.sHtML

[R21] 字符串长度
来源：http://3g.fktsv.cn/Article/details/gntmvsvet.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gixlxydgv.sHtML

[R22] 截取子串
来源：http://read.share.yfazqb.com/Article/details/gpvnjnyss.sHtML

echo "${s:0:5}"
来源：http://mobile.fktsv.cn/Article/details/gvrsmmses.sHtML

[R23] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpfcyjud.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.yfazqb.com/Article/details/gervztvem.sHtML

[R24] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/guatedhfu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gtrxfroza.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.bbcook.cn/Article/details/gutxwncvo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gzvckuekz.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gebbtjles.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gzizyutyi.sHtML

[R27] 算术展开
来源：http://www.blog.epnwcf.com/Article/details/gstqbykpv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.bbcook.cn/Article/details/gzxvtqhod.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/gkmonhazm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gvqamnblg.sHtML

[R29] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gckacusnw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.yfazqb.com/Article/details/gqzxgpoql.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/ghhdiyrwj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gtzyomwtl.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/gijgbttxk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gzjzgjivb.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/glvsuujlt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gfdivauro.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/gjphyjbqi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gvtvmktin.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gcrdpupda.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gmwudkahw.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/glolujjxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.bbcook.cn/Article/details/gpgcxhpgk.sHtML

[R36] 并发执行多个任务
来源：http://baike.yfazqb.com/Article/details/gqtgqvzvy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gjcodfexo.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gwilhhwon.sHtML

files=$(ls -1)
来源：http://www.m.share.fktsv.cn/Article/details/guwudzatx.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gxdvfiuwx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gguvpevfb.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.tarul.cn/Article/details/gbuczsrbi.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/geauwyqun.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gdyyzuwrd.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gjdryrwqe.sHtML

[R41] 丢弃输出
来源：http://baike.vehdjk.com/Article/details/gkeipbsej.sHtML

cmd >/dev/null 2>&1
来源：http://baike.vehdjk.com/Article/details/gjodxrbqi.sHtML

[R42] 输入重定向
来源：http://www.m.share.epnwcf.com/Article/details/gpxaarsty.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gfxhwhmyp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fktsv.cn/Article/details/gektvbtdi.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/glkhkafmb.sHtML

[R44] 按修改时间查找
来源：http://m.share.yfazqb.com/Article/details/gbiyacosa.sHtML

find . -mtime -7 -type f
来源：http://baike.tarul.cn/Article/details/gwzibctco.sHtML

[R45] 批量删除
来源：http://www.share.sjlbkw.cn/Article/details/glrabuqzg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.epnwcf.com/Article/details/gexyfwzdx.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.yfazqb.com/Article/details/gaczbdifs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.tarul.cn/Article/details/ggiqxhvhj.sHtML

[R47] sed 单行替换
来源：http://blog.epnwcf.com/Article/details/guihfqhmg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.yfazqb.com/Article/details/gskwfbngn.sHtML

[R48] awk 取指定列
来源：http://m.share.vehdjk.com/Article/details/gsgxkhqyf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gbywrpism.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gnhhmfsrn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.bbcook.cn/Article/details/gqmmdihiy.sHtML

[R50] awk 求和
来源：http://3g.sjlbkw.cn/Article/details/gydnjshtz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.yfazqb.com/Article/details/gkomwirvz.sHtML

[R51] 排序去重取前几
来源：http://wap.vehdjk.com/Article/details/gunjroqwv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.yfazqb.com/Article/details/goawbblnr.sHtML

[R52] 统计行数
来源：http://3g.sjlbkw.cn/Article/details/gxofxgavn.sHtML

wc -l a.txt
来源：http://read.share.bbcook.cn/Article/details/gvezxjkti.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.bbcook.cn/Article/details/gavcrkkqc.sHtML


<!-- 参考信息 -->