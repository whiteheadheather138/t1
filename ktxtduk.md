代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gxpfpbxat.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gvknwigxj.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gpygybchx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gyacwnhpx.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.yfazqb.com/Article/details/gzxwuduwo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/gqlginuhz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/gcvskbyjo.sHtML

[Q15] 查询全部
来源：http://baike.bbcook.cn/Article/details/gttrnssso.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/gwvwtpjup.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gvnkpklbv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtgsvgwya.sHtML

[Q17] 条件查询
来源：http://www.m.share.bbcook.cn/Article/details/gdvjgsoom.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gleroqhgx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gqqnslvyr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fktsv.cn/Article/details/gxlxzpxnq.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/govrtksfg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/gacqtsmtg.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gfrmklthc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.tarul.cn/Article/details/ghldsidfw.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gonaqhcrb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gmctwebvr.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gcvuaeely.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gtefbwizs.sHtML

[Q23] 分页
来源：http://mobile.sjlbkw.cn/Article/details/gkcnalxxj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gdkwgnlxa.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gyqhferzl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzejyjnzv.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gaadqclui.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gmavryuwg.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gsrgusmlt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gtawkijaj.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gksqoyqxm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gxwmlnidc.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/ghsuiarhi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gxbocwncm.sHtML

[Q29] 最大最小值
来源：http://blog.tarul.cn/Article/details/gxldgatqx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gqzqtvsld.sHtML

[Q30] 分组统计
来源：http://3g.sjlbkw.cn/Article/details/gjjzeopak.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/guysnzqug.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/grauuejsg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/gvagehzsg.sHtML

[Q32] 分组拼接字符串
来源：http://3g.sjlbkw.cn/Article/details/gqlfbcrdu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gmaybmwto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/giivzmyys.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gwivgqbki.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.bbcook.cn/Article/details/gfevgjeri.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gbnjueawn.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/gguwdsdhm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gytrxbnwu.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gunrjyctj.sHtML

[Q35] 内连接
来源：http://3g.bbcook.cn/Article/details/glglmojgv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/ghzxkdsea.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gmmpiuyzg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gmgqqbars.sHtML

[Q37] 右连接
来源：http://www.m.share.tarul.cn/Article/details/glzujqgdn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gvhsvtsxy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gykjmphgm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/goqknggys.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gfxsxbozz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gfeaagiep.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/grnxerhxi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gwbzpnzan.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.yfazqb.com/Article/details/goqmsxsjf.sHtML

[Q41] 多表连接
来源：http://read.share.sjlbkw.cn/Article/details/gcpvtjvhu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.tarul.cn/Article/details/gxriziihf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/guqypcbap.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gzskstoxe.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gisulimdx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.tarul.cn/Article/details/gvtxdzvnr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gnhjjnjyn.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gswfbbvgt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gbjbcogtp.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/gbswcvwtw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gbnsznhrq.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gkzvfkaya.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdngzhnfg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.bbcook.cn/Article/details/gxryozwos.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gwrlgjcwb.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gvfeauaqs.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.tarul.cn/Article/details/gjpcnimsu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/ghlzuxakc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gejyzdbbw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/ghnkljmhq.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/geavfzvzw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/glysnrkmi.sHtML

[Q50] 批量更新
来源：http://wap.bbcook.cn/Article/details/gijcdwlmz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.epnwcf.com/Article/details/gvzyxotyw.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/gjtstfngn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gdaigaokw.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gtiseiotp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gimaqgcww.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gejvddmaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/grjsgacuy.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gllrkyead.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gfmckeoib.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/gnxjtqinr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gcudfcpfg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.vehdjk.com/Article/details/gzrevkonv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gklovngdc.sHtML

[Q57] 行号
来源：http://www.m.share.bbcook.cn/Article/details/gonebojlb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gbtszowti.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/gkyasykbh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/grxfhdhto.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gxyujqgeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gtxhodqgw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gyklmjojh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gsgnsgyyv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gncuqolox.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gmxyjkmqe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/ghiwtereq.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gmsgibylq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/grihkkvcr.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gehodmzov.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gdujltcrk.sHtML

[Q64] 提交事务
来源：http://m.share.yfazqb.com/Article/details/gvfbfwlyj.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gbkomdxww.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gzfhpknks.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/ghsnpleuk.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gvlmpzfrh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gczhnwgfo.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/gpvgfgsec.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gbzjewuek.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gajitvtus.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gqjgretau.sHtML

ROLLBACK TO sp1;
来源：http://blog.epnwcf.com/Article/details/gkphdagaa.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gzgaguxtf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gosoxyosf.sHtML

