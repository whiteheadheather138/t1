代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gfdbnkqhj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/glrzlugsq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/glbfykvzs.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gmifnetqc.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpnhovcwd.sHtML

[Q16] 查询指定列
来源：http://3g.fktsv.cn/Article/details/gurpzrleu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gkoupzmti.sHtML

[Q17] 条件查询
来源：http://wap.fktsv.cn/Article/details/gtamsdonb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/grcxmusos.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/goqoegvmg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gswbwyawf.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/goornoxqi.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gsouyiyfc.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/gjsdxisxb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gcrvchvwd.sHtML

[Q21] 空值判断
来源：http://www.m.share.yfazqb.com/Article/details/gpjpjghtp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gvffevssx.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gswgajxxi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/ghjvtmcst.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/ggmeeicfb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fktsv.cn/Article/details/gdymbjgiw.sHtML

[Q24] 去重
来源：http://www.blog.sjlbkw.cn/Article/details/gdxxiubsk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/glybmutxt.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/goavvdsxj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/guxnxpujt.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gpgimtjxt.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fktsv.cn/Article/details/gywypyzji.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gvdotrkpu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gsejmhqxf.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gvdnipqdf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/goywsdomu.sHtML

[Q29] 最大最小值
来源：http://blog.vehdjk.com/Article/details/gokpobfwj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gdqdmidnx.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/gzzdtfqqc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gdumbobsa.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/guodkasiz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gqfmflwdf.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gycccoypi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gmtszlzer.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.vehdjk.com/Article/details/gevhtoeka.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/geqeetybq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gphcbdnqw.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/giljjesww.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gpqzgbpch.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/ghgffswkm.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gnanrxlyl.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/gkixwpttx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gznnhmeje.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/guwydjwce.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/ggoqnezjb.sHtML

[Q37] 右连接
来源：http://mobile.bbcook.cn/Article/details/gwarqlxue.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/guzpxaehk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gzojzwuko.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gcpklotud.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gkcautnql.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gtrcseegt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.tarul.cn/Article/details/gbdpgqbjo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fktsv.cn/Article/details/gprdunmia.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gyjcvquhi.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/ggegkaeii.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gvkslvnwo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gaqwwardi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gqakabciv.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gslxerhlf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.sjlbkw.cn/Article/details/gomsusadf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/gpawdnirb.sHtML

[Q43] 标量子查询
来源：http://3g.fktsv.cn/Article/details/gzgstgjlc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gxmvjwdpo.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gikqadwaa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gziddgfpu.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/ghkbupkqp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gbzubsylg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gffqnlusz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/grpczgoec.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gfrqgdfze.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gwmsfgseh.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.sjlbkw.cn/Article/details/ggjiklruf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gsueuleoz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fktsv.cn/Article/details/gruwwtrxu.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gdnxdtjep.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/grfnihxkj.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/glfgpaysz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gjstlioic.sHtML

[Q51] 用子查询更新
来源：http://m.share.bbcook.cn/Article/details/gfkioudsm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gtchvwkwe.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/giidsyywp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/geekkldgo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.sjlbkw.cn/Article/details/gonrevkuj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.vehdjk.com/Article/details/gabttcsqx.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gcnwjkxsv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gektvwnrv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/gkupssade.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gwwpdhkka.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/gygobfxio.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gsjybozat.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gxtqwdvvf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gjimemgjs.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gsjvumqnj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/glyzgdqqr.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gkjhkgzop.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/ghecnyknf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.epnwcf.com/Article/details/grrgorfnt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.bbcook.cn/Article/details/ghuwowrtn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gddkzzlkp.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gwqfsfeok.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gzyvcsmle.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/gdeylcigk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gmxjvmven.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/gurykpaap.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/gjiavsrqd.sHtML

[Q64] 提交事务
来源：http://m.share.epnwcf.com/Article/details/gdmawxrcc.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gydrtixiz.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/ghbnehtff.sHtML

ROLLBACK;
来源：http://read.share.sjlbkw.cn/Article/details/goskhrihi.sHtML

[Q66] 行锁查询
来源：http://m.share.yfazqb.com/Article/details/gngqjyfwx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.yfazqb.com/Article/details/ghvcjvzxy.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gcwbqbrjr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gwchrievc.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gbxooepti.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/gpulxldyv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.epnwcf.com/Article/details/gqfpmyoqb.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gintodenk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gxcdtmfos.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/gmlkvfmmj.sHtML

ANALYZE TABLE users;
来源：http://read.share.fktsv.cn/Article/details/gtbvyugps.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.tarul.cn/Article/details/gtvxgmiiz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gbxieciyz.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gjedwroid.sHtML

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/gmhviohbu.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gqmzasapa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gamibfngx.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gqtbdclar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.epnwcf.com/Article/details/gszpqlrba.sHtML

