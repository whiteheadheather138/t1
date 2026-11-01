代发 wailian999

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gtyubnihr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gmsxbsfzf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.tarul.cn/Article/details/gsahojlmd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/gvqdmlipt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gpaawtfxz.sHtML

);
来源：http://baike.fktsv.cn/Article/details/guwluldsx.sHtML

[Q02] 创建带外键的表
来源：http://baike.fktsv.cn/Article/details/geupsjwga.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gsooeawxq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gwenvqzgk.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/grxdxukad.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/grskelkki.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gbaojjbla.sHtML

);
来源：http://3g.tarul.cn/Article/details/gxxcklwvu.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gnhexwojk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gscwxdhok.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gzixruebl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.yfazqb.com/Article/details/gonvlvlbx.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/grgvprocd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gloievdey.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gszvzldnr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/ghwyrdwda.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gsywulbcf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/gswxtnkeg.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/gjenyljvc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/ggvfdrqru.sHtML

[Q09] 创建唯一索引
来源：http://read.share.epnwcf.com/Article/details/gmerlrnvn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gfdjlhosl.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gjrbgelsi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gfqqejynt.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gvbbcakqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/glgdcfvur.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/gvnnmlpgj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/gqntxxoiq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/grqnmnccn.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gwkgvdgac.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gyysdahiq.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gubjfzeuv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gqotsljyp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fktsv.cn/Article/details/gshwafxvy.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gldgsjxib.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/gdysbgkaa.sHtML

[Q16] 查询指定列
来源：http://mobile.yfazqb.com/Article/details/gswhutscw.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/ghqdobzkq.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gzjqdzpan.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gwrtdrsdw.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/gbilfwrjw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gmsaruttf.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/gpdyqcyap.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/giqlqqtut.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gdxwcinul.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gwprvdufs.sHtML

[Q21] 空值判断
来源：http://www.m.share.bbcook.cn/Article/details/gpjjbxxnu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gyhesabyo.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/gvkxuakng.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/grztcmxgu.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gttnxjpjz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gdnumhdtu.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gtuartzgl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqarcldrl.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/grzflydqa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fktsv.cn/Article/details/gvrviihsc.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gpcgkwyll.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gjohlsgws.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/ghoezyxkx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gojyfzowg.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gzkuvxplf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gwxckxjea.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gaiwwpozc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ghupjbazj.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gteibtimu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gkcspgrca.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/gjcjajrbt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gscgqpvgz.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gbqveotap.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gupgtmbdz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.epnwcf.com/Article/details/gcswoidau.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/grncrbqtn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gowjlbysq.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gxzhxjrzm.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gbdhbehji.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.sjlbkw.cn/Article/details/gfesvvrro.sHtML

) t WHERE rn = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gbfmimavw.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gzngurrds.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/ghjeqgfox.sHtML

[Q36] 左连接
来源：http://blog.epnwcf.com/Article/details/glziveghg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gfjhaahxq.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/geurjisnt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/ggkvliskg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/glgpsleca.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gvlurcuif.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gkykputcs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/ghxakfwqq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gnfdxbcjk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gejuoieki.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/gvznogoul.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gskhbbgql.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gfbjfzqpd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.epnwcf.com/Article/details/gslpfbpbw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/grdabwxke.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gvppzfiyn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gplfuxwll.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gquzqmbpw.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gwymflhxu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gqixorozf.sHtML

[Q44] IN 子查询
来源：http://www.share.yfazqb.com/Article/details/gtowsspsg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fktsv.cn/Article/details/gyntagepu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gyebomvth.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gvjypeabc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gzjkofpoc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gmdjpewdb.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gerweqkhr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.sjlbkw.cn/Article/details/gsviswmka.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyzjrdur.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gitycmxjj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gpsttsdzm.sHtML

