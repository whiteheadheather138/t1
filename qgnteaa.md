代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gdzmwwifv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gusjefcod.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gnxcvzxhs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/gjoemgjrt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/grujaixmy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gtcsxqlaa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gbfbeqssi.sHtML

[Q15] 查询全部
来源：http://m.share.fktsv.cn/Article/details/gmoueihfh.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gafxnjnph.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gsefkonfd.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/ggirrbaej.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gekcyptoq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/giwmovnth.sHtML

[Q18] 模糊匹配
来源：http://blog.vehdjk.com/Article/details/gmnqyvgdc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/ghqohlwfw.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gnxrtpafu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gwrkxascs.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gohkvbvpi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gptheqysm.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/gvqffzjzb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gbwjiybxp.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/gjrjvjzoz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/guslvgjic.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gryihoxal.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gvhtfojgx.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gmsbzzgld.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/ghymvqtch.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/guuoijhwj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/gwynmxfjv.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/gghawsire.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvhekzbvd.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gqiqlxqzw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gftkwtzpt.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gskpzhdig.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gghdlvpmc.sHtML

[Q29] 最大最小值
来源：http://3g.fktsv.cn/Article/details/ghoxrfykm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/geyzkechj.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gqeygcxww.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gkimjlecy.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gmrkrlgoq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/gaitumotx.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gryndilke.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gmebedkck.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/gupgeucoi.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/gcjwvgcuh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/getrcfafp.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gpavuypbz.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/grfbzcujk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gpvptzgpj.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/gqpvfkhrt.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/ghanebsqw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gwaddopzq.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gjjumkgqx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gxcjokewn.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/ggwrmldcr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gdzeyxgeq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/glvkhpwbr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gqvjbpqxn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gwzuhynjh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gkwmreqst.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.epnwcf.com/Article/details/gnrggyozy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gcjrzuflk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gbstofmlo.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gehpsyhow.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/gjgzzoaoh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/gzwktoygb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gnrldnsor.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gficqqcqz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gvderwwfc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/grtnewlvt.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gvuxlagod.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gmcrlknhx.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gxufrbvik.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gbsonbszx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gqvwnrqzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gyuddfpsn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/glxclznbr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gazoaxwmd.sHtML

[Q47] 与平均值比较
来源：http://read.share.tarul.cn/Article/details/gcrwczxuv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gvrviqman.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gjswruopp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gchfxnhag.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/gropyuivi.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/gjjtbczxa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/glpnhbebo.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gshrkgmqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/grnkxmmvg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gllzcsgyx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/grpkooacx.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gmjxesoty.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/gsnghbzak.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gfrnlzamt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gpqthrqvz.sHtML

[Q54] 清空表
来源：http://www.share.sjlbkw.cn/Article/details/gqlnoznjg.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gymkpdpxm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.yfazqb.com/Article/details/guasxmnva.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/guotycnib.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gmxaxabvc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gwslpdeop.sHtML

[Q57] 行号
来源：http://m.share.epnwcf.com/Article/details/gbrtiymbx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gbmiepyeu.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/getcglris.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gyjqkzzlm.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gadzfpjov.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gphilghjc.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.epnwcf.com/Article/details/gdmayyqxl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gicqdcmwg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gzadmuibu.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/gfnhskncx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gvaelmlrr.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/geudkrrmv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gqzsqnhwz.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gdjumejlb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/ggdwybvfd.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gudtancfg.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gxjhyuldk.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/gzljhowiu.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gjxenwgqe.sHtML

[Q66] 行锁查询
来源：http://www.m.share.vehdjk.com/Article/details/grhcpapwr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.vehdjk.com/Article/details/gokostmft.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gsminpmkg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gwtcqerdp.sHtML

[Q68] 保存点
来源：http://m.share.fktsv.cn/Article/details/gyfujkmmc.sHtML

SAVEPOINT sp1;
来源：http://mobile.yfazqb.com/Article/details/gcgohnkns.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/gplsbxkco.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/gzduwxfdl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gqxgghqxk.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gqbsqwfna.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/ghnvadjwe.sHtML

[Q71] 查看建表语句
来源：http://baike.epnwcf.com/Article/details/guciypaxy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.bbcook.cn/Article/details/gnbgiwkdw.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gfcusmgsx.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/giirhyuow.sHtML

