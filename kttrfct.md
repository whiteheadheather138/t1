代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gqfuhhpnz.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gqdvsrtui.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/guvmopkwp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gavpdjvjn.sHtML

);
来源：http://baike.tarul.cn/Article/details/gfkxonbhp.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gumalpgzj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gjjjgqogp.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/ggdywkrvw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/gogacfsra.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gfcxzejpw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gyxlqzibu.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/geieehukd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.tarul.cn/Article/details/gkumrmmio.sHtML

[Q07] 删除表
来源：http://wap.vehdjk.com/Article/details/gvbqpctex.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gdftwdqnm.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/govxdrxut.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gkckmjhil.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gsbrdtdtj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gzekpyxve.sHtML

[Q10] 插入单行
来源：http://read.share.sjlbkw.cn/Article/details/gvjhifydt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gqfatqmwh.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/gkbovpzcj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gaxlzvbre.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fktsv.cn/Article/details/gouwhqrsn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/glzjyfmcs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/gcuycihah.sHtML

[Q13] 忽略重复插入
来源：http://wap.bbcook.cn/Article/details/gjkhmotio.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gqkektqpa.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gqhvnqtvo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gbuxpltmt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gdscpwyer.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gzwpdamwc.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gpoqsdgif.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gcbqkwkxw.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gclnhgyfj.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gzkzxearf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gwdmnwkzp.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gymjzefhg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gyompjkle.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/grepamqoq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gthtmodvq.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gjuyfgmit.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gayloklwk.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gilkxexhm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/guqjwmuje.sHtML

[Q22] 排序
来源：http://www.blog.epnwcf.com/Article/details/gzfngivnp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/gxtlwhhih.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/giegvnzne.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/guqwzwemi.sHtML

[Q24] 去重
来源：http://baike.bbcook.cn/Article/details/gmfsawcsw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gvyivwhoy.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/gqesdmpdn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gaemvejzj.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gbkbcllny.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gulzgemyx.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gzacvmzfg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gzjuojywf.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gueasrplg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/ghirjgcav.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gfkphfkrw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gcrlmmjgk.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gzszykseb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gsbplttmo.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gdxthzbef.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/gdayoewth.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gytnnmosn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/grqghoulv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gtfcxcctw.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/gexagpbrn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/glmxutuds.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gmfqttxkv.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/glmvuunir.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gywieubqz.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gtqqwyzoj.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gptlzvsux.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/ggyfaczvw.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gmucihmec.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gwarqpyns.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/ghwxzexjv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/gkxxemibx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gzhqkgett.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gmbmzacjn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gmdtkicow.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/glmlbllpi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gdtgoucjw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/ggzlmelyv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gfgcfwpbj.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gziwpoerr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/ghhyzktro.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/gkogudyte.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/gkkrujvtn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gfdbnuxpm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gdzzckhey.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/grxoayyxa.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gwnxaqcid.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/gsyncgilj.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gamwjvkym.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gcfewojku.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fktsv.cn/Article/details/gxbnsojxh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/ghngigveo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/goxokdhiu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/ghmbdzhkb.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gvdjibyhg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/glkkjjmff.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gvfvmepha.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.vehdjk.com/Article/details/ggovnomet.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gzpkblhzy.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gjahigwny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gdqwfsxsr.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gittvnhqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/ggjqcqybl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gylrvzojl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.vehdjk.com/Article/details/gcklkpwvz.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gpxyqidwo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/ggkkqafih.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gbktbqyxc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gmiwroxoz.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gmswnahlj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.epnwcf.com/Article/details/gggghffts.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gzouvgfne.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/ggfyqphgl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gyyznjeim.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gevbyiize.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gucicmioi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gvuyxnmka.sHtML

