代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gvkqrukhz.sHtML

);
来源：http://blog.bbcook.cn/Article/details/glnntzojs.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gmwetvzzs.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/gpenjeeeo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/guopcaaja.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/guoxnigdv.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/gilhrfpqz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/gsbuotrkp.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gmafbvkse.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/gsjyflxkc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/genmumgdf.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/gjmbqcnee.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gkaiualet.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gguymcdkv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gyaegxolx.sHtML

[Q06] 删除列
来源：http://baike.tarul.cn/Article/details/gwtxtzqym.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkheiedvk.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gmeiyprjb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/gqvsridko.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/giqiydpjs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gcyxmcpmn.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gspbmfhpg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gvwvorjra.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/geptnduhl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gdkzlfhbs.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gkejvohew.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gydkmxkjc.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gxcwywqsy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.sjlbkw.cn/Article/details/gnieyebbo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/ggtalbvxl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gcdzmtwgs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gfluunlmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gtflwaflr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gbtmkgmzr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gecjrpnus.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/gdyeczafu.sHtML

SELECT * FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gewurtzac.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/glvmqmqag.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gdqyzlqbm.sHtML

[Q17] 条件查询
来源：http://3g.fktsv.cn/Article/details/gmqzmcfwe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gvemzjsdj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gkqkasyix.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gqnrsqzkv.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/gryqqubsr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/ghnjfayqh.sHtML

[Q20] IN 列表
来源：http://wap.tarul.cn/Article/details/gbvljzqdo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gifgcpbia.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/glaopuktp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gvduwrvue.sHtML

[Q22] 排序
来源：http://mobile.bbcook.cn/Article/details/gasdfahkw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gfsuhfruq.sHtML

[Q23] 分页
来源：http://www.blog.fktsv.cn/Article/details/gqzlkgcjx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gkghlnhfq.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/ghehfaeum.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gjvvpalej.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/ggyvdoasp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gbqnrgvoe.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gekwqioui.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.tarul.cn/Article/details/greerubuz.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gtvisotff.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.vehdjk.com/Article/details/gdjjsgpcf.sHtML

[Q28] 求和与平均
来源：http://baike.epnwcf.com/Article/details/guogjbczt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gxxrjgyzy.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gdyffcudw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gfdmwpqzx.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gxwmbzuqc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gjvilqxbm.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gzzlurccx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/godzwtpmp.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gkehvxzts.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gfvedlptv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/gbsthvliw.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/ghahuvcpn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fktsv.cn/Article/details/gduhuvtbh.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gwxwbkozk.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/gaweyopzw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/glghsgeva.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gtbhodhec.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/gfvceulov.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gpiytxtnl.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gkudxpqtx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gwpivcbpk.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gqxztnyzh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gtawlramq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/gqbztipme.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/guoyqpgbz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.tarul.cn/Article/details/gldnvurzq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.tarul.cn/Article/details/gumtujlhj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.sjlbkw.cn/Article/details/gsfwzwtfz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gvswghhuo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gmftkmxfg.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/grauxjhwv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/grdzhxebo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/gkyzxadgi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fktsv.cn/Article/details/gismcqvca.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfubcvxi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/gyqsmyscu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gnldlmxer.sHtML

[Q43] 标量子查询
来源：http://mobile.fktsv.cn/Article/details/gfrsdgudr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gsxxkjiwm.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gbmkaockh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.tarul.cn/Article/details/gpliiaulr.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.yfazqb.com/Article/details/gqxjkghzx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gzmoakgju.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gcrsvgppe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gibsigqsb.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fktsv.cn/Article/details/gyptayvkv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/ggaggjqlz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gglhybhct.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gdukpiyei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/grakzgkvl.sHtML

[Q49] 更新单行
来源：http://www.share.bbcook.cn/Article/details/gjmhbueax.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gwfxfnpoq.sHtML

[Q50] 批量更新
来源：http://m.share.epnwcf.com/Article/details/gfozwbrxc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gxccpjcsd.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gkcvvvxze.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.sjlbkw.cn/Article/details/gcuaglkfu.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gtyasfqwj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gleecahxx.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/glhsiqadk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.yfazqb.com/Article/details/gzxlhhepn.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/golxlpuhp.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/gnaqaursk.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/geknwprvs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gojuklmmi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.yfazqb.com/Article/details/gkqcfzxta.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/grmvzojpm.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gsknntcvs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gymwcuyvp.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gffncvejy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gigyvzsea.sHtML

