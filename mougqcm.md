代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gggogaevy.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/ggiupbuof.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gnllglgsv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.sjlbkw.cn/Article/details/gylepziix.sHtML

);
来源：http://baike.tarul.cn/Article/details/ghfmgdsml.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gaenlvbls.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gxepnbfao.sHtML

[Q04] 修改列类型
来源：http://read.share.bbcook.cn/Article/details/ghjjpguyv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/guzjqwxqp.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gkqedahms.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gzapgpndd.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gkmxkedjh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gyotlvnvh.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gsmuosryy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fktsv.cn/Article/details/gclputsya.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gtcplajia.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeqpgudc.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/glejyoted.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gkpjjdvzx.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gampehbou.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.tarul.cn/Article/details/gmitouxog.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gilskaryq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/gifdoqhvf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/gozbmnvuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gitngtukm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.yfazqb.com/Article/details/gxkbxtyhq.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/gcwsttvnc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/goyrhynas.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gadfqbvvj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gazlddvvo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/gcvxhmmov.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gapfidseb.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gzizzezbp.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gjuottazd.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/guzdxgsxg.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/gzecajvul.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gwksmhdmw.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gsnokdpuz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gcmrzigej.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/ghtbtuwsc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.bbcook.cn/Article/details/gdvizyrqo.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gkqbhmryw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/guevxczit.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/grjputrmb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gouengepk.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gtoiktoeo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/grlpgcbwn.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gnxjliucs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gttcxihax.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/guejkiwmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gadncwfgy.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/glbylgord.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/gqsujsipg.sHtML

[Q26] 计数
来源：http://read.share.bbcook.cn/Article/details/gxajhaunu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfeaeftiq.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/glkbyyiep.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/glcljlvaf.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gtblmwopg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/gypdtrrwx.sHtML

[Q29] 最大最小值
来源：http://wap.fktsv.cn/Article/details/gsvzrclat.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/gpnocipjx.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gnljczgnj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gpcnmtkva.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gzovedhfc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/gmnwdlsbl.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/guqvjnqqo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gujsncgcj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fktsv.cn/Article/details/gbxbqocrs.sHtML

[Q33] 多列分组
来源：http://3g.fktsv.cn/Article/details/gsipaqdkl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gqmikamts.sHtML

[Q34] 每组取第一条
来源：http://read.share.tarul.cn/Article/details/gyaftaauy.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gzokjzwmz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/gyajisxzd.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/gznxnjclf.sHtML

[Q35] 内连接
来源：http://wap.tarul.cn/Article/details/gnfxhfdxu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gsxqgxjni.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gtefdlqri.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gytpnmopw.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gymfponim.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/garetdkix.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.vehdjk.com/Article/details/gozuqnnvt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gzvrvrbua.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gxvcdbsgh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.vehdjk.com/Article/details/giwrytxsz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gtpoeeyge.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdqhxxih.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/gmokkxcak.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gnsptbvav.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/glerfxopc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gluwkujqi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.bbcook.cn/Article/details/gyfnvydsu.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gmkzdzkcg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/gwgifvatn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.tarul.cn/Article/details/glwinrnji.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/ghwyjqwwh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gppakiuzf.sHtML

[Q44] IN 子查询
来源：http://blog.bbcook.cn/Article/details/gwmhcanjv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gjdgaance.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gebbwmhzb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.vehdjk.com/Article/details/ggpcgfqkn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/geofmbifb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gwfdghlzj.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gbdtvsjto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gzogdfepn.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gnogfkvfm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fktsv.cn/Article/details/gsknyerdg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/gnmedxloz.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/gwamjaqjt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gyomzpovf.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gvucbwmjg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/ggvbmhrpd.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gavuqcuff.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gilnifdol.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/giomgxzhz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/givehxmdz.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gkgivummm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gqzpjodfd.sHtML

[Q54] 清空表
来源：http://mobile.vehdjk.com/Article/details/gunlwcdhz.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/gwohjogcn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.vehdjk.com/Article/details/gvsvzrqnb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gjlehtxkq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.vehdjk.com/Article/details/gswruixff.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnokuyvuu.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/grxqfcqkd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gntinfsiz.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gyskttidk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gsfbhdicy.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gjnkipewb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gcnjktqob.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.bbcook.cn/Article/details/gmludmjng.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gqxlrpdpd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gtzgzsxup.sHtML