[Q70] 更新统计信息
来源：http://mobile.bbcook.cn/Article/details/gjxqwgxgn.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gbhuegzix.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gpypgrcbn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gwxabdcbh.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gmzfsbgeb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gdjffdywd.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gjnmrfjzh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/godubhoic.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/gvkhepfrk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/girvyhine.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gjpppqrab.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gblgewxsw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gavyrhvyl.sHtML

[Q76] 按天统计
来源：http://read.share.tarul.cn/Article/details/ghsdhihdl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.bbcook.cn/Article/details/gbabhegxn.sHtML

[Q77] 时间加减
来源：http://www.share.epnwcf.com/Article/details/gpizdqcqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.sjlbkw.cn/Article/details/gcwfermjn.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/gdluiatvs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/glfmajfsp.sHtML

[Q79] 字符串拼接
来源：http://mobile.sjlbkw.cn/Article/details/ggmtwuaxg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gjgxmizri.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gbzudnopa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.tarul.cn/Article/details/gaijrgqnv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gsrblqtyn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gthvcyxpb.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/gaavmlzvl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gcercrowk.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gpliynsit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gtuthmyhk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gfxmzdmyj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/giarwmjjh.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/gqawcvxje.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/gfccyskwb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gjxombutt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gctzjpsvj.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gkfixlvjp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gpissaydi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gopyoliag.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.yfazqb.com/Article/details/gxrzsekvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdvobcqaq.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gazwuchoh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gcscuxbmv.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/gihyarpyd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gtcjaoeve.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gzfcwrlvv.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/glkiomvau.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gotzyyjwo.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gmekkhrow.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gyexuqdux.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gicopocjv.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gqecjdvpc.sHtML

name="Tom"; echo "$name"
来源：http://wap.vehdjk.com/Article/details/gxvrdrvbw.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gnuengcfv.sHtML

readonly PI=3.14
来源：http://m.share.yfazqb.com/Article/details/gmjtduxzu.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gbmcysgho.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gejqwkkes.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gxjvpkzgq.sHtML

name="${1:-default}"
来源：http://www.blog.yfazqb.com/Article/details/ghmonenlx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gmoyclwmd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gxsobogir.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/gsykrgxgc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gbemoxllh.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gutlqgcta.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gnwttjiis.sHtML

[R09] 字符串比较
来源：http://blog.epnwcf.com/Article/details/gxulzrqvd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/ggbhxclii.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gsyjmqabr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/ghsptoxjv.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gurgwwgry.sHtML

case "$1" in
来源：http://baike.tarul.cn/Article/details/gduqbbewu.sHtML

start) echo "启动" ;;
来源：http://wap.fktsv.cn/Article/details/gliyuwpkt.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gpbobated.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gmlghekug.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gedxzsuiz.sHtML

[R12] for 遍历文件
来源：http://baike.sjlbkw.cn/Article/details/gjghggxxe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gulisixff.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gvfexuwds.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdqojuvm.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gwlrophnd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.epnwcf.com/Article/details/gosshyhay.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/gxfjzepgo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.bbcook.cn/Article/details/gufzkxvwg.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/gdvvjnbyq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.epnwcf.com/Article/details/gryqmnuxx.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gpcbkccwb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gdjjgiujf.sHtML

[R18] 遍历数组
来源：http://mobile.epnwcf.com/Article/details/gzxlmrurw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.sjlbkw.cn/Article/details/gqnfhcsyg.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gvkdoncdk.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gomjimywf.sHtML

[R20] 关联数组（字典）
来源：http://wap.bbcook.cn/Article/details/gxsymvcrk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.sjlbkw.cn/Article/details/gnfyvbqtq.sHtML

[R21] 字符串长度
来源：http://www.share.vehdjk.com/Article/details/gsmbzkepk.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/govaiqzcf.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/glukvywkv.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gamtahoai.sHtML

[R23] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/gygynghcx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/gvqcqukzt.sHtML

[R24] 大小写转换
来源：http://blog.vehdjk.com/Article/details/gutoayvaj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.tarul.cn/Article/details/geecmfihh.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/gmvqbcgmo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.sjlbkw.cn/Article/details/graprepid.sHtML

[R26] 命令替换
来源：http://www.blog.fktsv.cn/Article/details/gbtzgeaot.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/ggzttcwyo.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/gsrlshipl.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/gyighpjmu.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gxfapucpc.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/gjbsglkrl.sHtML

