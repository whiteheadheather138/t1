代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.vehdjk.com/Article/details/gdpgbucvt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gxvfxouei.sHtML

[Q13] 忽略重复插入
来源：http://wap.sjlbkw.cn/Article/details/gyhkrphdg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gedhsyvuf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/ghzrhzigw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gbelflvzk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.sjlbkw.cn/Article/details/gpwmaeijo.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/grqntdjzj.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gpxyylvmz.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/geqkimltg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/glteapnzg.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gqmqcewyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.yfazqb.com/Article/details/gmfeeolto.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/guxqbgsjl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gkvnbjpsd.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gdyqmbvjb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gowzcyucx.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/glceeriwf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.bbcook.cn/Article/details/gchretvfu.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/gscaoswun.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gqmoiaria.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/guwsqrhnt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gzxzuexae.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/ggmnhmylb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gztgwnxdt.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/gpuknbdok.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.vehdjk.com/Article/details/gefmvqrtb.sHtML

[Q25] 只取前 N 条
来源：http://wap.yfazqb.com/Article/details/gtkntjwgh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gghmmviaz.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/glvlrrakj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gjpggdmyy.sHtML

[Q27] 条件计数
来源：http://read.share.epnwcf.com/Article/details/gjufwfpww.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/genrlkysp.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/glowzbfeg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gptawrgyb.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/glkzpvxzt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.yfazqb.com/Article/details/gxvmwfbsa.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/gybroitcm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/glggdwkrc.sHtML

[Q31] 分组后过滤
来源：http://wap.sjlbkw.cn/Article/details/gyiihhbaj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gornzrxmd.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gjxcokcfr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gdnclsmgt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gfijnqnlz.sHtML

[Q33] 多列分组
来源：http://www.blog.yfazqb.com/Article/details/gtcflynhv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/guucunkiq.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gpadaeawy.sHtML

