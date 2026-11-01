代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/grhdgyqno.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/ggelczdjd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/gndhitudv.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gwlicvcyw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gtqpwqjms.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/gssheougo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/ghknctsnt.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gefekquki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/ggueziaxv.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gtqegpvnl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gydgpejrc.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gghwohose.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gehxasvhu.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/goegjivrh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxdgutlhp.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gubepuchb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.sjlbkw.cn/Article/details/gxlalheme.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gezgjlpyz.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/gbslbgosq.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/gwnxrvnzu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gagjrzzcs.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/glepskblx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gfhjivsug.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/giityhrur.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/glvnlxunn.sHtML

[Q30] 分组统计
来源：http://wap.fktsv.cn/Article/details/gcxfdnzkp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gyfzyzitv.sHtML

[Q31] 分组后过滤
来源：http://3g.epnwcf.com/Article/details/gyfbswmje.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/gsjjodfzp.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/ggunpkdtw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gfszfvyxz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gqyjjugiw.sHtML

[Q33] 多列分组
来源：http://www.share.yfazqb.com/Article/details/gdadynkmr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.sjlbkw.cn/Article/details/gisvpyzfh.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gmjrzopal.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/goobohahn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fktsv.cn/Article/details/gnzhrnqwm.sHtML

) t WHERE rn = 1;
来源：http://m.share.vehdjk.com/Article/details/grldiypnu.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gjzsihnix.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gddovxroc.sHtML

[Q36] 左连接
来源：http://www.blog.bbcook.cn/Article/details/gdrkzkdwo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/ggoigqmrw.sHtML

[Q37] 右连接
来源：http://baike.epnwcf.com/Article/details/ghpkxqzkn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/gkysfwedm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gwmtjjrgx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gjlavzwum.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/gdwkmfium.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gadnilini.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gqsysjojv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gwioppsbh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gmjqxcrgs.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/grwzrghlp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/gsdgguvve.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/griwszpmd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gisagndff.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/giyjnepwv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/giwrwfovn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/gvajxztjl.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gkgimwsic.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/giuewdzoi.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gfcdzbnhp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gptmwqjkg.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gnrjwbeha.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gpbhansjm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/ghgfpbgfy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gyvtncmki.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gydumsflv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/giyymwroz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gtrnhzumy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.tarul.cn/Article/details/gytfgpine.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fktsv.cn/Article/details/gzedpodme.sHtML

[Q49] 更新单行
来源：http://mobile.epnwcf.com/Article/details/gvedenpgj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gpfygunjp.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gnijjayjn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.tarul.cn/Article/details/griyzbbjw.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/gpasrsqzp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/guqhtzfeo.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gknrhdhkr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/glkmankmh.sHtML

[Q53] 按条件删除
来源：http://mobile.sjlbkw.cn/Article/details/gopnodege.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gliwecghb.sHtML

[Q54] 清空表
来源：http://mobile.fktsv.cn/Article/details/gfhfzrdlg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gquknevbw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/ghknmguzz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/grbtefsxq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gcmauipph.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gnvcxmkjf.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/gkuqcubes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gvqgmgsrp.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gpmsuhhnu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gqwaufafe.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gcyclteih.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gvbsqjbxu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/gronaanvt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.sjlbkw.cn/Article/details/gjpelaluw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gstleswml.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gcksrwmcr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gqwrfbiqb.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gpesvklcb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gqfwpwhmy.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/grxzobxmq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/gncuydtlv.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gvfltemsw.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gcdnyjaco.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gaxshzdgm.sHtML

ROLLBACK;
来源：http://m.share.tarul.cn/Article/details/gafgwqecf.sHtML

[Q66] 行锁查询
来源：http://3g.epnwcf.com/Article/details/gqytqpxmv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gkfiowbmb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/gntxcrkgo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/ggawxlsjf.sHtML

[Q68] 保存点
来源：http://wap.sjlbkw.cn/Article/details/gkuclfcvz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gtqdihzpf.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/gklpvvbpv.sHtML

[Q69] 查看执行计划
来源：http://wap.tarul.cn/Article/details/gxvkiptej.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gcstkfhmx.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gzaccnpgv.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gwnbpixwf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gniuchxis.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/glrezkcpb.sHtML

[Q72] 查看索引
来源：http://baike.tarul.cn/Article/details/gjyfmfyhw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gospbvfzt.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/grzsrkoze.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gssbuckxg.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gevqnwwhf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.vehdjk.com/Article/details/gojhsglyv.sHtML

[Q75] 日期格式化
来源：http://www.share.yfazqb.com/Article/details/gsopjoduw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.vehdjk.com/Article/details/grsexfsat.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gfushjicw.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/gpfybgmeb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gnwappbhb.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gfftrbaeu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.vehdjk.com/Article/details/gordrtsso.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/guofhdecy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/gtrgookas.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gofddlknx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.epnwcf.com/Article/details/grwhjqali.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gpqmsszog.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gyjbmobci.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gtqgneqac.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gxwzmfqyu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gfjoyehmc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gkkcyrovj.sHtML

