代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://blog.bbcook.cn/Article/details/gejxpxmnw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.tarul.cn/Article/details/gkliixcti.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/genfvkrhz.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/gvydusjtv.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gudxiejwc.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/ggjxpzjvu.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/ghinnfboo.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/ggzvmdkaf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.tarul.cn/Article/details/glkvlfhzi.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gtklgwlji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/gzqmbtiiw.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gukbseaph.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/gnxsqiggf.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gnxmpwifr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.tarul.cn/Article/details/gpczkincb.sHtML

[Q21] 空值判断
来源：http://3g.tarul.cn/Article/details/grwbaltsm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.yfazqb.com/Article/details/gsxtfmmrr.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/glgmfukmh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/ghcmkbczr.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gbtniiqhe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.epnwcf.com/Article/details/guzsewtgp.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gxdebhisk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fktsv.cn/Article/details/gcplldnnu.sHtML

[Q25] 只取前 N 条
来源：http://3g.fktsv.cn/Article/details/gbymesnqr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gdieadhrb.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/grpidzisy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gltbkcsrx.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/gsrsgvyjo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gyxmvstcw.sHtML

[Q28] 求和与平均
来源：http://3g.vehdjk.com/Article/details/gwnlvvlpb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/giriskfxp.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gzarhrklp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/goxpudbay.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gyswwwobs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gfecuyiyi.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/gbifxnqlx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gjnfyqwiu.sHtML

[Q32] 分组拼接字符串
来源：http://wap.epnwcf.com/Article/details/ghjhuxfhm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/ghdvjvqpq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gybovimim.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gfgrqhldd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzenfnllz.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gdxzjojmn.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gwnkgrgtb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fktsv.cn/Article/details/gyldbybcd.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/gxeovhyoa.sHtML

[Q35] 内连接
来源：http://www.share.epnwcf.com/Article/details/ghrzbmrky.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gsztetncv.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gyrcikmlm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/grsmwzeyt.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gircrabxc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gdypowaeo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/geovaqlgc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.tarul.cn/Article/details/gebsxjexj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.epnwcf.com/Article/details/gpmggxanq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.bbcook.cn/Article/details/gvocgnfmb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.tarul.cn/Article/details/gavacowzg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.yfazqb.com/Article/details/gjyhasiot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/gezipvcik.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gfzplqfyp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.epnwcf.com/Article/details/gngkztgrv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gwqwgtscg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gtlitycfa.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/goclsbjfk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gqpjhakez.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.vehdjk.com/Article/details/gfzcfkkep.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/gesrqzitq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gxoorumne.sHtML

[Q44] IN 子查询
来源：http://blog.vehdjk.com/Article/details/gbrjrmnzj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/gybekrreu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/ggevwtpoi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/glnlqhadx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gdyugkawx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gbnjrslee.sHtML

[Q47] 与平均值比较
来源：http://mobile.tarul.cn/Article/details/gghjnqupg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gykcgjklh.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gbaobfscw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gesuosqdq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/ghvnkpcax.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gjggscrce.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gzeoxkjok.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gedwwzqkv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/ggbbrbsgv.sHtML

[Q51] 用子查询更新
来源：http://m.share.yfazqb.com/Article/details/gnrwqefwi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/ggifisdsp.sHtML

[Q52] 删除指定行
来源：http://www.share.sjlbkw.cn/Article/details/gdxobixfi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/guvuuqwbm.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gscrawrxe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gvgsyvtvb.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gbntqqkuc.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/grcpguide.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gjxgftoqi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gbguzvmmq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/gmzihnfej.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gawswokst.sHtML

[Q57] 行号
来源：http://3g.sjlbkw.cn/Article/details/gxwvyaaxr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/gibwtfofj.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gwizbnpst.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gufehhhai.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gylqiwkxm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gridalwxx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/ggumuslsf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gvykxbjss.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gcbmhxikk.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/guzypbooh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gludsepxc.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/gywdauthf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gntafheco.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/guarbubpp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gjhadsivw.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gpmhaprcm.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/guecngscw.sHtML

[Q65] 回滚事务
来源：http://www.share.fktsv.cn/Article/details/geynwbskg.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/gqoagtxtc.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gcxxtodih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fktsv.cn/Article/details/gyjzfksdy.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gecfbozca.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/gwspkkgxa.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gypfulrad.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gcujvfnym.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gbxjfsxjv.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gmtycxmne.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.bbcook.cn/Article/details/gavzbwydo.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/glfcxvinx.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gilheprhd.sHtML

[Q71] 查看建表语句
来源：http://www.share.bbcook.cn/Article/details/gjxnxoipn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/glckwellx.sHtML

