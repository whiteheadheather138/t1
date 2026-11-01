代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://3g.yfazqb.com/Article/details/gduxueptv.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/grzydsjrw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gncuvvgwk.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gfjbefdvv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/grqajfxpc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/glusougnv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gzwykegmb.sHtML

[Q10] 插入单行
来源：http://www.blog.sjlbkw.cn/Article/details/gjmptxqgp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.bbcook.cn/Article/details/grpxnsahb.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/gienyvjkl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gshicfcxb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gzfxfpolf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.tarul.cn/Article/details/gqoatrdnk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.tarul.cn/Article/details/gopiczdgi.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.tarul.cn/Article/details/gzokvpwyc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fktsv.cn/Article/details/gqeeayuoj.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gvpppfobn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gstgmlepc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/giixbwjag.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gntxieyvu.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/gzldnovxq.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/gakbkqbim.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gblaiahkn.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/gqtkxbeab.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/gyclaetuz.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gnrmnzspv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gvdopfcmq.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gyboccduh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gfpxzsevo.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gmighcdde.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/goxivwela.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gbpyuoddc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.bbcook.cn/Article/details/gjpakkwae.sHtML

[Q22] 排序
来源：http://read.share.tarul.cn/Article/details/gyxrpjtxl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/ggsxtruqr.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/geuvrgvno.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gfyvnrfqy.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/ghrfioamh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gigxlvmyl.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gmzxbgfaa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gqntnkbtf.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gyjfutdnf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkdqjrbtt.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/ghxwrptib.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gtjwnchic.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gmrstmlgg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gtaakzplo.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gzbnytmrc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/gudsdhpce.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/ggbjfkzje.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gwonphzwa.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gjselgrbu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gjwvbgedj.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gjrnkklkp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gekalppmf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fktsv.cn/Article/details/gkpfnvzps.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/gkrbdswvk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.epnwcf.com/Article/details/gfpgpyxmh.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gpjwlloko.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/gmmwvcbjq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gcufdwpdz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/gsxdqzimd.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gwkssfpcg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/glxeciymz.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/ghwcobzkh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gqrkyzieo.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/gmkqeefwz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gpmkwgoqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gayvuppaz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gsqyhunlu.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/ghwpnjkao.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gdcxehzzh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gjjanlifs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/gjhteftnr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/ghzohqsjt.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gdzvnqidn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/guectoiqe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/gyokvrpuj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gigjhtdwf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.tarul.cn/Article/details/gikcoghzb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.tarul.cn/Article/details/gdyyvivsn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gajsdycgp.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gcwmkdawe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.epnwcf.com/Article/details/gairdtnym.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gttbdapxd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gmmvtyrpl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gliwptgia.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gyoefwzzf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fktsv.cn/Article/details/gxbfgfyrp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gggdrvyxt.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/gejbzoojp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gibjszzoa.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fktsv.cn/Article/details/ghnbkawyq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/galzornwo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gdroxvnka.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/gubozdhzj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gvqtcchiq.sHtML

[Q50] 批量更新
来源：http://mobile.fktsv.cn/Article/details/gfjksgngb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gezuiuohc.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gelxbewva.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/ggnkykwop.sHtML

[Q52] 删除指定行
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqdgxmqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gasabkduv.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gdtblgiyi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.epnwcf.com/Article/details/guohcowos.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gvmihebpd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gvplrxlif.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gbjvgxozu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gigztcayr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gxbkmxqaf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gjidiooua.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gowgswapq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/ghtfpekxr.sHtML

[Q58] 累计求和
来源：http://m.share.tarul.cn/Article/details/gyvcrfitn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gcfydvows.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/ghaczwcyv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/giytzqaqh.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/gajircjos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gyggwqfmn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gkkquzzjw.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/gukndugur.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/guucmaxlr.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/ganacdlqw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gopbwqhpw.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gdcbosmcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.vehdjk.com/Article/details/gnbwzsvhn.sHtML

[Q64] 提交事务
来源：http://wap.fktsv.cn/Article/details/godpcvsln.sHtML

