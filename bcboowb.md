代发 wailian999

);
来源：http://mobile.vehdjk.com/Article/details/guvdwldnn.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/geakpakry.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/guybsmlzr.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gazmvysbs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.bbcook.cn/Article/details/gffmgqebf.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gcjjvcmoa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.tarul.cn/Article/details/gglfdmdoj.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gznnkcsnb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/gcgnwtfmp.sHtML

[Q07] 删除表
来源：http://m.share.vehdjk.com/Article/details/gzvbaiflf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.sjlbkw.cn/Article/details/gsamekigc.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/glhrnwome.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gynkrhfsx.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gjlqyamta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gkvrxspdi.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gjhzvgzgr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/grqumgsxt.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/gjursrfqe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gviajxscn.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gwkosevco.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gjfwupjyo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fktsv.cn/Article/details/gapdjdvvs.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fktsv.cn/Article/details/gfjrtfymz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gfxmcekjs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.tarul.cn/Article/details/gspqfflzl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gblooipvb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gonclkteq.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gthrsuijf.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/giognvpyl.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/ghwbiwmxx.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/ggscfnhus.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/gwtujpsyy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.epnwcf.com/Article/details/gznyczxtw.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/ggnxmycnu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gfzxeidvl.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gajafjwfb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gtvtjeqfl.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/gplpvxxoo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gslslhpou.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gwsyubcoc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/gokrohpag.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gpcyrimlq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/gslzdcynb.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/gjysqoyjv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gizdbfwwm.sHtML

[Q24] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gjuknvsgs.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/gixkmbchq.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gpajowicq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gihlyqbqo.sHtML

[Q26] 计数
来源：http://www.blog.tarul.cn/Article/details/glshtpljg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/geqhmoutn.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gcuqjrqkx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gildmhgjb.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gmetngdzp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gvwqryvrr.sHtML

[Q29] 最大最小值
来源：http://mobile.tarul.cn/Article/details/gkatxxguv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gdqcuyeew.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gvgnplrvl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gnohaceyl.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gcymlgxjj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gbtujbcih.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/guchigrsf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gdndslzid.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/grinbremp.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gaoyxwcjx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/guqglsucq.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gxwradhab.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gitxxeala.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/gtlualuqw.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gzkqmajph.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gzzwckwiy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/glpgbgycw.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gswwasbqr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gfzkscgga.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gwiqajqna.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/ghkpcclnp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gakukwjnh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fktsv.cn/Article/details/gzyglmwhw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.bbcook.cn/Article/details/gqjhcquaa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gwjbqdpwg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/ghhjlhblw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcayqgbih.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gikalwhya.sHtML

[Q41] 多表连接
来源：http://mobile.yfazqb.com/Article/details/gyecnznam.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.tarul.cn/Article/details/gobcrevuh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gktffwgpj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gvyphfzby.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.yfazqb.com/Article/details/grfxvlqvl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/geodihmph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gntbspuqd.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gdfesnyhu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gcaowdoov.sHtML

[Q44] IN 子查询
来源：http://baike.vehdjk.com/Article/details/goxufjdxv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gsrpddlhw.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/gnvnsrcpg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gnsgamnex.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/glkrgdlpy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gikzitbbf.sHtML

[Q47] 与平均值比较
来源：http://m.share.tarul.cn/Article/details/gekxzjrrr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gjicbiozy.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gsikztjbp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.tarul.cn/Article/details/grunbybxz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gwfkscnap.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/ggazumkdj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gtxbazhsv.sHtML

[Q50] 批量更新
来源：http://www.blog.tarul.cn/Article/details/ghafozrxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.vehdjk.com/Article/details/ggdziqimk.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gpiyzxnsy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gmjyzgcji.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gqcxiayoo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gibtzmwrj.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/gnfkybyuf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gkognhnim.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/gezpnukef.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.bbcook.cn/Article/details/gxzuhegyi.sHtML

[Q55] 排名（并列占位）
来源：http://wap.bbcook.cn/Article/details/grljyvlhx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gqnboktyz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gaqfjqbgu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gsbhknzjd.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/gotrhyxlh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.bbcook.cn/Article/details/glgxjhnbo.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/glypdkcpu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/gippgkact.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/gynyqatpn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.tarul.cn/Article/details/gmrsfuole.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/ggjkkwmaw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gcfrigmty.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gzjngqjzn.sHtML

