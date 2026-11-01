代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gmsrdtljf.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gnidsmcaq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/ginepyyev.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.vehdjk.com/Article/details/gzzbksgxl.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gerdozozd.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gccgddusj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/ghlbxnqak.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gtgtoacle.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gsnwwqzka.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gyagrehcf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gnbwujzcz.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gxiwfhnpj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gcjbhqjgo.sHtML

[Q07] 删除表
来源：http://www.share.yfazqb.com/Article/details/gcqwapyjp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gxvcnwmzv.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gbnvxklyx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gxpdqkzlj.sHtML

[Q09] 创建唯一索引
来源：http://blog.vehdjk.com/Article/details/gyvrantmt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gmpscmvjy.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gfwgzcthq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gyrgymqpp.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gxqedyoqc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gyygrmxgj.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/gpriepirc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/gdcsmeisb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gshotyuvi.sHtML

[Q13] 忽略重复插入
来源：http://wap.tarul.cn/Article/details/gdmikctff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/gabyyxcle.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/grliemfxc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/guhcsykji.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.sjlbkw.cn/Article/details/ganiunudy.sHtML

[Q15] 查询全部
来源：http://blog.epnwcf.com/Article/details/giqtvgxol.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gfaylqmdd.sHtML

[Q16] 查询指定列
来源：http://www.share.yfazqb.com/Article/details/gvzrhkcbv.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ggebvitxz.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gijeplbxm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gbqxahayu.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/guuznyhgj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.tarul.cn/Article/details/gvcoxtral.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/gyfzrvbbm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gktqthunf.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gknxjxicf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/ggtgaatrw.sHtML

[Q21] 空值判断
来源：http://www.blog.tarul.cn/Article/details/gnsfrhrvi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gvuhjgxtc.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gbvdqgjay.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/gzgifcaoa.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gjxcmwcfm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gdanskcab.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/glhzcighs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gvrrpgpub.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/gtwayctgj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/gmijsxpdr.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/gqnargtja.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/ghlcrnnke.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gcufjcdpx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gipcvaidn.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gutjabaie.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gkdncpsfy.sHtML

[Q29] 最大最小值
来源：http://m.share.yfazqb.com/Article/details/giixdrwor.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjallhxfk.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gzeifdjru.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gzsytqbvp.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/geupgekal.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gsrjmpock.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/ggesarija.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gakkantmm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.bbcook.cn/Article/details/ggzgpzynr.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gdlusmtpz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gxsengoef.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/ghygwdmbp.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gpmnebrss.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/gdklwemha.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/ggcfyjmoz.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/gtalzirde.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gfgrlszbc.sHtML

[Q36] 左连接
来源：http://read.share.bbcook.cn/Article/details/gexrclnuu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gycgclfhb.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/gmaehjkll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gjnjkpuha.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/giwsxflei.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gkgbhfvsb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/ghhlhfzrg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/geegusggl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fktsv.cn/Article/details/gflyiuqjv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/gewrmpgak.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fktsv.cn/Article/details/gcspmxdaj.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gooqoclzz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/gbgcekmjc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.sjlbkw.cn/Article/details/gsxcfovgq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gsyjxnoso.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gvzvrrwmw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/govyyutlu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gllvwxuol.sHtML

[Q43] 标量子查询
来源：http://www.blog.vehdjk.com/Article/details/gvhiimfpl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/gubjpsknn.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gitnsywjs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gbhvascjo.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.epnwcf.com/Article/details/gouxukzbn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/grelvpest.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/ggequioht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gynoqhoep.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gnvegarnw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gyqmhvlyf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gfhxyfkwd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gaxlhjpcb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/gezharhic.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/gnjfqjupm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gstcncqyw.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gacwbircl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gpcsymxun.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gobuewrgk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gqllzpxzn.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/gkeogajpj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/grsmkyynw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gjsnejnht.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gjtbcyvqo.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gdvxutpce.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gvcqxcrsw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.bbcook.cn/Article/details/gbvozilsf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gusflkula.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gfwbysogs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gzqjdcbee.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/grvhbfjej.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gamchffxu.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gpgzydkfb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gfzehzzgf.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gnoaqzinx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gyrpccpjc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gwhfqyakd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpabzldas.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gofekpufe.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gwpzbreva.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gwhmyibuf.sHtML

