代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://read.share.bbcook.cn/Article/details/glfwutjev.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gdheghfxj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/grsuwoegp.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gpqhpshep.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gcaihkfof.sHtML

[Q16] 查询指定列
来源：http://mobile.yfazqb.com/Article/details/glyzhbker.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gdafhsalb.sHtML

[Q17] 条件查询
来源：http://www.m.share.yfazqb.com/Article/details/gbomafuia.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gojuilzrm.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/guympzeln.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjaejwio.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gcbngrglb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.yfazqb.com/Article/details/gkcomcvav.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gnehskdkx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.sjlbkw.cn/Article/details/gvexyrwhn.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/gfjfjkghm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gboifvkuk.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gsyrklgpz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gnsrjxepe.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/ghkehriot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gqucmpryb.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/gxoipjlrf.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.bbcook.cn/Article/details/gnipbuafr.sHtML

[Q25] 只取前 N 条
来源：http://wap.fktsv.cn/Article/details/gtmirnalh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/gpjtasobb.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gtrutxybe.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/goyiclije.sHtML

[Q27] 条件计数
来源：http://3g.sjlbkw.cn/Article/details/ggmfftjsr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/ggmbuttsm.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gdfiorwyi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gythdosxt.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/giazripvq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gkuyhvsot.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gjvpedfbm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gdrvtvpnb.sHtML

[Q31] 分组后过滤
来源：http://blog.yfazqb.com/Article/details/gajhtyepp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.epnwcf.com/Article/details/gcxkydtaa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gjcishcds.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/goessbunw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/grfvgrqwg.sHtML

[Q33] 多列分组
来源：http://read.share.fktsv.cn/Article/details/ggkfjdlgv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/gtgzvdjfp.sHtML

[Q34] 每组取第一条
来源：http://www.share.vehdjk.com/Article/details/gjzakuyen.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gicnamnxj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gueifrszx.sHtML

) t WHERE rn = 1;
来源：http://3g.bbcook.cn/Article/details/gohifoxin.sHtML

[Q35] 内连接
来源：http://wap.sjlbkw.cn/Article/details/gmrvgpskb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gnvzioskj.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/guyqjjagb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gmkeotuef.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gsmlvisja.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/goxdedmtl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/gkhvmhqzp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.sjlbkw.cn/Article/details/gwxvcdfoc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gyqnjfbui.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/gmynvshke.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/gpivsfwmj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gfjmyzutc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gakmbauhm.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/gleasptpu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.bbcook.cn/Article/details/gibbvqjsa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gpwfdgpoq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gsmubiqmk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gwxpqdwak.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.bbcook.cn/Article/details/gponchtxc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gvqgtifxs.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gwqatjozp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gpchohzdp.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gryaiayte.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.tarul.cn/Article/details/gkkcbehcx.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gyzhoqgwo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gsrmmdoip.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.vehdjk.com/Article/details/gtmrunhry.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gagqefdtg.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gyicntjcb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/gowbpycfq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.yfazqb.com/Article/details/giykuchob.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.epnwcf.com/Article/details/gqqxukjee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/ghqefuwrg.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/gcqolixlv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.yfazqb.com/Article/details/giqfaukcg.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/gzdwyqqbk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/grxzfueln.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/gtucpyjwd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gkaleoigt.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/gbmgncivv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gmuhemlsj.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gvgcxkrru.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/gfddzdgjc.sHtML

[Q54] 清空表
来源：http://baike.epnwcf.com/Article/details/gwmxhnkof.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gunhjglss.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gelfgzzbm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gtpsnsokd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gxdwgbdtl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/ggmbsrtwy.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gjsoertdh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/gswwdpoen.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/gdkymnevl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gvpryehsc.sHtML

[Q59] 分组内累计
来源：http://3g.fktsv.cn/Article/details/gfogciner.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gonuuydzj.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.epnwcf.com/Article/details/ghxpbzvtt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gjtiplxqn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gixnwuggp.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gvwqlkqpf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ghazrkdlk.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/goegosywx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gwtnrgkbc.sHtML

[Q63] 开启事务
来源：http://mobile.epnwcf.com/Article/details/gdumpsndo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.bbcook.cn/Article/details/gligoewtx.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gtnmjaaoq.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gdocgjolb.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gigszssrp.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/gchoxxwrz.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gbwddkgkx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gkilgfgab.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gkziltowe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gejnkcubw.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gknpcueau.sHtML

SAVEPOINT sp1;
来源：http://blog.yfazqb.com/Article/details/ggoxlranp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/giugywmet.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/gstcbpyoa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.bbcook.cn/Article/details/gsiobmwob.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gmokcasat.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/ggpjxxqdh.sHtML

[Q71] 查看建表语句
来源：http://3g.bbcook.cn/Article/details/gaksvpkyy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gokgyvkru.sHtML