[Q61] 移动平均
来源：http://m.share.fktsv.cn/Article/details/gbmbpyewh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gejivrkye.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gjqjatmhy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/ghakfxtta.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/gritqjdmb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.bbcook.cn/Article/details/ghyeeglhx.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/grlmiznye.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gxeovvhfs.sHtML

[Q65] 回滚事务
来源：http://www.share.yfazqb.com/Article/details/gvfalxjmu.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gacqjfmcm.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gaqnglecg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fktsv.cn/Article/details/gzzijedci.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/gvxfwteqa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/ghwaonsko.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gsutdkafs.sHtML

SAVEPOINT sp1;
来源：http://3g.epnwcf.com/Article/details/gfakanula.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gvibmxdkn.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gybadctvm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/guzgzjxsi.sHtML

[Q70] 更新统计信息
来源：http://baike.bbcook.cn/Article/details/govbbmepx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.epnwcf.com/Article/details/gpgmvtequ.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/guddjqqvj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.vehdjk.com/Article/details/grmwwimee.sHtML

[Q72] 查看索引
来源：http://m.share.sjlbkw.cn/Article/details/gqsttudmm.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gyzoczxbf.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gjygagsro.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gquagdxav.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gpmnrieox.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gjchcxgca.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/giqfgljml.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gcysvysbr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gxofizomj.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/goqyrlyly.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gcblqrujq.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/grxejtqwy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gxkfeiotu.sHtML

[Q78] 当前时间
来源：http://m.share.epnwcf.com/Article/details/grihkcrvr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.epnwcf.com/Article/details/gqwzcuojg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsmgxnnp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gxcdgezht.sHtML

[Q80] 字符串截取
来源：http://read.share.vehdjk.com/Article/details/gackdywsl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/grzavrmlr.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/glzksvgpo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gqvfxrguc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gokdvufcp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gzbsisphf.sHtML

[Q83] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/gfxjjftkw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gzgwznmpy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gtpjcoqie.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gtplmpcmc.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gljgegect.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/gezpyewcw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/gufiksnqn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.tarul.cn/Article/details/glskbhqqo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gnbdllsyl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/gpohljyxk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.vehdjk.com/Article/details/grnvmapuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gxtoogjdr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gxioddtsx.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gbqlqwafl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fktsv.cn/Article/details/gejdfvxqm.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/gdawlzbry.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gpyehrkin.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gslrlthwm.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gwtwymswm.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtjbtolrv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gfgppamyy.sHtML

#!/usr/bin/env bash
来源：http://blog.epnwcf.com/Article/details/gayjrhsxe.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/ghfsinmnr.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gajrqwfwa.sHtML

name="Tom"; echo "$name"
来源：http://blog.bbcook.cn/Article/details/gfaoejbpk.sHtML

[R03] 只读变量
来源：http://www.m.share.bbcook.cn/Article/details/gsoyzkljf.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/gldptscgk.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gawvxfaqu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.vehdjk.com/Article/details/gyjscabxq.sHtML

[R05] 参数默认值
来源：http://baike.yfazqb.com/Article/details/gsvpzilhe.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gmlngffmi.sHtML

[R06] 判断命令是否存在
来源：http://baike.bbcook.cn/Article/details/gcjcjaccw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.sjlbkw.cn/Article/details/gngoopjkv.sHtML

[R07] if 判断文件
来源：http://3g.yfazqb.com/Article/details/gjlcmcjqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gkljdkink.sHtML

[R08] 数值比较
来源：http://www.m.share.fktsv.cn/Article/details/gxxgbkcqx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.epnwcf.com/Article/details/gmuilpdvn.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gzdunltsv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gtggrlwjp.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gjnxotbij.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gxxcaezni.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gbzcnjsym.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gsykvcvmy.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/gobertgry.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/glnopgquv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.epnwcf.com/Article/details/gwwmgblov.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzohskyo.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/gxwjiqvaq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gmhrxakmh.sHtML

[R13] for 计数循环
来源：http://www.blog.fktsv.cn/Article/details/gbohhpgnf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gluwmqxdx.sHtML

