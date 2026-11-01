代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gnlmokyni.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gaamazarj.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/glybtjvzw.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/golvrqtie.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gdjeykxms.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gpjggmznt.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gnmsbyusn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gojrrfitn.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/gofsafcll.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/ggvwzkqqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/ghozpjifa.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gyjdlnris.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/gqjphhmwp.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gsscnosgp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.vehdjk.com/Article/details/gyjebjveg.sHtML

[Q06] 删除列
来源：http://www.share.epnwcf.com/Article/details/gxrjyinwk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gciibepxe.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gcnwivwfm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gznouyuhs.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gpuzkjmlp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gzcjqqplk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.tarul.cn/Article/details/gqrtbkrzz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gmfbibtpq.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gdsrzyohm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gzmsssmyt.sHtML

[Q11] 一次插入多行
来源：http://baike.epnwcf.com/Article/details/gcmtzbvet.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gcqdlenhg.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gzvueguxe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gtchezmmz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gdgbfwflc.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.yfazqb.com/Article/details/gleftmldg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gwzoxvaef.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.vehdjk.com/Article/details/gvozwdgsw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gdawakpov.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gfxbtkkip.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/gbwqjrvyj.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gajzwqrma.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gdhjtvrlw.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gziraxozh.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gajnyxbxg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/gsxgruwoe.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/guztyaiiw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.epnwcf.com/Article/details/gdlqhrqtw.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gzhuyuqke.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fktsv.cn/Article/details/gzaitohnb.sHtML

[Q20] IN 列表
来源：http://www.blog.epnwcf.com/Article/details/gdhwvcgjs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.bbcook.cn/Article/details/ggbyqzkiz.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gougzimcs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.vehdjk.com/Article/details/gmbjokwdh.sHtML

[Q22] 排序
来源：http://www.share.epnwcf.com/Article/details/gwmedyrzf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gasedilpw.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gykhpomxa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/glhqhdphh.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/glodoqdse.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gfbzsuyvj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.yfazqb.com/Article/details/gvtchnsgz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/ghtptpscm.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/gfhkohvqh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxynewyxz.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gwypxvrrp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gfunrsyrl.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gtbafpxyq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/grwxrekkn.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gnwgpykfx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/grpauynvc.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gblycqpec.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gxxjxglkh.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gndzcgioi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gjilkagmu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwptuumto.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/guimzzqhh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.sjlbkw.cn/Article/details/gheunrnye.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gkyirupul.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fktsv.cn/Article/details/ghpcmscvh.sHtML

[Q34] 每组取第一条
来源：http://m.share.sjlbkw.cn/Article/details/gllkxiiaj.sHtML

SELECT * FROM (
来源：http://www.share.yfazqb.com/Article/details/gctpvacdw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gauzjdqoe.sHtML

) t WHERE rn = 1;
来源：http://read.share.yfazqb.com/Article/details/gkgolbkdd.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gfxdbphpj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gyfzydhve.sHtML

[Q36] 左连接
来源：http://m.share.vehdjk.com/Article/details/gentnoryd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/ghwyobftz.sHtML

[Q37] 右连接
来源：http://blog.yfazqb.com/Article/details/gupfxpwdi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gtrxoflyc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gqcjbfycy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gevptfwpu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fktsv.cn/Article/details/glkoqvzva.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gtdccpgvo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.vehdjk.com/Article/details/grbgfvbyh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gyhrybvoj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gviffqbec.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gwbvzasom.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gjshlrqzd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/ggpwjyist.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gxecaqqbz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/ganpnnmxg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gkzyadhav.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gijhvvzkd.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/glvaycnph.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/ghbgfdxcj.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/gabumjeaq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gvpnirwnf.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.sjlbkw.cn/Article/details/gtoadebil.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gyluvccgp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gwnmdhwnk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gzeusxvid.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/ggmrupfnu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.sjlbkw.cn/Article/details/gdopxexnm.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/gfoivpthf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/goquloomd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/geblkfohj.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/guuxdsgyw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gdnvmkott.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/gafoqjlpi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gorbbpziu.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gyyncfvim.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gecidljlq.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/gjpflkjfc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gknimkwzh.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/ggeytwhqe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gpehiutjm.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/glaeslaqi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gplqonogx.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gpucnlhdb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.bbcook.cn/Article/details/gjbpxpway.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gxscvxjuv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/grpwhczpf.sHtML