[Q72] 查看索引
来源：http://read.share.epnwcf.com/Article/details/gxidwvpyb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvtuqtvqg.sHtML

[Q73] 查看表状态
来源：http://wap.tarul.cn/Article/details/gfimnfiwf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/givlfvmxk.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gngkdoqlk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gewscgxqr.sHtML

[Q75] 日期格式化
来源：http://3g.tarul.cn/Article/details/gcxysikaz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gltvzvtxr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gdliobdvs.sHtML

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gxnfcfejq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fktsv.cn/Article/details/gugjllzty.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gnvbwzdso.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gngftzptu.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gvfpfedoo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gqrskecpy.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gziqnxqth.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/gekchtvej.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/gzviunmgi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gkfuxsoqr.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gpmulbgdr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwonbxvw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/gjaurygtk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gujdbqsqv.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gikovyvfi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/gfuraxmtj.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gwtljyxcl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.vehdjk.com/Article/details/gjggnxsap.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gpxxfskrn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.yfazqb.com/Article/details/gfemvexgh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/ghckqglck.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.bbcook.cn/Article/details/gydavoysm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/goyvwnerj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gamhcaubj.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gvqxfwqpj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.yfazqb.com/Article/details/gjybvtdsp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.vehdjk.com/Article/details/gdvcdzgsy.sHtML

[Q89] 判断表是否存在
来源：http://read.share.bbcook.cn/Article/details/gyctobfjk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gnfbwngue.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/glopwjvai.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.tarul.cn/Article/details/gsrugjnhx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gojnbsyeh.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/gamcudwvv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gspcryqzh.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/giaqfmdcc.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gdikwgwdq.sHtML

set -euo pipefail
来源：http://www.m.share.yfazqb.com/Article/details/glbnunboj.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/goobzfvlw.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gzitsucgr.sHtML

[R03] 只读变量
来源：http://blog.vehdjk.com/Article/details/ggnsbemgu.sHtML

readonly PI=3.14
来源：http://wap.sjlbkw.cn/Article/details/genvhpwtx.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gaznlztmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/glonhjudi.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gfsleevmc.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gvzenlbge.sHtML

[R06] 判断命令是否存在
来源：http://m.share.sjlbkw.cn/Article/details/ghupgavgt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gizctollf.sHtML

[R07] if 判断文件
来源：http://m.share.sjlbkw.cn/Article/details/gqqrtczrp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fktsv.cn/Article/details/gfawnafmn.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gvbedndic.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.epnwcf.com/Article/details/gyitiuzbo.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gdvxqwpfd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/gnztuoera.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gmphylonw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gerxvpmmo.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/gqeyatkhy.sHtML

case "$1" in
来源：http://3g.fktsv.cn/Article/details/ggysyrarr.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gziahwifv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gmrjpefiv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.bbcook.cn/Article/details/ggbgvehzy.sHtML

esac
来源：http://3g.sjlbkw.cn/Article/details/gnjmjjzwc.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/ghtytdhet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gmfcqrsxv.sHtML

[R13] for 计数循环
来源：http://3g.tarul.cn/Article/details/gmabnquky.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fktsv.cn/Article/details/gfcsreoee.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gfwebgfqo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gvkstxhwu.sHtML

[R15] while 逐行读文件
来源：http://wap.yfazqb.com/Article/details/guwbjcoaq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.tarul.cn/Article/details/gzvixktin.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/gywotupfa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gmaxhqizx.sHtML

[R17] 数组定义与取值
来源：http://www.share.fktsv.cn/Article/details/gopiczjmr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gmvordzxd.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gqrcfwxes.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gopknrrja.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/grvonriur.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.tarul.cn/Article/details/gacuzsqre.sHtML

[R20] 关联数组（字典）
来源：http://baike.bbcook.cn/Article/details/gfswcpwij.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.sjlbkw.cn/Article/details/grsmckdgw.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gcllojoix.sHtML

echo "${#s}"
来源：http://www.m.share.epnwcf.com/Article/details/gfvxlarfl.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gjcydonhd.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gwmfqjybv.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gwirhiqxg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fktsv.cn/Article/details/gkhxjduvo.sHtML

[R24] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/griwogptp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.sjlbkw.cn/Article/details/guqxlumyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/ggagmqqdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gldzrwnje.sHtML

[R26] 命令替换
来源：http://baike.epnwcf.com/Article/details/gyovvzzde.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.vehdjk.com/Article/details/gqsmoiroy.sHtML

[R27] 算术展开
来源：http://baike.sjlbkw.cn/Article/details/ggpeavvlm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gzwkrjscw.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gijuhtsop.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.epnwcf.com/Article/details/gmpujtiuk.sHtML

[R29] 定义函数
来源：http://3g.tarul.cn/Article/details/gnknqlmss.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fktsv.cn/Article/details/gcbwbxorl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gnecthzdg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.vehdjk.com/Article/details/gymkmahjb.sHtML

