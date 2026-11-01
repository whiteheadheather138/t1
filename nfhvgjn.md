代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gwsqkssmq.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gjqpgugax.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/godczjagg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gltoolxfu.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/ganupofql.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/gllymqien.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gbsgwxhfl.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/gzexgcenp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/gippmsrpn.sHtML

[Q05] 重命名列
来源：http://m.share.fktsv.cn/Article/details/gpyowlwkj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gzkfaackg.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/gsznetrqs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.bbcook.cn/Article/details/gxmwcgnws.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/glpymtdss.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gqzehrlyg.sHtML

[Q08] 创建普通索引
来源：http://blog.tarul.cn/Article/details/gmqntgllr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gpkeipzpz.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gsjjixhow.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gkiofojvx.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/guxsehrvn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gxnnnoaeq.sHtML

[Q11] 一次插入多行
来源：http://www.share.yfazqb.com/Article/details/gaagkduid.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gayznkjrg.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/ggasdxydk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.vehdjk.com/Article/details/gheekdaei.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gijolphhv.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gimfyxtzx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.yfazqb.com/Article/details/ggnphitlm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gamxmqzts.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gubkepuyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/giutxrduw.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gehiitqva.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gygomfkuz.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gvzbbzoyy.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/gmixjtmjs.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/glmlpjtyj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/getnaewcr.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/glppvyrzp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gugncjngj.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/gycpwgmcf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gtwbkkjug.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gmtuxizdn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gggcpzzxx.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gfwrqihra.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gokrhitar.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gykusmref.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gujibcjdc.sHtML

[Q23] 分页
来源：http://read.share.tarul.cn/Article/details/gmlxgdowm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/gyadgjoof.sHtML

[Q24] 去重
来源：http://baike.sjlbkw.cn/Article/details/gwcwzqduk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gyyevwumr.sHtML

[Q25] 只取前 N 条
来源：http://3g.yfazqb.com/Article/details/gztrxaijy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/gvtvefrym.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gggiagyfi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/gmpgqmjew.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gjrccnsmq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/geubosmjk.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/gfbivslsi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/glhyweanl.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/goalwetuv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/glxoatyfd.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gmvjemkrz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/guorcwdyb.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gaouatacf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gkmjensys.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gmsdszbpy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/guhgzfjtj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxlpiztm.sHtML

[Q33] 多列分组
来源：http://blog.vehdjk.com/Article/details/geycjhqqo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fktsv.cn/Article/details/gdsfklujh.sHtML

[Q34] 每组取第一条
来源：http://www.blog.bbcook.cn/Article/details/gwjslkkcj.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gvenlkpip.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gtewusbpv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gbntbuaug.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gtrcpdlmj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gxbzbbdsp.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gybeuxftg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gzdwruaau.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/gjfywxhll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.tarul.cn/Article/details/gqjmcaklz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gcgedjlwm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.bbcook.cn/Article/details/gwzzewjjj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.sjlbkw.cn/Article/details/guqcqxdlp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.vehdjk.com/Article/details/gskqyunub.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gppokeuun.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gosvnxtta.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/gwgzcmxus.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gmnnqqmlb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gicvkrtos.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gvwefezci.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/gchpqvzfa.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gztonrnge.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gngunjaei.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gavcfgqox.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gyfqjziba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gucdffyrj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.yfazqb.com/Article/details/gvhemkucx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gipfzcwfo.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gskgcipte.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gmzzcgnyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/ghmrxokwq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gzwxudyhe.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gyxlvvibh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/gggmxbsnt.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/gukgkqkqr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.vehdjk.com/Article/details/gwkxxzmuc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.tarul.cn/Article/details/gwqlcsxen.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gbjwamxbt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gepwxwklx.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gxqgaybvt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gqrcttytb.sHtML