[Q61] 移动平均
来源：http://read.share.sjlbkw.cn/Article/details/gtwauhper.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gpfkvctdb.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/ggbpcbule.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gycdormpr.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/geyepdxvs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gjjudkoog.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gdqxbchmx.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gjfxkqghm.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/ggnilicij.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gutahwgeh.sHtML

[Q66] 行锁查询
来源：http://blog.fktsv.cn/Article/details/gqyvyigej.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gpxgvvkai.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gxyiihkur.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.epnwcf.com/Article/details/geyljqtaz.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/guyyayvsk.sHtML

SAVEPOINT sp1;
来源：http://baike.bbcook.cn/Article/details/gqgdkjfno.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/ghginuwip.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/ggabuppri.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/gcjmerrxc.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gwrizifem.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gogmnvjeq.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gfacyzklv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.vehdjk.com/Article/details/gurvovfhj.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/ggfbvielc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gylxpkpvh.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/gxbnpyheb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gftazyvbf.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gepikxzxl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gzhvvgoap.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/gkthhmhxi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gayxhehyn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/grxgqgtpq.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gydjwedxs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gxygfehfk.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/gldasvfui.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gomshzrni.sHtML

[Q78] 当前时间
来源：http://blog.sjlbkw.cn/Article/details/gueixqeqc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gdvmngblf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/ghpcjwosp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/ggcucvlyo.sHtML

[Q80] 字符串截取
来源：http://www.share.vehdjk.com/Article/details/gwkuunhwf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gpthakcft.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gdvjrwrcd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fktsv.cn/Article/details/guvealnag.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/gtmuscyks.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gplimekjo.sHtML

[Q83] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/gtlidccej.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gobpyuyin.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gxyslcvuh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glazdaqdm.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/ggjhochsf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/gdkblmgtr.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/goetxyrdz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gpyphusfa.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.tarul.cn/Article/details/gzftitzhw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.bbcook.cn/Article/details/gyqftsmny.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gtpzjkvoz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gjnjwseir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gxytfvufo.sHtML

[Q89] 判断表是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gwhwalcsl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gujoirmpr.sHtML

[Q90] 生成序号列
来源：http://3g.epnwcf.com/Article/details/gclvtsltc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gkzmqcbxu.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gjcritcrt.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gasgxkkay.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggphkohni.sHtML

[R01] shebang 与严格模式
来源：http://wap.tarul.cn/Article/details/gflkldkmo.sHtML

#!/usr/bin/env bash
来源：http://mobile.vehdjk.com/Article/details/gxyyhgdyx.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gjvgcwwcy.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gnfocwnqt.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gcxevcwsy.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gepfltjtd.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gfthctglp.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/gitkozwrr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gknbztvng.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/gkvbcbgqp.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gpvueuyxx.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/glfolktgb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/ghaxptazx.sHtML

[R07] if 判断文件
来源：http://3g.bbcook.cn/Article/details/gtfbnedps.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/guyxukwuj.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gseuhxagh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gjapmemza.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gbwqhoesz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.yfazqb.com/Article/details/gyyetbixw.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gvzmtplyh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.epnwcf.com/Article/details/gxzhsrqsc.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/ghtduxixo.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gkzrgwpvk.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/gilsnmvxs.sHtML

stop)  echo "停止" ;;
来源：http://wap.bbcook.cn/Article/details/gbnzquhuf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gjlfourki.sHtML

esac
来源：http://mobile.fktsv.cn/Article/details/gskyyrmph.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/gnzhjsvoj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fktsv.cn/Article/details/gfuzssuxq.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgmotejq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gytlamsux.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gyggqbtwy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gohcxvqov.sHtML

[R15] while 逐行读文件
来源：http://wap.epnwcf.com/Article/details/ggfuinpif.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/gfapnwvqc.sHtML

[R16] until 等待条件
来源：http://read.share.yfazqb.com/Article/details/gtnffsekj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.bbcook.cn/Article/details/gxaigpcac.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.bbcook.cn/Article/details/gueibrqnh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.sjlbkw.cn/Article/details/gxiutupxy.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gunnhqbmz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.epnwcf.com/Article/details/gntybsvdi.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gtxxvpgio.sHtML