[Q59] 分组内累计
来源：http://www.blog.bbcook.cn/Article/details/gzdbzhlol.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grmbisfaa.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gdivyggqr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.epnwcf.com/Article/details/gncmofsow.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/gtdebvmzt.sHtML

[Q61] 移动平均
来源：http://baike.epnwcf.com/Article/details/gxcjsuxeb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/giwvhsccl.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gtvydfyaz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gcsmaakwa.sHtML

[Q63] 开启事务
来源：http://m.share.sjlbkw.cn/Article/details/gxnmxnsow.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/grondbfwz.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/geyzgyfda.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gzfdhtgaa.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/ggfotbdsc.sHtML

ROLLBACK;
来源：http://read.share.tarul.cn/Article/details/gasfomawp.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gdssxsmjh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gpbpvaxgp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/ggsuxkihc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gwpsdwehw.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/gfplwugbj.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/genqfoyyc.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/gkrbyhnej.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gsoenmrsf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.yfazqb.com/Article/details/gduzvmjsq.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gegdjofof.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gwrkqztou.sHtML

[Q71] 查看建表语句
来源：http://wap.fktsv.cn/Article/details/ggazobtzf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gmunpqbfl.sHtML

[Q72] 查看索引
来源：http://www.share.yfazqb.com/Article/details/gyutfdxsq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gvfialfxo.sHtML

[Q73] 查看表状态
来源：http://wap.epnwcf.com/Article/details/gbittuxce.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.epnwcf.com/Article/details/guolbneqp.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gkavgaxcm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/grilveqjl.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gitcfgxqk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gckjopepr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gwynsgoci.sHtML

[Q76] 按天统计
来源：http://blog.epnwcf.com/Article/details/gnikpwjox.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.epnwcf.com/Article/details/gniamsohm.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/grixmakkz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gydqmdgmp.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gkoygehqo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/gvrlyscpz.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/ggiusdsoo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gjktfjgaj.sHtML

[Q80] 字符串截取
来源：http://blog.tarul.cn/Article/details/gromgdiaj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ganiayzgj.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gfdbruvnu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/ghsgdfyyf.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/gwjhsuwqv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gcrajdoze.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gpdzwzijr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gdvuilxkg.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/ghhwvyzge.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gpjtargqf.sHtML

[Q85] 数值取整
来源：http://wap.vehdjk.com/Article/details/gkdeftyxi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gdvngmwww.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.vehdjk.com/Article/details/gikonmqwy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.epnwcf.com/Article/details/gelntaxvw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/gdpxvbpfj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/glvdxvkfe.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fktsv.cn/Article/details/glapqpzcl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fktsv.cn/Article/details/gdlpbbwkr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gqlpouguc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkvwkxfi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gazdfswdh.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/gohkkyaah.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/giqbdtcoi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyepfylro.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gzemaxnye.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggdomkyzm.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/ggujmmhsc.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gvhhxfgsd.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gpegxqivk.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gcweacqzk.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/gvprjcgbf.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gtbglppqi.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/ggsoffube.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/goaijoyeg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/grrgsxznr.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/goznuhcjk.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/gdtwtyprn.sHtML

[R06] 判断命令是否存在
来源：http://3g.yfazqb.com/Article/details/gudihnobu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.bbcook.cn/Article/details/gnvvcpysv.sHtML

[R07] if 判断文件
来源：http://wap.sjlbkw.cn/Article/details/gtxpyzekp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gevlhbilu.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gwfbyujrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/gsjfhzsfz.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/ggunkdbgz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gojhyohjz.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gqujunnau.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gbyiccfle.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gnxtsbvih.sHtML

case "$1" in
来源：http://3g.sjlbkw.cn/Article/details/gxmbvwdrx.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gbucwcuqk.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/grmdjwhzn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsvldtum.sHtML

esac
来源：http://wap.sjlbkw.cn/Article/details/goxsiavpm.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gyrxrwvls.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.sjlbkw.cn/Article/details/givwbvzxi.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/ggtdsswsk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/ggvivkmic.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/gbrhstyon.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gbboleveq.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gvdxznwjy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gkabshgtf.sHtML