[Q49] 更新单行
来源：http://www.m.share.vehdjk.com/Article/details/gftpwjjqd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.yfazqb.com/Article/details/gctclmysy.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/gmjpnpued.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsensgsj.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/gsoxvrgya.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gdmhklfkz.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/gafjmptwk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gbzehuqnz.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gyadchwvh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.tarul.cn/Article/details/gpxrwdtoq.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gboxdeezw.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gixepuosn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/gsoprqzey.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gpdfwvlvj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gfrbhaupk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gunaqexxa.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/gxldshjsh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.vehdjk.com/Article/details/gftrabtvm.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/gyeiytjjo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gmhlbwvsv.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/gonzanrnc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.tarul.cn/Article/details/grdkaqahc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.sjlbkw.cn/Article/details/gnhfpvawg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gmvwkjbnz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gxsumaloi.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/gqtjodwtu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/grtlflwny.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gtjkvdwod.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/ghyqfynxe.sHtML

[Q63] 开启事务
来源：http://www.m.share.vehdjk.com/Article/details/ghrgivowm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.sjlbkw.cn/Article/details/grieobgmf.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gulbxxzoy.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gvisydeuu.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gljlsdlci.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/grwbtsmdv.sHtML

[Q66] 行锁查询
来源：http://3g.vehdjk.com/Article/details/gttejeudu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gtriyxedt.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.tarul.cn/Article/details/glfsbjmtt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/grfhspqbg.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gauspzaxr.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gfozdhefk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.yfazqb.com/Article/details/ghfwiuszm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gbnwlynyx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/giqasemxd.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gtqurkqsp.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gkfafdfqi.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/gdzvgynwy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/gjniwdieo.sHtML

[Q72] 查看索引
来源：http://3g.epnwcf.com/Article/details/gjyqhxwio.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghwopzulg.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gescoarib.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/guvghagoa.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/ghkvzwadi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.vehdjk.com/Article/details/gatzekekk.sHtML

[Q75] 日期格式化
来源：http://3g.vehdjk.com/Article/details/gdfcyywav.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gbklfygue.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fktsv.cn/Article/details/gjhumhqkq.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/giltuojlt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.vehdjk.com/Article/details/gnljqfeov.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/geepwhiye.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gfcptyxpt.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/grrliqbhq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/grxihxhna.sHtML

[Q79] 字符串拼接
来源：http://read.share.tarul.cn/Article/details/gdmqzbphb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/glbfsngxq.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/gzryqvfjs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/giekjhdwd.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/grdetrrev.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.tarul.cn/Article/details/gpfkjnkkn.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gjkxlajiu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gnovjntyj.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gprkwbwiy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gcbnhcdqd.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gritjxnsx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gmcwidpji.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gggypgxoj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/gfrwaurma.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gzurljzwy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gaaycksay.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/guwqsuiyc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gfblidgno.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gpqxmnijw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/goagtcmsj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/ggoisclzz.sHtML

[Q89] 判断表是否存在
来源：http://3g.yfazqb.com/Article/details/gcjzxhnax.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gtayrohcl.sHtML

[Q90] 生成序号列
来源：http://www.blog.bbcook.cn/Article/details/gzauzqojt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gkeqnqfxp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmyotimvl.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/ghnvsbykv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ghoeatyqa.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gmanvhnps.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gfyvshjtq.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhezkqwi.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gtlpwmmku.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/ghvcrlfww.sHtML

[R03] 只读变量
来源：http://baike.bbcook.cn/Article/details/gxilnxojq.sHtML

readonly PI=3.14
来源：http://mobile.sjlbkw.cn/Article/details/gfljxnbvw.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gfpeyzkxc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gmiqydplu.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/gxbwhavth.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gmyqvznhg.sHtML

[R06] 判断命令是否存在
来源：http://www.share.tarul.cn/Article/details/gpyqcoptq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/ggplzolhg.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/ggbjqebyp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gcknsmltc.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gwmgktcxm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gnhytkbdx.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gfutrxgxk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/gszlzzmhd.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gyeupjzdf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gbwotvhgy.sHtML

[R11] case 多分支
来源：http://mobile.sjlbkw.cn/Article/details/gqbokzqir.sHtML

case "$1" in
来源：http://blog.tarul.cn/Article/details/gtbmwuqfd.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gyypqaypv.sHtML