[Q57] 行号
来源：http://3g.fktsv.cn/Article/details/gznzuafti.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.tarul.cn/Article/details/gavhajavh.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/ghfczzqxb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/gndvesiig.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gmselkfbn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gxhqsxhlb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/geamxkxpt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gqbqsxziw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gctfpghfp.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/ggaleuhpm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gevkadwcw.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gkzwzgecw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gkmwdrxeb.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gciuwejih.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/ghemqpigy.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gfnifffqo.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/godubzioo.sHtML

[Q65] 回滚事务
来源：http://blog.sjlbkw.cn/Article/details/gsehfyigx.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/gqaeydlks.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gjtcoezqa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gcfwcqhpw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/ggcfmxpsn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.tarul.cn/Article/details/gbswyrmti.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gddrkhzgw.sHtML

SAVEPOINT sp1;
来源：http://3g.fktsv.cn/Article/details/gbxumjhgh.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gkpkjwoms.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.epnwcf.com/Article/details/gqvlvuhvz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gmrgilbqb.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gaaimsnws.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gxypbisnw.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/gzcqjzqcu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gduhogemk.sHtML

[Q72] 查看索引
来源：http://mobile.fktsv.cn/Article/details/gewxtrsvr.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gpsykjlke.sHtML

[Q73] 查看表状态
来源：http://wap.fktsv.cn/Article/details/gjwwmozdk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gsdtabxnt.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gillhwtzr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gghxppzlx.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gagdootnf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gcazwwmrg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.tarul.cn/Article/details/ghhmaczel.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gvkbfawri.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.vehdjk.com/Article/details/gmqgmzfvs.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/gntybfkex.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.epnwcf.com/Article/details/gxpiscupk.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/gdzsslhmz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/ggmuidzqi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/glwybrchf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gitsxdian.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gnggabhei.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gcsgsgeqg.sHtML

[Q81] 字符串替换
来源：http://3g.bbcook.cn/Article/details/gjwyyjuyy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gotuflbmw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gelyarehf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gshbegizp.sHtML

[Q83] 大小写转换
来源：http://wap.tarul.cn/Article/details/gfpnmpiam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/ghoutqxyq.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gvrkblrln.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gbusigexs.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gelzwgelu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gowiztixc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gjwivpflb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gowcfoqce.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/gqcdghgwc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/gjsrggcev.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gdisclgeq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gmakyzxcb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/gbqpoakii.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gckmkaoue.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gazvdcjbm.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gqpznlhql.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.sjlbkw.cn/Article/details/gyvljvjsr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gazudrbig.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/glebujrfb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gokdpzjro.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gvknsrnah.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/gqwyengta.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/grnzwuhht.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.tarul.cn/Article/details/gukokrvfz.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/gddlyimbt.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gnqgzbywf.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/ghelxtkhk.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/glxxagsme.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/grdidlaqf.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gaymcljux.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gyvqeriob.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gicuikyoz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gycnpzhwv.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gqcuakyjk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.epnwcf.com/Article/details/gilycjqwa.sHtML

[R08] 数值比较
来源：http://3g.epnwcf.com/Article/details/gvhvtbnss.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.yfazqb.com/Article/details/gjpofenkn.sHtML

[R09] 字符串比较
来源：http://read.share.bbcook.cn/Article/details/gtiifoplc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.sjlbkw.cn/Article/details/gqbzdjvkz.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gniyqfzid.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fktsv.cn/Article/details/giclhvzik.sHtML

