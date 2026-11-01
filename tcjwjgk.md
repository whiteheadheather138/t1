代发 wailian999

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/gaafpeetg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gmkegzgfs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gicnskzui.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gdwbttjyl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.fktsv.cn/Article/details/gldtcugzw.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gwskegava.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gnrbvxlun.sHtML

CREATE TABLE orders (
来源：http://www.blog.bbcook.cn/Article/details/gqveqmjfz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gbsgrpdtd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/gjmpdzdrx.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gltmoljig.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gwwdmwgnj.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gigybgbjq.sHtML

[Q03] 增加列
来源：http://read.share.vehdjk.com/Article/details/gppvkdpoo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/ghqrhrdje.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gnmjeekqt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gawtjfjre.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/geskispvy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/ghdwefdyg.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gljlrbxva.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.bbcook.cn/Article/details/gsqnnpuzo.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gbndqvjum.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gwvqxxavg.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gmcesvhhk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gjxpdflto.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.epnwcf.com/Article/details/ghmkfbwgc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/ggnjtmmat.sHtML

[Q10] 插入单行
来源：http://read.share.tarul.cn/Article/details/ggenwgdhp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gxcadrzaw.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/ghblobmpq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gcgcuukvr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gezwtyrci.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.sjlbkw.cn/Article/details/gzygdptgx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gzufgtnkc.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/goolyepor.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gmlbkaujl.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gzmixzgmi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.vehdjk.com/Article/details/guyelvipu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/gcsisflwv.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gjihsypwl.sHtML

SELECT * FROM users;
来源：http://3g.bbcook.cn/Article/details/gxgorqbvm.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/gkfdsxngu.sHtML

SELECT id, name FROM users;
来源：http://www.share.yfazqb.com/Article/details/gsqflsmkk.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gweycifuc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gzplurltr.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gcmkzmfzg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gcxdhvscw.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gkhwerjgk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gckcjrrrl.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/glzlgirzc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/ggcpgqnad.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gmkjzwank.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.bbcook.cn/Article/details/gpqougckr.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/gfphysuxm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gxzlrgrfd.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/giienldnu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gimerqmot.sHtML

[Q24] 去重
来源：http://m.share.vehdjk.com/Article/details/ghjjjmgkh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.bbcook.cn/Article/details/ggcwgqsqk.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/gupygasho.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.vehdjk.com/Article/details/gmnvmxclh.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gdysovjlk.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gubnvodbq.sHtML

[Q27] 条件计数
来源：http://www.share.bbcook.cn/Article/details/gpayoxidn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/ggcxrcvoy.sHtML

[Q28] 求和与平均
来源：http://baike.fktsv.cn/Article/details/gwyhpniqk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gonsahgbc.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gfnbyukka.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbhlkzslj.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gykhjzgyw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gxhdbelxt.sHtML

[Q31] 分组后过滤
来源：http://www.share.tarul.cn/Article/details/gbbrqszdu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.vehdjk.com/Article/details/gsyriylgw.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gghefgvul.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gqclzwrve.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gzaarrnrn.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/glyxidafz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gefzhfhbj.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdjxzprg.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gwcyfmqsp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gkulitzbl.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gcpkpztaw.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/ggfsbwvfn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gbsrxrufi.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gebhfhjmw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gydwaholf.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gyrlkvfpg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gshzrsoml.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gjqfnbgiy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gzyrvvcsx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gynfntniv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gxhgszmgn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/getxsapsi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/gttofngdd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.yfazqb.com/Article/details/grlbnncja.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gxqxmabnh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gvepinfcy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fktsv.cn/Article/details/gznujnqqg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/gtlfecuyh.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gjmwhtwzz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gmkfhkovb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gxgxqwwas.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/gurtyqulf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gywllsgoa.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gubxbympz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/gpbhhbarj.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.tarul.cn/Article/details/gojqtitkv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/ghyywzmtn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/gfewynals.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gmwfbafyf.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/goxjagpbu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gwsgkmfbn.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gagisgdls.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gebzucfey.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/glftgpuqy.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gmlayfqcu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/gmkcykdwb.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gdqcvxrav.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gfrevzoyn.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gihnbhnft.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gttymwgdg.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/gxqpwwugc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/grrrwqnvp.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gvufwngkw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gnkwszqpu.sHtML

[Q54] 清空表
来源：http://www.blog.bbcook.cn/Article/details/gsfpgggwz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gggozkaeq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/gcdlawcui.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gwoxmhslg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fktsv.cn/Article/details/gwnkcxjsz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gzvabsoxo.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gkjyrayoo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gwodfjejf.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gymuuasby.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.epnwcf.com/Article/details/gcvorfllc.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/gfohjocxv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gdioghzus.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/gvagkbogq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/gbccfclrv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/grxrrqxwe.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gjwzoprnj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gnpzvumno.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gbznzevmc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/glplosdbr.sHtML

[Q63] 开启事务
来源：http://blog.epnwcf.com/Article/details/gsniljxqk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/grxzoapik.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/grgxzbjlp.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gxwdphnxd.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/ghngpmpkw.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gbykljryd.sHtML

[Q66] 行锁查询
来源：http://blog.fktsv.cn/Article/details/gjdenhoaf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gqxbidpee.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gayfjnnzv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/gyfuobbgz.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gzfzhftfy.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/ghsvwajct.sHtML

ROLLBACK TO sp1;
来源：http://3g.tarul.cn/Article/details/gvejwdfms.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/ggnhafuwv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gikleivcv.sHtML

[Q70] 更新统计信息
来源：http://wap.fktsv.cn/Article/details/gwokaidyj.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gymtrjzzf.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gzwlwuvdq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/gtpcicpem.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gtqjakuty.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gzvbffigh.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gsaxaumev.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/ghdqiylbf.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gqdvjaies.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.vehdjk.com/Article/details/gouqjgpzk.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gktzfwrun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gxhrhrgdk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gdeycwcnd.sHtML

[Q76] 按天统计
来源：http://mobile.epnwcf.com/Article/details/ghxxrttkh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/gxyxjoejz.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/gktycbztf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gvjfvcpzi.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gmxcywode.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/gbllbmtza.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gxukmjauy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/guneaclqt.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gpxcrgndc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvhpmmhtu.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gngnhbhog.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gyljghopw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gbjkndvis.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gstksjvpk.sHtML

[Q83] 大小写转换
来源：http://wap.tarul.cn/Article/details/glozrvhsb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gutksyptk.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gbefnpkji.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/guiqaqcbq.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/ghdepzpza.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.yfazqb.com/Article/details/gocsqyruv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/gaxygxevp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gpbpgpfct.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gqakrnknp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gadxsujme.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gppzyvprb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.sjlbkw.cn/Article/details/gzsujkqvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpuheuont.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gkvyfxouc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gslcpebah.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gkawifmyx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fktsv.cn/Article/details/gnijyrujr.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gatevkmla.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gwmcttiua.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqlcjsyim.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gnfgokzwn.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gtwkbqpzp.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gpbkjtevx.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gqvxlpayn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/gdtexnqss.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gqanmngvb.sHtML

readonly PI=3.14
来源：http://blog.fktsv.cn/Article/details/gypjgzdrw.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gxsdjtifk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fktsv.cn/Article/details/gpsalakqf.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gzyvzgvzs.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gkvrqjjhe.sHtML

[R06] 判断命令是否存在
来源：http://read.share.tarul.cn/Article/details/gpjvdbsrw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gpmjuevnc.sHtML

[R07] if 判断文件
来源：http://m.share.tarul.cn/Article/details/gluqrjezw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gcbbfmvsb.sHtML

[R08] 数值比较
来源：http://www.blog.yfazqb.com/Article/details/gbnagydos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/guacipged.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gzcbbhsbu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.tarul.cn/Article/details/gwgacwoxj.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gtylwtvge.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/gwsrtngue.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gdrvasnfl.sHtML

case "$1" in
来源：http://blog.epnwcf.com/Article/details/gvwwzwbwh.sHtML

start) echo "启动" ;;
来源：http://blog.fktsv.cn/Article/details/gzuiyrjrm.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gaejslmag.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gvwpresnm.sHtML