[Q62] 分组占比
来源：http://wap.yfazqb.com/Article/details/gzbkhcncu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gsfzbuyir.sHtML

[Q63] 开启事务
来源：http://blog.sjlbkw.cn/Article/details/gnupbuffk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gryjwheio.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gsmvvzube.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gumkxtlzl.sHtML

[Q65] 回滚事务
来源：http://m.share.bbcook.cn/Article/details/gimowmekt.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/gporkliww.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gronafirn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.sjlbkw.cn/Article/details/gofddjffy.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/geyqefbrv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gqvyuzusw.sHtML

[Q68] 保存点
来源：http://m.share.epnwcf.com/Article/details/ggjlgmwvs.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gqhukkusn.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gxcjreclc.sHtML

[Q69] 查看执行计划
来源：http://www.share.epnwcf.com/Article/details/gtgpsebyh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.bbcook.cn/Article/details/gnqcyluux.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/gvtpgidpu.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gpqbpfvcg.sHtML

[Q71] 查看建表语句
来源：http://3g.sjlbkw.cn/Article/details/gfwinmdua.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.vehdjk.com/Article/details/ggbuolmyx.sHtML

[Q72] 查看索引
来源：http://m.share.vehdjk.com/Article/details/gymkskual.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gixdvvhph.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gwxdaokrb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gujekzjhd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gdualjbjs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.yfazqb.com/Article/details/gtnjawnxm.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/gsryfnyva.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gmuaksxsr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gisofnwaa.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gxcunyxge.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/grmowspyp.sHtML

[Q77] 时间加减
来源：http://mobile.vehdjk.com/Article/details/geasvwshg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/gdguallrc.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/gjctxpgoh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.epnwcf.com/Article/details/ggchllctp.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/giwgjbskx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gbzrcayag.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gojgvmzkm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gumabcnoc.sHtML

[Q81] 字符串替换
来源：http://www.share.tarul.cn/Article/details/ghbvoqwzv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gycrngixg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gzttjaldt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gppwljstj.sHtML

[Q83] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/gshtjivjq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/govpctqcg.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/ghgvcvhdd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gfasnadcj.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/guzkjvozo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gaziojkhx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gnbevyxpd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gmneuoedy.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/glzdfpbkk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gdhtgezff.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/gvyskhxio.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.tarul.cn/Article/details/gjgivtdik.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gmomcilhk.sHtML

[Q89] 判断表是否存在
来源：http://wap.epnwcf.com/Article/details/gfqntiipg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/gsunqzszi.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gbphbqfay.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/gsfmaqgaf.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gfvyjhtlv.sHtML

R. Bash 专题
来源：http://read.share.sjlbkw.cn/Article/details/gutcrkhri.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guryisejd.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gddmuydcm.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/grzgxahsm.sHtML

set -euo pipefail
来源：http://3g.tarul.cn/Article/details/gdodlotgh.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gwadsnkti.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/gcvnmdawj.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/grxuxbbbu.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gvqjbfjqm.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/goatwiven.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fktsv.cn/Article/details/gaiaugjxi.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/gjhxqlgfk.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gakwmxqlf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/glexszrad.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gulsiynrd.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/gvtzjuwjs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gkxxfwqvo.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gemvjidzf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gwmkvszet.sHtML

[R09] 字符串比较
来源：http://www.share.yfazqb.com/Article/details/gijcfiyvo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gqpvkvfaf.sHtML

[R10] 正则匹配
来源：http://baike.sjlbkw.cn/Article/details/gcesmtxps.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/gstbxhxfr.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gslkkxkmz.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gkfowsfku.sHtML

start) echo "启动" ;;
来源：http://wap.epnwcf.com/Article/details/ghbiiillx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gajfvhsbk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/gvcajbgiw.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/geturuzvb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/glmaauxmy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.vehdjk.com/Article/details/gstmnurdp.sHtML

[R13] for 计数循环
来源：http://blog.vehdjk.com/Article/details/gesqadjlq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.vehdjk.com/Article/details/grtvozlcy.sHtML