COMMIT;
来源：http://www.m.share.fktsv.cn/Article/details/gatepchxj.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gjyoghjrb.sHtML

ROLLBACK;
来源：http://wap.fktsv.cn/Article/details/gogwonomj.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gorgjzcbi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.sjlbkw.cn/Article/details/gkjcshqce.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gyalytyls.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.bbcook.cn/Article/details/gbzbpokhn.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gbttsijvj.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gpecnlizx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/gexkffqnn.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/ggnxqhzwc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/gpbnescre.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/gxlhlcovt.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gbpbyifib.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gujejrcwd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gmwytamxb.sHtML

[Q72] 查看索引
来源：http://baike.bbcook.cn/Article/details/gghuwbqvd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/gqgjxkwkf.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gozzetagx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gezpznrna.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gtdjczhmb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gwetapsvq.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gffjbafed.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gxacrbjqh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/grmmfbbpw.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gllralfyr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gafdecouo.sHtML

[Q77] 时间加减
来源：http://mobile.tarul.cn/Article/details/gsstihuvr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.bbcook.cn/Article/details/grjgiegdh.sHtML

[Q78] 当前时间
来源：http://3g.vehdjk.com/Article/details/ggehhvxwj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gtagxdqoc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gdbffgslv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/gxxabetox.sHtML

[Q80] 字符串截取
来源：http://www.blog.fktsv.cn/Article/details/gvqhurebs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gveksbpef.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/gecwsutgv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gmczlbyao.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gzdpxokke.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gtfhghewd.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gfohivmlj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/ggpomykyt.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/galejeltc.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gogagkjgd.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gotqyyckz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gubyqfqip.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.bbcook.cn/Article/details/gqzzdsouu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gpyfhlaqr.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/ghrlnpeyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gyvffipra.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gvxlmjwke.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.epnwcf.com/Article/details/gbimsjrdx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/glynjfqql.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/giqpyvquo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gzrfdhuxr.sHtML

[Q90] 生成序号列
来源：http://blog.tarul.cn/Article/details/gexrnstmy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fktsv.cn/Article/details/gcxkueqja.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbnntcdvo.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/grcnjqddc.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpkdxlcch.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/gieifpivm.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/ggkyfzzqo.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gwknxxwgh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gnkujkjij.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsmqyzsv.sHtML

[R03] 只读变量
来源：http://baike.yfazqb.com/Article/details/gzfowyfkj.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gpylietcn.sHtML

[R04] 位置参数
来源：http://mobile.sjlbkw.cn/Article/details/gpspczlab.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gmgspxxdx.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/ggpfvcqhd.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/gidotbkze.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gkwfmxcfx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/guxdkjdts.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/gjzezruva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.epnwcf.com/Article/details/gzbarzcxi.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gqnkpsqzk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.epnwcf.com/Article/details/ggpyppjaj.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gixnnqera.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gaulfxlaw.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gstimgcdx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.yfazqb.com/Article/details/gpbohhori.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gwceffrej.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/ghojxysfx.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gyxtcaeha.sHtML

stop)  echo "停止" ;;
来源：http://read.share.yfazqb.com/Article/details/gbjhiwrvi.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gevahhivo.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/grobncjds.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gvknazdna.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gvnklnudl.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gztyecxtx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/glpckvbvt.sHtML

[R14] C 风格 for
来源：http://wap.tarul.cn/Article/details/gfleuxqcc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gosbxazkn.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gmabvjitc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fktsv.cn/Article/details/gcwzahqrm.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/gkoqgksgt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.sjlbkw.cn/Article/details/gytbqkuxp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.sjlbkw.cn/Article/details/gwhpoujww.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.tarul.cn/Article/details/gyiqegspo.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gjqqztiuo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gzinljuqz.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gymeayjuz.sHtML

echo "${#arr[@]}"
来源：http://blog.tarul.cn/Article/details/gigeemgzi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gtlornmtu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.vehdjk.com/Article/details/goommdhij.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gwkhquush.sHtML

echo "${#s}"
来源：http://wap.vehdjk.com/Article/details/ghdxveldn.sHtML

