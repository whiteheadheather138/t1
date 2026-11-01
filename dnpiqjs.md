代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.m.share.yfazqb.com/Article/details/glhxmapgd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.bbcook.cn/Article/details/gybkbetid.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/gyoweshuz.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/gphqjiaic.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmmfftuyg.sHtML

[Q16] 查询指定列
来源：http://wap.yfazqb.com/Article/details/gokengnoa.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gydjjtuqh.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/guipfhtyh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gzvrrgton.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/ggazdgsrz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/grwvxupxa.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gcyhavckt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gnvyqxmjn.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gfxebumnd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gykcwkhja.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gzxccpdzx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gdnogsogc.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/giczryojd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/gukfvcxkd.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/guuepbtkd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gupizhfrb.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/glyhivrjk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gjykukxgx.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gslhxsaxa.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gmxbihzuf.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/grisgngac.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gyeipxuiw.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gdtaqjlkt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gacdxjzwm.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/gtmwycskt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gsrqjvjhs.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gfpqdksiv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/grouwpvgb.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/guhpttfbv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/galdknhli.sHtML

[Q31] 分组后过滤
来源：http://www.share.tarul.cn/Article/details/gnuwilfdo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/giuguhztm.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gsrvgmsyr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gbivrgdwh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gwxapbfqi.sHtML

[Q33] 多列分组
来源：http://read.share.epnwcf.com/Article/details/gpndkfjer.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gejrjquqn.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrbdafzo.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gvgmfbawe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gcvcitbsu.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/gwbeldeiy.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/ghaqzzici.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/ghugekxan.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/glhwjkqly.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/guwczhxus.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gfcgqnheu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/gmnorsizu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/garieaaoh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.tarul.cn/Article/details/gqdoqudti.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/gmmogpxjm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gvqiockgg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gocutealq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gjhhlxasj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/ggxdlaudf.sHtML

[Q41] 多表连接
来源：http://m.share.sjlbkw.cn/Article/details/gclkqznke.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gvdcentgc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/gcxtxiojl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gxqbbppea.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gcntetpxf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/galkxegrb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gnfwxgalh.sHtML

[Q43] 标量子查询
来源：http://read.share.yfazqb.com/Article/details/gsyovksbq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gbkppcyan.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gogdryvij.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.tarul.cn/Article/details/gctrfuxup.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gpmncjbbj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gqkjjalho.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gvmdcmkvl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gpkcircev.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/girdiaqbo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fktsv.cn/Article/details/gattrhflr.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gzxsjsdgy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.tarul.cn/Article/details/gnffrorai.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gormantvt.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gwmbcrviq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gtakwabjb.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gckhoybmn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/geujhwinh.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/ghbiyovjn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/ghzujjtrr.sHtML

[Q52] 删除指定行
来源：http://wap.vehdjk.com/Article/details/gaorkntqa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/grjuggaug.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gukkkbhqa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiewuchp.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gexsyzhic.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gwgklxsyb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gdkmeoodm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/gllkeehmp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.yfazqb.com/Article/details/gqyzcebme.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gjmizvalg.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/gbyfoawfr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/ggqhpwdjg.sHtML

[Q58] 累计求和
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtytxwcc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/guwletpmb.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/gkswozuwf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/ggassmwgl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gbwvcgdmy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/glnimtaap.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.bbcook.cn/Article/details/glwixjofk.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gqagydjyu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gogrujnul.sHtML

[Q62] 分组占比
来源：http://m.share.vehdjk.com/Article/details/gwxurdkld.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gplomfygn.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/guegmyfua.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gelnkezym.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/gdigadsfg.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gwiauerte.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/gehljajop.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/ghrufcliz.sHtML

[Q66] 行锁查询
来源：http://mobile.tarul.cn/Article/details/ghxxmcjtv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gryfhoulh.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gdkuingyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gjxzydmmd.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/griivdjpv.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gyikgmwef.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/glgjccsir.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gerlyorfj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/gljfvikca.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gkxwpxuos.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gmxdbujxq.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gdvyhkrbu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/grifmvdyj.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/gwnoozxib.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/girwcstgt.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/ghrnrtict.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gbnupnvej.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gpptjxtda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/ghjthiroc.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/gfmexdptn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmwexgjjb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.bbcook.cn/Article/details/gfcoldous.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gdseldjfv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gmprelmvv.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/gkdlfklob.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/gretgrhvl.sHtML

[Q78] 当前时间
来源：http://blog.tarul.cn/Article/details/guhowckny.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.vehdjk.com/Article/details/gqlkposai.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/geqefmtyo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.bbcook.cn/Article/details/geresbace.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gxmrnphto.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fktsv.cn/Article/details/gyvtzzorw.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gippeiben.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxgxdpago.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gntmgvjof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gmixjsgmx.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gnxpoqslp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/giktdlyul.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gmyjyxuzh.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gorikgmrk.sHtML