[Q58] 累计求和
来源：http://www.m.share.epnwcf.com/Article/details/gklzsgyzj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/ghlmfpmgu.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gjkqmfbny.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gwnvnhcur.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.yfazqb.com/Article/details/gmoayhtpa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gustffjkx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.tarul.cn/Article/details/gwgfutnki.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gpxvfohnn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gzsvxxcou.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gnbxvtsgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gjqsyjoqs.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gghhztjld.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gwehoknuy.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gwbnyhplt.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gpepamloc.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/gndznsruk.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gtmviabiq.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gvakzeckg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/gydlmnbtk.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gtjvyhxdu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.vehdjk.com/Article/details/gdndlwcoy.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/gqoauawdl.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gaxbyvcdu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gmvzgqtav.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gwqgjrfrp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gnkxcqixt.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/grmgfdvdg.sHtML

ANALYZE TABLE users;
来源：http://read.share.fktsv.cn/Article/details/getzngfpb.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/ghbyskwfd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.bbcook.cn/Article/details/gilonyvkn.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gvwrvsrbh.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqyoolpdg.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/grydnrovq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gmjhebdns.sHtML

[Q74] 强制使用索引
来源：http://blog.sjlbkw.cn/Article/details/ghbjkaqjq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gdumptjqq.sHtML

[Q75] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gybbuwxgx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gkstrgxgu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gmewujkoo.sHtML

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/gtvwitdbm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/gdsumfqvf.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/ghidnfhpj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gvypbgrzf.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gznijkcie.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gbmpcfmdd.sHtML

[Q79] 字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gcnnvtzka.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/giqqyjigx.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gsrtralwt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.tarul.cn/Article/details/giaxwsmso.sHtML

[Q81] 字符串替换
来源：http://m.share.fktsv.cn/Article/details/glejklznh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gkkzsfsxf.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.vehdjk.com/Article/details/gnncjzxfk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/ggvpevdnl.sHtML

[Q83] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gkdjowbpm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gvodgrxgj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/gwasumjsn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gnhjyvrvn.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gtdrsigoj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gdkwghzpr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/gpaksfdxl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gyxmhycej.sHtML

[Q87] JSON 字段做条件
来源：http://baike.bbcook.cn/Article/details/gchubqufa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.tarul.cn/Article/details/gpjcceobi.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.vehdjk.com/Article/details/glkzbcggu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gieifkubk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gmvsisfbz.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gnyiyxmts.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gblgudefb.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gydmovrqd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gnqjoopcw.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gpfmcheax.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/grutzllnh.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gdvjhzqfe.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gzqzmifok.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/gqqyxximm.sHtML

set -euo pipefail
来源：http://mobile.tarul.cn/Article/details/gtcsuwbwj.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/glspsmksq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gbjejaord.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gqcjfnkoq.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/glzrtnisq.sHtML

[R04] 位置参数
来源：http://mobile.yfazqb.com/Article/details/gdkifklle.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gmwrozbfz.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gmzszhrvl.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/gcqwcjyox.sHtML

[R06] 判断命令是否存在
来源：http://baike.fktsv.cn/Article/details/gtfnjprfm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gckunbkjf.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/gtxzabvty.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.tarul.cn/Article/details/gtyilgvfi.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gckotzjbb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.yfazqb.com/Article/details/gfgihsxxx.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/ghkvjkdzw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gjywtckdi.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/ggnvzxzlj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gszgxkjrz.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/gjkgbqpbg.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gplegzjld.sHtML

start) echo "启动" ;;
来源：http://read.share.tarul.cn/Article/details/gkltmbghq.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gbjfjqhke.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gvtodndzf.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gxyxegrqc.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/genjdewth.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/goreranrq.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gchexvzwf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gnmuaenvh.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gpjmitbqt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gnauvdbhg.sHtML

[R15] while 逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gseegkldl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/ggdamyvng.sHtML

[R16] until 等待条件
来源：http://wap.sjlbkw.cn/Article/details/gdqgitcil.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/ggcgpjnht.sHtML

[R17] 数组定义与取值
来源：http://baike.tarul.cn/Article/details/gmabdhlah.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.epnwcf.com/Article/details/guslrabnl.sHtML

