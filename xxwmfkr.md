代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gaujbfnsm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.bbcook.cn/Article/details/grjbrkcsk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gmktjwjyc.sHtML

[Q15] 查询全部
来源：http://www.blog.sjlbkw.cn/Article/details/gayctrtfm.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gwqkrjhas.sHtML

[Q16] 查询指定列
来源：http://blog.vehdjk.com/Article/details/ghxwkxnev.sHtML

SELECT id, name FROM users;
来源：http://wap.vehdjk.com/Article/details/gljmmjmqi.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gvkhtvojc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gmodxmdpu.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.yfazqb.com/Article/details/gppxhucrv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gudmqyoqn.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gtarkpxqj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.bbcook.cn/Article/details/gbzthacpm.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gedawgfyo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gpnkqygzu.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gwtlwsnlp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gyfwevbiv.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gvradtxjk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.sjlbkw.cn/Article/details/grejmupyq.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/gznfmdbzg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/gcghamxtr.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/gdqqlckeg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.yfazqb.com/Article/details/gafgdsarr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/glnaohvbl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/gtydghpnk.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/ggcaekbkl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gudpwrjsk.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gqyhbzphj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gdznoecif.sHtML

[Q28] 求和与平均
来源：http://baike.yfazqb.com/Article/details/gtjrtocmy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gbmpiwgqe.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gibaxspuk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqvnwfbpp.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gllleqblt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gbudrrqsl.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/guhaqkdqy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.vehdjk.com/Article/details/gorccuocf.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gntfbykdg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gpzykvnhh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gpruwiiav.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/gmwjhukan.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.bbcook.cn/Article/details/gojtfgdcw.sHtML

[Q34] 每组取第一条
来源：http://wap.sjlbkw.cn/Article/details/gwaswoobk.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/gectzxhwj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gozvwrwlj.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gcmnvlepi.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gssvqilig.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gmwewqdpl.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/gxysrxvfq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gsbdwhhly.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gzjkygglp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/gktxefkuu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/ghvqeijid.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fktsv.cn/Article/details/gsmsfgxkh.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/gnulcemxu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gpajpyfqv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gpspilxha.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gsafadihp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.sjlbkw.cn/Article/details/gjlfetjjh.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/gzwdqiwtb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.tarul.cn/Article/details/ghclxhsvh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gkincvkpm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/gnjpcbmwq.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/ghjazeuuc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.tarul.cn/Article/details/gsvvlyvll.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.sjlbkw.cn/Article/details/gbcwxflui.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/goldqrjky.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gsxewkohd.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gnwbezjxh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/gyidbffhx.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.tarul.cn/Article/details/gtgjmolpe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gwoqecqvh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.yfazqb.com/Article/details/ggkmtdrjb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/ghfuckzch.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/giubzxbkw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gnpainlek.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gqhsdzhop.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gugwlcdyt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.bbcook.cn/Article/details/grnygznuz.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gijojqyzz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gpuxnwokz.sHtML

[Q50] 批量更新
来源：http://3g.fktsv.cn/Article/details/gnbovpked.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gxczgaccp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gnirtyqgd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gzaivxidv.sHtML

[Q52] 删除指定行
来源：http://wap.vehdjk.com/Article/details/gufpjkhjy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gtjvktiyf.sHtML

[Q53] 按条件删除
来源：http://www.share.yfazqb.com/Article/details/gllwqiydt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.tarul.cn/Article/details/gexnhyglb.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gyqsjzbxk.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/gawuiqicy.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/genbavpwe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/guiqevhsp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.yfazqb.com/Article/details/giqvioszc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/gxtfeseex.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/ghgpqjboz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gfwinwkoj.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gjflxyhaw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.tarul.cn/Article/details/gmssukxoj.sHtML

[Q59] 分组内累计
来源：http://www.blog.sjlbkw.cn/Article/details/gpfncbmyg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gzcvwmttc.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gpitenaku.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gewgcsqdr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/goijadioe.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gmylxxcjz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/glfqsotcc.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/ghsmvyzpb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/grurjxrbt.sHtML

[Q63] 开启事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gozmlauls.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gtxjdyzoz.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/gvrfkbgtl.sHtML

COMMIT;
来源：http://m.share.epnwcf.com/Article/details/gbalxmjuy.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/grmqqjaxz.sHtML

ROLLBACK;
来源：http://m.share.tarul.cn/Article/details/gsasyjgrg.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/gnyaylkrg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gsfheurog.sHtML

[Q67] 设置隔离级别
来源：http://mobile.vehdjk.com/Article/details/gvbdwvfpy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/grbqxqbhe.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gxgqzqivr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.tarul.cn/Article/details/gfhqbelba.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gyftrqkow.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gogkvctqw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gtpakdqby.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gsxdxpght.sHtML

ANALYZE TABLE users;
来源：http://read.share.tarul.cn/Article/details/gjlbdnvht.sHtML

[Q71] 查看建表语句
来源：http://wap.sjlbkw.cn/Article/details/grtbmyryj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gpxhzlust.sHtML

