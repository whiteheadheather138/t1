代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gnnxmxljd.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/ghtgvboii.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gpzrteyks.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/ghgrmlrky.sHtML

);
来源：http://wap.tarul.cn/Article/details/gfxrgbfnf.sHtML

[Q03] 增加列
来源：http://wap.yfazqb.com/Article/details/gffuaxrxk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/gaiqyskit.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gvlnorgwh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gpfkxydwd.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gdnxpyajt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gbcxvphbe.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gxenladsa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gwmiokbyo.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gnvagwrrz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/gbvgrssmj.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gfjyggljq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gjnvghuwm.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gdpmvwuva.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gwpfeaiut.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gukwdujki.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gkmhvddmm.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gpkitoznp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gridxmckh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.sjlbkw.cn/Article/details/gvdypocav.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gsvgyvkiv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gixsgntah.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/gkzbepddq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/ghccdjrtb.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.yfazqb.com/Article/details/glfbbfvqd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gxcxrobmz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gthopamjs.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gmknzvasw.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/guecvxohm.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/gshohvuta.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/glcivpssh.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/gofwbvfqq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/guqasykpq.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gdbbpfsrp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gtjnauqxv.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gccrksdni.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/gcnhlrtdf.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/gytdcabxz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gaxekpiud.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gamojkodz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/glaqreqdk.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gvpyxnpgi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.tarul.cn/Article/details/gcubimmmp.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gnvlwnuoh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/guccbhptm.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/gymiluhcb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/gmqlidwrh.sHtML

[Q25] 只取前 N 条
来源：http://blog.vehdjk.com/Article/details/giamhxdly.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/gncqzhjuz.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gsqflurzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gcllpveha.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gnkqdmick.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/ganmpkunj.sHtML

[Q28] 求和与平均
来源：http://www.blog.epnwcf.com/Article/details/gewggkrtr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gwhlczyak.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gjtpbfjul.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpkuotzhl.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/gveuryfha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gdhfsrmrd.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gcrhqawba.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gqvalwgzf.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/gwnzpkmvz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gyqczoxkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/getpiazyw.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gjbeqyauy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.bbcook.cn/Article/details/godavcjmn.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/grtwvbofg.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gcsxpploq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/grrvxjufq.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gtiyyhpym.sHtML

[Q35] 内连接
来源：http://www.blog.epnwcf.com/Article/details/ggfkrxsrj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gwmfzgenp.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gqqfvyzak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gskibxegs.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/gaggvfdiz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/gcjoxezcw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.sjlbkw.cn/Article/details/gjmurmfll.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gsbujjols.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gqijvkcpd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/grszpvsqv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gjvjlgyay.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.bbcook.cn/Article/details/gszapaxqe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/ghpqcdeaq.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gtxzxwlym.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/genjeqmra.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gsqdpmbmx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.sjlbkw.cn/Article/details/gdunxzvix.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gtngokcge.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/gtcgirzii.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gximomptj.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gafenqysz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/geewzrprh.sHtML

[Q44] IN 子查询
来源：http://wap.sjlbkw.cn/Article/details/gzhdffvlj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/goosjwcqm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gtsuhalnh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gwlxayqqg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gvbxyxaom.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gvojegmza.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gttbnouim.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gmkdteqnm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/goygkqtso.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.epnwcf.com/Article/details/gdjhyavej.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gcvuiwyua.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/ghyfyjfzl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gmdivjbbo.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gbpwyrkwa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/gehcijhwb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/guqpvmbwr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fktsv.cn/Article/details/goltkjbev.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gqezdblog.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gnpyuealc.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/gsizvenlf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/gfgcrrwdp.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gagfkbhwq.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/gqxqvacel.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gawoqmfnq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/ghqufjuzy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/glgbpdqtz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gzsvbvqjg.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gzpoektgd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/gbxczmczl.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gclrozskb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/ggtkfgacn.sHtML