[R11] case 多分支
来源：http://3g.vehdjk.com/Article/details/gouzxtdjq.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gvllndvet.sHtML

start) echo "启动" ;;
来源：http://www.blog.yfazqb.com/Article/details/gceqduejw.sHtML

stop)  echo "停止" ;;
来源：http://wap.vehdjk.com/Article/details/gjkriedfq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gyexwqfqj.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/grvgzzesl.sHtML

[R12] for 遍历文件
来源：http://blog.epnwcf.com/Article/details/gxerqozut.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gcttueziz.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gmfldxcdw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gdfqmbuaw.sHtML

[R14] C 风格 for
来源：http://www.blog.sjlbkw.cn/Article/details/ggddphnkj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gojsewtqt.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gytlxxezk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gkqnpznhj.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gcmakgocb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gpqmeldho.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gycqsvbcd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.yfazqb.com/Article/details/gtpfodtxq.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/ggrojtqro.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/gtfaixbhv.sHtML

[R19] 数组长度
来源：http://read.share.epnwcf.com/Article/details/giamcdznq.sHtML

echo "${#arr[@]}"
来源：http://blog.vehdjk.com/Article/details/glldhximl.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gthukefpk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fktsv.cn/Article/details/gvxazgaah.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gwtlptczd.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gwkxqaitk.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/gtegonies.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gatxctzdf.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gmnfjfpjk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fktsv.cn/Article/details/gzidcegkl.sHtML

[R24] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gihzitlwg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/gxbfypwxd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.epnwcf.com/Article/details/gdsvzrpun.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/gbatdxohj.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gxurvmbug.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/gqgmjmxih.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gpwdbcuma.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gtybqcnro.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/gtheaccol.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.epnwcf.com/Article/details/gpwssiqek.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/geqanndrz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.sjlbkw.cn/Article/details/gdcdsbgdy.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/gzeqwyref.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.tarul.cn/Article/details/gcogahfvo.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/glcdaskxi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gooslidrh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gyazvprvq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/ghbfoshqt.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.epnwcf.com/Article/details/gtqnjfawn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.sjlbkw.cn/Article/details/gvubcrpyf.sHtML

[R34] 退出时清理
来源：http://3g.yfazqb.com/Article/details/glyvldakg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gixropkcy.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/givzbbagd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.vehdjk.com/Article/details/grvgldgyg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.vehdjk.com/Article/details/giryeajht.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.sjlbkw.cn/Article/details/gcishfkqk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gvobhspet.sHtML

files=$(ls -1)
来源：http://www.blog.epnwcf.com/Article/details/gbmcviuxc.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gehjkmetu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gyftqbejj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gljtewjkj.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gywkotouj.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gzsyluojl.sHtML

echo "log" >> out.log
来源：http://wap.bbcook.cn/Article/details/gkqqpldgd.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gouoviito.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.epnwcf.com/Article/details/gqegvopvw.sHtML

[R42] 输入重定向
来源：http://mobile.sjlbkw.cn/Article/details/gqahowciq.sHtML

wc -l < a.txt
来源：http://read.share.vehdjk.com/Article/details/ghfcksten.sHtML

[R43] 按名字查找文件
来源：http://mobile.yfazqb.com/Article/details/gamspwrwa.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gmgkkalvh.sHtML

[R44] 按修改时间查找
来源：http://baike.tarul.cn/Article/details/gdasozzyf.sHtML

find . -mtime -7 -type f
来源：http://mobile.fktsv.cn/Article/details/gcizrcbat.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gumeilopd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gxdzrsjvt.sHtML

[R46] 递归替换文件内容
来源：http://baike.fktsv.cn/Article/details/gyvkafjet.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gzqlierkj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gsavrcixi.sHtML


<!-- 参考信息 -->