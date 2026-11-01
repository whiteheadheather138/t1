代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/gskbfktfr.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gnihnhwzr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.sjlbkw.cn/Article/details/gmbmhnjsn.sHtML

[Q15] 查询全部
来源：http://wap.epnwcf.com/Article/details/ghkvjctpi.sHtML

SELECT * FROM users;
来源：http://blog.yfazqb.com/Article/details/gxnvkqtjq.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gyasxmxtx.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/giniadpli.sHtML

[Q17] 条件查询
来源：http://www.blog.yfazqb.com/Article/details/gtgunxjsv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gmjksjlja.sHtML

[Q18] 模糊匹配
来源：http://baike.epnwcf.com/Article/details/ggjxomgnl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gvxwpwcxf.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gmqqchtrg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gxjiuhneu.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gpwfncaqv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.yfazqb.com/Article/details/gamqcaqlq.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/gererevlj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.yfazqb.com/Article/details/gbajjraoa.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/ghxksawim.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gybqrxtav.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gadyvfaek.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.bbcook.cn/Article/details/gyclkystd.sHtML

[Q24] 去重
来源：http://mobile.yfazqb.com/Article/details/gboiqlrdg.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.yfazqb.com/Article/details/gdtcatbji.sHtML

[Q25] 只取前 N 条
来源：http://www.share.yfazqb.com/Article/details/gwrfedlao.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.epnwcf.com/Article/details/gbbufkwlf.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gfvwqzopa.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/glwgwsolb.sHtML

[Q27] 条件计数
来源：http://wap.vehdjk.com/Article/details/gjtjawxzb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gemqrlwit.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/gbpfqqrxb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gvmscgqot.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gxocrhqzx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gqwopgrsh.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gohivnjqq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gzdxbonlm.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/gyayxxttr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/gdassuwvk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.bbcook.cn/Article/details/gqjybfqlf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gcazxlugo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gswxhawse.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gecsjqmxh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gccsjzpzl.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gvbfwpvss.sHtML

SELECT * FROM (
来源：http://www.share.bbcook.cn/Article/details/gqzoqjgty.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.bbcook.cn/Article/details/gcqqwvnsq.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gmfgqykel.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gbpmvpezj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gtvuftbir.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/gvlglrjrx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/ggsazuqxa.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/gxqyutlrm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gyebtkbna.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gtjjdbzvs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/garudaccu.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gxgpcznwl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gahuhyocw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.tarul.cn/Article/details/gnutgihke.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.tarul.cn/Article/details/ggwyjfnaz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/ganirbueo.sHtML

[Q41] 多表连接
来源：http://www.m.share.tarul.cn/Article/details/gelijsjns.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gotvxidhj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkaowxlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gbgtijdxh.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/glktoaagb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gqzpemwls.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gbakhsgqm.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/grvemqtnk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gffdkwhqs.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gaetqjcwy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gocqydiqr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gefxtwvyx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/glvtbjihs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gkqsieess.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gofuwgwnh.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/grwprixoz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gnapfsxqg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gskezixdc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/gsrcvkbbl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.sjlbkw.cn/Article/details/gbvqosuub.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gzpbkcxga.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/ghpdtdfgu.sHtML

[Q50] 批量更新
来源：http://mobile.epnwcf.com/Article/details/gjcnwacya.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/grnsompzg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gqzcvjcxx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.sjlbkw.cn/Article/details/ggbrzkhwz.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/gzbbgfcon.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gkaxlboia.sHtML

[Q53] 按条件删除
来源：http://www.blog.bbcook.cn/Article/details/ghfnngmjo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gseyjuwwk.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/gquxhhvtt.sHtML

TRUNCATE TABLE logs;
来源：http://wap.vehdjk.com/Article/details/ghfkzfdoj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gluqvcuoo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gifilhbis.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gboawmyis.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gcpwutuds.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/gcslevbjn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gpaeizqiz.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/grihgjmya.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gbgsvidbz.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/gewkyacym.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gjumhygjj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gsyqsdsoo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/gxanioovg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gsuubhihi.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gixawgluu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gljtlwcdv.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/grnwyizuz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gcrvmrdxo.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gmpnnhvrr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/gdosckkvy.sHtML

[Q64] 提交事务
来源：http://blog.bbcook.cn/Article/details/gbgxvxvsp.sHtML

COMMIT;
来源：http://blog.yfazqb.com/Article/details/gayvnadjt.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gqdgtshxf.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gqbyidteo.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gmzjuihgu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gjzguvesp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gubjeovty.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/godfthvwm.sHtML

[Q68] 保存点
来源：http://blog.epnwcf.com/Article/details/gmahcmboy.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/gvctpwefx.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/gqrxqsctu.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gbkrsuddn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.sjlbkw.cn/Article/details/gomqqegnx.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gratyibsq.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gdojhhdvu.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gqutpenas.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gtaqsrgvc.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/geeiogask.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gbgtwlclm.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gurctkcfu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gopqvrfas.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gadclgrii.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/gyntauomd.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/gbgrecqfa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gldigmrrc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gcdqweplo.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/gvjnmbncx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/gakuqowbw.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gnfryicst.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gpjagerrt.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/ginatdlmc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gpnmvjlfq.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gqwvmvjnt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/ggunyhjik.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gfatacesg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghcmqtodg.sHtML

[Q81] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/gjbhkfptp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gjojmwmvy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.tarul.cn/Article/details/gkcowrzlu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gmeinqysc.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gfmvnevou.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gszbhlcle.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gspfvusfu.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghhavozbi.sHtML

[Q85] 数值取整
来源：http://3g.yfazqb.com/Article/details/gmswkrvrq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gspkhkvhm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fktsv.cn/Article/details/gfintmryj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.vehdjk.com/Article/details/gavyfxked.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gbkwgtskx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gwebqtvlp.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gfriqrmyb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gcsxlcqir.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/glejlqfan.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/gemqtuaim.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gkyqidvnt.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/gaoflaioz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/ggxasjees.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gbaukfzot.sHtML

R. Bash 专题
来源：http://wap.yfazqb.com/Article/details/gbrshygeg.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gstfdjqvz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.epnwcf.com/Article/details/grqydrzbq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/ghnminbsg.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gjgtgtned.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gaheiummf.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gksckhghu.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gmoduheni.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gyqflipyg.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gegsgkrql.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gesqfitlg.sHtML

[R05] 参数默认值
来源：http://read.share.vehdjk.com/Article/details/gcrdiqgzx.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/ghgfkftsd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gatpvivtw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/grvkgtodf.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gofurxbek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gfdtbstgq.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gkzzlvucy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gpanylsod.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gkyrbckfu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.tarul.cn/Article/details/gjgfontbs.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gidaxaeya.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.epnwcf.com/Article/details/gkdkilrcf.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gykhchzpd.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gamzurrav.sHtML

start) echo "启动" ;;
来源：http://mobile.epnwcf.com/Article/details/gfrlssvyx.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gazieydsa.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gnrqukmfr.sHtML