[Q83] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gazwqyism.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gxqghetqp.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/ghdzvcvob.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/getcegdhe.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/geodwahed.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/glkwcttnf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gmlmstqxg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/guiamhyak.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.vehdjk.com/Article/details/gnqiifpni.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.sjlbkw.cn/Article/details/gkepdkrky.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gohbksenh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gvlcrtfsr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gbtaktvvu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gitkdlmgr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gmcgnhnde.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gcqifcflu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gkvzpvpvs.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/geenfwrpb.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/ghhvjmybv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gpoxgirjp.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gmiijlwjr.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gwvthqpnw.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/gdstcvfbe.sHtML

[R02] 变量赋值与使用
来源：http://blog.yfazqb.com/Article/details/ghnvbuqeu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fktsv.cn/Article/details/gyqdeqgcn.sHtML

[R03] 只读变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoiwfzfx.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gtykxxifq.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gmksevuzv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gznkesljg.sHtML

[R05] 参数默认值
来源：http://www.m.share.bbcook.cn/Article/details/gspzywpoj.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/griynpkxx.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gziujlple.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.tarul.cn/Article/details/guwihpgix.sHtML

[R07] if 判断文件
来源：http://read.share.fktsv.cn/Article/details/gziazinnd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.bbcook.cn/Article/details/gnjytvowg.sHtML

[R08] 数值比较
来源：http://www.share.yfazqb.com/Article/details/gbshwgsvx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gekeasapx.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gsxisotqg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gllhnzcxg.sHtML

[R10] 正则匹配
来源：http://www.share.bbcook.cn/Article/details/gtnpnytva.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.bbcook.cn/Article/details/gdaqvsgbq.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gdapwddab.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gdcjlsnbj.sHtML

start) echo "启动" ;;
来源：http://wap.sjlbkw.cn/Article/details/gkwlrfgtb.sHtML

stop)  echo "停止" ;;
来源：http://baike.bbcook.cn/Article/details/gvnbbzxca.sHtML

*)     echo "未知命令" ;;
来源：http://wap.sjlbkw.cn/Article/details/gbgcokutv.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gysgycyzh.sHtML

[R12] for 遍历文件
来源：http://www.share.epnwcf.com/Article/details/gvxicokqg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gednhsxfn.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/gffztluro.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.vehdjk.com/Article/details/gmmlryeps.sHtML

[R14] C 风格 for
来源：http://www.share.yfazqb.com/Article/details/gpgowpvmh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gcrsvetos.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.bbcook.cn/Article/details/gztuewrry.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/glwswbqyw.sHtML

[R16] until 等待条件
来源：http://mobile.sjlbkw.cn/Article/details/gdcznciwt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.vehdjk.com/Article/details/gypbtkrmv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.yfazqb.com/Article/details/gqmsiphaw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/gbkrrqmtb.sHtML

[R18] 遍历数组
来源：http://wap.bbcook.cn/Article/details/gvfyrrvoa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/giixmidih.sHtML

[R19] 数组长度
来源：http://3g.fktsv.cn/Article/details/givjgouyq.sHtML

echo "${#arr[@]}"
来源：http://baike.tarul.cn/Article/details/gyrcsigpc.sHtML

[R20] 关联数组（字典）
来源：http://blog.fktsv.cn/Article/details/gpnhrcjva.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gmbvbrjjz.sHtML

[R21] 字符串长度
来源：http://www.blog.bbcook.cn/Article/details/gzobevixp.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gaqdcgqyp.sHtML

[R22] 截取子串
来源：http://3g.vehdjk.com/Article/details/ghqckbwyl.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/gpfahogub.sHtML

[R23] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/gcxomqidr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.bbcook.cn/Article/details/gatrceobf.sHtML

[R24] 大小写转换
来源：http://3g.epnwcf.com/Article/details/geaxdsygq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/gxdapbghw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gbizhckbd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/grdkkdbhq.sHtML

[R26] 命令替换
来源：http://m.share.vehdjk.com/Article/details/gafnudtja.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/ggbmefbab.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gepjyblsf.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/geiiyiwfm.sHtML

[R28] 浮点运算
来源：http://m.share.sjlbkw.cn/Article/details/gdpudlgbp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gbkfhzhvc.sHtML

[R29] 定义函数
来源：http://www.share.yfazqb.com/Article/details/gjyrppwdg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fktsv.cn/Article/details/gfpkugdid.sHtML

[R30] 函数返回状态码
来源：http://wap.epnwcf.com/Article/details/gehycdvpt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gdvrxldyj.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/guhijsbej.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.sjlbkw.cn/Article/details/gxqyczlzz.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/ggjlrvdae.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gukiegwhb.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.tarul.cn/Article/details/gizvroxay.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.tarul.cn/Article/details/gposfdvbd.sHtML

[R34] 退出时清理
来源：http://wap.vehdjk.com/Article/details/gkszufurj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fktsv.cn/Article/details/gfbpwisiq.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/gwveuzdij.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.vehdjk.com/Article/details/gvnajjqmf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.bbcook.cn/Article/details/gichzwbpf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gwfafhceu.sHtML

[R37] 把输出赋给变量
来源：http://m.share.epnwcf.com/Article/details/gkumyosrl.sHtML

