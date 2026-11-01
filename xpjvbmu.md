代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gvfcqvszc.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gfcqpuatl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gdutugvll.sHtML

[Q06] 删除列
来源：http://wap.epnwcf.com/Article/details/gmacdauuu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gwdanqdjy.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/gtmemwhhg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/graqcwwwh.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gtkmiqajp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/giavcjezy.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gfwhnnfwq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gukzxtmid.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/gdwwiixta.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/gwahhskmc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/gbgohdsyo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gfbabgzks.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gdlydxecu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.vehdjk.com/Article/details/gkbddbprt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gployijez.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gdddiaylm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gjarbpnyk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gtzkxpkpr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gsdkghgwh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/gyhhtzitr.sHtML

[Q15] 查询全部
来源：http://www.share.epnwcf.com/Article/details/glahriqwg.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gzlzhhtzt.sHtML

[Q16] 查询指定列
来源：http://www.m.share.bbcook.cn/Article/details/gogvtbihi.sHtML

SELECT id, name FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gnikzilhh.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gsoqaruaw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gvkrilady.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gnkwjplfd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/gowyziodp.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gevbonbqy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gmduyzzrz.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gxirdcxfc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gthnnmnny.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gprzamtok.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/ghojpxzgd.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gxwxzkhux.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/grdytdhfa.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gsgfqofhs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/ghlcrkoqe.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gwcrtgmrx.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gulxgdzji.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gdoiskrsc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gmicysiaq.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gyqfvgbnl.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gyehxrzvh.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gigdtxzop.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gdnjrvjlg.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/glqclgdsr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gkregbmzl.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/gcqyzsiri.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gbusxozvz.sHtML

[Q30] 分组统计
来源：http://www.m.share.tarul.cn/Article/details/giuygydhu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/galgipeti.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/ggnkibejb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gguetrtgm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/ghkucgnza.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gcfzxqtwf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.epnwcf.com/Article/details/ginpyxrck.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gpvvxxofi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gfmksmruu.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gwacwilel.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/gtbaxsacm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/glymsxrve.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gumwgpvab.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gnpghtuyo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gvkkbwrlj.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/ghbuoxcax.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gdpjpafyu.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gzuftiyhv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/ghpxlospj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/gsuiicgyp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.tarul.cn/Article/details/gzmtwxexo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/ghkxdtmzx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gwgrqxryb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gpkshyxgk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gunetilqv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gfukpwktu.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gjgjtidar.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gcfxckgza.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gjooazdig.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gesdpuwos.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.epnwcf.com/Article/details/gcjzxrnvp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gzwmtqzlg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.vehdjk.com/Article/details/gmsyvnbhw.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gslgieqhq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/glamiahvy.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/geevxvaww.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gbsijliyf.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/gpifhqajr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gybnfysbz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gbzckxzun.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gmlhmkjrm.sHtML

[Q47] 与平均值比较
来源：http://3g.tarul.cn/Article/details/gibtofbud.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gmtojgdfk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/gqjmfrkcl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/guucvdbwl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gqzdhchqr.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/gwndzpbez.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gwedksvch.sHtML

[Q50] 批量更新
来源：http://www.share.epnwcf.com/Article/details/gnmqdpikw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/groqxfbez.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gxiysmqhm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.vehdjk.com/Article/details/gihokaqye.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gidzjizij.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gpoyoybfs.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gwhiupewh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gnlcvmkfk.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gylbaeoxb.sHtML

TRUNCATE TABLE logs;
来源：http://3g.epnwcf.com/Article/details/ggmzydfxc.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gtfcerzvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gvtivuxrh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/gzhcpmulj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gvdrqwpmy.sHtML

[Q57] 行号
来源：http://mobile.sjlbkw.cn/Article/details/gadfukjlv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gijfgqrbz.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gppzorxuq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gokypvsmw.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/goddwuffn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdzcougp.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gxijeucdx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gbjxartui.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/ggzzmjnba.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gwwuntscd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gbbujbhpw.sHtML

[Q62] 分组占比
来源：http://www.share.sjlbkw.cn/Article/details/gwzkmawoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gfwrrttwr.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gfgwobqdp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gbfggtpvf.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/gejlyebgp.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gcwyoelig.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gmnxvdrwb.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gobrmalno.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/gvqiortny.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gtelpibvc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gkcvioeyf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/goqwgdqen.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gfjocvnki.sHtML

