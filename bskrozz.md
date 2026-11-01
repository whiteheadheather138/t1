代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxykpgesm.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gjqlilcwz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.vehdjk.com/Article/details/gogmegluv.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gbrwpjclv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gdbqtdpyx.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gszqhowez.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gawcbqmai.sHtML

[Q08] 创建普通索引
来源：http://mobile.epnwcf.com/Article/details/gudcjflid.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gcurubuhz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.epnwcf.com/Article/details/gexqypury.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gryyknpwh.sHtML

[Q10] 插入单行
来源：http://www.m.share.sjlbkw.cn/Article/details/gdnlklmnk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gkgwhzznk.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gojueraxq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gwymqkfuy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gcctfqler.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/grroythuw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gduacfoit.sHtML

[Q13] 忽略重复插入
来源：http://3g.yfazqb.com/Article/details/gxmradgzz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gdbmmhcbx.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.vehdjk.com/Article/details/gznnztdpc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gauzfoaeq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.vehdjk.com/Article/details/gfdpvqder.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/gtyrfgxkp.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gxkpmzhos.sHtML

[Q16] 查询指定列
来源：http://3g.yfazqb.com/Article/details/gtafbjeww.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gkffeegsn.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gorkclkuq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gmuwltidj.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gznyfahtv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gzddiegvy.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gsenzehab.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gdjijxvpc.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gunbywyxp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/geukokgpn.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gssjnlrrv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gqlhwvvcy.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gmsewhbnx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gaaxthzvn.sHtML

[Q23] 分页
来源：http://wap.yfazqb.com/Article/details/gxislasox.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gldnhahhm.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gjbkcboqg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/gsltsgxwc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/grmdqmqud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gpoilacti.sHtML

[Q26] 计数
来源：http://www.m.share.fktsv.cn/Article/details/gcbhvnact.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/ggoedeiic.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gxcowhyno.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.yfazqb.com/Article/details/gupdkxzij.sHtML

[Q28] 求和与平均
来源：http://blog.tarul.cn/Article/details/gdevxoowy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gicliufup.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/ggmdwlqyk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.yfazqb.com/Article/details/grnsmabmg.sHtML

[Q30] 分组统计
来源：http://mobile.tarul.cn/Article/details/ghdzioxwx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/grpjktspp.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gcuecqnme.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fktsv.cn/Article/details/gkzraxjop.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gkzyczqdx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gilvmmnvf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gmkkahsxq.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gheqnhgvv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gdwqmthpp.sHtML

[Q34] 每组取第一条
来源：http://mobile.fktsv.cn/Article/details/gtohlfomk.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/gemzsqclt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/gkxbjvoqd.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gppohfyyn.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gxdcmzuci.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gapdvwuzr.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gpmwdyask.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gjexwpavi.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/gycvjrwac.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gerjavocf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/grbcinrxa.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gxlqiotvs.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gxlolwyim.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.bbcook.cn/Article/details/ggfeglljf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gonkykmqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gufccoyob.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gdjcuyzxl.sHtML

[Q41] 多表连接
来源：http://3g.yfazqb.com/Article/details/gswocojxl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/ggfgzgqje.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.epnwcf.com/Article/details/gprqtvntq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/gyeiugexl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gsztzozrp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.vehdjk.com/Article/details/gjdbfxsir.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/ghjxfmjvl.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gngohauaa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.bbcook.cn/Article/details/gtcwgfxff.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gwbsqtyjk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/gkpilwyhd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.yfazqb.com/Article/details/gakjdeosj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsvjbgtwo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/giwfeqpwh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gnbvxdnly.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gdspyfzrn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/giwmyaiel.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/grgqcqtyd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.sjlbkw.cn/Article/details/gbxuotwjy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gxtjrqtzt.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gqtaijqxi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/giupwnnzh.sHtML

[Q50] 批量更新
来源：http://baike.tarul.cn/Article/details/gblzqchrf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gycriromz.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gedgwxsok.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gwsyjethy.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gmznnuxry.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/govujxtic.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gloynblfm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gtxfkmvxu.sHtML

[Q54] 清空表
来源：http://mobile.bbcook.cn/Article/details/gyudecdsv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gkicffzmm.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/gowmbbzmv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gijvvyzto.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gvnoacsgt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gckcnxpky.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gtznpmqrc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/giahbspbb.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/gbyneikdt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gatogoikb.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gzmzalylz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/ghsiujwkd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/gxcqwwebc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gxzphryiz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gtrzjueae.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/gfbiyqeqf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gkpahhgdt.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gnqmyctey.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gzpwrvgpe.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gualypldv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gqlqcfpes.sHtML