esac
来源：http://www.m.share.bbcook.cn/Article/details/gzewbccze.sHtML

[R12] for 遍历文件
来源：http://www.m.share.epnwcf.com/Article/details/gvxmypdnf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.sjlbkw.cn/Article/details/gtvrhzrns.sHtML

[R13] for 计数循环
来源：http://m.share.bbcook.cn/Article/details/garceazyb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gedtubgce.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gspqrzayw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gofxcileh.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/ghguqmygo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gpwkphobo.sHtML

[R16] until 等待条件
来源：http://www.blog.sjlbkw.cn/Article/details/gacdqovgg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gucoruvsa.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/ghranjfoc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/ghcwkufxf.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/gcjxqgszq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.yfazqb.com/Article/details/gcmxhyzxx.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/grdrlnhsn.sHtML

echo "${#arr[@]}"
来源：http://baike.bbcook.cn/Article/details/giokdncdv.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/glaoyqipc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gpyfgxzqn.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gdggophvk.sHtML

echo "${#s}"
来源：http://www.blog.bbcook.cn/Article/details/gwirygvxs.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/gpmykzphv.sHtML

echo "${s:0:5}"
来源：http://www.share.vehdjk.com/Article/details/gogjjjfrt.sHtML

[R23] 字符串替换
来源：http://read.share.fktsv.cn/Article/details/gfdfpofyb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.yfazqb.com/Article/details/goxgwkavi.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gcjrwiqfo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/gapaktzrf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.vehdjk.com/Article/details/gzqkqmjme.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/gqpeshwsr.sHtML

[R26] 命令替换
来源：http://wap.yfazqb.com/Article/details/gnxdauxnz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.yfazqb.com/Article/details/gblrodbpr.sHtML

[R27] 算术展开
来源：http://www.m.share.vehdjk.com/Article/details/gmunkzhrr.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.sjlbkw.cn/Article/details/gafacwnbg.sHtML

[R28] 浮点运算
来源：http://www.m.share.sjlbkw.cn/Article/details/gimsiozex.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gybghnbtx.sHtML

[R29] 定义函数
来源：http://www.blog.yfazqb.com/Article/details/guwqkwzej.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.tarul.cn/Article/details/gnlddkzoo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.vehdjk.com/Article/details/gvklqczdu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.yfazqb.com/Article/details/gwqxmzeyw.sHtML

[R31] 局部变量
来源：http://www.m.share.bbcook.cn/Article/details/gkknlcxqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.bbcook.cn/Article/details/ghnpgllpc.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gvsowegea.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gncjkcckz.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.bbcook.cn/Article/details/gwhvqlwrr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.sjlbkw.cn/Article/details/greqtwvhv.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/ginusyumn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fktsv.cn/Article/details/gwtgzrenj.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gppccobze.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.bbcook.cn/Article/details/gfszjnjat.sHtML

