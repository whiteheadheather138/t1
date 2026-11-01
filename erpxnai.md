代发 wailian999

);
来源：http://www.blog.fktsv.cn/Article/details/glrcoebfv.sHtML

[Q03] 增加列
来源：http://blog.bbcook.cn/Article/details/gzjsyimqs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/ggbhiigtv.sHtML

[Q04] 修改列类型
来源：http://www.blog.bbcook.cn/Article/details/gieqbeilt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/gmzkfuwdi.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/guhsvkjdm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gjqsoqeok.sHtML

[Q06] 删除列
来源：http://www.blog.fktsv.cn/Article/details/gzcalvcay.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gzmmoequm.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gpnqcpaob.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gymjaksqw.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gpefyuuyg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gbhdfxuzo.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/gatgzoghn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gkcuvfcrk.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gqrxceluk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gcbjmqrqu.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gepuepkrk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gpxbyubnh.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gtlbsacip.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/gzahsxrzw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gjtkwvcjh.sHtML

[Q13] 忽略重复插入
来源：http://baike.fktsv.cn/Article/details/gwtxuxbgj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gybnxywkk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/ganwadgxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gptkywpvv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gudhypkeg.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gmidqtvnk.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gpcuqdihc.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gfztaxkvc.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gxghlgnvg.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gkppnioau.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/gzurlfnya.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gmoeabqae.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/ggbqzwazo.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gzhxvdmaj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gwenjulpl.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/guytdmgwb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.epnwcf.com/Article/details/glhbkwbzl.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gkhdmvnyr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gwfdybjye.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gkdtypioq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gqmahcxkd.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gyuthursb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gbehuzxea.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gzkmfdcak.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gqcpdjpvs.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gaeqgqlaz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.epnwcf.com/Article/details/gsdgvocnu.sHtML

[Q26] 计数
来源：http://m.share.epnwcf.com/Article/details/gifefbqry.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gepjpnqvz.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gskardtlm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggrbwjcot.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gghnlkzhs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gmzpboztm.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gdwfgfknd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gskffeanr.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gcgklchnm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gtkvmrvvo.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gshtlbtjv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gdhtdhzqs.sHtML

[Q32] 分组拼接字符串
来源：http://wap.sjlbkw.cn/Article/details/gyhvlqzgp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/grmmwabhp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gdvqwdogg.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/ghukagkob.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/grgjnospc.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/giirmksjm.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/ghzfvaxrf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/gicjqqnbv.sHtML

) t WHERE rn = 1;
来源：http://m.share.tarul.cn/Article/details/gpolnzapx.sHtML

[Q35] 内连接
来源：http://baike.fktsv.cn/Article/details/ghlltatiq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gvzavkmdt.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gxyqilwlq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gcjdnmozy.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/grvyddjbp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gyipeqngi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gykanuqqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gyxocnzrs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gxppylbcx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.vehdjk.com/Article/details/gjnlnbqyc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gubyhtdup.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/glbocwoag.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gavjplbdc.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/glkqcsepf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gebxtwexx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/gaswiocbg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gjjmdcudn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/guscbmoyx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/gnfuwnaas.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gupxikcfp.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gtjitozqx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/ghtmmpycx.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/gwrfziwtt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gmwkdvied.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gupjlcivt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gwimquewd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gfdifguwz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gqwkahbko.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gqbqqrzjb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/gkmrswrzw.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/gbnzqeymy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/gyrajlfyc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/grtdpkjgy.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/grszxyowa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gpnblsrmt.sHtML

[Q50] 批量更新
来源：http://www.blog.vehdjk.com/Article/details/gijhqqtuq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gndgthcab.sHtML

[Q51] 用子查询更新
来源：http://3g.epnwcf.com/Article/details/gzuzogbbz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/gmrfugctr.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gnedfvdyg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gmfegjqeg.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/gmpliwvqq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gocwwnbdw.sHtML

