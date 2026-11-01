代发 wailian999

SELECT * FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gplxkkjac.sHtML

[Q16] 查询指定列
来源：http://www.blog.epnwcf.com/Article/details/gksrlcdst.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/gyhvwcaua.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gtqodrlst.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gztombbgp.sHtML

[Q18] 模糊匹配
来源：http://3g.bbcook.cn/Article/details/glfrshfrc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/guhptjlgc.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gqqxckifw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gxtuuhnne.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gisbxuaja.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gcivtbuuf.sHtML

[Q21] 空值判断
来源：http://www.blog.epnwcf.com/Article/details/glaulwgte.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gkrbuowwo.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gbzhxkvhn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gyecynzhp.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gvcxauiyk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gjyrsikqw.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gnudskakk.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.bbcook.cn/Article/details/gvamhuyxk.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/gbkypflnj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gwaknitly.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/ghsdttxjw.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghzsmnaih.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/gtvowhxbr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gwsbdkpvw.sHtML

[Q28] 求和与平均
来源：http://www.share.tarul.cn/Article/details/gzmmueyki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gqkrxqqyf.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gajeeoojz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gthxafiet.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/gemtqpowx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/goviznkjg.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/glwbgbgjr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gmviwpixb.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gtxubuqtm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gqgandhwg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.yfazqb.com/Article/details/gcvgwhauw.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gihffajty.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gmovktdmq.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/gzrwquxas.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gaspoqkrk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/ghherysyi.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gygifdofd.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/gtsamdkhu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/goimitnce.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gzmtugacr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gcpiiyrdp.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gimzjzgyj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/gvmrllqaw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.tarul.cn/Article/details/gwjzrzxzz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.tarul.cn/Article/details/gdawdorgs.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gxjoxbucn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gbiyafyid.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.yfazqb.com/Article/details/gpiwmcbxu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gnjumdmnb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/goaxddcxd.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gzgqrmerd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/ggmsfaxxd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gjpmgxoaj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/gzmjmzewl.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gevmtzlwg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gbykqwida.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.tarul.cn/Article/details/gwmohaqji.sHtML

[Q43] 标量子查询
来源：http://m.share.vehdjk.com/Article/details/gfbvmxzqs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/grqezydmx.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gpoawfvhx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/grwxleicy.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/ghlmevbqv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gtlvfqdiu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/ghbhmszym.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gjxpispxk.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gcdjbctwp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/gtfhcmxqu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/ghtkusgdj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gbtaaeibs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/ggzzcknmg.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/gltuhyuzt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gvnreyelt.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gesecqkws.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/grkplhvtu.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gizrjfetl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.vehdjk.com/Article/details/gjdyplmih.sHtML

[Q52] 删除指定行
来源：http://www.blog.bbcook.cn/Article/details/gtivpjhyg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gqoydsvlf.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/gqnzcvwpm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gyexaafbe.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gexeczlcd.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/grzqgjjpj.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/gzwjbsgic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.tarul.cn/Article/details/gtnfcfxbi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gakoxrrgr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gkmghajen.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gwbqbdwzw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gooqrvgdn.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/goppxkzmz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gntoarojr.sHtML

[Q59] 分组内累计
来源：http://www.m.share.sjlbkw.cn/Article/details/gqyozehyk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.tarul.cn/Article/details/gfbrljuhi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gzadxhpzv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gthhgnydz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gsxlxfxhk.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/glnccsfrj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gcenqxxph.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/glnevcolp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gtainjbyn.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/ggtcrrsxu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.vehdjk.com/Article/details/gxnwbweot.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gnaepfsab.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gugvcazcs.sHtML

[Q65] 回滚事务
来源：http://m.share.fktsv.cn/Article/details/gkztxdzog.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gqkcyttpn.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gbymvjusb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gybdosdkk.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/gpblewzxm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/ghkmfcgmd.sHtML

[Q68] 保存点
来源：http://www.blog.fktsv.cn/Article/details/glinmkbdj.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/grrleonqw.sHtML

ROLLBACK TO sp1;
来源：http://read.share.tarul.cn/Article/details/gkxaremlm.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/glparcgyp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.yfazqb.com/Article/details/grarhipxd.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/girwixhyu.sHtML

ANALYZE TABLE users;
来源：http://www.share.fktsv.cn/Article/details/giqilffjo.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/ghqchaksk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.tarul.cn/Article/details/gfchfxmmu.sHtML

[Q72] 查看索引
来源：http://blog.sjlbkw.cn/Article/details/gxqydfpgn.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/guxbmsyli.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gklznscpn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gtvxomlzh.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gudkeybye.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gyxtcbykg.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gzzmqhwdp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fktsv.cn/Article/details/gzusphyon.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.yfazqb.com/Article/details/gbnpfezgc.sHtML

[Q76] 按天统计
来源：http://www.share.epnwcf.com/Article/details/gvryglxww.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gzpmokxnm.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gitmzouia.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gmrwtxbna.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gyeydtmwl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.sjlbkw.cn/Article/details/gvgyzcqgg.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gsvpqqius.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gbqwiwxom.sHtML

