代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/gmkbixqsh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gzbpqbvol.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/gkzvxbroe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gvadaxmxv.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gglbwvzub.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gdezjqaxz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/gdwpbxhux.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gpdgxscte.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ggqphubau.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gympmarid.sHtML

SELECT id, name FROM users;
来源：http://blog.fktsv.cn/Article/details/gzledetij.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gjqsnxlsi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fktsv.cn/Article/details/ggnuvsidx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.yfazqb.com/Article/details/gbxtaabji.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/ggvwcnrbu.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/galkexdff.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.yfazqb.com/Article/details/gtkcechnk.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gibajgaij.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gpjxfgtgj.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gtvkevnvy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fktsv.cn/Article/details/goopbctwp.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gfnfbiqqe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/giynjdnxv.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/gtigzjqzd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/gubtmyiah.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gwprzsbut.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/grlcoowuc.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gokadxbpy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gkyhtqkkn.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/gxmzaipfh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gwcqxlibx.sHtML

[Q27] 条件计数
来源：http://mobile.epnwcf.com/Article/details/gkhncfjer.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/gwjbzokml.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gehorzqje.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/ggwnwujol.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gydjguyms.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gvhsdynxt.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gkeanehqz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gaftvslao.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/gninbysik.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/gbcuprbwb.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fktsv.cn/Article/details/gthdujtzn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gdiofdmrl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.vehdjk.com/Article/details/gsyhkjfud.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/gtbkkflvl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gcbrhllit.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gbqnlxefs.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/gouqwhygb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gedusdior.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/glsycsruc.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gqurdjems.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/grcobmuyq.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gleyzajdr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gbwyzyrzi.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gljrkpwqa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fktsv.cn/Article/details/guzosxtbe.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fktsv.cn/Article/details/gcuvnolhv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gkdgwpsih.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.bbcook.cn/Article/details/gkldriyfc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/gurledjoq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gdlwjjzxo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.yfazqb.com/Article/details/gnlgqcqwm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.vehdjk.com/Article/details/gxntxngem.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gpnxocbsi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/gxlkmhxis.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gilaxhuky.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.tarul.cn/Article/details/gvlhajnuo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gouxrrfrb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/guxsxzswp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/gqyzvibed.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gbhgviwiq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gkipwsbct.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/gycszdwsq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.bbcook.cn/Article/details/gujkbidaf.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.tarul.cn/Article/details/gusygafqo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gcjdnnvni.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gnllxglde.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gibfwyqzm.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gpiuwiend.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gjfmsrhor.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.sjlbkw.cn/Article/details/gflqzvbwa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gjgnvrmhh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gaaijmbxf.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/ghikscovs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gtzfmfvqd.sHtML

[Q50] 批量更新
来源：http://www.m.share.tarul.cn/Article/details/guonmkflw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gddpcjejd.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gtkikywso.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/gpsvqewsd.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gmjxcvjrv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/gmiqitkcq.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/ghlomujje.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/giwlkgscs.sHtML

[Q54] 清空表
来源：http://wap.yfazqb.com/Article/details/gdhbgkgjk.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/gpdkoyliu.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gwfdhelzc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmyntvpfp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.sjlbkw.cn/Article/details/gficstcpj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gbrjsmqtw.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gpgtflktx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/ghxctpyxm.sHtML

[Q58] 累计求和
来源：http://read.share.epnwcf.com/Article/details/giqsnydte.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gfhnckauv.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gulsuuyat.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gjsiifcxx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gzlbwubgn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.bbcook.cn/Article/details/ggakxpwjf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/gtyftprpp.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwxyvktd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/ggvrdexwu.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gjxfvwimi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gzfbtrisn.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gfzyplqdj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gljfokhfj.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gphlinepo.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gatdpuniq.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gtfzokdbh.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/guwgphfrc.sHtML

[Q66] 行锁查询
来源：http://www.blog.tarul.cn/Article/details/gbrflxfys.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/guofuyibx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/gentshaci.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.vehdjk.com/Article/details/gwhmmsheg.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/ggwqgyvjy.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gpfmoeuxm.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/grvqytxje.sHtML

[Q69] 查看执行计划
来源：http://blog.vehdjk.com/Article/details/gsiqaffxd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.yfazqb.com/Article/details/gpddymkws.sHtML

[Q70] 更新统计信息
来源：http://blog.sjlbkw.cn/Article/details/gpcujeigu.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gbpazsziz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.bbcook.cn/Article/details/ghpjzhufo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.vehdjk.com/Article/details/gxgkfoarh.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/ggnybhvok.sHtML

SHOW INDEX FROM users;
来源：http://blog.yfazqb.com/Article/details/gbndddeqk.sHtML

[Q73] 查看表状态
来源：http://wap.sjlbkw.cn/Article/details/gqwqwkyyr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/gifrtikgc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.sjlbkw.cn/Article/details/gdgiahtbk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/grbzsptjk.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gtvnqapzy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gfcjqfrdb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.vehdjk.com/Article/details/gfvawtiml.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gksrgiayc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.epnwcf.com/Article/details/gitlgsegh.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gchfcatlf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/gtvdxdwhs.sHtML

