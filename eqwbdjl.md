代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gtvoqvoaq.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gsdaxwdbm.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gcndhxwqu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/goevxvviw.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gwiutvcdt.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gnccdpipe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gwsuyqzpl.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gehtisvfa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gsrhjkcpg.sHtML

[Q05] 重命名列
来源：http://3g.epnwcf.com/Article/details/gnwbfzbhi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/gmevbppyt.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/grnjljfvv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gbbpvgegx.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/glkuzmrjy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/gobimbjlw.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/gzmemhddp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gaskemjdb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/gkxhlnayl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gzbyxywfn.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/gvvcajzhu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/ganqhykek.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/gsxxoxzcp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/geujedjkq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/gedpmoimh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.tarul.cn/Article/details/ggvqppesu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gpoaofchr.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gnatxjvzc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/garaheofw.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gffcqywov.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gcvbjlqob.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gmyajpmgj.sHtML

[Q15] 查询全部
来源：http://blog.tarul.cn/Article/details/gljieozob.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/gbsaxnsmq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gdoxmcrkf.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/gbuwvaodd.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gjrzabvod.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/glcvkhftc.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gsfspgtct.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.vehdjk.com/Article/details/gyijchvic.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gbdkvhqmv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gtkxkvstk.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gdnkuusmy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/gzbzyltbu.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gtsldmryh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/gjdwuonoj.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gayaufxfl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.tarul.cn/Article/details/gdgzmsqdr.sHtML

[Q23] 分页
来源：http://mobile.sjlbkw.cn/Article/details/getckohgh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/gkdhkgeyu.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gkdhhczxv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gnzyuskml.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/guiqepaoa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.tarul.cn/Article/details/gwbgnjacc.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gmhpwubds.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gzwhqjbla.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/ggwyobroz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gjpyskfcp.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gansavgjt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gwpcqupwn.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gajgcgzbz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gbastfsbe.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gndwtzegh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gmrqwubqb.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/gfmbpfves.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.bbcook.cn/Article/details/gqtgqczcb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gscyirbyi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gxcrbzzlz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gzwmubflv.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/gdugfuyal.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.tarul.cn/Article/details/ggdopcuvc.sHtML

[Q34] 每组取第一条
来源：http://m.share.tarul.cn/Article/details/gtnyiwmxl.sHtML