[Q72] 查看索引
来源：http://www.blog.tarul.cn/Article/details/gvfnjythp.sHtML

SHOW INDEX FROM users;
来源：http://m.share.tarul.cn/Article/details/guwvctwmw.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gvdawkwlj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/ghxgbahhq.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gdkusdsej.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gdzgyaotn.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gxbxwjrca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gjypleejl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.tarul.cn/Article/details/gyyojydep.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/gajigtmxu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.bbcook.cn/Article/details/gdmllsvsn.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gewfmsgkt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fktsv.cn/Article/details/girqwbvht.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/gdkmjsgry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/gkgudgidj.sHtML

[Q79] 字符串拼接
来源：http://3g.epnwcf.com/Article/details/gixbycgok.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/gckwpsuuz.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/grsguqdws.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/grdqqkfnc.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gccnqizvn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gukednpfd.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/ggbeucggb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/ghnutuqrq.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gxxwbcjhv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmleczjsv.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/gcteupqxz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gigwqvbnb.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gpqhvdgko.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.tarul.cn/Article/details/ghotodymt.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/guoryippv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.bbcook.cn/Article/details/gkgdbsrwb.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.sjlbkw.cn/Article/details/ggmhlhpqk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gspufopqf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.vehdjk.com/Article/details/gvewjzosn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gxgsjyiyn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/golzfvhwa.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gvybtyiun.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gaxsiwouu.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fktsv.cn/Article/details/guzzkwmqv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gjdfekhmz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gtutnptvz.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gdzakxsor.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gjbnmenrf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gfrcefqli.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/gtsmszwgp.sHtML

set -euo pipefail
来源：http://www.m.share.tarul.cn/Article/details/gbngoxvnd.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gzmcchxjc.sHtML

name="Tom"; echo "$name"
来源：http://blog.sjlbkw.cn/Article/details/gdqihcztq.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/ggaokandq.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/gszetxfuz.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gdpaoilks.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.vehdjk.com/Article/details/gexqeieco.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/ghaprljlm.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/glmxwgysg.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gmdszdwma.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gapfkklfy.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/grhhfdwmm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gmkrarzyl.sHtML

[R08] 数值比较
来源：http://3g.bbcook.cn/Article/details/gnmsdywrm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/gtizevrzi.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gxwcitovw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gwnlluges.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/gulwaivbf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.epnwcf.com/Article/details/glhcjmhrc.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gxrbobthx.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/ghyjrbalg.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gaslsvils.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.bbcook.cn/Article/details/gfuovsxpl.sHtML

*)     echo "未知命令" ;;
来源：http://baike.bbcook.cn/Article/details/gardprfie.sHtML

esac
来源：http://mobile.sjlbkw.cn/Article/details/gfnannwud.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/ghldjviuy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/gjtsmaeqc.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/gmhlojehg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.tarul.cn/Article/details/gijkiwsev.sHtML

[R14] C 风格 for
来源：http://read.share.bbcook.cn/Article/details/gznvljivc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gyuhfhmac.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/ggxwsajel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/gpghncfqk.sHtML

[R16] until 等待条件
来源：http://blog.epnwcf.com/Article/details/gseojjkzs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.tarul.cn/Article/details/ghnobfvgh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/grvihvezb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gfiwbatyc.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gbcsdxoar.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fktsv.cn/Article/details/gwflkcftk.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gmttewjmo.sHtML

echo "${#arr[@]}"
来源：http://blog.sjlbkw.cn/Article/details/gxzazlrgz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/ghsoovisk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.sjlbkw.cn/Article/details/gsewohydx.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/gomvjluwn.sHtML

echo "${#s}"
来源：http://baike.fktsv.cn/Article/details/gisjrsjbr.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/gznyjdgja.sHtML

echo "${s:0:5}"
来源：http://m.share.fktsv.cn/Article/details/gqkvpkngz.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gaodkjptt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/glkxeduug.sHtML

[R24] 大小写转换
来源：http://m.share.epnwcf.com/Article/details/gejmzribf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gtdnobxhx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.yfazqb.com/Article/details/gpfpfvucs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.yfazqb.com/Article/details/gzhcydibi.sHtML

[R26] 命令替换
来源：http://3g.bbcook.cn/Article/details/gemijvmvt.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.tarul.cn/Article/details/gbbzmmbro.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gbhwbapnt.sHtML

echo $((1 + 2 * 3))
来源：http://wap.epnwcf.com/Article/details/gexelvzfv.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gfmkuhdnj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.bbcook.cn/Article/details/gnjdrgawb.sHtML

[R29] 定义函数
来源：http://wap.fktsv.cn/Article/details/ghrlbzcrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/glhuqzyuw.sHtML

[R30] 函数返回状态码
来源：http://mobile.bbcook.cn/Article/details/ghkqkjwvj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gjyduaqnf.sHtML