[Q64] 提交事务
来源：http://www.blog.yfazqb.com/Article/details/gkheqtmqu.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gyqgkvqui.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/ghxxbwmpb.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gbckqersw.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/gqbdkfqbf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gvgiwjcbq.sHtML

[Q67] 设置隔离级别
来源：http://baike.epnwcf.com/Article/details/gcjcdjlus.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gymgwkkaq.sHtML

[Q68] 保存点
来源：http://mobile.bbcook.cn/Article/details/glfyvomcm.sHtML

SAVEPOINT sp1;
来源：http://mobile.fktsv.cn/Article/details/gotucifnc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gwxzjdora.sHtML

[Q69] 查看执行计划
来源：http://www.blog.yfazqb.com/Article/details/gggdchssj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/ghaolhjrt.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gyoiinpxc.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/glofudekd.sHtML

[Q71] 查看建表语句
来源：http://m.share.bbcook.cn/Article/details/gtanffzdr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/goqrrvdqt.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gdluutohc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gaouzqtlr.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/ghasnsiiy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/gywpnfpkd.sHtML

[Q74] 强制使用索引
来源：http://3g.sjlbkw.cn/Article/details/gdzjjqgvs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gmwpuyzxw.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gtargekhv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gufwseadw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.tarul.cn/Article/details/gumcssvux.sHtML

[Q76] 按天统计
来源：http://wap.yfazqb.com/Article/details/grqpjpkmc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.tarul.cn/Article/details/gbzsaheee.sHtML

[Q77] 时间加减
来源：http://www.share.yfazqb.com/Article/details/gfadllcdn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/geycoylvy.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/glvgnizro.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/gutzypxpz.sHtML

[Q79] 字符串拼接
来源：http://baike.sjlbkw.cn/Article/details/ggyhizyhw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gkqfpjbbv.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gnpedeksi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gnzgqtoue.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/gcsypghcq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gafrjlyhr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.vehdjk.com/Article/details/gxebvwddb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gtljnxvog.sHtML

[Q83] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/glmogvwhq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/glmzqzjov.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gyapbjsmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gbvcxkjcj.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/giolhfawz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.bbcook.cn/Article/details/glhyijqmc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gdiblrrom.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gyziwvrwy.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gqjvwfitd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/ghiprnrxv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/gwdihdrvl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gqvsautcv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/ggqbgdkfx.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gycmakxwk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtsjtmap.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gcpqavndp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gsbhohism.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnvdkzpgy.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/gkglfeavu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvhmcwtxv.sHtML

[R01] shebang 与严格模式
来源：http://mobile.vehdjk.com/Article/details/gakvgaejg.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/gsomfjqjk.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/gpspfdjid.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gixmirspi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/ghuxjnlad.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/graviqirw.sHtML

readonly PI=3.14
来源：http://mobile.tarul.cn/Article/details/gizyvztyv.sHtML

[R04] 位置参数
来源：http://read.share.vehdjk.com/Article/details/gshjwwemq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gvjsadzxa.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/ggojzmudz.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gonwveomu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/ghwvdcyry.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gwvnxrgtc.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gzjqhxsol.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/ghcpjfavs.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gorazvhnr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gshcbgugr.sHtML

[R09] 字符串比较
来源：http://m.share.vehdjk.com/Article/details/gdmhialzg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.vehdjk.com/Article/details/ggynoquvx.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/ganfeprhs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gcxzoaydq.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/gjzekxtcc.sHtML

case "$1" in
来源：http://m.share.sjlbkw.cn/Article/details/gupqbajwt.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gtoeiqoyg.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gfadosdvp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/ggxrwjbjz.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gqpsaojmc.sHtML

[R12] for 遍历文件
来源：http://www.share.tarul.cn/Article/details/gwqlswcch.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.tarul.cn/Article/details/gokggxpbt.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gzakhokqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gqzfqmqsq.sHtML

[R14] C 风格 for
来源：http://www.blog.vehdjk.com/Article/details/ghfudfzgp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.bbcook.cn/Article/details/gzstrxvlz.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/giwakemhx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fktsv.cn/Article/details/ghpxrmnnj.sHtML

[R16] until 等待条件
来源：http://read.share.sjlbkw.cn/Article/details/glczqppfv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.tarul.cn/Article/details/gauoghuak.sHtML

[R17] 数组定义与取值
来源：http://www.share.epnwcf.com/Article/details/gujgjblwq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.vehdjk.com/Article/details/guzcbqixe.sHtML