SELECT * FROM (
来源：http://baike.sjlbkw.cn/Article/details/gzrnqtbms.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gbxdgkrui.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gzlibybzj.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gwyfblnlu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/ghnxstszi.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gbgylyggw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/ghtncboay.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gyzhaxcec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/gwteabozr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.tarul.cn/Article/details/gfoimbhdq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/ggnngyeam.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/gyqvnbzuf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gtwpgyryh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gohbnqpzd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gpivrkjse.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gmeiwganc.sHtML

[Q41] 多表连接
来源：http://m.share.vehdjk.com/Article/details/grpaxwaxc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/ggrhxmphz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/gubanzbhd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gttchvtbr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gjqnmawxe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gbhjxbeqj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/goaedwpfq.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/gbstgyvan.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/gamvptmlj.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gcmeuvjig.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gukyguvjy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.yfazqb.com/Article/details/gqmavkdcn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/glzctgndx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gcokbcetq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gyuiximhi.sHtML

[Q47] 与平均值比较
来源：http://m.share.sjlbkw.cn/Article/details/gpycgibmc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.tarul.cn/Article/details/gxqklffms.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fktsv.cn/Article/details/gxeohdrbn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gbqiamubv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gtkgcaokq.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gqqajdlqg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/glfokdajq.sHtML

[Q50] 批量更新
来源：http://www.m.share.epnwcf.com/Article/details/gidgvnyzd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/grutzthqw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gwupayqte.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gpsdwlsyq.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gylevnzpk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/guietpwiw.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gwgpvqvil.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.bbcook.cn/Article/details/gownanyzd.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/ggnyzhtbi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gvehjtnkt.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gjdsvotzr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gisypmngx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.vehdjk.com/Article/details/gorzyefat.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gewcwppth.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/gmldeicte.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gqrodiibh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gdxcbrzpq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gnnhobvkh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gfkrtbndb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gtjblkkjh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.bbcook.cn/Article/details/gmxarfntk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/ggzzpijft.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gvrjbshcx.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gpioiayjn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gqcklzlod.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gctchahaq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gsgwqwubg.sHtML

[Q63] 开启事务
来源：http://wap.vehdjk.com/Article/details/ggciszpcj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gwrwndjue.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/gusexsmgf.sHtML

COMMIT;
来源：http://www.m.share.yfazqb.com/Article/details/gvwfzfgyc.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gzfjelyzr.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gdbuccnhd.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gwvdputit.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gpemnkgyo.sHtML

[Q67] 设置隔离级别
来源：http://mobile.sjlbkw.cn/Article/details/grkoqzblu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmpqkwcy.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gyovebnyb.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gmsgiuatk.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gawfzsujq.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/gifjakkfl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/geugxoxdp.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gxakryhtd.sHtML

ANALYZE TABLE users;
来源：http://3g.yfazqb.com/Article/details/gxwhmllxq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gegqdbikk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/ggcaaqgmf.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/gahiisxdv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/guxgywzfm.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gunohnbfh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gbacgcfdc.sHtML

[Q74] 强制使用索引
来源：http://m.share.sjlbkw.cn/Article/details/gliewhfue.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.vehdjk.com/Article/details/glvrrptnl.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gxjfvnjlx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gghtzhuyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gjaiqkxzm.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gsmiqpmdp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gsqrcwhrt.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/guemkwslx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gprbrtsun.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/glddrghyr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.yfazqb.com/Article/details/gyfoftjhu.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gigrhdhai.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gzkkcalhz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/gibvhspgn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.yfazqb.com/Article/details/grkbrdsil.sHtML

[Q81] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gjybxlior.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gilzwskrq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkwepymb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gsnkmsgga.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/giimqrymc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gvzoqjjgg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gqjufurag.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gebgwsnek.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gjsjfmotv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gftqdvhzq.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/goxshxtuz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gxmmffqld.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/grbusnasq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gxycfbwwp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gjryklhzk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.sjlbkw.cn/Article/details/gyodjaceb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfjokcyia.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gkumwqugw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gzmqdikvf.sHtML

[Q90] 生成序号列
来源：http://wap.vehdjk.com/Article/details/gbxzfiaal.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gdyemenye.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gnqdkxiea.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/guybvmrvt.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghymqbqje.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gyyqnizcm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/guwlzjzec.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gpxkayrvh.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gbmtbbzpq.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gsipbuqgi.sHtML

[R03] 只读变量
来源：http://www.blog.epnwcf.com/Article/details/geyjaampw.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/gvxgivzin.sHtML

[R04] 位置参数
来源：http://m.share.vehdjk.com/Article/details/ghsgvojtm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/guearnbff.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gbwachjnn.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/guajmjkis.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/gdaoldlln.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.vehdjk.com/Article/details/gcqatvddk.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gsggyxqhh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gzcwydnlp.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/giecjcvkh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gelcbnwqr.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/guspxcseq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.sjlbkw.cn/Article/details/grdnxjlfd.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/gbzgdkklo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/gegonlblf.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gvbymzgwz.sHtML

case "$1" in
来源：http://www.share.epnwcf.com/Article/details/gfgtfesrc.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gioxthusw.sHtML

stop)  echo "停止" ;;
来源：http://3g.vehdjk.com/Article/details/guwhvqlzy.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gneqcatug.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/golkqosje.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/gixmlknkb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gifelqjyu.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/giynggfqy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gtdqqhfeo.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gfjtsidgr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gbjklvugm.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gdfmshjcu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gswmdgqlv.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gehbbzwdh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.epnwcf.com/Article/details/gcvkbnfnj.sHtML