esac
来源：http://www.m.share.yfazqb.com/Article/details/gwesmmdlo.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gzqogstwb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gefznuasz.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gqmzxhaxh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gnamykdra.sHtML

[R14] C 风格 for
来源：http://m.share.fktsv.cn/Article/details/gsqvxmwmk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.yfazqb.com/Article/details/gjjjpxome.sHtML

[R15] while 逐行读文件
来源：http://m.share.yfazqb.com/Article/details/gipjsgghl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.tarul.cn/Article/details/gjelothvd.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/ggjznzren.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fktsv.cn/Article/details/gelhtxfmm.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/gkglrbfjy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.epnwcf.com/Article/details/gtubzbuwr.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gdafurqyk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gevjpxftq.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/goebpkcgj.sHtML

echo "${#arr[@]}"
来源：http://blog.bbcook.cn/Article/details/gwvqytvok.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gknqmsome.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/groivjuob.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gtbqzwxbj.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gwvkrhlni.sHtML

[R22] 截取子串
来源：http://read.share.epnwcf.com/Article/details/gxhxxcoee.sHtML

echo "${s:0:5}"
来源：http://wap.sjlbkw.cn/Article/details/gashfncki.sHtML

[R23] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/ghmsyywhk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.sjlbkw.cn/Article/details/gvowggkpn.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gjgmhgize.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fktsv.cn/Article/details/gklwksdxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.vehdjk.com/Article/details/gddvbeqnr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/gcwsdmwpv.sHtML