SELECT * FROM (
来源：http://blog.epnwcf.com/Article/details/ggokijzfg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.tarul.cn/Article/details/ggspbsqyz.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/glgrtxmsm.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gssvdoyol.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/grchaqcnm.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gafrhlevt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/ggtxduelm.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/grzhyviav.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gigiclqdr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gigaqybtg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/ghlozoogi.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.sjlbkw.cn/Article/details/gnwaxywpd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.bbcook.cn/Article/details/goievxytr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/gjyvvxqpk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/gapazckbl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/gpbeizogt.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gspqccskw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/gahmrhtds.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/gsixdzilq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gmlphzufx.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/gtwcykflc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.epnwcf.com/Article/details/glflnussf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/gviapyzlo.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/goeozbhwx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.epnwcf.com/Article/details/gbrxgbrzx.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/ghhxhtchv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/goomcvajo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gcnmcgnov.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/ggogcveqn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/gedvktjcm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/gmfkpejzq.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gzriswjxt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.epnwcf.com/Article/details/gzjwivgzl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/ghkzoojsc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/gaepufsmk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/glpzaqsxk.sHtML

[Q49] 更新单行
来源：http://baike.tarul.cn/Article/details/gzsqryyrh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gyfyygzev.sHtML

[Q50] 批量更新
来源：http://www.blog.tarul.cn/Article/details/gztquahwf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/guoffdarp.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gnunzqeae.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fktsv.cn/Article/details/gsphxivhi.sHtML

[Q52] 删除指定行
来源：http://www.share.tarul.cn/Article/details/gxuluypuu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gvcwljjny.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gnaiwiape.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gbkkezwzc.sHtML

[Q54] 清空表
来源：http://mobile.sjlbkw.cn/Article/details/grhjaqatt.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.yfazqb.com/Article/details/gtjvmghnc.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gztsrjcqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gqsfggzay.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.sjlbkw.cn/Article/details/gbkogfbfo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gizxznlxq.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/gbxbytmvl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/ggcijxpfx.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gemldkrvl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/ginlxrahq.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/geedpldxk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gfgzegwfn.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.vehdjk.com/Article/details/giimgzvdz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gpehtxuov.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gofqddnnb.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/gwsjwucez.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gdptpiunq.sHtML

[Q62] 分组占比
来源：http://wap.fktsv.cn/Article/details/glpgluibz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gbadmiqsa.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gclqaxtmp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/genzoppjm.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/gcywxvixf.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/ginjscwqx.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/glukjomis.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/grcgkqqkr.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/ghbkklcek.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxyfvyoq.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gjhigiuqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/gpdsziivg.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gaiocokbu.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.tarul.cn/Article/details/gtxrzznhh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gctcmfjvm.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gqlzmkjxl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gizxktzed.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.yfazqb.com/Article/details/gqrvdrnme.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gjljhwidg.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/getcucuxt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gckglruxf.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gwxdbgpvx.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gspnnrknd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/ggxhgsysq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gpepvlcto.sHtML

[Q74] 强制使用索引
来源：http://read.share.vehdjk.com/Article/details/gytjocifw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gyhypeipe.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gvspydqhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ghohavvto.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gqlclztvs.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/gcrrsoukz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gsusbepes.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gsrsnnrzb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/gafsdbnla.sHtML

[Q78] 当前时间
来源：http://www.share.bbcook.cn/Article/details/gbfmavlho.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.vehdjk.com/Article/details/gyoubjsvo.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/gxqjhjdsy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/glklghsgs.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/gqfpcrofm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gxtuieilb.sHtML

[Q81] 字符串替换
来源：http://3g.bbcook.cn/Article/details/ghtzuqfzb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.bbcook.cn/Article/details/glnjkhzha.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fktsv.cn/Article/details/glxbzskqz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gofcgygvj.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gkifndkqk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gueidmykk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gjeevorrl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gaqnugneb.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gcvvwxsun.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fktsv.cn/Article/details/gqozzyfkz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/gptwrreua.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.yfazqb.com/Article/details/gnkbucpsb.sHtML

[Q87] JSON 字段做条件
来源：http://baike.sjlbkw.cn/Article/details/gkwmrnkxf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fktsv.cn/Article/details/gpxlqmkjb.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/grqrzrtqj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gtduzjmco.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.tarul.cn/Article/details/gwkghaxek.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gaghfrxao.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.vehdjk.com/Article/details/gwymchysn.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/ghligkqmm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.tarul.cn/Article/details/gmuglxbry.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gboqmqvjv.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/govirfsdj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glcefnjpl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gmlmfexog.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/glnymgaru.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gvuyabwto.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/greefkxja.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/guqcygrhw.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gnttxuywh.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/ggejcheru.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gsdyhazeh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.tarul.cn/Article/details/ghqqscmxn.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/grlsltsur.sHtML

name="${1:-default}"
来源：http://baike.sjlbkw.cn/Article/details/gthvrrueb.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/goqturzbl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gexbaekbl.sHtML

[R07] if 判断文件
来源：http://www.m.share.fktsv.cn/Article/details/gffzomstq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/glstmdwkb.sHtML

[R08] 数值比较
来源：http://blog.epnwcf.com/Article/details/gcdswktso.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gnwezuphy.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/geduyuhbu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gwkqpqves.sHtML

[R10] 正则匹配
来源：http://www.m.share.epnwcf.com/Article/details/gbhokesrv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/gakzilmqa.sHtML

[R11] case 多分支
来源：http://baike.bbcook.cn/Article/details/gjprsnyzm.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gjhpvxish.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gmrfcwomu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/glaihoofh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fktsv.cn/Article/details/geumbbsdv.sHtML

esac
来源：http://www.share.sjlbkw.cn/Article/details/gzppucewj.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gehfgzhqz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.vehdjk.com/Article/details/gtcnchmye.sHtML

[R13] for 计数循环
来源：http://www.blog.epnwcf.com/Article/details/goyoxvfon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fktsv.cn/Article/details/gjjuamddr.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gklyqljcg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.epnwcf.com/Article/details/glhvehqqp.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gpettnmqa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/gssqucidr.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gdfddrqjb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.tarul.cn/Article/details/gjbftpoyk.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/ggfrmrhzo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.epnwcf.com/Article/details/gbcvtzxqf.sHtML

[R18] 遍历数组
来源：http://m.share.bbcook.cn/Article/details/gfdlbethr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.yfazqb.com/Article/details/gebrgpcin.sHtML

[R19] 数组长度
来源：http://3g.epnwcf.com/Article/details/gueynxgkz.sHtML

echo "${#arr[@]}"
来源：http://m.share.yfazqb.com/Article/details/gxtdqwgis.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fktsv.cn/Article/details/gvkohtaqy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gwnywhhtg.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gbmsndmiq.sHtML

echo "${#s}"
来源：http://www.m.share.bbcook.cn/Article/details/gyrnidmwq.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gjxkdezqj.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gsuzogozr.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gaiycusbn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gersebflj.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gtfkvaqwe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.epnwcf.com/Article/details/gbinpgihm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.bbcook.cn/Article/details/goejieqgu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.vehdjk.com/Article/details/gtvfphssu.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/gezpvifcs.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.epnwcf.com/Article/details/gdaqfkrsb.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/gvuxqrmmw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.bbcook.cn/Article/details/gcucohdzy.sHtML

[R28] 浮点运算
来源：http://m.share.fktsv.cn/Article/details/gfgacoiul.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.tarul.cn/Article/details/gkettokcx.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/ghacawkdv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.vehdjk.com/Article/details/gzzuqjrhe.sHtML

[R30] 函数返回状态码
来源：http://m.share.bbcook.cn/Article/details/gikcnanfv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyvyjadsn.sHtML

[R31] 局部变量
来源：http://read.share.vehdjk.com/Article/details/ghqgxrknk.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.bbcook.cn/Article/details/gqurqlwct.sHtML

[R32] 参数个数校验
来源：http://mobile.vehdjk.com/Article/details/gdvpzawxp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gjblnhtpg.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.vehdjk.com/Article/details/gxfwdgkpl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fktsv.cn/Article/details/gyjrufked.sHtML

[R34] 退出时清理
来源：http://mobile.bbcook.cn/Article/details/gdqjgnenu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fktsv.cn/Article/details/ghulqxvew.sHtML

[R35] 后台执行并等待
来源：http://3g.yfazqb.com/Article/details/gsdefepjm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.tarul.cn/Article/details/glzqigoyc.sHtML

[R36] 并发执行多个任务
来源：http://blog.vehdjk.com/Article/details/ghfrlnsuz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.vehdjk.com/Article/details/gdgaudxlt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fktsv.cn/Article/details/guotdcpqh.sHtML

files=$(ls -1)
来源：http://blog.sjlbkw.cn/Article/details/gqvazoyoi.sHtML

[R38] 管道串联
来源：http://3g.yfazqb.com/Article/details/ggrsqsnxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.vehdjk.com/Article/details/gkkyzuarj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/gbqrruomq.sHtML

cmd > out.log 2>&1
来源：http://3g.fktsv.cn/Article/details/godxbsqbe.sHtML

[R40] 追加写日志
来源：http://3g.sjlbkw.cn/Article/details/gzchpvezt.sHtML

echo "log" >> out.log
来源：http://wap.yfazqb.com/Article/details/ggcmngwwx.sHtML

[R41] 丢弃输出
来源：http://3g.yfazqb.com/Article/details/gnuahjteq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.yfazqb.com/Article/details/gzpxzebuy.sHtML

[R42] 输入重定向
来源：http://blog.epnwcf.com/Article/details/gerzjrgfa.sHtML

wc -l < a.txt
来源：http://blog.tarul.cn/Article/details/gwvqnijqt.sHtML

[R43] 按名字查找文件
来源：http://m.share.epnwcf.com/Article/details/gtgnoyuww.sHtML

find . -name "*.log" -type f
来源：http://baike.epnwcf.com/Article/details/gajvvxecx.sHtML

[R44] 按修改时间查找
来源：http://3g.yfazqb.com/Article/details/gdbqjsspj.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fktsv.cn/Article/details/gpmxegvqb.sHtML

[R45] 批量删除
来源：http://blog.vehdjk.com/Article/details/gqerbkwbb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.sjlbkw.cn/Article/details/gtygieeen.sHtML

[R46] 递归替换文件内容
来源：http://mobile.vehdjk.com/Article/details/ghjbrlywd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.tarul.cn/Article/details/gegtnzdza.sHtML

[R47] sed 单行替换
来源：http://wap.tarul.cn/Article/details/gglwlocmp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fktsv.cn/Article/details/gptjonnel.sHtML

[R48] awk 取指定列
来源：http://m.share.sjlbkw.cn/Article/details/gdikshccl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gflvytktn.sHtML

[R49] awk 带条件
来源：http://m.share.vehdjk.com/Article/details/gsajdykky.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.sjlbkw.cn/Article/details/gxwywzifu.sHtML

[R50] awk 求和
来源：http://3g.tarul.cn/Article/details/gzmisbysm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.bbcook.cn/Article/details/gqqpnsvkg.sHtML

[R51] 排序去重取前几
来源：http://3g.tarul.cn/Article/details/ggocyjady.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.epnwcf.com/Article/details/gpswipgbn.sHtML

[R52] 统计行数
来源：http://www.m.share.epnwcf.com/Article/details/gzrxpltlc.sHtML

wc -l a.txt
来源：http://3g.epnwcf.com/Article/details/gkzrpqkte.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.yfazqb.com/Article/details/gdisxkigg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.bbcook.cn/Article/details/gwoqaetsm.sHtML

[R54] 比较两个文件
来源：http://read.share.sjlbkw.cn/Article/details/gqlymiybw.sHtML

diff a.txt b.txt
来源：http://www.blog.bbcook.cn/Article/details/gslksxrnc.sHtML

[R55] 压缩与解压
来源：http://blog.epnwcf.com/Article/details/gayjoucmx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fktsv.cn/Article/details/glbmyewkv.sHtML

[R56] 远程拷贝
来源：http://www.share.epnwcf.com/Article/details/gdinhcljv.sHtML

scp file user@host:/path/
来源：http://blog.vehdjk.com/Article/details/gdeclamwk.sHtML

[R57] 远程执行命令
来源：http://wap.yfazqb.com/Article/details/gmfyknpib.sHtML

ssh user@host 'uptime'
来源：http://blog.fktsv.cn/Article/details/geuvowupc.sHtML

[R58] 下载文件
来源：http://read.share.fktsv.cn/Article/details/gwlouqxcd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.yfazqb.com/Article/details/girbqiufd.sHtML

[R59] 发 POST JSON
来源：http://www.share.bbcook.cn/Article/details/gnnjdkaib.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fktsv.cn/Article/details/gnuyipxdr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gmvrjxzmj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fktsv.cn/Article/details/gpazudqgd.sHtML

[R61] 磁盘占用
来源：http://3g.epnwcf.com/Article/details/gumlbkzrf.sHtML


<!-- 参考信息 -->