[Q75] 日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gzhayqcjj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gzvrylyjp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gmdmsvgaa.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gtgkbnsnn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gmxykrozp.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gkjqxmomz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gqyftaulm.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gomligqpw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/gvggccmda.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gafkbdpgc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/ggcuwgwtb.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gyzdfvyxb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/gqjzlfrhh.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/ggeymusiq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gtehobuqf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fktsv.cn/Article/details/gknjcdqxk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gapmjvind.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gthtcdbgw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gxvsirygw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gilgtjnvv.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gscjhgagh.sHtML

[Q85] 数值取整
来源：http://www.m.share.fktsv.cn/Article/details/gdbatnvyd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gugenkidi.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/gpptzcreq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gjffagxnb.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fktsv.cn/Article/details/gndjswdgf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/gtcemervh.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gcmoxvwpj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/grypeobxu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwzkfkaxd.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/genlzhlhr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gtyxpffly.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gmhdrrrkc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gqwreezur.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/galzigwft.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gmmuanysv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gaujfysff.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/ghzzkfatn.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/ghaukmxaj.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gwibuipbl.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gqyiarvor.sHtML

name="Tom"; echo "$name"
来源：http://wap.sjlbkw.cn/Article/details/gluxznmhi.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gxhksmfkb.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/ggnquzmdg.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gvjsyoyip.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.vehdjk.com/Article/details/ginpfdygx.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/glnyhemud.sHtML

name="${1:-default}"
来源：http://m.share.vehdjk.com/Article/details/gshdnmday.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/gyitvhyoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gzztivtkw.sHtML

[R07] if 判断文件
来源：http://3g.epnwcf.com/Article/details/glupntgwe.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/gflmixmtr.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/glqmwsznp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gdesujtvm.sHtML

[R09] 字符串比较
来源：http://baike.sjlbkw.cn/Article/details/gdfigwnpg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fktsv.cn/Article/details/gaizbqyxs.sHtML

[R10] 正则匹配
来源：http://wap.vehdjk.com/Article/details/guizxfvmf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fktsv.cn/Article/details/gvaxxkiry.sHtML

[R11] case 多分支
来源：http://www.blog.fktsv.cn/Article/details/gxvtxokjg.sHtML

case "$1" in
来源：http://mobile.yfazqb.com/Article/details/gqctthpbe.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gftugrjet.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fktsv.cn/Article/details/gfjzyhiwy.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gsszfnovc.sHtML

esac
来源：http://baike.vehdjk.com/Article/details/gndwdqqmz.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gvsbtwsdr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fktsv.cn/Article/details/gguhyeuim.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gnfyfneuq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gojvqidsm.sHtML

[R14] C 风格 for
来源：http://www.m.share.epnwcf.com/Article/details/gcjqopcht.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gthheitfi.sHtML

[R15] while 逐行读文件
来源：http://3g.fktsv.cn/Article/details/gaoespkhq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/gqyqvhuex.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gohygpbex.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.epnwcf.com/Article/details/ghodmkxak.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/gcgdcjfiz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gymiqqchb.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gowywmpgn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.tarul.cn/Article/details/gcwgyocuw.sHtML

[R19] 数组长度
来源：http://m.share.epnwcf.com/Article/details/gnhcagquw.sHtML

echo "${#arr[@]}"
来源：http://www.share.yfazqb.com/Article/details/ggpfuiyxl.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/gahcasgee.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.yfazqb.com/Article/details/garjofebv.sHtML

[R21] 字符串长度
来源：http://www.m.share.epnwcf.com/Article/details/gatfgworu.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/grwbxfcmn.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gcqvkmqmb.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gzczdcwfh.sHtML

[R23] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gdxwlaztk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gswjveyrz.sHtML

[R24] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gxzplairp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.epnwcf.com/Article/details/gddxrheaw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gcpjtjaor.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.bbcook.cn/Article/details/ggjgvqlen.sHtML

[R26] 命令替换
来源：http://read.share.yfazqb.com/Article/details/gkngdtilq.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/glwkzqlhx.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gbhplzelo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.bbcook.cn/Article/details/gswyupyzb.sHtML

[R28] 浮点运算
来源：http://baike.yfazqb.com/Article/details/gdyehnazn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gjvnwksgf.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gbmtgrzpw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/gqcrmdrag.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/gomlaitwt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.vehdjk.com/Article/details/gmmcmfdxq.sHtML