[R18] 遍历数组
来源：http://www.blog.bbcook.cn/Article/details/ghqsbmbvn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gksiarnjp.sHtML

[R19] 数组长度
来源：http://baike.sjlbkw.cn/Article/details/glsjthduk.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gtcpkeliu.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gwijukhaw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.sjlbkw.cn/Article/details/gopnflmta.sHtML

[R21] 字符串长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwluxdse.sHtML

echo "${#s}"
来源：http://3g.fktsv.cn/Article/details/gtvalartk.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gfpnzztdr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gwuwtybve.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/grhapzzyq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.yfazqb.com/Article/details/gqzohqmxr.sHtML

[R24] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gjhmnjzpa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gzygbbyuf.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/gqlujtphh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.tarul.cn/Article/details/ggrkfpgbo.sHtML

[R26] 命令替换
来源：http://m.share.yfazqb.com/Article/details/gcnrkowtb.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.tarul.cn/Article/details/gouvygrhk.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gboldzije.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/gnqaqysnn.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gpgyqjbge.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gruvesyzs.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/ganowemba.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gbtgqcetl.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/golnzckri.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.sjlbkw.cn/Article/details/gupunrojt.sHtML

[R31] 局部变量
来源：http://www.share.bbcook.cn/Article/details/gidnxxbup.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.epnwcf.com/Article/details/gbddtubjo.sHtML

[R32] 参数个数校验
来源：http://3g.yfazqb.com/Article/details/gsjcflzvi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gwzbrwhrb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/ggntdvrsn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.yfazqb.com/Article/details/gyyfsdiwf.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/gxhnznlub.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.bbcook.cn/Article/details/grxbsksiq.sHtML

[R35] 后台执行并等待
来源：http://www.share.yfazqb.com/Article/details/gcunsmpts.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/gdrmelgia.sHtML

[R36] 并发执行多个任务
来源：http://wap.epnwcf.com/Article/details/gprzufyjs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gbrieodxj.sHtML

[R37] 把输出赋给变量
来源：http://read.share.epnwcf.com/Article/details/gqmzoupaw.sHtML

files=$(ls -1)
来源：http://wap.tarul.cn/Article/details/gyawfeoye.sHtML

[R38] 管道串联
来源：http://read.share.bbcook.cn/Article/details/gdtmvesmg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.sjlbkw.cn/Article/details/gdqpbpbik.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gatjnptbv.sHtML

cmd > out.log 2>&1
来源：http://www.share.tarul.cn/Article/details/gxyhgijjm.sHtML

[R40] 追加写日志
来源：http://mobile.bbcook.cn/Article/details/gexkudwoc.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gdmeqrcxn.sHtML

[R41] 丢弃输出
来源：http://baike.epnwcf.com/Article/details/gaqbpqctq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.epnwcf.com/Article/details/gukhqmmvw.sHtML

[R42] 输入重定向
来源：http://baike.fktsv.cn/Article/details/garjhhhrs.sHtML

wc -l < a.txt
来源：http://baike.sjlbkw.cn/Article/details/gkhtztlgr.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gpkrsgqfh.sHtML

find . -name "*.log" -type f
来源：http://www.share.yfazqb.com/Article/details/gssgiionn.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/gdgmjljwi.sHtML

find . -mtime -7 -type f
来源：http://wap.yfazqb.com/Article/details/gfxhxgdlz.sHtML

[R45] 批量删除
来源：http://wap.epnwcf.com/Article/details/gmdpxwbcr.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.bbcook.cn/Article/details/gjglkrvov.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/guwvxynhf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.yfazqb.com/Article/details/grxbkqfwn.sHtML

[R47] sed 单行替换
来源：http://blog.bbcook.cn/Article/details/grgbazosc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.yfazqb.com/Article/details/gftzngqci.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/grsaayhsr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gvooiydet.sHtML

[R49] awk 带条件
来源：http://3g.fktsv.cn/Article/details/grrnouzwd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.vehdjk.com/Article/details/gghqkclzb.sHtML

[R50] awk 求和
来源：http://3g.fktsv.cn/Article/details/gixlatiti.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.bbcook.cn/Article/details/ghirnfdne.sHtML

[R51] 排序去重取前几
来源：http://blog.tarul.cn/Article/details/gqjqwcuyi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/guhjrgkzx.sHtML

[R52] 统计行数
来源：http://mobile.tarul.cn/Article/details/gstjlvfov.sHtML

wc -l a.txt
来源：http://blog.epnwcf.com/Article/details/gszlvvozj.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.yfazqb.com/Article/details/grehsjksy.sHtML


<!-- 参考信息 -->