SAVEPOINT sp1;
来源：http://blog.yfazqb.com/Article/details/gddeudgio.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gqlsxoxpo.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gbeofepmt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/ggibudauu.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gqgpihbqk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/gaznrncyr.sHtML

[Q71] 查看建表语句
来源：http://baike.sjlbkw.cn/Article/details/gkkrtfzoo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gsaxquuvf.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gplmnjegu.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gnkkovbkd.sHtML

[Q73] 查看表状态
来源：http://read.share.tarul.cn/Article/details/gqbpccuzy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gewycerzc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/gqkrfrwrl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gwkzwwzzc.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gfohyaoav.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.epnwcf.com/Article/details/gxffzynao.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gulpmdwcq.sHtML

[Q76] 按天统计
来源：http://3g.epnwcf.com/Article/details/gcbbysxnd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gmuxjzazk.sHtML

[Q77] 时间加减
来源：http://blog.vehdjk.com/Article/details/grwxjdwid.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gnkkpqbnx.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gwicwzhbi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gvtbxykjt.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gatyfpqab.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gdmejdiib.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/gnlzvvvgm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gpjdafsqu.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gerkimebm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gvrbwstpx.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.sjlbkw.cn/Article/details/gnuaeuyns.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gyhgpgmjt.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gfwtjpkfm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/ghcwbbffd.sHtML

[Q84] 去除首尾空格
来源：http://read.share.epnwcf.com/Article/details/gjyibyqvi.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gjnhvvyiy.sHtML

[Q85] 数值取整
来源：http://wap.epnwcf.com/Article/details/gxhxawqyq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/glnaloqfl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.epnwcf.com/Article/details/gnwvrtmrp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fktsv.cn/Article/details/gzvbhtptx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.tarul.cn/Article/details/gwzrmwldo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gzrdveqfq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.tarul.cn/Article/details/gpngitqym.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gvtuieuoc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gadojtwea.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gvdlzeuqz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/ghyposzbm.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gmayaemyy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/gejuegfkd.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcmmitvcl.sHtML

R. Bash 专题
来源：http://wap.fktsv.cn/Article/details/gucpuyztn.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gyvuodbgx.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gltyneaer.sHtML

#!/usr/bin/env bash
来源：http://www.share.tarul.cn/Article/details/gdjlbhdwh.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gnerujtyw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.epnwcf.com/Article/details/grvyswhnc.sHtML

name="Tom"; echo "$name"
来源：http://3g.bbcook.cn/Article/details/gkooimovq.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gqcbgpxcz.sHtML

readonly PI=3.14
来源：http://wap.tarul.cn/Article/details/gvdrpnxbu.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/goooutbun.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.yfazqb.com/Article/details/gfdkinszw.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/ghodqidbl.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gkvtytvie.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/grbwkallc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/giuxhzfav.sHtML

[R07] if 判断文件
来源：http://m.share.sjlbkw.cn/Article/details/girpozmbg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.yfazqb.com/Article/details/gnmqhhzpp.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/glyibqiei.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtkgsnxj.sHtML

[R09] 字符串比较
来源：http://m.share.bbcook.cn/Article/details/giucrxsmb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.epnwcf.com/Article/details/goidrijrb.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gkdmyrhwk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/gchqknlaw.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gvasjfuxc.sHtML

case "$1" in
来源：http://read.share.tarul.cn/Article/details/gezhdpkdj.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gyhvzhqep.sHtML

stop)  echo "停止" ;;
来源：http://wap.sjlbkw.cn/Article/details/gvzxtzmye.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/ghylvitrf.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gtcybnxmi.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gfbyfmrfq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.vehdjk.com/Article/details/gcssxgsxs.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gincnggwq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gvyxohgig.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/gbffzdgfc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gqlrqtmhi.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/gclvrezzi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gnlijmrlp.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gtwbisfaw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gcqggfqdc.sHtML

[R17] 数组定义与取值
来源：http://mobile.bbcook.cn/Article/details/gbhamtsle.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.vehdjk.com/Article/details/gghtgqhsl.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gqbymledd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.bbcook.cn/Article/details/gavsbkgzk.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/gkauxbcss.sHtML

echo "${#arr[@]}"
来源：http://www.share.tarul.cn/Article/details/gfabtzzol.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gsjjarbjv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gfvijemsm.sHtML