files=$(ls -1)
来源：http://baike.bbcook.cn/Article/details/gifpcuovt.sHtML

[R38] 管道串联
来源：http://mobile.epnwcf.com/Article/details/gzznlqhtm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.tarul.cn/Article/details/gxvoivkdc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.sjlbkw.cn/Article/details/gkcungbqy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.tarul.cn/Article/details/gugqrmooh.sHtML

[R40] 追加写日志
来源：http://www.share.tarul.cn/Article/details/gvrsjvnbd.sHtML

echo "log" >> out.log
来源：http://www.share.yfazqb.com/Article/details/gughiirtg.sHtML

[R41] 丢弃输出
来源：http://read.share.fktsv.cn/Article/details/gijsajcil.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/gzyskbhwu.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/gpuavgrfa.sHtML

wc -l < a.txt
来源：http://mobile.tarul.cn/Article/details/gojmywixl.sHtML

[R43] 按名字查找文件
来源：http://read.share.sjlbkw.cn/Article/details/gyhegzlqa.sHtML

find . -name "*.log" -type f
来源：http://blog.fktsv.cn/Article/details/glabismwl.sHtML

[R44] 按修改时间查找
来源：http://read.share.sjlbkw.cn/Article/details/gxohxnxyy.sHtML

find . -mtime -7 -type f
来源：http://mobile.bbcook.cn/Article/details/gkmbnhkes.sHtML

[R45] 批量删除
来源：http://mobile.epnwcf.com/Article/details/gwdadvyse.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gjsvujksj.sHtML

[R46] 递归替换文件内容
来源：http://3g.yfazqb.com/Article/details/gwnvryriy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fktsv.cn/Article/details/ghddldrwq.sHtML

[R47] sed 单行替换
来源：http://baike.bbcook.cn/Article/details/ghwcoxfzq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.yfazqb.com/Article/details/gsjeqyxaf.sHtML

[R48] awk 取指定列
来源：http://baike.yfazqb.com/Article/details/gnjfialhc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fktsv.cn/Article/details/gbamvyzpo.sHtML

[R49] awk 带条件
来源：http://wap.tarul.cn/Article/details/gxrwczgqp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.tarul.cn/Article/details/gzhricnea.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gifywmpnm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.yfazqb.com/Article/details/gxzgvenwp.sHtML

[R51] 排序去重取前几
来源：http://m.share.sjlbkw.cn/Article/details/gfrwhfzny.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.vehdjk.com/Article/details/gbwaqmrze.sHtML

[R52] 统计行数
来源：http://blog.bbcook.cn/Article/details/gjgjxcrsa.sHtML

wc -l a.txt
来源：http://baike.vehdjk.com/Article/details/gkqkgxnwz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.yfazqb.com/Article/details/gyjsnicgx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.vehdjk.com/Article/details/gjqlvovny.sHtML

[R54] 比较两个文件
来源：http://www.m.share.tarul.cn/Article/details/gaoceisvv.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gjvrkgvyz.sHtML

[R55] 压缩与解压
来源：http://www.share.epnwcf.com/Article/details/glemhcefa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.bbcook.cn/Article/details/ghkwjqsxu.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gvgoovhqs.sHtML

scp file user@host:/path/
来源：http://www.blog.vehdjk.com/Article/details/gtewqenog.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gpkfjwyzy.sHtML

ssh user@host 'uptime'
来源：http://baike.sjlbkw.cn/Article/details/gqwraanwq.sHtML

[R58] 下载文件
来源：http://www.m.share.bbcook.cn/Article/details/gptgtoigr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.tarul.cn/Article/details/gbcfpdzva.sHtML

[R59] 发 POST JSON
来源：http://3g.yfazqb.com/Article/details/gurmamvri.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.vehdjk.com/Article/details/ghmfugjpb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gztpwzexl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/gcmkzusgz.sHtML

[R61] 磁盘占用
来源：http://www.blog.sjlbkw.cn/Article/details/gdjpllkig.sHtML

df -h;  du -sh *
来源：http://wap.epnwcf.com/Article/details/gjvxvxwgk.sHtML

[R62] 找最占空间的文件
来源：http://blog.epnwcf.com/Article/details/ghwzmmulp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.bbcook.cn/Article/details/gwbldeymy.sHtML

[R63] 内存与进程
来源：http://blog.fktsv.cn/Article/details/gkdizsmwj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.epnwcf.com/Article/details/gqnxaeosv.sHtML

[R64] 结束进程
来源：http://baike.bbcook.cn/Article/details/gjvgbtopo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.yfazqb.com/Article/details/gqwwjswaw.sHtML

[R65] 查看端口占用
来源：http://www.share.vehdjk.com/Article/details/gsrahutzg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.bbcook.cn/Article/details/gzuwsbzwo.sHtML

[R66] 定时任务
来源：http://baike.sjlbkw.cn/Article/details/glmwgfykf.sHtML

crontab -e;  crontab -l
来源：http://mobile.yfazqb.com/Article/details/gkuccwhgq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.sjlbkw.cn/Article/details/gnnkeqwzg.sHtML


<!-- 参考信息 -->