[R31] 局部变量
来源：http://read.share.yfazqb.com/Article/details/gddvfpysl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fktsv.cn/Article/details/gayaqhoou.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gyukovtwc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/ggjhyjvch.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fktsv.cn/Article/details/gvjoczrve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.yfazqb.com/Article/details/gsjggpoiz.sHtML

[R34] 退出时清理
来源：http://www.share.bbcook.cn/Article/details/gfcevhcbr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gqcqaares.sHtML

[R35] 后台执行并等待
来源：http://3g.vehdjk.com/Article/details/ghuagugbv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gqrkmiuks.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fktsv.cn/Article/details/gtwydmexv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gmurwukls.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/guemjqzvg.sHtML

files=$(ls -1)
来源：http://www.m.share.tarul.cn/Article/details/gbhcltwje.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gvjpzksjr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fktsv.cn/Article/details/glsxzilux.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/grqhesfcl.sHtML

cmd > out.log 2>&1
来源：http://mobile.sjlbkw.cn/Article/details/gvbwygsha.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gmlkhcjmg.sHtML

echo "log" >> out.log
来源：http://blog.vehdjk.com/Article/details/gydzanhew.sHtML

[R41] 丢弃输出
来源：http://www.share.vehdjk.com/Article/details/grfaqbowu.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.sjlbkw.cn/Article/details/gslfntqdw.sHtML

[R42] 输入重定向
来源：http://m.share.yfazqb.com/Article/details/gjldzsace.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/gwumqvzay.sHtML

[R43] 按名字查找文件
来源：http://www.blog.tarul.cn/Article/details/gwqkxttkw.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gnkzluipf.sHtML

[R44] 按修改时间查找
来源：http://read.share.epnwcf.com/Article/details/gdhnuylnv.sHtML

find . -mtime -7 -type f
来源：http://blog.sjlbkw.cn/Article/details/gcxttezut.sHtML

[R45] 批量删除
来源：http://m.share.epnwcf.com/Article/details/gejtakcvy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fktsv.cn/Article/details/gnrbuvsec.sHtML

[R46] 递归替换文件内容
来源：http://baike.vehdjk.com/Article/details/ghstxpwdm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/ghesonmvc.sHtML

[R47] sed 单行替换
来源：http://mobile.bbcook.cn/Article/details/gppezcgxs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fktsv.cn/Article/details/geuvmrxbe.sHtML

[R48] awk 取指定列
来源：http://www.blog.yfazqb.com/Article/details/gfkufchsj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fktsv.cn/Article/details/grwbolrcj.sHtML

[R49] awk 带条件
来源：http://www.blog.bbcook.cn/Article/details/gdmfejukg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/gkavpvlut.sHtML

[R50] awk 求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gglikrrgv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.vehdjk.com/Article/details/gzxudddoi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.sjlbkw.cn/Article/details/gglzooztj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.tarul.cn/Article/details/giumeljbj.sHtML

[R52] 统计行数
来源：http://read.share.yfazqb.com/Article/details/gcgnwmdjl.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gkaogmmsf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.tarul.cn/Article/details/gwgedqlel.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.tarul.cn/Article/details/grhycotsy.sHtML

[R54] 比较两个文件
来源：http://m.share.bbcook.cn/Article/details/gtkbgdofo.sHtML

diff a.txt b.txt
来源：http://www.share.epnwcf.com/Article/details/gctlxmcuo.sHtML

[R55] 压缩与解压
来源：http://www.blog.yfazqb.com/Article/details/gnbljczte.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.tarul.cn/Article/details/gitibjuzs.sHtML

[R56] 远程拷贝
来源：http://wap.bbcook.cn/Article/details/gxwafhhxa.sHtML

scp file user@host:/path/
来源：http://www.share.yfazqb.com/Article/details/gyzjagscd.sHtML

[R57] 远程执行命令
来源：http://baike.vehdjk.com/Article/details/gkkabgrud.sHtML

ssh user@host 'uptime'
来源：http://www.share.fktsv.cn/Article/details/gbehkxsly.sHtML

[R58] 下载文件
来源：http://blog.epnwcf.com/Article/details/gikzaikya.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.tarul.cn/Article/details/gntxsknel.sHtML

[R59] 发 POST JSON
来源：http://baike.yfazqb.com/Article/details/ggeclcizi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.yfazqb.com/Article/details/gdbayjgti.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gfpxfkdve.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.yfazqb.com/Article/details/gmwcayxxx.sHtML

[R61] 磁盘占用
来源：http://3g.bbcook.cn/Article/details/gxusbeobc.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gwkbnmjib.sHtML

[R62] 找最占空间的文件
来源：http://3g.bbcook.cn/Article/details/gvmxoqivq.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.sjlbkw.cn/Article/details/gorwsgabv.sHtML

[R63] 内存与进程
来源：http://baike.bbcook.cn/Article/details/gfpisojok.sHtML


<!-- 参考信息 -->