[R18] 遍历数组
来源：http://baike.sjlbkw.cn/Article/details/gawdeyghk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gwfqqiloc.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gbvfyilyy.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gfjwyvsdl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/giqgtdlui.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.vehdjk.com/Article/details/grcolvass.sHtML

[R21] 字符串长度
来源：http://www.blog.vehdjk.com/Article/details/gxzkamjim.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/gpvlcqhwl.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gxdoepcia.sHtML

echo "${s:0:5}"
来源：http://blog.sjlbkw.cn/Article/details/gtfyfstav.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gfbmpnxqn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gryzbmfnb.sHtML

[R24] 大小写转换
来源：http://3g.vehdjk.com/Article/details/gfsuiihfr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.sjlbkw.cn/Article/details/ghiyltnrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.tarul.cn/Article/details/gozuwlcqc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/gkmhgdxzo.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/giumioyeg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fktsv.cn/Article/details/gkkosvurm.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gdrugyxvi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.vehdjk.com/Article/details/gwtttyjgm.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gbwvhrixn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.yfazqb.com/Article/details/gtgjvjkni.sHtML

[R29] 定义函数
来源：http://www.share.vehdjk.com/Article/details/gccywpbvl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.bbcook.cn/Article/details/gmwdgwdbw.sHtML

[R30] 函数返回状态码
来源：http://mobile.tarul.cn/Article/details/glhfysodd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.vehdjk.com/Article/details/gpuymhkpk.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gjabandew.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.sjlbkw.cn/Article/details/gefndsfzm.sHtML

[R32] 参数个数校验
来源：http://mobile.fktsv.cn/Article/details/gvhiadfrv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/ggdjqtpop.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gvzfvosgu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fktsv.cn/Article/details/gsyasiiya.sHtML

[R34] 退出时清理
来源：http://read.share.vehdjk.com/Article/details/gprbivxnl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gpvgrugtf.sHtML

[R35] 后台执行并等待
来源：http://www.share.sjlbkw.cn/Article/details/gjgefvfcn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/ggjmyompi.sHtML

[R36] 并发执行多个任务
来源：http://mobile.yfazqb.com/Article/details/gbjovxnrz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.yfazqb.com/Article/details/gwrbjadot.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/gcfsnxgrr.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gxkekydyw.sHtML

[R38] 管道串联
来源：http://m.share.bbcook.cn/Article/details/glybivstp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.tarul.cn/Article/details/goufuwfnk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gbkqnzitv.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fktsv.cn/Article/details/gfkmsonuz.sHtML

[R40] 追加写日志
来源：http://www.blog.epnwcf.com/Article/details/gxoiiiyqj.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gqziwxtpc.sHtML

[R41] 丢弃输出
来源：http://read.share.tarul.cn/Article/details/gucebbhme.sHtML

cmd >/dev/null 2>&1
来源：http://baike.yfazqb.com/Article/details/gzafpawfd.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/gzznwwbfc.sHtML

wc -l < a.txt
来源：http://3g.tarul.cn/Article/details/gsmetuoay.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gfovhmkgb.sHtML

find . -name "*.log" -type f
来源：http://www.blog.yfazqb.com/Article/details/gmgjpqngb.sHtML

[R44] 按修改时间查找
来源：http://3g.fktsv.cn/Article/details/gikkqfjcx.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.epnwcf.com/Article/details/gmxxqvpyy.sHtML

[R45] 批量删除
来源：http://read.share.fktsv.cn/Article/details/gunxqfzer.sHtML

find . -name "*.tmp" -delete
来源：http://wap.bbcook.cn/Article/details/gminsbipy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gcofjxzrz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.epnwcf.com/Article/details/gvhqjvxls.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/garcjjyoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gjoszngcl.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gxtdlyelm.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gkkkmcojp.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/gkiasyili.sHtML


<!-- 参考信息 -->