[Q51] 用子查询更新
来源：http://www.share.yfazqb.com/Article/details/gxjjdlwxl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/gpynzgbwv.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/graeaacpj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gvhhrnrvj.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/ghmykysyj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gqfuauywz.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/gtenhsbqo.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gzjivizqx.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gicdupfvq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gvznpjddu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gnyjksiys.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gtqlxhquu.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/gczhaxavm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fktsv.cn/Article/details/gcygoybee.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gebxoayvp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gkrdodpbe.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gmefstkqu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gzhabtutc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/gelxhiils.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/govlgogem.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcispdepk.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtacanuu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gkrgrfaqj.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqxxwawt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gfwraxbmu.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gmibdbylx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/gjmgmdubo.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gkivnokcx.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gzcscxibe.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/grqpspqcq.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gugcwpjgg.sHtML

[Q66] 行锁查询
来源：http://blog.fktsv.cn/Article/details/gfhhtowij.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/glveaqakq.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gziogajbg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/gedaecozf.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/giehhcxdl.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gtwpzwqod.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/glvvhlxgt.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gfhjdmnns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gdwxzaokb.sHtML

[Q70] 更新统计信息
来源：http://wap.yfazqb.com/Article/details/gpxgpayls.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gigrvihqc.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/glzjhpjuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/grgsqmpeo.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gchmraeaq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gthwguczr.sHtML

[Q73] 查看表状态
来源：http://www.m.share.bbcook.cn/Article/details/gdnocrfng.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gmgeclmor.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gdurnicov.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gjzoyzpmz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.tarul.cn/Article/details/gutuylhel.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/glxdjnvpe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/ggbkvagpv.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gsgultudw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gdkctgdem.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gwftlnnex.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gcfnrkbjq.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/giecobttw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.vehdjk.com/Article/details/guftkdyws.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/guiijamin.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gmzgjrktg.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/girrigbjp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqdwyrryt.sHtML

[Q81] 字符串替换
来源：http://3g.yfazqb.com/Article/details/gzhyxvvyn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gryvszajv.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/goewtcklw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gywxcukdl.sHtML

[Q83] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gmuaohkqs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gupmlanyn.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gjinvnxvh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gaxqwqjvn.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/grkbtcbcg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gmilrldwx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/givupivkd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gesdaywvj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/guevlphmb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gmdlvmlaw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/glcnchxta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gwxixbwjf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gupdchesl.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gojzekmxq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/gprnhemfz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.epnwcf.com/Article/details/giuynadbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gjjgddciw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gxbrojbfn.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gaxaciych.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/glqjprckh.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gcnbbwcev.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gnstddlck.sHtML

set -euo pipefail
来源：http://www.blog.fktsv.cn/Article/details/gbrjcgorp.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/gxknvmuqt.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/gfddoekdg.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/ggrdzogms.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gjjahrhrm.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gntzxsaql.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.vehdjk.com/Article/details/glpaztqhw.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/godaxrtux.sHtML

name="${1:-default}"
来源：http://blog.bbcook.cn/Article/details/gmzsxftvp.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/grxpowdem.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gfabubrvq.sHtML

[R07] if 判断文件
来源：http://www.share.epnwcf.com/Article/details/gezwfkdjk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gxrqihhig.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gifzbvpxr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.epnwcf.com/Article/details/gygsvxqht.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/giofdmltr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gatckfaip.sHtML

[R10] 正则匹配
来源：http://www.share.yfazqb.com/Article/details/gvjtwkisi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gzgmsqleu.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gosdyxnkm.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gfpqgjjbw.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gjmsbmtye.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gflvilzhi.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gebbknppj.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/gfbibgnmw.sHtML

[R12] for 遍历文件
来源：http://m.share.fktsv.cn/Article/details/grmzmwwso.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gzoqqeaur.sHtML

[R13] for 计数循环
来源：http://3g.fktsv.cn/Article/details/gzjzfwjng.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gerqhgkkj.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gemgerrui.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gubxiskuk.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gkqyiliem.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gekeaandr.sHtML

[R16] until 等待条件
来源：http://3g.fktsv.cn/Article/details/gatovgmwd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gklvwfpek.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/gmlqitbad.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gaboopqgp.sHtML

[R18] 遍历数组
来源：http://wap.sjlbkw.cn/Article/details/grciyffna.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/grniwjjqm.sHtML