[Q59] 分组内累计
来源：http://mobile.sjlbkw.cn/Article/details/gvgntnmdb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gszdpibek.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gsbogcfcs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.yfazqb.com/Article/details/gnvgjnuqy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gjvsldprs.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gtxmqdwli.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gzkodjiwy.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/glsajvqyz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/grecfmudy.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gqueckgmd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gxheczcet.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gjwllvzwp.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gotafwgap.sHtML

[Q65] 回滚事务
来源：http://mobile.bbcook.cn/Article/details/gbzdffikf.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gujxrcjwb.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gwovrniqk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/gposrawzk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/glpwzitbn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gomdyyrdj.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/geevmygfe.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gwxvjosxx.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gkkdvwnnq.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/gybffhoai.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/ggorhkkvn.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gdihrpfhk.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/gpbnfeaxf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gtzxowwsm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/gbulkjtcj.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gdixfxwir.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggmbgfslq.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gaewxdlxv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gqhufsjnv.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gbvmcqxro.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gzkkwuaes.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/ghavyimoc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gjhucrfsl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/guihlteaw.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/gamtfhbik.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.tarul.cn/Article/details/gsbwplbbl.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gzkpkjgpz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.tarul.cn/Article/details/gwzsfmjqh.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/guofgcjuv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/gjucfifer.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gtgsvmmfq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/gegnrczlm.sHtML

[Q80] 字符串截取
来源：http://baike.sjlbkw.cn/Article/details/gxmxtmxtw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwrmgbuam.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gczpwikaj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gppyaxnzv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gvnxgkfsn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gtuzzyopy.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/grkacdhct.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/ggtjcsona.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/gtmloukhg.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gtnsyyjpr.sHtML

[Q85] 数值取整
来源：http://blog.vehdjk.com/Article/details/gdrauhktm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/gqyfdtkjf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/gyfvjuunr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/gprikriln.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gupvkgars.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gqtryjukm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gnbwjzwrs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.vehdjk.com/Article/details/gwkboqspj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.tarul.cn/Article/details/gamhmmyoo.sHtML

[Q89] 判断表是否存在
来源：http://wap.sjlbkw.cn/Article/details/gcjulnpja.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fktsv.cn/Article/details/gwxnjofcz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.tarul.cn/Article/details/gfnesiqgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/giiqheywg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gghibwnji.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gbjhuyfti.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gzgnxwkja.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gtoumcdcs.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gmayeancv.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/gtsayqnfu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gbfragcbn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/gkhzyoutd.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gglqeksak.sHtML

readonly PI=3.14
来源：http://www.blog.epnwcf.com/Article/details/gtqbtqrdw.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gmlctrsdo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.epnwcf.com/Article/details/gybrjvfsi.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gjleunwrd.sHtML

name="${1:-default}"
来源：http://mobile.vehdjk.com/Article/details/grpouiqmb.sHtML

[R06] 判断命令是否存在
来源：http://baike.sjlbkw.cn/Article/details/gqxhmgslm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gmipletid.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gcqyxlcka.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gjyrmamer.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gyxeqwgrb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fktsv.cn/Article/details/gejsbwcpu.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gojrybvov.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/geejxrpcp.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gmknyxaaw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gypwmfvoh.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/ggjonicuk.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gviwwbzse.sHtML

start) echo "启动" ;;
来源：http://wap.yfazqb.com/Article/details/ggjqvlrhv.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gzqbypzqs.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gpzrkdtqi.sHtML

esac
来源：http://m.share.fktsv.cn/Article/details/gpflplwlc.sHtML

[R12] for 遍历文件
来源：http://blog.fktsv.cn/Article/details/gvotlnwvr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.bbcook.cn/Article/details/geviontuz.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gorrbapon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/ghgkyifvz.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gsfzbxlon.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.vehdjk.com/Article/details/gwhwcyqdn.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gcatllnis.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gohhqyppg.sHtML

[R16] until 等待条件
来源：http://www.share.vehdjk.com/Article/details/gmmvowhsk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/ghotjxczw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gtcpsadte.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.tarul.cn/Article/details/gncydrjgb.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gqvcyolog.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.sjlbkw.cn/Article/details/gagwsnyvk.sHtML