[R21] 字符串长度
来源：http://blog.fktsv.cn/Article/details/gjstxboue.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gaetungui.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gdaeirzwq.sHtML

echo "${s:0:5}"
来源：http://wap.yfazqb.com/Article/details/gtuqewunu.sHtML

[R23] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gyameikqu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gpjptqrsc.sHtML

[R24] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gwkwvmiyc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.yfazqb.com/Article/details/gisojjedb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.sjlbkw.cn/Article/details/grgtudxdc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/gbiqmrqfs.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/gclxwxclz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gqxnktiri.sHtML

[R27] 算术展开
来源：http://read.share.epnwcf.com/Article/details/gbdsopboz.sHtML

echo $((1 + 2 * 3))
来源：http://3g.tarul.cn/Article/details/gpxmcskhk.sHtML

[R28] 浮点运算
来源：http://m.share.yfazqb.com/Article/details/gqvkrlpal.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fktsv.cn/Article/details/gnsqkyxeh.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/getdkprbj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/gdtrwdbrn.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gzhwcaxkq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fktsv.cn/Article/details/gtlwsooxh.sHtML

[R31] 局部变量
来源：http://read.share.epnwcf.com/Article/details/gmhoawdwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gmzmyanzo.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gfkgqrnqq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gdjvormlo.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gaobwxscw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.tarul.cn/Article/details/gsvjsbiac.sHtML

[R34] 退出时清理
来源：http://baike.yfazqb.com/Article/details/gzbjkxcme.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gxzwdhjfz.sHtML

[R35] 后台执行并等待
来源：http://baike.epnwcf.com/Article/details/ghppowchb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.bbcook.cn/Article/details/gpmkldduv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.sjlbkw.cn/Article/details/gtauzculk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/ghsbuhcfh.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gnjmhxgdh.sHtML

files=$(ls -1)
来源：http://mobile.sjlbkw.cn/Article/details/glhvfvxxs.sHtML

[R38] 管道串联
来源：http://baike.sjlbkw.cn/Article/details/gqeacankv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/guxhnofof.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.bbcook.cn/Article/details/gxcjytsye.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gkgheipin.sHtML

[R40] 追加写日志
来源：http://wap.epnwcf.com/Article/details/gsvwlhkto.sHtML

echo "log" >> out.log
来源：http://read.share.vehdjk.com/Article/details/girlwpenp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.epnwcf.com/Article/details/gmacerbgj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fktsv.cn/Article/details/gvykmmuqu.sHtML

[R42] 输入重定向
来源：http://www.m.share.vehdjk.com/Article/details/gdxjihqza.sHtML

wc -l < a.txt
来源：http://www.blog.epnwcf.com/Article/details/ghyizqhrg.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/gyfuwogup.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/ghjqazawn.sHtML

[R44] 按修改时间查找
来源：http://blog.tarul.cn/Article/details/grrnwcpab.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/gbhgdbkcd.sHtML

[R45] 批量删除
来源：http://3g.bbcook.cn/Article/details/gcjysgggb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gdkckfqnd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gairzyoqg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.tarul.cn/Article/details/gfxzhxitd.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fktsv.cn/Article/details/ggrdrsrao.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.sjlbkw.cn/Article/details/ggznuznuk.sHtML

[R48] awk 取指定列
来源：http://baike.fktsv.cn/Article/details/gaqlfjppm.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.vehdjk.com/Article/details/gnuvdetgn.sHtML

[R49] awk 带条件
来源：http://www.blog.fktsv.cn/Article/details/glydrikdi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.yfazqb.com/Article/details/ghhrkogil.sHtML

[R50] awk 求和
来源：http://baike.epnwcf.com/Article/details/gtvqgsizf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fktsv.cn/Article/details/gtovcexxl.sHtML

[R51] 排序去重取前几
来源：http://wap.tarul.cn/Article/details/gypizjuks.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.vehdjk.com/Article/details/gabzdrpfn.sHtML

[R52] 统计行数
来源：http://wap.fktsv.cn/Article/details/gfgfdohun.sHtML

wc -l a.txt
来源：http://m.share.bbcook.cn/Article/details/gsqnuacgn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.epnwcf.com/Article/details/gvwmkvxfd.sHtML


<!-- 参考信息 -->