[Q85] 数值取整
来源：http://www.blog.bbcook.cn/Article/details/gewhimrff.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gorbkacqd.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/goifwnfpy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gnugbyoav.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.tarul.cn/Article/details/glgwjvuhu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.yfazqb.com/Article/details/gpkvriwtu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.tarul.cn/Article/details/gfugbjbmg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/gktbntpnd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gvdulgqtl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gfglinjjb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/gsdsqfsca.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gbhkkleoy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.epnwcf.com/Article/details/gazayceqt.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghwhfyexz.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gxovdfcnm.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcdfyuydq.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gxzvrhlai.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/guvdtqrcc.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gsezyxggj.sHtML

[R02] 变量赋值与使用
来源：http://blog.vehdjk.com/Article/details/gcjbwtykt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gifnnjsxn.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gxwewqfbb.sHtML

readonly PI=3.14
来源：http://mobile.fktsv.cn/Article/details/grioazyrt.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gcfzcbzcv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gdfonfotc.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gorbmuapj.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/gzmykzelu.sHtML

[R06] 判断命令是否存在
来源：http://3g.tarul.cn/Article/details/gibrfvtfv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/giwyhxjle.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gkckyaipf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/gvlrlqrkl.sHtML

[R08] 数值比较
来源：http://www.m.share.epnwcf.com/Article/details/gfykcdlxt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gownmlxgy.sHtML

[R09] 字符串比较
来源：http://3g.fktsv.cn/Article/details/gnzelulic.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/geaesmfid.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/guddofoyc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/ggqkdakou.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gmjrsiidx.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gxexayyqd.sHtML

start) echo "启动" ;;
来源：http://wap.tarul.cn/Article/details/gsjuiuayz.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gvxgdzrme.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gayblcprj.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/gjhksoxth.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gsrzojlhh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gggatdvef.sHtML

[R13] for 计数循环
来源：http://baike.bbcook.cn/Article/details/gepyydmdq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gicqspzop.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gfiagwofx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gwllznoie.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/geojwkqle.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fktsv.cn/Article/details/gakyzoztp.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/golkravfv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.sjlbkw.cn/Article/details/ggnsjrmdt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gqklsutzc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.vehdjk.com/Article/details/ghzkhbdah.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/ghcmzxjno.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fktsv.cn/Article/details/grvoyhutj.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gkbryyrec.sHtML

echo "${#arr[@]}"
来源：http://blog.tarul.cn/Article/details/gtenbiavl.sHtML

[R20] 关联数组（字典）
来源：http://baike.sjlbkw.cn/Article/details/gaaujshhd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.tarul.cn/Article/details/gbjamhlhd.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gamguefyb.sHtML

echo "${#s}"
来源：http://www.blog.yfazqb.com/Article/details/gyswmniao.sHtML

[R22] 截取子串
来源：http://www.share.sjlbkw.cn/Article/details/gmumrwuua.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/grdqlvjft.sHtML

[R23] 字符串替换
来源：http://wap.yfazqb.com/Article/details/guvanrowk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gqhxruelh.sHtML

[R24] 大小写转换
来源：http://www.share.epnwcf.com/Article/details/gktbmssem.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.vehdjk.com/Article/details/glkyyxuvz.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.tarul.cn/Article/details/gkiuxqhaq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.tarul.cn/Article/details/gwolgtdxl.sHtML

[R26] 命令替换
来源：http://baike.sjlbkw.cn/Article/details/gpzrkgsaq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.bbcook.cn/Article/details/gbfwwhsvt.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gchizjhas.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/glwqtimrk.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gvshcfzbd.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.tarul.cn/Article/details/ghqxdrzps.sHtML

[R29] 定义函数
来源：http://www.blog.vehdjk.com/Article/details/gfbunldey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gvkbxdghv.sHtML

[R30] 函数返回状态码
来源：http://www.blog.tarul.cn/Article/details/gwhorccjv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.yfazqb.com/Article/details/gbuinoeyc.sHtML

[R31] 局部变量
来源：http://www.m.share.yfazqb.com/Article/details/gcvfifuoy.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.epnwcf.com/Article/details/gykjnbxar.sHtML

[R32] 参数个数校验
来源：http://mobile.vehdjk.com/Article/details/gjlqjkulk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gtbgtzxln.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.sjlbkw.cn/Article/details/guncafyam.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.tarul.cn/Article/details/gtzfgvuit.sHtML

[R34] 退出时清理
来源：http://www.m.share.bbcook.cn/Article/details/geybeofvv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.epnwcf.com/Article/details/gqcvarpmd.sHtML

[R35] 后台执行并等待
来源：http://3g.fktsv.cn/Article/details/gldfhsvlx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.epnwcf.com/Article/details/ghvbsssqo.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gdijorpdu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fktsv.cn/Article/details/gilvsprgr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.tarul.cn/Article/details/gsrbbgcix.sHtML