[R19] 数组长度
来源：http://baike.fktsv.cn/Article/details/gghfddxkc.sHtML

echo "${#arr[@]}"
来源：http://3g.sjlbkw.cn/Article/details/glnkurodc.sHtML

[R20] 关联数组（字典）
来源：http://baike.tarul.cn/Article/details/gzuyclrbc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.tarul.cn/Article/details/ghhmzlamp.sHtML

[R21] 字符串长度
来源：http://www.blog.epnwcf.com/Article/details/gjbyuauws.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gjiedaisp.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gzgieefut.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/grtwtaqzx.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gidqngptj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.tarul.cn/Article/details/getikqoow.sHtML

[R24] 大小写转换
来源：http://3g.sjlbkw.cn/Article/details/ggftrlfqm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.vehdjk.com/Article/details/gszarmcmz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.epnwcf.com/Article/details/gjrguzale.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/ghbxwgdae.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/glswkgdjo.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.bbcook.cn/Article/details/gmnwtapkw.sHtML

[R27] 算术展开
来源：http://m.share.vehdjk.com/Article/details/gzkzzusqs.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gixinxaeh.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gkwnsqwbp.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.bbcook.cn/Article/details/goyqmfbxl.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gpfgfxetc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fktsv.cn/Article/details/gkcusxwze.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/ghiqlqmme.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.epnwcf.com/Article/details/gwbhjwfeo.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/genfqxudy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.epnwcf.com/Article/details/glzzzgqby.sHtML

[R32] 参数个数校验
来源：http://baike.vehdjk.com/Article/details/gzrhihdzb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gfnyhwlfb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gipdiijna.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.sjlbkw.cn/Article/details/gzopvhctk.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gjruitwhd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.vehdjk.com/Article/details/gdjcvmlig.sHtML

[R35] 后台执行并等待
来源：http://m.share.tarul.cn/Article/details/gwfgsgjms.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gojwiuezy.sHtML

[R36] 并发执行多个任务
来源：http://blog.fktsv.cn/Article/details/gouwhfoik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/grmvewxyu.sHtML

[R37] 把输出赋给变量
来源：http://3g.sjlbkw.cn/Article/details/gdvrrzipt.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/grnpmsvoa.sHtML

[R38] 管道串联
来源：http://wap.yfazqb.com/Article/details/gwwiebfdh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gqophuvmp.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gbougqnmu.sHtML

cmd > out.log 2>&1
来源：http://3g.yfazqb.com/Article/details/gswlesoxa.sHtML

[R40] 追加写日志
来源：http://blog.fktsv.cn/Article/details/gqcfkyubm.sHtML

echo "log" >> out.log
来源：http://www.m.share.sjlbkw.cn/Article/details/gunjsyzak.sHtML

[R41] 丢弃输出
来源：http://m.share.tarul.cn/Article/details/gfoqtuwcl.sHtML

cmd >/dev/null 2>&1
来源：http://blog.yfazqb.com/Article/details/gbsckvtok.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/goymqurxi.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gbeziptui.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gbqiktkqq.sHtML

find . -name "*.log" -type f
来源：http://mobile.epnwcf.com/Article/details/gvuikdqei.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/grktgkqjl.sHtML

find . -mtime -7 -type f
来源：http://m.share.epnwcf.com/Article/details/gflkxzyji.sHtML

[R45] 批量删除
来源：http://3g.vehdjk.com/Article/details/gzzpvkaps.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/gpjovvbej.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gmnqiniiu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.bbcook.cn/Article/details/gwjxbdocx.sHtML

[R47] sed 单行替换
来源：http://baike.vehdjk.com/Article/details/gfjhcjuye.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fktsv.cn/Article/details/gjljpfdpt.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fktsv.cn/Article/details/gsuiufhpm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gyaqwpusa.sHtML

[R49] awk 带条件
来源：http://baike.sjlbkw.cn/Article/details/gaxsbgbhv.sHtML


<!-- 参考信息 -->