[Q78] 当前时间
来源：http://3g.sjlbkw.cn/Article/details/gmhgvpyns.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gxvzlgwdj.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gmiathqqm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.bbcook.cn/Article/details/geaaqxjqj.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gweecysad.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/grobtbxhu.sHtML

[Q81] 字符串替换
来源：http://baike.bbcook.cn/Article/details/gmtbmdhue.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/gpkfaszjr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/ghptvzpsa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/guurusogf.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gleqagugq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gzzblyatr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/ggewjonmr.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/grbplluza.sHtML

[Q85] 数值取整
来源：http://www.share.tarul.cn/Article/details/gtgvjbmyc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.yfazqb.com/Article/details/godpzyjjz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gqgsdzxjw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gyecihduq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gyudhiipd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gutvqkzhn.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.epnwcf.com/Article/details/gkhzjyfck.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/glqbqelkg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqucltogx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/guantlqwe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gqlwtxogg.sHtML

[Q90] 生成序号列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhuhfpwq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/givrkrwgq.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggdebzygg.sHtML

R. Bash 专题
来源：http://www.share.tarul.cn/Article/details/gdfvovmky.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gutjbfemw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gzfxxakug.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gnllltrvb.sHtML

set -euo pipefail
来源：http://www.blog.bbcook.cn/Article/details/gacqbqaer.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gaqheiyii.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.epnwcf.com/Article/details/gqsjeeixf.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gizongoun.sHtML

readonly PI=3.14
来源：http://www.share.vehdjk.com/Article/details/gbwuhlalz.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/gkctmbdxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gcptiebac.sHtML

[R05] 参数默认值
来源：http://www.m.share.fktsv.cn/Article/details/gjtgjlhkf.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/guvokkwts.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/gwjiocjgg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.epnwcf.com/Article/details/gxixpiuyt.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/geykrgrvt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.epnwcf.com/Article/details/gymlucvey.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/gtheisnlp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/geqrehpky.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gzzcaiddr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/ghwgobahe.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/ggrqdcnkh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/grzhftzfs.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gbpjrwaoe.sHtML

case "$1" in
来源：http://read.share.epnwcf.com/Article/details/glqfmbmxx.sHtML

start) echo "启动" ;;
来源：http://m.share.fktsv.cn/Article/details/guinbxzok.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/ghkrgvesj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.bbcook.cn/Article/details/gyneciauv.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/gypqbekxl.sHtML

[R12] for 遍历文件
来源：http://m.share.bbcook.cn/Article/details/giqixjbla.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.bbcook.cn/Article/details/gqbtrvhgy.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/glcgfvquq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gaqaivpbh.sHtML

[R14] C 风格 for
来源：http://m.share.tarul.cn/Article/details/gamcjyefm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gvihtdnub.sHtML

[R15] while 逐行读文件
来源：http://mobile.fktsv.cn/Article/details/gsublzrib.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.yfazqb.com/Article/details/glnebartc.sHtML

[R16] until 等待条件
来源：http://read.share.epnwcf.com/Article/details/gpcvtccpd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gtgqldjum.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/ghtskzrtx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.vehdjk.com/Article/details/glctlgujb.sHtML

[R18] 遍历数组
来源：http://read.share.sjlbkw.cn/Article/details/gkvdutaec.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fktsv.cn/Article/details/gowikhosj.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gckfskgyj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.yfazqb.com/Article/details/gwxoaqwto.sHtML

[R20] 关联数组（字典）
来源：http://m.share.vehdjk.com/Article/details/gxleziebi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.epnwcf.com/Article/details/gkwszzgwi.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gbwkljtzl.sHtML

echo "${#s}"
来源：http://3g.tarul.cn/Article/details/gxpqmrrbs.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/grbfoioru.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/ghaztrdik.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gofmycokk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyqhwirx.sHtML

[R24] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/ggvyvnxog.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fktsv.cn/Article/details/gruaiunum.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.vehdjk.com/Article/details/glsjodcjz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.sjlbkw.cn/Article/details/gneqoissr.sHtML

[R26] 命令替换
来源：http://read.share.epnwcf.com/Article/details/gohgisdwm.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.epnwcf.com/Article/details/gydnnqpzp.sHtML

[R27] 算术展开
来源：http://m.share.fktsv.cn/Article/details/ghnouuvhc.sHtML

echo $((1 + 2 * 3))
来源：http://baike.tarul.cn/Article/details/gzsvextwv.sHtML

[R28] 浮点运算
来源：http://www.share.vehdjk.com/Article/details/gosrsblsa.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gquwhuwus.sHtML

[R29] 定义函数
来源：http://baike.bbcook.cn/Article/details/ggdugfbbf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.sjlbkw.cn/Article/details/gfflxpdtb.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/gubosouyl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.epnwcf.com/Article/details/geohlmydv.sHtML