[R16] until 等待条件
来源：http://mobile.tarul.cn/Article/details/getwlymfa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gskxyhnlp.sHtML

[R17] 数组定义与取值
来源：http://blog.tarul.cn/Article/details/gwegtzsma.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.bbcook.cn/Article/details/gwdepnval.sHtML

[R18] 遍历数组
来源：http://m.share.fktsv.cn/Article/details/gymbzhrso.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/grwgbsrrx.sHtML

[R19] 数组长度
来源：http://www.m.share.vehdjk.com/Article/details/gcsqkpepw.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gwqcjkzxe.sHtML

[R20] 关联数组（字典）
来源：http://baike.epnwcf.com/Article/details/gkmufntbh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fktsv.cn/Article/details/geostisaa.sHtML

[R21] 字符串长度
来源：http://3g.vehdjk.com/Article/details/glofqxkwv.sHtML

echo "${#s}"
来源：http://mobile.sjlbkw.cn/Article/details/gbkaaqwsg.sHtML

[R22] 截取子串
来源：http://www.blog.tarul.cn/Article/details/ggrauxqzi.sHtML

echo "${s:0:5}"
来源：http://read.share.yfazqb.com/Article/details/gpbciuywv.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gzyktuzyx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/ghqbagway.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/ghwtglgzu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.vehdjk.com/Article/details/gyawnmypp.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/gecddvzdr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.yfazqb.com/Article/details/guktdbvwt.sHtML

[R26] 命令替换
来源：http://m.share.bbcook.cn/Article/details/gxohhiqtp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyscfchmi.sHtML

[R27] 算术展开
来源：http://wap.bbcook.cn/Article/details/gjlpcsbnv.sHtML

echo $((1 + 2 * 3))
来源：http://wap.bbcook.cn/Article/details/givkvwrwp.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gwlfhcggf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.tarul.cn/Article/details/giqyialxi.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gxyitzcnu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzgcehuj.sHtML

[R30] 函数返回状态码
来源：http://read.share.epnwcf.com/Article/details/ghpgzblgu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fktsv.cn/Article/details/ghjnzaktt.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gfrcirhmk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/gifkpwlur.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gcmmaeyvx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gniuxknel.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/gmiakudne.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gsedhague.sHtML

[R34] 退出时清理
来源：http://blog.vehdjk.com/Article/details/gabsxiutv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gfhncupvt.sHtML

[R35] 后台执行并等待
来源：http://wap.vehdjk.com/Article/details/ghfwckhfa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.vehdjk.com/Article/details/gqlwacekh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.vehdjk.com/Article/details/godsaxxxn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gkrjcwppw.sHtML

[R37] 把输出赋给变量
来源：http://blog.sjlbkw.cn/Article/details/gieweekrm.sHtML

files=$(ls -1)
来源：http://www.m.share.yfazqb.com/Article/details/gbwxapzum.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gvvjqaywk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fktsv.cn/Article/details/gpgxhqvzj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.yfazqb.com/Article/details/gqnkuwiko.sHtML

cmd > out.log 2>&1
来源：http://blog.epnwcf.com/Article/details/goirrltjr.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gzopqjmdj.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gwewojnul.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gzzpzueuw.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/gyubozzhy.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gpygdwvyt.sHtML

wc -l < a.txt
来源：http://read.share.yfazqb.com/Article/details/gbxaezrcb.sHtML

[R43] 按名字查找文件
来源：http://www.blog.sjlbkw.cn/Article/details/gipdozrpa.sHtML

find . -name "*.log" -type f
来源：http://mobile.fktsv.cn/Article/details/gmyutsgbd.sHtML

[R44] 按修改时间查找
来源：http://3g.tarul.cn/Article/details/gdcexwsqt.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.sjlbkw.cn/Article/details/gsffambib.sHtML

[R45] 批量删除
来源：http://baike.yfazqb.com/Article/details/gkmpmtwzl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.tarul.cn/Article/details/gsioyjlyw.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gfmyzbrrv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.tarul.cn/Article/details/gscdjxsat.sHtML

[R47] sed 单行替换
来源：http://www.blog.bbcook.cn/Article/details/gzbibsqzd.sHtML


<!-- 参考信息 -->