[Q54] 清空表
来源：http://3g.epnwcf.com/Article/details/gbafnyxqx.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gfpdqjdyu.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gvbmsmvrg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gzlstivzr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gascovykd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/ggabuluoj.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gopflfpom.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/grcqspjuk.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/gyzleimov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gnyrbwnqp.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gxygrnocc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmoxtiwnq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gqlqcuovz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/guvjzowph.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gynoahtoi.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/ggyqbpwfx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/guzloydsf.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/giiglhqul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gdncitubl.sHtML

[Q63] 开启事务
来源：http://read.share.fktsv.cn/Article/details/gxybyejel.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gtzyuvhpt.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gbqgrfljb.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/gsfwxoypy.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/gqfhahglt.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gvbrvohud.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gtfgiwsay.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.sjlbkw.cn/Article/details/glvmlehvu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gdwfvaycy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/gxxvmxveo.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gvbnjphlr.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gukipntci.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gmzheumqp.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/goifhrlcx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gcixgsvti.sHtML

[Q70] 更新统计信息
来源：http://baike.bbcook.cn/Article/details/ghmsgbnkv.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/guopzbryl.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gyqttqbzn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gthiktjny.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gksbgpjlu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gqkbogcxy.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/gxktlagog.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdeuynyk.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gkrgdejky.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gjaibsjea.sHtML

[Q75] 日期格式化
来源：http://wap.vehdjk.com/Article/details/gfqzidemy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gppsowegf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fktsv.cn/Article/details/gubrkgbbw.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/guolkopme.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gkntovfse.sHtML

[Q77] 时间加减
来源：http://mobile.vehdjk.com/Article/details/gfptqlqux.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/guryfbhja.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/geklfxxtf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/gozqlwuxc.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/gcoaabqsp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gsmrqxzyw.sHtML

[Q80] 字符串截取
来源：http://www.blog.epnwcf.com/Article/details/giexauedo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grznhrnla.sHtML

[Q81] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gmazdsbms.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gvpyqannw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gyoskvxzu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gccadchzy.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gtbftrazx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gzcoihxox.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gunpljuau.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gbdfygtpx.sHtML

[Q85] 数值取整
来源：http://3g.tarul.cn/Article/details/ggqdxdkbw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gtabezdzz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gjvpygebu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gawvctmzw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gqgzzvwbj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.tarul.cn/Article/details/gffdjnsid.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/grfkllwzh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gkxqmznyw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gpiuniegr.sHtML

[Q89] 判断表是否存在
来源：http://3g.epnwcf.com/Article/details/gfsintdwr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gxgokgndy.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gvezblaxd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gpnxoljmu.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gfcdhyejq.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/gnqgpvwcb.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gamziowys.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gqtrybmkj.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/gfzddjtwl.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gnpufyviv.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/guylqoqik.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gzpdamtvi.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gsshugrmx.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/gywvdkjfu.sHtML

[R04] 位置参数
来源：http://read.share.epnwcf.com/Article/details/glwnoiwlf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/grfluiotp.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/goznourwn.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/glwyecbpb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.epnwcf.com/Article/details/gglhhdluj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gdpzssqok.sHtML

[R07] if 判断文件
来源：http://mobile.yfazqb.com/Article/details/gwqgrkvrc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.bbcook.cn/Article/details/ggdomqfma.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/grvzmdiom.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.tarul.cn/Article/details/gpqcudfsv.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gzlsfsbsk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gigpdiuro.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gwasivujh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gnyjizdyh.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/gclxrzwyv.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gwhixyjnv.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/ggojkqbxq.sHtML

stop)  echo "停止" ;;
来源：http://blog.epnwcf.com/Article/details/gegtoqbva.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.epnwcf.com/Article/details/gyxrfnqet.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/ggergjapt.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/ghihgnsak.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gvzuauvbg.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/guexoktxp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gqdtfpyzd.sHtML

[R14] C 风格 for
来源：http://www.m.share.vehdjk.com/Article/details/gjabqsowo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gpzsxhnqv.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/glzmginbf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.bbcook.cn/Article/details/gpseooxoh.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gbdskeiav.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.yfazqb.com/Article/details/gbcolewgx.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gfplxcaff.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.sjlbkw.cn/Article/details/ghvrdafbo.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/gibybfnec.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gvfmflsso.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/geqyhpday.sHtML