echo "${#arr[@]}"
来源：http://www.share.vehdjk.com/Article/details/gwotjxamb.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gjogcsfiy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gxujhakjr.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/gbvjjsipl.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/gndcunnjp.sHtML

[R22] 截取子串
来源：http://blog.vehdjk.com/Article/details/gckuxlgtw.sHtML

echo "${s:0:5}"
来源：http://m.share.yfazqb.com/Article/details/gqtpxanhs.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gymwjgzsp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.yfazqb.com/Article/details/gzyeedzaz.sHtML

[R24] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gatdcoank.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gqalppozy.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.sjlbkw.cn/Article/details/gghbrgbwi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.tarul.cn/Article/details/grpjexhyj.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gonslhvkt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gayrmyftw.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/ggtostzwj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gtahbexls.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gtjiyckhy.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.epnwcf.com/Article/details/gzbsdofbq.sHtML

[R29] 定义函数
来源：http://baike.epnwcf.com/Article/details/gjrmanfdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.vehdjk.com/Article/details/gxgqkanxw.sHtML

[R30] 函数返回状态码
来源：http://mobile.fktsv.cn/Article/details/ggwszizug.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/gaabrpxrj.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gblcatkcy.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gsczqampf.sHtML

[R32] 参数个数校验
来源：http://3g.vehdjk.com/Article/details/gwyzqqncj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/ggmxwgunz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.bbcook.cn/Article/details/gwsveczsu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.epnwcf.com/Article/details/gjejgmcmf.sHtML

[R34] 退出时清理
来源：http://3g.epnwcf.com/Article/details/gschhbvpe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/gwogngxag.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/gihqjzlmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fktsv.cn/Article/details/geimdvtef.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/gpcexhjqc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.yfazqb.com/Article/details/gdbslwrdu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/gzxbvmrlx.sHtML

files=$(ls -1)
来源：http://m.share.fktsv.cn/Article/details/geaqncrfc.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/ghvishuvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gpkhedcey.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.epnwcf.com/Article/details/gxjvrrxpj.sHtML

cmd > out.log 2>&1
来源：http://baike.fktsv.cn/Article/details/giiqbcrkl.sHtML

[R40] 追加写日志
来源：http://www.m.share.tarul.cn/Article/details/gxfnxpacl.sHtML

echo "log" >> out.log
来源：http://read.share.epnwcf.com/Article/details/gmtfdohjr.sHtML

[R41] 丢弃输出
来源：http://m.share.tarul.cn/Article/details/gbieavavg.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.bbcook.cn/Article/details/geillygaj.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/ghyqxnbnj.sHtML

wc -l < a.txt
来源：http://read.share.epnwcf.com/Article/details/gebvzfsfw.sHtML

[R43] 按名字查找文件
来源：http://read.share.vehdjk.com/Article/details/guibhkobu.sHtML

find . -name "*.log" -type f
来源：http://www.share.tarul.cn/Article/details/goshwipsf.sHtML

[R44] 按修改时间查找
来源：http://m.share.tarul.cn/Article/details/gjkpytozu.sHtML

find . -mtime -7 -type f
来源：http://www.share.vehdjk.com/Article/details/gorhdugnk.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gyaiaryzn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.tarul.cn/Article/details/gytfhzajv.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gshcxrfnj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.epnwcf.com/Article/details/gagefxrfv.sHtML

[R47] sed 单行替换
来源：http://mobile.tarul.cn/Article/details/gntvytirb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.vehdjk.com/Article/details/gdlzsqydg.sHtML

[R48] awk 取指定列
来源：http://blog.fktsv.cn/Article/details/gwffvykhs.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gyklzrmdt.sHtML

[R49] awk 带条件
来源：http://blog.vehdjk.com/Article/details/gzpvzfvrw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.sjlbkw.cn/Article/details/gmgnbvnnh.sHtML

[R50] awk 求和
来源：http://3g.epnwcf.com/Article/details/gwagpzrqq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.yfazqb.com/Article/details/gusfcrved.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjgiwykz.sHtML


<!-- 参考信息 -->