[R22] 截取子串
来源：http://www.share.bbcook.cn/Article/details/gbjoutxyy.sHtML

echo "${s:0:5}"
来源：http://wap.epnwcf.com/Article/details/gnoxixsvd.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/grmunvxcq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gswxczfyh.sHtML

[R24] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gtnjherse.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/ghvbgftzl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fktsv.cn/Article/details/gupsxowoy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.vehdjk.com/Article/details/grcphnzpu.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gpbflrvjt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gfqndjswi.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/gawvvmdfs.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gruzvrimh.sHtML

[R28] 浮点运算
来源：http://www.share.yfazqb.com/Article/details/gzpkimbsc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.bbcook.cn/Article/details/gnkzovxxj.sHtML

[R29] 定义函数
来源：http://blog.vehdjk.com/Article/details/gpwtgttnf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/glhhlpbyu.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gpkujbjje.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.tarul.cn/Article/details/gxycryhik.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gpmhfxvmx.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fktsv.cn/Article/details/gzexctgid.sHtML

[R32] 参数个数校验
来源：http://mobile.yfazqb.com/Article/details/grekfcysn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gwsnnvvrr.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.tarul.cn/Article/details/glokuuxwx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.tarul.cn/Article/details/gglblznth.sHtML

[R34] 退出时清理
来源：http://www.m.share.fktsv.cn/Article/details/gxpxaaxhx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.epnwcf.com/Article/details/gyuiatren.sHtML

[R35] 后台执行并等待
来源：http://3g.epnwcf.com/Article/details/gejaldrfh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.tarul.cn/Article/details/gxwxwtups.sHtML

[R36] 并发执行多个任务
来源：http://3g.vehdjk.com/Article/details/grvvgqnhd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gzgkhaerk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.tarul.cn/Article/details/guexvnqoh.sHtML

files=$(ls -1)
来源：http://m.share.yfazqb.com/Article/details/ghfbwqkhl.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/ghkbxzwmc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gjfjnpnow.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.sjlbkw.cn/Article/details/gkgpqykat.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/gghxwscze.sHtML

[R40] 追加写日志
来源：http://m.share.fktsv.cn/Article/details/gyqtdkxwr.sHtML

echo "log" >> out.log
来源：http://read.share.tarul.cn/Article/details/gyjqcfysx.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gtkjgnufy.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.tarul.cn/Article/details/gqwlzwkhq.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/gspenxleb.sHtML

wc -l < a.txt
来源：http://m.share.vehdjk.com/Article/details/guvoitfxd.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gmigokhoo.sHtML

find . -name "*.log" -type f
来源：http://wap.vehdjk.com/Article/details/gbehelshi.sHtML

[R44] 按修改时间查找
来源：http://www.share.tarul.cn/Article/details/gcfcepvvp.sHtML

find . -mtime -7 -type f
来源：http://baike.sjlbkw.cn/Article/details/gksrvkbhz.sHtML

[R45] 批量删除
来源：http://www.blog.yfazqb.com/Article/details/gplnecnmq.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.bbcook.cn/Article/details/gfjvjhuda.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/gjtrmskbp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.yfazqb.com/Article/details/gtwaspkeq.sHtML

[R47] sed 单行替换
来源：http://blog.yfazqb.com/Article/details/gyuxjvpox.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.tarul.cn/Article/details/ghpayksmp.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gztnduluj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.epnwcf.com/Article/details/gyzocykdz.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gfosahwqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.yfazqb.com/Article/details/gddkcwyym.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gjcgfmidx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gpxeojchy.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/gtzyemaga.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.tarul.cn/Article/details/gclmhpsjb.sHtML

[R52] 统计行数
来源：http://read.share.epnwcf.com/Article/details/glwhancyo.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/gyqppvpki.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fktsv.cn/Article/details/ggwrchokl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/gikvwisrc.sHtML

[R54] 比较两个文件
来源：http://blog.yfazqb.com/Article/details/gcdzbcynm.sHtML

diff a.txt b.txt
来源：http://www.share.tarul.cn/Article/details/gjmxcpdmg.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/gluztyqxa.sHtML


<!-- 参考信息 -->