[R26] 命令替换
来源：http://www.blog.bbcook.cn/Article/details/gmlgrdjsk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gjzrjbsim.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gdepvngok.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gkudpmzga.sHtML

[R28] 浮点运算
来源：http://www.share.tarul.cn/Article/details/gagjsfyyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/gxojnsimo.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/guopkuumu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.tarul.cn/Article/details/goddzprql.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/gkoogkqvc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.vehdjk.com/Article/details/gfxosiael.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/gjgusyaui.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gthdiecmz.sHtML

[R32] 参数个数校验
来源：http://www.blog.sjlbkw.cn/Article/details/gjgmlhfnq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gfdtnistf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.vehdjk.com/Article/details/gaxfsdnxs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gwvwobplr.sHtML

[R34] 退出时清理
来源：http://mobile.sjlbkw.cn/Article/details/ganbuydtz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.yfazqb.com/Article/details/glgczkpaq.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gnpuhcluc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fktsv.cn/Article/details/gjqirvixf.sHtML

[R36] 并发执行多个任务
来源：http://mobile.epnwcf.com/Article/details/gezguaskr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/gaemxcppl.sHtML

[R37] 把输出赋给变量
来源：http://www.share.vehdjk.com/Article/details/gcyppdcij.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/geizvhzgx.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gxvarnrbh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.vehdjk.com/Article/details/guketxxwh.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.tarul.cn/Article/details/gelcnnnwc.sHtML

cmd > out.log 2>&1
来源：http://wap.sjlbkw.cn/Article/details/gybhpkxef.sHtML

[R40] 追加写日志
来源：http://mobile.tarul.cn/Article/details/ghgvpbrsm.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gedejoeaw.sHtML

[R41] 丢弃输出
来源：http://read.share.bbcook.cn/Article/details/gpuiestem.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fktsv.cn/Article/details/gxjljrxqv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fktsv.cn/Article/details/gsxbzclyn.sHtML

wc -l < a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gkmrfjjkd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gdftcbfja.sHtML

find . -name "*.log" -type f
来源：http://baike.tarul.cn/Article/details/gwxthnwxh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.sjlbkw.cn/Article/details/gyfvvwirj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/gvalqbrjt.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/grptolsek.sHtML


<!-- 参考信息 -->