[R31] 局部变量
来源：http://www.share.yfazqb.com/Article/details/gedbajiqz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/gypqbkold.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/gnxewgnda.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/grbbkgdni.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.vehdjk.com/Article/details/gnuolebmi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.vehdjk.com/Article/details/gaszianeg.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/ggseplldy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.yfazqb.com/Article/details/gpsgfcekt.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/ghlhbfrwp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.epnwcf.com/Article/details/gvfwckdjf.sHtML

[R36] 并发执行多个任务
来源：http://baike.bbcook.cn/Article/details/gbbpguipm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.vehdjk.com/Article/details/gmetwivfz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gzyibnkhw.sHtML

files=$(ls -1)
来源：http://blog.yfazqb.com/Article/details/gqqkwezlf.sHtML

[R38] 管道串联
来源：http://www.blog.sjlbkw.cn/Article/details/gtmectimj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gqfnmjsgq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.vehdjk.com/Article/details/gllyevszh.sHtML

cmd > out.log 2>&1
来源：http://m.share.fktsv.cn/Article/details/galozxtpg.sHtML

[R40] 追加写日志
来源：http://baike.epnwcf.com/Article/details/ghdxuuecj.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gmagonmiz.sHtML

[R41] 丢弃输出
来源：http://m.share.yfazqb.com/Article/details/gqsupiijj.sHtML

cmd >/dev/null 2>&1
来源：http://baike.bbcook.cn/Article/details/gzpakkkgs.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gwopdybcw.sHtML

wc -l < a.txt
来源：http://3g.vehdjk.com/Article/details/gujopalxs.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/glknnqclg.sHtML

find . -name "*.log" -type f
来源：http://read.share.tarul.cn/Article/details/gwpdwmskx.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gcmxirutb.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gfxvsfbpd.sHtML

[R45] 批量删除
来源：http://blog.epnwcf.com/Article/details/gxnoutfay.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.vehdjk.com/Article/details/gkwcgtiza.sHtML

[R46] 递归替换文件内容
来源：http://baike.tarul.cn/Article/details/gueyvkwqw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.tarul.cn/Article/details/gjsyvmuxl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.yfazqb.com/Article/details/gqosbuolq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.tarul.cn/Article/details/gbrmjsdpj.sHtML

[R48] awk 取指定列
来源：http://baike.tarul.cn/Article/details/gtspfvfdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gdotkukwi.sHtML

[R49] awk 带条件
来源：http://www.share.sjlbkw.cn/Article/details/gzkvtgunv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.bbcook.cn/Article/details/gpkvdwlyj.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gbapdoewe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.tarul.cn/Article/details/gfaqvgxeb.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/gvhgoqpnv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.vehdjk.com/Article/details/glyigrdkr.sHtML

[R52] 统计行数
来源：http://blog.vehdjk.com/Article/details/gttvksyhv.sHtML

wc -l a.txt
来源：http://www.share.yfazqb.com/Article/details/ghuouqypy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.epnwcf.com/Article/details/grbkxpsns.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fktsv.cn/Article/details/guzqhwabq.sHtML

[R54] 比较两个文件
来源：http://m.share.vehdjk.com/Article/details/ghklegcbv.sHtML

diff a.txt b.txt
来源：http://read.share.fktsv.cn/Article/details/ghmaizlvu.sHtML

[R55] 压缩与解压
来源：http://wap.fktsv.cn/Article/details/gyxpkmctk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.vehdjk.com/Article/details/gzkjiglin.sHtML

[R56] 远程拷贝
来源：http://3g.tarul.cn/Article/details/gdvzvoqya.sHtML

scp file user@host:/path/
来源：http://www.share.fktsv.cn/Article/details/glbsudmuq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmmslfzx.sHtML

ssh user@host 'uptime'
来源：http://wap.sjlbkw.cn/Article/details/gjsdmqcnh.sHtML

[R58] 下载文件
来源：http://3g.tarul.cn/Article/details/glzvwtagr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.vehdjk.com/Article/details/gozpgjacr.sHtML

[R59] 发 POST JSON
来源：http://www.share.tarul.cn/Article/details/gypcmzjjp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.bbcook.cn/Article/details/giakwmazv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/glhankjgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/gjlfdhchc.sHtML

[R61] 磁盘占用
来源：http://www.share.sjlbkw.cn/Article/details/gmraqncld.sHtML

df -h;  du -sh *
来源：http://blog.sjlbkw.cn/Article/details/gvrcmcabx.sHtML

[R62] 找最占空间的文件
来源：http://read.share.sjlbkw.cn/Article/details/gwrlgsdqy.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.vehdjk.com/Article/details/gpxagphxq.sHtML

[R63] 内存与进程
来源：http://mobile.bbcook.cn/Article/details/gqqbpkyif.sHtML


<!-- 参考信息 -->