[Q73] 查看表状态
来源：http://baike.bbcook.cn/Article/details/goigtrlyn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/gawgcmrqc.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gngjeunuh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gahdmhqsk.sHtML

[Q75] 日期格式化
来源：http://3g.sjlbkw.cn/Article/details/gfhhtywix.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gdygyrrpo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.yfazqb.com/Article/details/gzbdepsut.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gbauzpgus.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.epnwcf.com/Article/details/gujkkatoh.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/gxmqsgizv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.epnwcf.com/Article/details/gulwltrzj.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gudbtfujv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gzjllqsto.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gedjonauz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.sjlbkw.cn/Article/details/gowjxqfeb.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gpydfmmrq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ggfhbddri.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gjbjfidey.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gvbkyuxhh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/gtrtpgyeb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gjkjkdqfg.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/grujtrlih.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gporvygdt.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gnfgeksnp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdvxlwchm.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gqgoejutd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gekntznlg.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fktsv.cn/Article/details/gwgyvsacn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/gcxaojuhw.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.epnwcf.com/Article/details/gktlcbpjx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gzjgosegv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gergdkcvw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gfkhtxneh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gbwnsmzsd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gxyvxvojs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gixhwivgj.sHtML

[Q90] 生成序号列
来源：http://www.blog.fktsv.cn/Article/details/gttajjmod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.vehdjk.com/Article/details/gohfcxbqw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/guxhkgrzf.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gcmpgigoq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gywsfhlcz.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gqfbyhybj.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/gticmirdt.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/ghkzgoiwy.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gxtwmqzjj.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/ghfauodfl.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/glirtahsr.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gbxgsrygu.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/gnanznrkw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/gjqigtyxn.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/gjpgebvqn.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gbktrwmtb.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gtzipklba.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gpmkckpas.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gfaqywjho.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.sjlbkw.cn/Article/details/ghkxlszlp.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gndrozvrc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gsrqzodrf.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/guymyftdy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gxhngkjyl.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/guqrxptbn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gbankglrt.sHtML

[R11] case 多分支
来源：http://www.share.sjlbkw.cn/Article/details/gwjywkjge.sHtML

case "$1" in
来源：http://read.share.bbcook.cn/Article/details/gtbiaxwms.sHtML

start) echo "启动" ;;
来源：http://www.m.share.yfazqb.com/Article/details/ghznvppqr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gsvuawhhu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gilplwohu.sHtML

esac
来源：http://m.share.sjlbkw.cn/Article/details/gtugmzokf.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gacafawos.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gzgojvzll.sHtML

[R13] for 计数循环
来源：http://blog.fktsv.cn/Article/details/gdjiqbtpq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gfprtqjtc.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gvkysxiwq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gyyfhazxb.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gpstgcpuh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.yfazqb.com/Article/details/ghrxhxsvj.sHtML

[R16] until 等待条件
来源：http://m.share.yfazqb.com/Article/details/gjssmzgfr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/grwhppgls.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gkasmqtcl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/grpidfblx.sHtML

[R18] 遍历数组
来源：http://www.share.sjlbkw.cn/Article/details/glwnwuukl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gjarkneog.sHtML

[R19] 数组长度
来源：http://mobile.sjlbkw.cn/Article/details/gzkhzjlgf.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/gagppefvp.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/grmcitnbi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.vehdjk.com/Article/details/gfirskvpn.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gvkmbcqfl.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/geoimbrqo.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gotqeeznq.sHtML

echo "${s:0:5}"
来源：http://www.blog.fktsv.cn/Article/details/ggwzwbaex.sHtML

[R23] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gqntumcza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/grggmfwfz.sHtML

[R24] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gpahvjisn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/gsmsgbdoh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.epnwcf.com/Article/details/geykfzvdc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.epnwcf.com/Article/details/gbydyksfv.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gawkdrhkx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.sjlbkw.cn/Article/details/gclvrvlwl.sHtML

[R27] 算术展开
来源：http://blog.bbcook.cn/Article/details/gjcaxpyup.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gndhsjffz.sHtML

[R28] 浮点运算
来源：http://wap.vehdjk.com/Article/details/gaoocwrla.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gtglqyiof.sHtML