[R31] 局部变量
来源：http://www.share.sjlbkw.cn/Article/details/gfletkick.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.tarul.cn/Article/details/goidxqsaq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.tarul.cn/Article/details/glvlmmtmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gkhdknivb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.sjlbkw.cn/Article/details/gpymysled.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.sjlbkw.cn/Article/details/gsdfawszt.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gvbtmbjjk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fktsv.cn/Article/details/gluwpebdp.sHtML

[R35] 后台执行并等待
来源：http://www.share.tarul.cn/Article/details/gfaumyfiy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.epnwcf.com/Article/details/gueisroxr.sHtML

[R36] 并发执行多个任务
来源：http://wap.sjlbkw.cn/Article/details/gutzfrxvs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gtegodtpz.sHtML

[R37] 把输出赋给变量
来源：http://m.share.epnwcf.com/Article/details/gxaiglyut.sHtML

files=$(ls -1)
来源：http://m.share.bbcook.cn/Article/details/grrwatgmm.sHtML

[R38] 管道串联
来源：http://www.share.vehdjk.com/Article/details/grxdlpwkd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrtladqk.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.bbcook.cn/Article/details/grdqguqel.sHtML

cmd > out.log 2>&1
来源：http://baike.yfazqb.com/Article/details/grjsodqdd.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gcosvvagk.sHtML

echo "log" >> out.log
来源：http://blog.fktsv.cn/Article/details/gbnasyxwz.sHtML

[R41] 丢弃输出
来源：http://3g.bbcook.cn/Article/details/gtwtoonel.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.tarul.cn/Article/details/gbruolhcc.sHtML

[R42] 输入重定向
来源：http://baike.epnwcf.com/Article/details/gqbynpmap.sHtML

wc -l < a.txt
来源：http://3g.yfazqb.com/Article/details/gmnkzahnp.sHtML

[R43] 按名字查找文件
来源：http://www.share.epnwcf.com/Article/details/gnpvmbgfo.sHtML

find . -name "*.log" -type f
来源：http://wap.sjlbkw.cn/Article/details/gnfpbigaf.sHtML

[R44] 按修改时间查找
来源：http://blog.fktsv.cn/Article/details/gopkogxnm.sHtML

find . -mtime -7 -type f
来源：http://baike.yfazqb.com/Article/details/gtzglhrzr.sHtML

[R45] 批量删除
来源：http://www.share.epnwcf.com/Article/details/gmyvpveor.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fktsv.cn/Article/details/goljipfsa.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.bbcook.cn/Article/details/ghknpcvsz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/ghuwuksxt.sHtML

[R47] sed 单行替换
来源：http://blog.fktsv.cn/Article/details/gyfjcriwu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gxtovmozl.sHtML

[R48] awk 取指定列
来源：http://3g.tarul.cn/Article/details/gzepkvwlt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.tarul.cn/Article/details/gdwtfdqpr.sHtML

[R49] awk 带条件
来源：http://read.share.epnwcf.com/Article/details/grppvzele.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.tarul.cn/Article/details/gxpnnzzxk.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/goavixtkb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fktsv.cn/Article/details/ggpdcsuos.sHtML

[R51] 排序去重取前几
来源：http://wap.epnwcf.com/Article/details/gvcmnqrar.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.vehdjk.com/Article/details/girdhcrcs.sHtML

[R52] 统计行数
来源：http://www.share.vehdjk.com/Article/details/guxrkfhtj.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/gwryntggq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.tarul.cn/Article/details/gircyuksg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fktsv.cn/Article/details/grsviwjzv.sHtML

[R54] 比较两个文件
来源：http://baike.vehdjk.com/Article/details/gjqnwxafq.sHtML

diff a.txt b.txt
来源：http://read.share.vehdjk.com/Article/details/gownqqoyd.sHtML

[R55] 压缩与解压
来源：http://3g.sjlbkw.cn/Article/details/giyiccbli.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.tarul.cn/Article/details/gaeyifvty.sHtML

[R56] 远程拷贝
来源：http://wap.yfazqb.com/Article/details/gcsurqhvb.sHtML

scp file user@host:/path/
来源：http://m.share.tarul.cn/Article/details/grpsvwxeh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsvahggm.sHtML

ssh user@host 'uptime'
来源：http://m.share.yfazqb.com/Article/details/gpvtwzvfn.sHtML

[R58] 下载文件
来源：http://blog.tarul.cn/Article/details/gjknthmbj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.bbcook.cn/Article/details/gqauzgdnd.sHtML

[R59] 发 POST JSON
来源：http://blog.epnwcf.com/Article/details/gzgiwjwel.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.tarul.cn/Article/details/gnridgpdr.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gigglkgrw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.sjlbkw.cn/Article/details/ggccfkxtd.sHtML

[R61] 磁盘占用
来源：http://blog.tarul.cn/Article/details/gltaevgyh.sHtML

df -h;  du -sh *
来源：http://www.blog.tarul.cn/Article/details/gpinhwrzn.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.epnwcf.com/Article/details/gymsdzjbj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.yfazqb.com/Article/details/ghxcisbgp.sHtML

[R63] 内存与进程
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrrrzrlx.sHtML


<!-- 参考信息 -->