[R14] C 风格 for
来源：http://www.share.vehdjk.com/Article/details/gcdnloufp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gvqvgqjvu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/gxglqjtpg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.tarul.cn/Article/details/geaxzjazp.sHtML

[R16] until 等待条件
来源：http://m.share.bbcook.cn/Article/details/gbjymegvm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/gsbfmbzxk.sHtML

[R17] 数组定义与取值
来源：http://baike.epnwcf.com/Article/details/gvmtrmgjf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gutrkubdm.sHtML

[R18] 遍历数组
来源：http://www.share.epnwcf.com/Article/details/gibsgivha.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.epnwcf.com/Article/details/gzyvshpqm.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/ggwipjkvd.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/gwnysivqk.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fktsv.cn/Article/details/gxukwnwaq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gzvrdmwbz.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/gdafizfjf.sHtML

echo "${#s}"
来源：http://www.blog.vehdjk.com/Article/details/gmymmrdlz.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gclbslnud.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gasnyzhzm.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/gnhpnbqpk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/gowgestfx.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gpgvvxabu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gszzpfmlt.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.vehdjk.com/Article/details/ggkarxjdn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.epnwcf.com/Article/details/gfzpsaull.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gtsthkyvw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/gapqdgmgy.sHtML

[R27] 算术展开
来源：http://3g.vehdjk.com/Article/details/gzuijrowq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.bbcook.cn/Article/details/gkzbhjddw.sHtML

[R28] 浮点运算
来源：http://www.blog.fktsv.cn/Article/details/gdizhgpei.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/geafqaxuo.sHtML

[R29] 定义函数
来源：http://www.blog.epnwcf.com/Article/details/gdccosrle.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gzawvysfy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/gbijzbjzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/guyozzcak.sHtML

[R31] 局部变量
来源：http://blog.vehdjk.com/Article/details/giazcygzc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fktsv.cn/Article/details/geqmjfkft.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gggipnkag.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gnmbdkpmc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.epnwcf.com/Article/details/gvwdgxczn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gwfcuxxkr.sHtML

[R34] 退出时清理
来源：http://www.share.yfazqb.com/Article/details/gdzmzxbie.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.sjlbkw.cn/Article/details/gogumasvu.sHtML

[R35] 后台执行并等待
来源：http://mobile.bbcook.cn/Article/details/gokdjqals.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.sjlbkw.cn/Article/details/garbyhesh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.tarul.cn/Article/details/gqgfxndze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.tarul.cn/Article/details/ghvwhzfyx.sHtML

[R37] 把输出赋给变量
来源：http://www.share.bbcook.cn/Article/details/gfehmtmsj.sHtML

files=$(ls -1)
来源：http://www.share.tarul.cn/Article/details/gxuukoedx.sHtML

[R38] 管道串联
来源：http://mobile.yfazqb.com/Article/details/gdmbgowws.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.epnwcf.com/Article/details/gyhntmwbj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fktsv.cn/Article/details/gffhkbohf.sHtML

cmd > out.log 2>&1
来源：http://read.share.yfazqb.com/Article/details/gxohzdyqm.sHtML

[R40] 追加写日志
来源：http://baike.sjlbkw.cn/Article/details/gntinhfuz.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/ggcvfocgg.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gxqbuzthg.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gafwafuld.sHtML

[R42] 输入重定向
来源：http://www.m.share.yfazqb.com/Article/details/gevgpfkqo.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gjauxveik.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/ghuorvoxr.sHtML

find . -name "*.log" -type f
来源：http://m.share.bbcook.cn/Article/details/gpkkflcki.sHtML

[R44] 按修改时间查找
来源：http://www.share.sjlbkw.cn/Article/details/gxakonamh.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gvyjcukuo.sHtML

[R45] 批量删除
来源：http://www.share.bbcook.cn/Article/details/gqafknnux.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.tarul.cn/Article/details/gevjyusrj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.bbcook.cn/Article/details/gxdhzjgat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.epnwcf.com/Article/details/gqnncsekq.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gyeklyjhx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gqmusmefl.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/godhaqmdz.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fktsv.cn/Article/details/gfqtxqrjo.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/gucgsxksh.sHtML


<!-- 参考信息 -->