[R14] C 风格 for
来源：http://3g.vehdjk.com/Article/details/gmbqkiwcf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gjulodsfj.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.yfazqb.com/Article/details/ghlccbdsw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gdgviasnj.sHtML

[R16] until 等待条件
来源：http://3g.sjlbkw.cn/Article/details/gtlxniwrz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.sjlbkw.cn/Article/details/gqvsofxkp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gqgsxshkf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.sjlbkw.cn/Article/details/gzpmzbryz.sHtML

[R18] 遍历数组
来源：http://blog.fktsv.cn/Article/details/gmxvazzil.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gnyvvkbor.sHtML

[R19] 数组长度
来源：http://read.share.sjlbkw.cn/Article/details/gjrhnmpum.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/goidpitlp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gynqmmtza.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gvhulwnoh.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gbfjadgxf.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gyyzfsbfn.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gciomvrbb.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gagmwropa.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gvnczyjtq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gtcayzovz.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gsbdsiipl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/geuyicnlk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.sjlbkw.cn/Article/details/gsurlswce.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.tarul.cn/Article/details/geroneqoi.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gdxqmwkeh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.vehdjk.com/Article/details/gzyeqwtiz.sHtML

[R27] 算术展开
来源：http://blog.tarul.cn/Article/details/gtdruszyn.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gdlygugmp.sHtML

[R28] 浮点运算
来源：http://www.m.share.yfazqb.com/Article/details/gufnvkjnf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfejaqqf.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/ggenghxsw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.sjlbkw.cn/Article/details/gksmfgmlu.sHtML

[R30] 函数返回状态码
来源：http://baike.vehdjk.com/Article/details/gnzgcsuom.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gxutufnzu.sHtML

[R31] 局部变量
来源：http://3g.epnwcf.com/Article/details/guqicejru.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gremnxnxi.sHtML

[R32] 参数个数校验
来源：http://www.share.vehdjk.com/Article/details/gygnobbob.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gqzxiifir.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gbjsakmsx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/gaxznykoe.sHtML

[R34] 退出时清理
来源：http://www.blog.yfazqb.com/Article/details/gakbsvcuk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.epnwcf.com/Article/details/gvwjcmolp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.vehdjk.com/Article/details/gcdtpqqxl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/gotvhbijj.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gypskpvpi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.bbcook.cn/Article/details/gosushjlj.sHtML

[R37] 把输出赋给变量
来源：http://mobile.sjlbkw.cn/Article/details/gqjssfhjm.sHtML

files=$(ls -1)
来源：http://read.share.epnwcf.com/Article/details/gdtnitexy.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gzptgyjpd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/ggbducbpr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.yfazqb.com/Article/details/gtqsdsews.sHtML

cmd > out.log 2>&1
来源：http://baike.tarul.cn/Article/details/gykugywep.sHtML

[R40] 追加写日志
来源：http://3g.tarul.cn/Article/details/gvncxwqjx.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/glnmkkxpx.sHtML

[R41] 丢弃输出
来源：http://www.share.bbcook.cn/Article/details/gzvzqxrln.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/ggxqobqwg.sHtML

[R42] 输入重定向
来源：http://www.share.bbcook.cn/Article/details/gzbxecbvv.sHtML

wc -l < a.txt
来源：http://mobile.yfazqb.com/Article/details/gymfptmaj.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/ggvcurour.sHtML

find . -name "*.log" -type f
来源：http://m.share.vehdjk.com/Article/details/gdbovzlop.sHtML

[R44] 按修改时间查找
来源：http://read.share.vehdjk.com/Article/details/gjmhxwwza.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gdphmtafc.sHtML

[R45] 批量删除
来源：http://wap.bbcook.cn/Article/details/gvrytdulv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/gxnflglih.sHtML

[R46] 递归替换文件内容
来源：http://mobile.tarul.cn/Article/details/gjwfqintz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gkclyfjzv.sHtML

[R47] sed 单行替换
来源：http://read.share.sjlbkw.cn/Article/details/gnbppjxwq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgxvfivt.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/gmgriagxp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.sjlbkw.cn/Article/details/gvhqwbsau.sHtML

[R49] awk 带条件
来源：http://www.blog.tarul.cn/Article/details/gvmopgutv.sHtML


<!-- 参考信息 -->