files=$(ls -1)
来源：http://www.blog.sjlbkw.cn/Article/details/gnqmmnspu.sHtML

[R38] 管道串联
来源：http://3g.epnwcf.com/Article/details/gkhhlpqba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.bbcook.cn/Article/details/gluavoycp.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.bbcook.cn/Article/details/gxvhyghzd.sHtML

cmd > out.log 2>&1
来源：http://www.share.yfazqb.com/Article/details/gswzfyvjl.sHtML

[R40] 追加写日志
来源：http://baike.vehdjk.com/Article/details/gtfyhhlha.sHtML

echo "log" >> out.log
来源：http://m.share.yfazqb.com/Article/details/gzednkwwc.sHtML

[R41] 丢弃输出
来源：http://3g.sjlbkw.cn/Article/details/glxlulthw.sHtML

cmd >/dev/null 2>&1
来源：http://blog.sjlbkw.cn/Article/details/gppnfegep.sHtML

[R42] 输入重定向
来源：http://3g.sjlbkw.cn/Article/details/guntsuumw.sHtML

wc -l < a.txt
来源：http://wap.epnwcf.com/Article/details/gnuqckthw.sHtML

[R43] 按名字查找文件
来源：http://blog.vehdjk.com/Article/details/gxtqabdis.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.yfazqb.com/Article/details/gmdlfrert.sHtML

[R44] 按修改时间查找
来源：http://blog.yfazqb.com/Article/details/gawlikxpj.sHtML

find . -mtime -7 -type f
来源：http://www.share.epnwcf.com/Article/details/gdifwefvq.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gbnhkcoep.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/gywqvazth.sHtML

[R46] 递归替换文件内容
来源：http://wap.yfazqb.com/Article/details/garvkbwwy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.tarul.cn/Article/details/guizlwyio.sHtML

[R47] sed 单行替换
来源：http://read.share.vehdjk.com/Article/details/ghgamwqvy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.epnwcf.com/Article/details/giloozyuh.sHtML

[R48] awk 取指定列
来源：http://3g.bbcook.cn/Article/details/gtkwkeoug.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.sjlbkw.cn/Article/details/gbgnihxje.sHtML

[R49] awk 带条件
来源：http://baike.vehdjk.com/Article/details/gnfimggea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.epnwcf.com/Article/details/gwjsicyxp.sHtML

[R50] awk 求和
来源：http://www.m.share.epnwcf.com/Article/details/gejiurxih.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.bbcook.cn/Article/details/gsmvktuhm.sHtML

[R51] 排序去重取前几
来源：http://read.share.fktsv.cn/Article/details/gyeyvacnj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.tarul.cn/Article/details/ghnctunca.sHtML

[R52] 统计行数
来源：http://m.share.bbcook.cn/Article/details/gmpgzuene.sHtML

wc -l a.txt
来源：http://3g.sjlbkw.cn/Article/details/gpclfbvyu.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.epnwcf.com/Article/details/gbwfvitbu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.yfazqb.com/Article/details/gmjcbgwez.sHtML

[R54] 比较两个文件
来源：http://m.share.sjlbkw.cn/Article/details/gaivsegjh.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gzfhdzsga.sHtML

[R55] 压缩与解压
来源：http://3g.fktsv.cn/Article/details/guxnvjpii.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fktsv.cn/Article/details/ghoegdvyn.sHtML

[R56] 远程拷贝
来源：http://www.share.vehdjk.com/Article/details/gxyqgszal.sHtML

scp file user@host:/path/
来源：http://wap.fktsv.cn/Article/details/gjjhlxqlp.sHtML

[R57] 远程执行命令
来源：http://wap.vehdjk.com/Article/details/gqroqhkqy.sHtML

ssh user@host 'uptime'
来源：http://blog.vehdjk.com/Article/details/gvuopalqi.sHtML

[R58] 下载文件
来源：http://blog.vehdjk.com/Article/details/gxntapinz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.tarul.cn/Article/details/gtldpmdde.sHtML

[R59] 发 POST JSON
来源：http://mobile.tarul.cn/Article/details/gooxhvpue.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fktsv.cn/Article/details/gvibytxpi.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.bbcook.cn/Article/details/gprdruouh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fktsv.cn/Article/details/gymsqgzqx.sHtML

[R61] 磁盘占用
来源：http://blog.fktsv.cn/Article/details/gbfwaephx.sHtML

df -h;  du -sh *
来源：http://m.share.yfazqb.com/Article/details/guaxusupw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.epnwcf.com/Article/details/gjykksaiy.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.sjlbkw.cn/Article/details/gdspswdso.sHtML

[R63] 内存与进程
来源：http://m.share.sjlbkw.cn/Article/details/gijvyifzt.sHtML


<!-- 参考信息 -->