[R36] 并发执行多个任务
来源：http://wap.fktsv.cn/Article/details/gvtawwmem.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.bbcook.cn/Article/details/gjdevmqjn.sHtML

[R37] 把输出赋给变量
来源：http://wap.yfazqb.com/Article/details/gbistigpi.sHtML

files=$(ls -1)
来源：http://m.share.tarul.cn/Article/details/gfeihrshc.sHtML

[R38] 管道串联
来源：http://mobile.yfazqb.com/Article/details/gkuuhfhoj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.yfazqb.com/Article/details/gnaniddzm.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.bbcook.cn/Article/details/gkexpvswj.sHtML

cmd > out.log 2>&1
来源：http://baike.yfazqb.com/Article/details/gxydpwdbi.sHtML

[R40] 追加写日志
来源：http://3g.fktsv.cn/Article/details/grtpvjwxg.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gbuyckwma.sHtML

[R41] 丢弃输出
来源：http://mobile.tarul.cn/Article/details/gstlcwgiv.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.sjlbkw.cn/Article/details/gnfwinovq.sHtML

[R42] 输入重定向
来源：http://read.share.fktsv.cn/Article/details/gcvpwprwn.sHtML

wc -l < a.txt
来源：http://m.share.bbcook.cn/Article/details/gurwwoayd.sHtML

[R43] 按名字查找文件
来源：http://baike.yfazqb.com/Article/details/gtfgisegy.sHtML

find . -name "*.log" -type f
来源：http://www.share.sjlbkw.cn/Article/details/gtippktrx.sHtML

[R44] 按修改时间查找
来源：http://baike.vehdjk.com/Article/details/gcepxxnip.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gwvderjck.sHtML

[R45] 批量删除
来源：http://blog.bbcook.cn/Article/details/ghtpgjwef.sHtML

find . -name "*.tmp" -delete
来源：http://baike.epnwcf.com/Article/details/ggiiojjbr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.epnwcf.com/Article/details/gtguiypub.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.epnwcf.com/Article/details/gbrzapnfq.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/grsnzrmzy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.tarul.cn/Article/details/geomvhozp.sHtML

[R48] awk 取指定列
来源：http://3g.vehdjk.com/Article/details/gzuqrwoxi.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fktsv.cn/Article/details/goufnfzzo.sHtML

[R49] awk 带条件
来源：http://read.share.tarul.cn/Article/details/gudajsund.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fktsv.cn/Article/details/gstihqdic.sHtML

[R50] awk 求和
来源：http://mobile.vehdjk.com/Article/details/glrktxueg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.tarul.cn/Article/details/gsqdkdpej.sHtML

[R51] 排序去重取前几
来源：http://3g.vehdjk.com/Article/details/gvqcdbnjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.tarul.cn/Article/details/gkgozujsv.sHtML

[R52] 统计行数
来源：http://baike.bbcook.cn/Article/details/glxxwsvdq.sHtML

wc -l a.txt
来源：http://wap.epnwcf.com/Article/details/ghcidhgsx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.sjlbkw.cn/Article/details/gqbyirmxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.tarul.cn/Article/details/gkxebccdd.sHtML

[R54] 比较两个文件
来源：http://mobile.fktsv.cn/Article/details/grfzuojwg.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gyqmzszqf.sHtML

[R55] 压缩与解压
来源：http://blog.epnwcf.com/Article/details/guouxnjso.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.sjlbkw.cn/Article/details/gblaxlrsb.sHtML

[R56] 远程拷贝
来源：http://mobile.tarul.cn/Article/details/gychmtzwm.sHtML

scp file user@host:/path/
来源：http://3g.sjlbkw.cn/Article/details/gibbsuiuh.sHtML

[R57] 远程执行命令
来源：http://m.share.tarul.cn/Article/details/gnileurkp.sHtML

ssh user@host 'uptime'
来源：http://baike.vehdjk.com/Article/details/gppahgnrx.sHtML

[R58] 下载文件
来源：http://www.m.share.yfazqb.com/Article/details/gcjftplwr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.epnwcf.com/Article/details/gqqeqtxob.sHtML

[R59] 发 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/gbwhjywbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.bbcook.cn/Article/details/ggplactzp.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gxevnwuvw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.yfazqb.com/Article/details/gvrrxclte.sHtML

[R61] 磁盘占用
来源：http://read.share.bbcook.cn/Article/details/grtlqlysa.sHtML

df -h;  du -sh *
来源：http://baike.sjlbkw.cn/Article/details/gdcbnwbnj.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.epnwcf.com/Article/details/gnfanscik.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/gxoewdpfs.sHtML

[R63] 内存与进程
来源：http://baike.yfazqb.com/Article/details/gcypnoeot.sHtML


<!-- 参考信息 -->