[Q72] 查看索引
来源：http://3g.sjlbkw.cn/Article/details/goowwipkd.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fktsv.cn/Article/details/gqvuufzca.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gsikxbyhk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gomstmqes.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gznpshusw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gxajkswag.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gklvjnmoh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gtrcwohbk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gvshrzgqw.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/goghglthg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.sjlbkw.cn/Article/details/gankmabyx.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gbleeljmi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gizzcobrr.sHtML

[Q78] 当前时间
来源：http://wap.sjlbkw.cn/Article/details/gmupcufnj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/glzypeond.sHtML

[Q79] 字符串拼接
来源：http://3g.tarul.cn/Article/details/gcmkppkmw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.tarul.cn/Article/details/gfzznzcgu.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/gnyszamof.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gaefygyts.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/getjxsscp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwkdyddtk.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/gadbvrnof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gjtiwvcds.sHtML

[Q83] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gzvwknauu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gblfeavcr.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gwtwtofyd.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gtshbwuyq.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gvoozqbbx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gnpqmrccp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gnoyeqsvr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.sjlbkw.cn/Article/details/gezikmhic.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gscwhboov.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gusigdbne.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gxhzqnghe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/guyuynnke.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gglboxkfz.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gvfgbfpdm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/ghwbbdstb.sHtML

[Q90] 生成序号列
来源：http://baike.bbcook.cn/Article/details/gdninkrbw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fktsv.cn/Article/details/gwhujlndi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmzfxwvcw.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gvvobylzc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwvouhzrs.sHtML

[R01] shebang 与严格模式
来源：http://mobile.sjlbkw.cn/Article/details/guxhpvoyt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gazgrcrhg.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/gsoorbqgu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gmmuvhcdf.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/gbkhzhwmu.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gaalsdltt.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gvybyobcz.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gcgkpyaex.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/glegnnpui.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/gocmeqjku.sHtML

name="${1:-default}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhahsiiy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gdtpwjqwp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gpcjvxehb.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gwwdtbqdf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gbbslgvfv.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoizrtjc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/guypleanj.sHtML

[R09] 字符串比较
来源：http://wap.epnwcf.com/Article/details/gxxqqajii.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/gdpherpga.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gvfjaebjf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.vehdjk.com/Article/details/goeiqymas.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gpioovnob.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/gehohnnti.sHtML

start) echo "启动" ;;
来源：http://www.blog.fktsv.cn/Article/details/gcsxsopyi.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gxqveexuz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/giylidmip.sHtML

esac
来源：http://blog.vehdjk.com/Article/details/gqquyfzti.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gtttsvpxf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/gkksufdok.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/glchhegfz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.yfazqb.com/Article/details/gnmhtshbw.sHtML

[R14] C 风格 for
来源：http://wap.epnwcf.com/Article/details/gewbqhzpc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/gfctlkdld.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/grsencodo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gybrlobgu.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gohpgnrwr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gbgpyrkvh.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gtfzirbqz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gbzuslsrs.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/ghfejwtlv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.bbcook.cn/Article/details/gtbrvfynn.sHtML

[R19] 数组长度
来源：http://blog.epnwcf.com/Article/details/gtohgkhfo.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gveoqwoza.sHtML

[R20] 关联数组（字典）
来源：http://www.share.epnwcf.com/Article/details/gghgkbwff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.vehdjk.com/Article/details/gowbmlxjf.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gewhlqrkd.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/glgxumlku.sHtML

[R22] 截取子串
来源：http://baike.tarul.cn/Article/details/geciqzzub.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/gcjmczvaa.sHtML

[R23] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gioludday.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gmvkqtmkz.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/glmmhgifm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/gbsakvqgz.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/gbacbxklt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.tarul.cn/Article/details/gpzslmrsy.sHtML

[R26] 命令替换
来源：http://wap.sjlbkw.cn/Article/details/gxyudppgu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gdsamecmq.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/gjhcjxcfp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gxewmimhn.sHtML

[R28] 浮点运算
来源：http://read.share.tarul.cn/Article/details/gmhjkkjjp.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.tarul.cn/Article/details/grzktyjzc.sHtML

[R29] 定义函数
来源：http://read.share.tarul.cn/Article/details/gdvjplitv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.yfazqb.com/Article/details/guurbpjpj.sHtML

[R30] 函数返回状态码
来源：http://3g.bbcook.cn/Article/details/ggvnuawai.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fktsv.cn/Article/details/gawrvodhc.sHtML

[R31] 局部变量
来源：http://blog.epnwcf.com/Article/details/ggclcfhpx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.yfazqb.com/Article/details/gkubtfjcy.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gyfxqcoux.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/garsfjpla.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gqzymoumv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.tarul.cn/Article/details/gxdajzlyt.sHtML