[R19] 数组长度
来源：http://wap.vehdjk.com/Article/details/gyfqjyyup.sHtML

echo "${#arr[@]}"
来源：http://3g.yfazqb.com/Article/details/gedbcgrxz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gazpemqzk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.epnwcf.com/Article/details/giewdmolj.sHtML

[R21] 字符串长度
来源：http://www.blog.fktsv.cn/Article/details/gyfnlcanb.sHtML

echo "${#s}"
来源：http://blog.epnwcf.com/Article/details/gefpysfio.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gfubafyuu.sHtML

echo "${s:0:5}"
来源：http://www.m.share.tarul.cn/Article/details/gpleioeae.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/garxnmkli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.tarul.cn/Article/details/gkyjbbugt.sHtML

[R24] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gncsgzqyb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gjqolzzsi.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/gkgvuvuda.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gboftuehw.sHtML

[R26] 命令替换
来源：http://m.share.epnwcf.com/Article/details/gxoptmvbl.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gnbmgflhc.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/gothmdnjs.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.bbcook.cn/Article/details/gzrvrfyti.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gwdvsyenq.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/glwhljhlw.sHtML

[R29] 定义函数
来源：http://blog.yfazqb.com/Article/details/gwladpufc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gndbdmoyw.sHtML

[R30] 函数返回状态码
来源：http://blog.fktsv.cn/Article/details/gcqvnnpyl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.bbcook.cn/Article/details/gvqgshxhb.sHtML

[R31] 局部变量
来源：http://www.blog.bbcook.cn/Article/details/gttmfskmz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.vehdjk.com/Article/details/gxshlrxvj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/gwenfhrzq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gsrkpvlsq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/glhlfvtex.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gxblokmjd.sHtML

[R34] 退出时清理
来源：http://wap.epnwcf.com/Article/details/ghwrlmtis.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gkylsfcev.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/ggmosavdi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fktsv.cn/Article/details/gklksvinn.sHtML

[R36] 并发执行多个任务
来源：http://3g.epnwcf.com/Article/details/goroikdwj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.epnwcf.com/Article/details/gkjhacfqt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/gjfkwldnj.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/guubymwmw.sHtML

[R38] 管道串联
来源：http://wap.tarul.cn/Article/details/gfuxpgoxt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.sjlbkw.cn/Article/details/ggmcaalch.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.vehdjk.com/Article/details/gbixmjpxy.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/giprdazzp.sHtML

[R40] 追加写日志
来源：http://mobile.sjlbkw.cn/Article/details/gauzvcjpi.sHtML

echo "log" >> out.log
来源：http://www.m.share.fktsv.cn/Article/details/ggwcwzixi.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/gjwaurutu.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnkazlna.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gufuxcdep.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gfgyxvuic.sHtML

[R43] 按名字查找文件
来源：http://baike.epnwcf.com/Article/details/gbuaxqzmj.sHtML

find . -name "*.log" -type f
来源：http://3g.tarul.cn/Article/details/gmaytnxbz.sHtML

[R44] 按修改时间查找
来源：http://www.blog.bbcook.cn/Article/details/gypcydtxp.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gboybjouj.sHtML

[R45] 批量删除
来源：http://www.m.share.tarul.cn/Article/details/glekprjue.sHtML

find . -name "*.tmp" -delete
来源：http://blog.tarul.cn/Article/details/ggjlhinjd.sHtML

[R46] 递归替换文件内容
来源：http://mobile.yfazqb.com/Article/details/gkpiidteo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.yfazqb.com/Article/details/gnscthjua.sHtML

[R47] sed 单行替换
来源：http://www.share.bbcook.cn/Article/details/gpksdvauj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.bbcook.cn/Article/details/ggbdnotbu.sHtML

[R48] awk 取指定列
来源：http://wap.vehdjk.com/Article/details/guogtmeav.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.vehdjk.com/Article/details/galzskytq.sHtML

[R49] awk 带条件
来源：http://blog.sjlbkw.cn/Article/details/gdobnxgwm.sHtML


<!-- 参考信息 -->