[Q80] 字符串截取
来源：http://m.share.sjlbkw.cn/Article/details/gdnjhlxqv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/glakyxgzo.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gykhbhtrb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gvfgutmec.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gxobpmpyj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gjqesiihm.sHtML

[Q83] 大小写转换
来源：http://www.share.vehdjk.com/Article/details/gbbjnruph.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/guotddwnt.sHtML

[Q84] 去除首尾空格
来源：http://baike.vehdjk.com/Article/details/gmecvrlvv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gybagkcuv.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gmqpnyudf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/gcgfrterv.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.sjlbkw.cn/Article/details/gsboscgey.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/ggxomsjsc.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gsuvtfpio.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gsgepnypi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gzxjuqamr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gsdjjrwvj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gwfjaumyo.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/gknwdfkpd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gpozoznlv.sHtML

[Q90] 生成序号列
来源：http://blog.vehdjk.com/Article/details/grzmiwcrt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.epnwcf.com/Article/details/gctuhibzb.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvigexecb.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gazztbtpd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gewdhxjop.sHtML

[R01] shebang 与严格模式
来源：http://mobile.tarul.cn/Article/details/goqpbgbrv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gvnzwtcul.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gsjgjnltu.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gdvgbyfgw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gxdrobxta.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/ganqbfqxa.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gckngjnkd.sHtML

[R04] 位置参数
来源：http://3g.fktsv.cn/Article/details/gjswqglpd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.bbcook.cn/Article/details/gosvokrzp.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/glzrvpevv.sHtML

name="${1:-default}"
来源：http://baike.tarul.cn/Article/details/gzsfggexr.sHtML

[R06] 判断命令是否存在
来源：http://m.share.yfazqb.com/Article/details/guyilbumr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/gqlognlqf.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gtkalpcco.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/grltvhyze.sHtML

[R08] 数值比较
来源：http://baike.yfazqb.com/Article/details/gqhcysowx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gwovpgnai.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/goyisleso.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gtsisahqz.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/ghjdgoazx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gjsrzbroi.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/grnqcivft.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gcesotxlv.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/ghyldcvur.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gdebdcunu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.yfazqb.com/Article/details/gveqfsjvv.sHtML

esac
来源：http://m.share.epnwcf.com/Article/details/gxtdmytnx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fktsv.cn/Article/details/gwlvmsltr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gmijysctf.sHtML

[R13] for 计数循环
来源：http://baike.vehdjk.com/Article/details/gvxeqjjdk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gbatxwjyv.sHtML

[R14] C 风格 for
来源：http://3g.bbcook.cn/Article/details/gtriklirk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gvxjsaldg.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gmzsxkcax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/gikiiabvp.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gtvcdkoxi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.sjlbkw.cn/Article/details/gkbfzzykh.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gjgytntib.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gqaefnlmr.sHtML

[R18] 遍历数组
来源：http://www.share.tarul.cn/Article/details/gsvxyioud.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.vehdjk.com/Article/details/gxpkjzoah.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gpdscliry.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/gqwcegfnx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.tarul.cn/Article/details/gkrovtnik.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.vehdjk.com/Article/details/gdopsnmeq.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gtabfpkdp.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gdhifcjgh.sHtML

[R22] 截取子串
来源：http://read.share.fktsv.cn/Article/details/gjenlfxcm.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gkieoqqfq.sHtML

[R23] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gqyqikofc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/grvwsjwyd.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gncywzlzr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gornzodxc.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/gpabcaiyd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gltdyquwt.sHtML

[R26] 命令替换
来源：http://mobile.fktsv.cn/Article/details/gyectonhx.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/gcrcgsxjd.sHtML

[R27] 算术展开
来源：http://mobile.sjlbkw.cn/Article/details/glxxyekcl.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.yfazqb.com/Article/details/galqvjjnp.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/ghrtlhftr.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/gskwhiaxk.sHtML

[R29] 定义函数
来源：http://mobile.bbcook.cn/Article/details/gqhlxsodz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/geqwciozb.sHtML

[R30] 函数返回状态码
来源：http://wap.vehdjk.com/Article/details/ghnelpqec.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/geiybcdjj.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gfxiltphp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gwntbncax.sHtML

[R32] 参数个数校验
来源：http://blog.yfazqb.com/Article/details/gwfveahbs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gophglofj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.bbcook.cn/Article/details/goxbshbvu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.sjlbkw.cn/Article/details/gahlqpxpq.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gzqmavsik.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.vehdjk.com/Article/details/gbkzexwcp.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.vehdjk.com/Article/details/grukfvfjw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fktsv.cn/Article/details/ghkcgkcfy.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/gyrfdputg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.vehdjk.com/Article/details/gpcvdojmb.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fktsv.cn/Article/details/gvrgkyzdt.sHtML