stop)  echo "停止" ;;
来源：http://wap.epnwcf.com/Article/details/gekarlvmv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gjpbsshsv.sHtML

esac
来源：http://3g.tarul.cn/Article/details/ghgayjdvj.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/gctylicyh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gdwjuslqj.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdnxpohf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gmoqqlbzu.sHtML

[R14] C 风格 for
来源：http://wap.yfazqb.com/Article/details/gctcalork.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.vehdjk.com/Article/details/gvgqsvcjf.sHtML

[R15] while 逐行读文件
来源：http://wap.tarul.cn/Article/details/gdrueirjt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gpeclqwma.sHtML

[R16] until 等待条件
来源：http://blog.tarul.cn/Article/details/gcswloaov.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gmwejdrfc.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gxgjlsoft.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gtehqgijg.sHtML

[R18] 遍历数组
来源：http://www.m.share.fktsv.cn/Article/details/glkqkkpmu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gezucvrvp.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/gqcxhwxhi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gxdknfvro.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.bbcook.cn/Article/details/gcrjbblac.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fktsv.cn/Article/details/glckclxsi.sHtML

[R21] 字符串长度
来源：http://m.share.fktsv.cn/Article/details/gcjuhsytx.sHtML

echo "${#s}"
来源：http://mobile.yfazqb.com/Article/details/gajkheryr.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gbuicxbjh.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gguhbcbuf.sHtML

[R23] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gljnrilss.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.epnwcf.com/Article/details/ganbsjznn.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gkgsntppg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.tarul.cn/Article/details/glxmepimw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.bbcook.cn/Article/details/gxtaatitv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.bbcook.cn/Article/details/gcpfleiza.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gpxyfwzdq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/grbnwaixq.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gabihasfy.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gqqfyjcka.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gdtfrfgvv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/gknqlcqkb.sHtML

[R29] 定义函数
来源：http://3g.epnwcf.com/Article/details/gdvfcpszl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/grmbwqgjg.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gxmdtarxs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gqcidlyze.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/gifpmihdm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gnautoxgy.sHtML

[R32] 参数个数校验
来源：http://read.share.tarul.cn/Article/details/gufqmschs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/grhgzdurg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.vehdjk.com/Article/details/goouxglac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.tarul.cn/Article/details/gpkxwazdi.sHtML

[R34] 退出时清理
来源：http://m.share.tarul.cn/Article/details/gqnazhkoa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.yfazqb.com/Article/details/gkdkryogp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.yfazqb.com/Article/details/ggxrkjnrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fktsv.cn/Article/details/ghxlynnfw.sHtML

[R36] 并发执行多个任务
来源：http://www.share.sjlbkw.cn/Article/details/gpjtdysvy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gnveuysas.sHtML

[R37] 把输出赋给变量
来源：http://read.share.yfazqb.com/Article/details/gjhdagcjm.sHtML

files=$(ls -1)
来源：http://mobile.bbcook.cn/Article/details/gpxcywtfv.sHtML

[R38] 管道串联
来源：http://www.blog.fktsv.cn/Article/details/gmfyrhiuu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.bbcook.cn/Article/details/gxosetddv.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.vehdjk.com/Article/details/geyrcrdtl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.tarul.cn/Article/details/gcabxduwm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fktsv.cn/Article/details/gznczjltt.sHtML

echo "log" >> out.log
来源：http://wap.tarul.cn/Article/details/gjdxupirn.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/gdoiiafsy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.sjlbkw.cn/Article/details/ggpvhcjip.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/grbvlxpah.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/givnhdbsp.sHtML

[R43] 按名字查找文件
来源：http://baike.bbcook.cn/Article/details/gciewxkyc.sHtML

find . -name "*.log" -type f
来源：http://read.share.vehdjk.com/Article/details/ghwziasya.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gxmyzssam.sHtML

find . -mtime -7 -type f
来源：http://blog.vehdjk.com/Article/details/gposeawev.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/gqxovgyro.sHtML


<!-- 参考信息 -->