[R34] 退出时清理
来源：http://3g.sjlbkw.cn/Article/details/gepvdozcy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.tarul.cn/Article/details/ggjbhbtaz.sHtML

[R35] 后台执行并等待
来源：http://www.share.bbcook.cn/Article/details/gddepsjnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.yfazqb.com/Article/details/gcdkqhsww.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gydzmunkh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.vehdjk.com/Article/details/gbywfpxmz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fktsv.cn/Article/details/guevfaqzc.sHtML

files=$(ls -1)
来源：http://m.share.sjlbkw.cn/Article/details/gldnufppi.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/gjhtybzfv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gvcdscgcm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbxtvtgy.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/guiorqbvs.sHtML

[R40] 追加写日志
来源：http://www.blog.tarul.cn/Article/details/gkjscusdc.sHtML

echo "log" >> out.log
来源：http://blog.bbcook.cn/Article/details/gyzcznqjy.sHtML

[R41] 丢弃输出
来源：http://mobile.bbcook.cn/Article/details/giqecixuq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.bbcook.cn/Article/details/gpvvppifd.sHtML

[R42] 输入重定向
来源：http://www.share.sjlbkw.cn/Article/details/glzgroccj.sHtML

wc -l < a.txt
来源：http://wap.yfazqb.com/Article/details/gzhchzbit.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gpumftctk.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.vehdjk.com/Article/details/gavixtgah.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/gqlanaqfi.sHtML

find . -mtime -7 -type f
来源：http://mobile.vehdjk.com/Article/details/gzvzsfvhp.sHtML

[R45] 批量删除
来源：http://read.share.tarul.cn/Article/details/gdxgvnysh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.bbcook.cn/Article/details/ggjdulhvt.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/gjqkgrwjn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.vehdjk.com/Article/details/gstzqoyno.sHtML

[R47] sed 单行替换
来源：http://baike.epnwcf.com/Article/details/gyxwvthlv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gouizvgyw.sHtML

[R48] awk 取指定列
来源：http://www.m.share.yfazqb.com/Article/details/geycgneyx.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.tarul.cn/Article/details/gtyzopgfu.sHtML

[R49] awk 带条件
来源：http://baike.tarul.cn/Article/details/gllqsunzx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.tarul.cn/Article/details/gfbgotppf.sHtML

[R50] awk 求和
来源：http://blog.sjlbkw.cn/Article/details/gaamrbhsa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gprtebjwe.sHtML

[R51] 排序去重取前几
来源：http://blog.vehdjk.com/Article/details/gqxfjtwrk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.epnwcf.com/Article/details/gccclynbh.sHtML

[R52] 统计行数
来源：http://www.share.bbcook.cn/Article/details/gqibndpnv.sHtML

wc -l a.txt
来源：http://www.share.epnwcf.com/Article/details/gdfsunpik.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.tarul.cn/Article/details/gritnfitr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.epnwcf.com/Article/details/gjqrlcobt.sHtML

[R54] 比较两个文件
来源：http://read.share.vehdjk.com/Article/details/gvdaassev.sHtML

diff a.txt b.txt
来源：http://blog.epnwcf.com/Article/details/gyrgiyzpp.sHtML

[R55] 压缩与解压
来源：http://m.share.bbcook.cn/Article/details/gtyvfkvqa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.vehdjk.com/Article/details/gxbstvsnz.sHtML

[R56] 远程拷贝
来源：http://baike.bbcook.cn/Article/details/gnudknshe.sHtML

scp file user@host:/path/
来源：http://wap.vehdjk.com/Article/details/ghtrynmsj.sHtML

[R57] 远程执行命令
来源：http://www.share.sjlbkw.cn/Article/details/gbrnosdzl.sHtML

ssh user@host 'uptime'
来源：http://mobile.fktsv.cn/Article/details/ggduvjzww.sHtML

[R58] 下载文件
来源：http://mobile.tarul.cn/Article/details/gvatinhsl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fktsv.cn/Article/details/gxdqtixls.sHtML

[R59] 发 POST JSON
来源：http://www.blog.tarul.cn/Article/details/gccwqwonb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.sjlbkw.cn/Article/details/ggbsxedjq.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gmsgbsfya.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.bbcook.cn/Article/details/glitazawm.sHtML

[R61] 磁盘占用
来源：http://3g.sjlbkw.cn/Article/details/gejvkcrfy.sHtML

df -h;  du -sh *
来源：http://read.share.tarul.cn/Article/details/gavbqusri.sHtML

[R62] 找最占空间的文件
来源：http://mobile.vehdjk.com/Article/details/ghlrlbtcn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fktsv.cn/Article/details/gniryewtm.sHtML

[R63] 内存与进程
来源：http://baike.tarul.cn/Article/details/gtbphmiai.sHtML


<!-- 参考信息 -->