[R17] 数组定义与取值
来源：http://www.blog.vehdjk.com/Article/details/ghhaboobu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gmkyorxca.sHtML

[R18] 遍历数组
来源：http://www.share.fktsv.cn/Article/details/gjaxglrkb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.bbcook.cn/Article/details/gnqddlcmk.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/ghqgbagog.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gzugrrguz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.bbcook.cn/Article/details/gcahjrmcl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gnsxoygdg.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gljymbfeh.sHtML

echo "${#s}"
来源：http://blog.yfazqb.com/Article/details/gxgszefnq.sHtML

[R22] 截取子串
来源：http://wap.yfazqb.com/Article/details/grkmtqpwx.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/girzzfjir.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gnqenctqw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/ggldzdezq.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gavpwzrji.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.vehdjk.com/Article/details/gjcbqiudg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/gkhcgddyr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/goyhhneut.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gmmizqufv.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.tarul.cn/Article/details/gztxunmzp.sHtML

[R27] 算术展开
来源：http://www.share.tarul.cn/Article/details/gpgpqmzbj.sHtML

echo $((1 + 2 * 3))
来源：http://wap.vehdjk.com/Article/details/gntnyoqej.sHtML

[R28] 浮点运算
来源：http://blog.bbcook.cn/Article/details/gzovcmgyd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fktsv.cn/Article/details/gwqvdbvzj.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gipnsppoj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gfedywrog.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/gyggipwyx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gekngryoj.sHtML

[R31] 局部变量
来源：http://mobile.sjlbkw.cn/Article/details/gnormviim.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gaqcmtgku.sHtML

[R32] 参数个数校验
来源：http://www.share.fktsv.cn/Article/details/gkkipzvuj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gdbrjctmw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gedbtxafe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gvbdxmrci.sHtML

[R34] 退出时清理
来源：http://3g.tarul.cn/Article/details/gvhmlhluc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gawiobaec.sHtML

[R35] 后台执行并等待
来源：http://blog.tarul.cn/Article/details/gvhdmmofv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.sjlbkw.cn/Article/details/gvgpujsbs.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fktsv.cn/Article/details/gwjaykbny.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/glqadhlmh.sHtML

[R37] 把输出赋给变量
来源：http://mobile.bbcook.cn/Article/details/gsexxttwk.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gsdrdgihs.sHtML

[R38] 管道串联
来源：http://mobile.fktsv.cn/Article/details/ggganolae.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.bbcook.cn/Article/details/gltaojayx.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.vehdjk.com/Article/details/gosaeabnt.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.epnwcf.com/Article/details/grotebbyd.sHtML

[R40] 追加写日志
来源：http://baike.yfazqb.com/Article/details/gylcybihi.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/gnbqcljzs.sHtML

[R41] 丢弃输出
来源：http://www.blog.epnwcf.com/Article/details/gowijvhbv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gauuhsyda.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gkluvhqst.sHtML

wc -l < a.txt
来源：http://wap.fktsv.cn/Article/details/gpncjaxus.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/geetqvbsx.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gkylepxqb.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fktsv.cn/Article/details/gvlmfmeep.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gdsenduth.sHtML

[R45] 批量删除
来源：http://3g.epnwcf.com/Article/details/gintunlkp.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fktsv.cn/Article/details/gyhzuoieb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/ggbtlphcj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fktsv.cn/Article/details/gonyzxyfj.sHtML

[R47] sed 单行替换
来源：http://www.blog.tarul.cn/Article/details/gjzarmzgc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gsudghdrm.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gucnzhjyo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.epnwcf.com/Article/details/goiyjvukt.sHtML

[R49] awk 带条件
来源：http://www.m.share.fktsv.cn/Article/details/gozxutzza.sHtML


<!-- 参考信息 -->