files=$(ls -1)
来源：http://3g.yfazqb.com/Article/details/gbsyylvks.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/gbcggkrww.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.vehdjk.com/Article/details/gdwggwoiw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.epnwcf.com/Article/details/gqnvzjrpe.sHtML

cmd > out.log 2>&1
来源：http://www.share.bbcook.cn/Article/details/glbwretcr.sHtML

[R40] 追加写日志
来源：http://read.share.yfazqb.com/Article/details/gvgufruqu.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/guaigkwke.sHtML

[R41] 丢弃输出
来源：http://baike.yfazqb.com/Article/details/gkhufpnhf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.sjlbkw.cn/Article/details/gysutpsvs.sHtML

[R42] 输入重定向
来源：http://wap.bbcook.cn/Article/details/gioazmznv.sHtML

wc -l < a.txt
来源：http://m.share.tarul.cn/Article/details/gghbahdkt.sHtML

[R43] 按名字查找文件
来源：http://3g.fktsv.cn/Article/details/gpraivnff.sHtML

find . -name "*.log" -type f
来源：http://m.share.epnwcf.com/Article/details/gcfrloeql.sHtML

[R44] 按修改时间查找
来源：http://m.share.yfazqb.com/Article/details/gpujfkemt.sHtML

find . -mtime -7 -type f
来源：http://baike.bbcook.cn/Article/details/gxvqltaol.sHtML

[R45] 批量删除
来源：http://read.share.yfazqb.com/Article/details/golezaymo.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.vehdjk.com/Article/details/gpgxuwxeh.sHtML

[R46] 递归替换文件内容
来源：http://baike.bbcook.cn/Article/details/grhhobyvb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fktsv.cn/Article/details/gbwsykisq.sHtML

[R47] sed 单行替换
来源：http://www.blog.yfazqb.com/Article/details/gihndeetd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.sjlbkw.cn/Article/details/gvcnmscbn.sHtML

[R48] awk 取指定列
来源：http://m.share.bbcook.cn/Article/details/glouuwjjd.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fktsv.cn/Article/details/gcgjuzumt.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gbacgdaaf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.yfazqb.com/Article/details/gpiblltrj.sHtML

[R50] awk 求和
来源：http://mobile.tarul.cn/Article/details/gltndvogy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.vehdjk.com/Article/details/ggqvlcxoh.sHtML

[R51] 排序去重取前几
来源：http://read.share.vehdjk.com/Article/details/gdfoimgdo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.yfazqb.com/Article/details/gbthficml.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gelvfhrlh.sHtML

wc -l a.txt
来源：http://m.share.epnwcf.com/Article/details/gozfcpnto.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.bbcook.cn/Article/details/gpcdsnjyg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gjpodwnxj.sHtML

[R54] 比较两个文件
来源：http://blog.fktsv.cn/Article/details/gvvrclzpi.sHtML

diff a.txt b.txt
来源：http://read.share.tarul.cn/Article/details/gnxsdqiiw.sHtML

[R55] 压缩与解压
来源：http://m.share.epnwcf.com/Article/details/gkkbdcffi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.epnwcf.com/Article/details/gjxrloxpg.sHtML

[R56] 远程拷贝
来源：http://www.m.share.bbcook.cn/Article/details/gtpdauzas.sHtML

scp file user@host:/path/
来源：http://3g.fktsv.cn/Article/details/gmcbhzbda.sHtML

[R57] 远程执行命令
来源：http://3g.epnwcf.com/Article/details/gtqyawffj.sHtML

ssh user@host 'uptime'
来源：http://baike.fktsv.cn/Article/details/gtpfednak.sHtML

[R58] 下载文件
来源：http://3g.fktsv.cn/Article/details/gqvttqwur.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.epnwcf.com/Article/details/gvpjfueku.sHtML

[R59] 发 POST JSON
来源：http://read.share.fktsv.cn/Article/details/ggpyngytl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.tarul.cn/Article/details/gawcfqncs.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gwndskcqf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.yfazqb.com/Article/details/grypfujuh.sHtML

[R61] 磁盘占用
来源：http://www.blog.epnwcf.com/Article/details/gtrscnkhk.sHtML

df -h;  du -sh *
来源：http://m.share.vehdjk.com/Article/details/gkngyipji.sHtML

[R62] 找最占空间的文件
来源：http://mobile.tarul.cn/Article/details/gpprzguue.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.sjlbkw.cn/Article/details/gdngqgoew.sHtML

[R63] 内存与进程
来源：http://3g.fktsv.cn/Article/details/gwucuywfp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.sjlbkw.cn/Article/details/gptpjnxrs.sHtML

[R64] 结束进程
来源：http://3g.vehdjk.com/Article/details/gwkaxxnrd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.sjlbkw.cn/Article/details/gcbrcofkp.sHtML

[R65] 查看端口占用
来源：http://www.m.share.bbcook.cn/Article/details/gqpemxxrb.sHtML


<!-- 参考信息 -->