[R29] 定义函数
来源：http://blog.epnwcf.com/Article/details/gchtcqkos.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.bbcook.cn/Article/details/gczmwnemu.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gdqlnnpys.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.vehdjk.com/Article/details/gdkyfmpkb.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gkutzigcq.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gsdyzvvgv.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gnwqolxco.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/gizjhvyrj.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gvjeamhlq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/gqocmmlfj.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/gdvmnrzgv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.yfazqb.com/Article/details/gvvthugzq.sHtML

[R35] 后台执行并等待
来源：http://m.share.sjlbkw.cn/Article/details/glynrvwea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.vehdjk.com/Article/details/guotxtxho.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fktsv.cn/Article/details/gulmzambv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fktsv.cn/Article/details/gmnibymio.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gbohaxqci.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/ghhstrrav.sHtML

[R38] 管道串联
来源：http://3g.sjlbkw.cn/Article/details/ghalaxgpb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gzejhecce.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gklnmrktf.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gbpfxjebi.sHtML

[R40] 追加写日志
来源：http://read.share.sjlbkw.cn/Article/details/gpuhzsokh.sHtML

echo "log" >> out.log
来源：http://3g.tarul.cn/Article/details/gzltoxbvl.sHtML

[R41] 丢弃输出
来源：http://baike.tarul.cn/Article/details/gwxanbglr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.epnwcf.com/Article/details/gingjfute.sHtML

[R42] 输入重定向
来源：http://blog.bbcook.cn/Article/details/gxicxduxv.sHtML

wc -l < a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gtcqlioiw.sHtML

[R43] 按名字查找文件
来源：http://baike.fktsv.cn/Article/details/getvvwzfr.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fktsv.cn/Article/details/ggkrrucgg.sHtML

[R44] 按修改时间查找
来源：http://blog.sjlbkw.cn/Article/details/gwhdxrazx.sHtML

find . -mtime -7 -type f
来源：http://www.blog.tarul.cn/Article/details/gefaotupb.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gfeglkdyu.sHtML

find . -name "*.tmp" -delete
来源：http://wap.tarul.cn/Article/details/grgsylhem.sHtML

[R46] 递归替换文件内容
来源：http://wap.vehdjk.com/Article/details/gqhexlgeq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.bbcook.cn/Article/details/gvpnylist.sHtML

[R47] sed 单行替换
来源：http://mobile.vehdjk.com/Article/details/gfgmydhqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/gcyghdqgl.sHtML

[R48] awk 取指定列
来源：http://wap.bbcook.cn/Article/details/gvaoiytjn.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.epnwcf.com/Article/details/gjgjmhlxt.sHtML

[R49] awk 带条件
来源：http://baike.bbcook.cn/Article/details/gghbpkpyl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.tarul.cn/Article/details/gpjggwdxy.sHtML

[R50] awk 求和
来源：http://www.share.sjlbkw.cn/Article/details/grsvkbkid.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.epnwcf.com/Article/details/gtrtexxiz.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gpktumval.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.yfazqb.com/Article/details/gnkmxcoox.sHtML

[R52] 统计行数
来源：http://wap.vehdjk.com/Article/details/gzkfqcgjh.sHtML

wc -l a.txt
来源：http://www.share.vehdjk.com/Article/details/gieyhrflt.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gwzfhvthc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.vehdjk.com/Article/details/gwgtbwgux.sHtML

[R54] 比较两个文件
来源：http://mobile.yfazqb.com/Article/details/gsreqmubn.sHtML

diff a.txt b.txt
来源：http://read.share.yfazqb.com/Article/details/gjzzsogrn.sHtML

[R55] 压缩与解压
来源：http://www.blog.fktsv.cn/Article/details/gxrchoddq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.epnwcf.com/Article/details/gycqahspn.sHtML

[R56] 远程拷贝
来源：http://www.blog.sjlbkw.cn/Article/details/goekjhczu.sHtML

scp file user@host:/path/
来源：http://www.blog.epnwcf.com/Article/details/gkccmoyqf.sHtML

[R57] 远程执行命令
来源：http://read.share.epnwcf.com/Article/details/gjfdxukud.sHtML

ssh user@host 'uptime'
来源：http://www.share.epnwcf.com/Article/details/gpgnesedk.sHtML

[R58] 下载文件
来源：http://mobile.epnwcf.com/Article/details/gtqgpgoja.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.tarul.cn/Article/details/gnqqifvcd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/geokiuhfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gcdwbqhtl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.epnwcf.com/Article/details/gpkmmldpz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/gicxzjbcg.sHtML

[R61] 磁盘占用
来源：http://m.share.bbcook.cn/Article/details/gpjltupmd.sHtML


<!-- 参考信息 -->