[R31] 局部变量
来源：http://3g.yfazqb.com/Article/details/gngdmncgj.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.tarul.cn/Article/details/gjwuxrwku.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gtvflinar.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.vehdjk.com/Article/details/gauldjtvn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.epnwcf.com/Article/details/gqeyzijbh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.bbcook.cn/Article/details/gxozhrosp.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gwsqqxfbx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gmvapnrwi.sHtML

[R35] 后台执行并等待
来源：http://blog.fktsv.cn/Article/details/gljszlbtw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.tarul.cn/Article/details/gvdinnlwm.sHtML

[R36] 并发执行多个任务
来源：http://baike.sjlbkw.cn/Article/details/gkgjtwwdn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.vehdjk.com/Article/details/gbtklitvs.sHtML

[R37] 把输出赋给变量
来源：http://baike.sjlbkw.cn/Article/details/gimbpfhtk.sHtML

files=$(ls -1)
来源：http://3g.bbcook.cn/Article/details/gsoredkbc.sHtML

[R38] 管道串联
来源：http://blog.vehdjk.com/Article/details/gbtuakilu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fktsv.cn/Article/details/gfxgenins.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fktsv.cn/Article/details/gfgzqouzd.sHtML

cmd > out.log 2>&1
来源：http://www.share.epnwcf.com/Article/details/gybsjktkt.sHtML

[R40] 追加写日志
来源：http://wap.tarul.cn/Article/details/gyavrninp.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gegyyqmkg.sHtML

[R41] 丢弃输出
来源：http://www.blog.yfazqb.com/Article/details/gepmwheds.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.vehdjk.com/Article/details/gokzymiwj.sHtML

[R42] 输入重定向
来源：http://mobile.yfazqb.com/Article/details/gxaflhxso.sHtML

wc -l < a.txt
来源：http://www.share.bbcook.cn/Article/details/gjrxdiyqj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gbjoqixvm.sHtML

find . -name "*.log" -type f
来源：http://3g.sjlbkw.cn/Article/details/gkpkyylwz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fktsv.cn/Article/details/giypgowxh.sHtML

find . -mtime -7 -type f
来源：http://blog.bbcook.cn/Article/details/gxsaxbgur.sHtML

[R45] 批量删除
来源：http://blog.tarul.cn/Article/details/gizjcadte.sHtML

find . -name "*.tmp" -delete
来源：http://blog.epnwcf.com/Article/details/gqoyvnffy.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gwxjuqusu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.bbcook.cn/Article/details/ggnajrext.sHtML

[R47] sed 单行替换
来源：http://read.share.epnwcf.com/Article/details/gzxiedttq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.tarul.cn/Article/details/gqfxnqlxu.sHtML

[R48] awk 取指定列
来源：http://blog.bbcook.cn/Article/details/ggwuhjpss.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.sjlbkw.cn/Article/details/gwliwatah.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/guoiwwzho.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.vehdjk.com/Article/details/gostfiwbv.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/gbuqthdxk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.bbcook.cn/Article/details/gvfplsgrl.sHtML

[R51] 排序去重取前几
来源：http://www.share.fktsv.cn/Article/details/gvatuinir.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.tarul.cn/Article/details/ggnfudpzq.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gjufrlqgq.sHtML

wc -l a.txt
来源：http://mobile.yfazqb.com/Article/details/gdtnsijpd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.vehdjk.com/Article/details/gvjkmqkuw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.yfazqb.com/Article/details/gdhxzvdff.sHtML

[R54] 比较两个文件
来源：http://mobile.bbcook.cn/Article/details/gdenekgrb.sHtML

diff a.txt b.txt
来源：http://mobile.fktsv.cn/Article/details/gecgklqai.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gwctkwpfb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/gasitbixo.sHtML

[R56] 远程拷贝
来源：http://www.blog.bbcook.cn/Article/details/gaaurfxaw.sHtML

scp file user@host:/path/
来源：http://www.m.share.vehdjk.com/Article/details/gsqsppajn.sHtML

[R57] 远程执行命令
来源：http://www.m.share.vehdjk.com/Article/details/gidxzknyy.sHtML

ssh user@host 'uptime'
来源：http://m.share.tarul.cn/Article/details/gpkjcsvxs.sHtML

[R58] 下载文件
来源：http://www.blog.fktsv.cn/Article/details/ggduqvimt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.sjlbkw.cn/Article/details/ggzlefpss.sHtML

[R59] 发 POST JSON
来源：http://baike.fktsv.cn/Article/details/gkatbqelx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.yfazqb.com/Article/details/gxpduxruf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gvrcwtkoe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.epnwcf.com/Article/details/gnoxzscrj.sHtML

[R61] 磁盘占用
来源：http://m.share.sjlbkw.cn/Article/details/gbhsjbvww.sHtML


<!-- 参考信息 -->