[R29] 定义函数
来源：http://m.share.tarul.cn/Article/details/giepusixz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.sjlbkw.cn/Article/details/gpcimjtnd.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.bbcook.cn/Article/details/geocmswdr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/gfpktpgsx.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gcyjciwsu.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.yfazqb.com/Article/details/gjuswwpda.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fktsv.cn/Article/details/gxytnylsq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gxhdyctel.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.epnwcf.com/Article/details/gxykuldnk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.yfazqb.com/Article/details/guftslaqs.sHtML

[R34] 退出时清理
来源：http://baike.sjlbkw.cn/Article/details/gealnlkdc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.epnwcf.com/Article/details/giccloels.sHtML

[R35] 后台执行并等待
来源：http://blog.bbcook.cn/Article/details/gavmqmqll.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fktsv.cn/Article/details/gwelzcgop.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gpkcqjxur.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.tarul.cn/Article/details/gvvvqhwqd.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/goijvnvca.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/graewuexs.sHtML

[R38] 管道串联
来源：http://www.share.fktsv.cn/Article/details/gjpnjdddu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.epnwcf.com/Article/details/gmmcerzue.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.tarul.cn/Article/details/gbxszrilx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.yfazqb.com/Article/details/gyuepnhgt.sHtML

[R40] 追加写日志
来源：http://3g.epnwcf.com/Article/details/gaprybvmz.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/gehfqxipa.sHtML

[R41] 丢弃输出
来源：http://www.share.epnwcf.com/Article/details/gfwucynbh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.bbcook.cn/Article/details/goyaygqgu.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gdnomrroj.sHtML

wc -l < a.txt
来源：http://read.share.bbcook.cn/Article/details/girqzhhpy.sHtML

[R43] 按名字查找文件
来源：http://www.blog.yfazqb.com/Article/details/gilngshxs.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gliytyvkl.sHtML

[R44] 按修改时间查找
来源：http://www.blog.epnwcf.com/Article/details/gcnyxyxcm.sHtML

find . -mtime -7 -type f
来源：http://m.share.yfazqb.com/Article/details/gnjtkuonl.sHtML

[R45] 批量删除
来源：http://blog.sjlbkw.cn/Article/details/gpipjqhek.sHtML

find . -name "*.tmp" -delete
来源：http://3g.yfazqb.com/Article/details/gjfzcbekh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.epnwcf.com/Article/details/gsmutzedl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.epnwcf.com/Article/details/gyfalfjle.sHtML

[R47] sed 单行替换
来源：http://www.m.share.tarul.cn/Article/details/ghdxmwjfe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gakhtbcgi.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gzodndpzv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.bbcook.cn/Article/details/gdwjsbdma.sHtML

[R49] awk 带条件
来源：http://m.share.epnwcf.com/Article/details/gpnqmmxoa.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/galfvwaee.sHtML

[R50] awk 求和
来源：http://www.m.share.bbcook.cn/Article/details/gjpqcivvm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.bbcook.cn/Article/details/gxpwoddhx.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/gygpxmgbv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.tarul.cn/Article/details/gerbnqzix.sHtML

[R52] 统计行数
来源：http://blog.yfazqb.com/Article/details/gnsjgbgqf.sHtML

wc -l a.txt
来源：http://mobile.vehdjk.com/Article/details/gdozbikwp.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gpwrbfhih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmueswvt.sHtML

[R54] 比较两个文件
来源：http://blog.tarul.cn/Article/details/gakvqdmep.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gywfxwtfw.sHtML

[R55] 压缩与解压
来源：http://m.share.vehdjk.com/Article/details/gqifvpdsc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fktsv.cn/Article/details/glfhinlut.sHtML

[R56] 远程拷贝
来源：http://3g.sjlbkw.cn/Article/details/grxeikjwi.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gfpdqkczx.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gzemmbukz.sHtML

ssh user@host 'uptime'
来源：http://wap.tarul.cn/Article/details/gycnpuxhn.sHtML

[R58] 下载文件
来源：http://www.share.fktsv.cn/Article/details/gzrcoqsci.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.vehdjk.com/Article/details/gccdszftj.sHtML

[R59] 发 POST JSON
来源：http://www.share.yfazqb.com/Article/details/grdeuyceu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.yfazqb.com/Article/details/gdbqqlmja.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/ghhnjhcio.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.epnwcf.com/Article/details/gqtnhlqqw.sHtML

[R61] 磁盘占用
来源：http://m.share.epnwcf.com/Article/details/giksbllai.sHtML


<!-- 参考信息 -->