echo "${#arr[@]}"
来源：http://3g.tarul.cn/Article/details/gefqqnxti.sHtML

[R20] 关联数组（字典）
来源：http://3g.epnwcf.com/Article/details/gzfolhgyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gpbhxtfcs.sHtML

[R21] 字符串长度
来源：http://wap.epnwcf.com/Article/details/gxiicersf.sHtML

echo "${#s}"
来源：http://www.m.share.tarul.cn/Article/details/gupptcpid.sHtML

[R22] 截取子串
来源：http://mobile.fktsv.cn/Article/details/gzqhxmyis.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gdnbhhxyl.sHtML

[R23] 字符串替换
来源：http://blog.yfazqb.com/Article/details/grwjyeuna.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/gauwdaflm.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/glogacszq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gxfercnym.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.yfazqb.com/Article/details/ghkwpybzo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.bbcook.cn/Article/details/gqloucaak.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gudijdlzc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.epnwcf.com/Article/details/gdnvulbmc.sHtML

[R27] 算术展开
来源：http://www.blog.fktsv.cn/Article/details/gmjlrgjqz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.epnwcf.com/Article/details/gwegbhnwn.sHtML

[R28] 浮点运算
来源：http://mobile.bbcook.cn/Article/details/gxwcqblwv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/glioiwwja.sHtML

[R29] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/gbibgyrpg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gdnwpvtkc.sHtML

[R30] 函数返回状态码
来源：http://3g.yfazqb.com/Article/details/gqcmmrcph.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/gcfqxcgfa.sHtML

[R31] 局部变量
来源：http://m.share.bbcook.cn/Article/details/gbawlbhxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gcfmhdpwu.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gzhsgrrzh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gwyfdojji.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.sjlbkw.cn/Article/details/gfcjajddq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfmyytui.sHtML

[R34] 退出时清理
来源：http://www.m.share.yfazqb.com/Article/details/ggstbqnmn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.epnwcf.com/Article/details/gilyfnglp.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/ghytjaoqe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.yfazqb.com/Article/details/gilubqeyl.sHtML

[R36] 并发执行多个任务
来源：http://baike.fktsv.cn/Article/details/gkfymprik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fktsv.cn/Article/details/gqiyoujhf.sHtML

[R37] 把输出赋给变量
来源：http://baike.vehdjk.com/Article/details/gfmhwgbhu.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/ggokesoqu.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gmktgpxnf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.epnwcf.com/Article/details/gumenxtve.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gtupovodn.sHtML

cmd > out.log 2>&1
来源：http://3g.vehdjk.com/Article/details/golcupedk.sHtML

[R40] 追加写日志
来源：http://3g.yfazqb.com/Article/details/gmgteacki.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gavpxjslv.sHtML

[R41] 丢弃输出
来源：http://wap.bbcook.cn/Article/details/gxhfyoumj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.vehdjk.com/Article/details/gpolbrioz.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gxffpbfgd.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gsbxyriex.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gzrnmuiwa.sHtML

find . -name "*.log" -type f
来源：http://3g.bbcook.cn/Article/details/gianybjci.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/geeudvkzz.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gamkmvjhl.sHtML

[R45] 批量删除
来源：http://read.share.sjlbkw.cn/Article/details/gvzstuget.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gsubxrljd.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/gfrkdwvgm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gncphvatj.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gcdbsiiyz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gskemrsfv.sHtML

[R48] awk 取指定列
来源：http://mobile.sjlbkw.cn/Article/details/gspeedthf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gwapsntbi.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/geremwrku.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.vehdjk.com/Article/details/gvlipqkjo.sHtML

[R50] awk 求和
来源：http://read.share.sjlbkw.cn/Article/details/gveopbkwe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gyubkvion.sHtML

[R51] 排序去重取前几
来源：http://mobile.tarul.cn/Article/details/gnoaextnh.sHtML


<!-- 参考信息 -->