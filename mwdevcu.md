代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gxsuwbwew.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/gmtymflqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gjnfmwgrx.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/galbrbvon.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/ghbesqyrs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/glzrpdxuv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gmutrsmpe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.epnwcf.com/Article/details/ghvzhkpri.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.tarul.cn/Article/details/gwfasgutp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.tarul.cn/Article/details/gelbvajyv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gviebnpkz.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gptmetfjf.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gdopsjkqp.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gylqfuihu.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/gngxziqed.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/ggagbgney.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gyxmxcwxp.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gqxrafhqz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.yfazqb.com/Article/details/gdhmorffd.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gxxkzmrun.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gjjtufwqg.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/ggdbrefig.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/grgxswrfi.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gguujhesa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gbpwadjyr.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gsqxjfrrh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gkepjtrfp.sHtML

[Q23] 分页
来源：http://baike.fktsv.cn/Article/details/gswktehgd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fktsv.cn/Article/details/gswhexama.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gfnhobvtr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gwinwvxnq.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gzzfdqsdo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/grzrjfkjd.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gbympxxya.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gpghrxybw.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gjdyawsyu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.bbcook.cn/Article/details/gjjnilqcc.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gwuhxnvtv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gjmvhbupl.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/ghypustlw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gtljqlofx.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gghlkxxaw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gnfvuqitr.sHtML

[Q31] 分组后过滤
来源：http://m.share.fktsv.cn/Article/details/ggiaxuamd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/gytbdmsmy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/ghicfhkrw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gonydnkwe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.vehdjk.com/Article/details/gzdyigzqj.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gqrtloivh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gwbbsajjz.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gvwlnovzk.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gvixnfkvb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gviawsmzp.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/grpmqfxur.sHtML

[Q35] 内连接
来源：http://baike.vehdjk.com/Article/details/gxseuxeaz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gpsyhaguh.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/gckhtszrf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gacspdwzo.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/gqiontrjl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gyecxhhit.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.tarul.cn/Article/details/gfepqunzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gsadetlod.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.tarul.cn/Article/details/ggmeacjit.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/grgoxxyrh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fktsv.cn/Article/details/gunvnbjaw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gmhclnbra.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.epnwcf.com/Article/details/ghbmknatd.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/grhgvjcae.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fktsv.cn/Article/details/ghumrmkxy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.tarul.cn/Article/details/gvaktvrke.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gqeukxtvt.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/gkildiheu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gbrlmwuve.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gezzltmjz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gdowfqwvh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gedwsjrbk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/gfxdqzusm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gneytteon.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gtoslyxsw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/grjjyuseq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gyhisqain.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gxlkkbabp.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/gfexieikz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gkdeocjli.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gpqukokfp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gscmgdfhy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/gxnexvfqb.sHtML

[Q49] 更新单行
来源：http://www.share.sjlbkw.cn/Article/details/gznuzeitw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gsdoxkrke.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gkivwvqsc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.bbcook.cn/Article/details/goxomgxlp.sHtML

[Q51] 用子查询更新
来源：http://m.share.sjlbkw.cn/Article/details/gfikuaeyw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/glffsixvy.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gciffsrek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gxeerfppi.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/gqkrbrypy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gneipvihl.sHtML

[Q54] 清空表
来源：http://read.share.tarul.cn/Article/details/gvvlvmqyw.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gjsptddfc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gvsvjmpfh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/gmrqtktww.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gslsdnsmy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/ghqzwasga.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/ggajfmtcw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gekajcnkl.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/gwuwfrtux.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/geadjmssx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gdgshjuao.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gkdkvhpqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.yfazqb.com/Article/details/gtohjwgrf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/gurjpnpjk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/ggtxmynar.sHtML

[Q61] 移动平均
来源：http://3g.fktsv.cn/Article/details/gqpndntoe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gmxuzucvg.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gmtqykuxl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gnjumweji.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gtlsiaqmn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gotmofbjq.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gwndfaoxk.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gixbuwltn.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/gueihivht.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gksckcled.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/gvimjogxv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gireymogx.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gfclezarb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqsyljtc.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gufxgruil.sHtML

SAVEPOINT sp1;
来源：http://mobile.bbcook.cn/Article/details/gehjmwfjl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gxouipzcc.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gmkbxxwbb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gsinqcrsd.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gpshhqosw.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gyvpbifun.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gyyvvyqvb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gvtgyljxr.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gufasgmjx.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gxbreceui.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gnjlefiky.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.yfazqb.com/Article/details/gnkorrerg.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/gafvwesfm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gbvwaukpp.sHtML

[Q75] 日期格式化
来源：http://m.share.fktsv.cn/Article/details/gnvbnldyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gnpklydxh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fktsv.cn/Article/details/gsdoktmye.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gysnnxeio.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.yfazqb.com/Article/details/gwmsmouvj.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/gmzuzpjeh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/guzgusxtk.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gimjgjqee.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gjduxskjr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fktsv.cn/Article/details/gpqaqqdpm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/glizwckmz.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/gbribrast.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.vehdjk.com/Article/details/giwdcipim.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/guwxytimu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/goswvirla.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fktsv.cn/Article/details/gtbkmthzv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/ggzzsyrip.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gfexubrge.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gzqsaxoba.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gpxfkngpy.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gtxdsqiob.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gicfsleqy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gbiqpacyf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gcuwtgbvz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gztjdafik.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gioladzrx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgsfougv.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gjrebpvcr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fktsv.cn/Article/details/gqkowxkby.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gobsuqbuk.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gvapeefzt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gzbrefxwm.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gcvpjcezc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/gguiipfrf.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/grhhfginc.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gpquevyou.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghfblplhb.sHtML

[R01] shebang 与严格模式
来源：http://blog.bbcook.cn/Article/details/gucyrbjoa.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/guztjsovv.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gvvkrfizq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.yfazqb.com/Article/details/geopxwkdg.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gxbdwiyty.sHtML

[R03] 只读变量
来源：http://m.share.yfazqb.com/Article/details/gqxhxiqfq.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gycycpgmf.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/ggvuijaiv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.tarul.cn/Article/details/grlgaazpd.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/ghtavscpp.sHtML

name="${1:-default}"
来源：http://3g.vehdjk.com/Article/details/gbzrxqyzf.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gypsrehks.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.epnwcf.com/Article/details/grdtgdzgp.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/gksrdiawb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gmllbyxrd.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gnctmrkri.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gyfhsunnr.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/gkyweghdp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.epnwcf.com/Article/details/gsvyyogzp.sHtML

[R10] 正则匹配
来源：http://www.blog.epnwcf.com/Article/details/gbshalzrf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.bbcook.cn/Article/details/gyrhemdtp.sHtML

[R11] case 多分支
来源：http://www.blog.tarul.cn/Article/details/gfshxdvaj.sHtML

case "$1" in
来源：http://m.share.vehdjk.com/Article/details/gzynjoswt.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/gohqhbjgk.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gnamifupk.sHtML

*)     echo "未知命令" ;;
来源：http://3g.sjlbkw.cn/Article/details/gxlsutdww.sHtML

esac
来源：http://www.share.vehdjk.com/Article/details/ghbeqyban.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/gfvinbkul.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/gecsewhgt.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gqnooftfj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.sjlbkw.cn/Article/details/gfuoiqmil.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/geeamjyqj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gbdxuvpxu.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/geamkwcml.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.vehdjk.com/Article/details/gfldtzncf.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/gcxbmlblx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/gzybxslsh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gugcyjiag.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.sjlbkw.cn/Article/details/glptflnta.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gerpmjotm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.bbcook.cn/Article/details/gahhjruhh.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gykhhpgqx.sHtML

echo "${#arr[@]}"
来源：http://m.share.vehdjk.com/Article/details/gjdjdpido.sHtML

[R20] 关联数组（字典）
来源：http://wap.vehdjk.com/Article/details/gxaycqdyg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gslrdqvhe.sHtML

[R21] 字符串长度
来源：http://mobile.epnwcf.com/Article/details/ggaplstki.sHtML

echo "${#s}"
来源：http://baike.bbcook.cn/Article/details/gwhfyuerl.sHtML

[R22] 截取子串
来源：http://baike.bbcook.cn/Article/details/ggdqwkiur.sHtML

echo "${s:0:5}"
来源：http://www.m.share.yfazqb.com/Article/details/gbnmcjyqd.sHtML

[R23] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gtiuxdqbj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.epnwcf.com/Article/details/gwdmjybgi.sHtML

[R24] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gekpbufct.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gkaoqgvpz.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/ggggzsitr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.epnwcf.com/Article/details/gkhvqqtqu.sHtML

[R26] 命令替换
来源：http://www.share.sjlbkw.cn/Article/details/gbddxchug.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gcgjjjzrw.sHtML

[R27] 算术展开
来源：http://wap.fktsv.cn/Article/details/gugascmpo.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fktsv.cn/Article/details/gvgvrihaz.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gxesbdfir.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.yfazqb.com/Article/details/girsoiiwg.sHtML

[R29] 定义函数
来源：http://baike.vehdjk.com/Article/details/gjtmueiqc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.sjlbkw.cn/Article/details/gdpuuvmqe.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gzlhntupv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.sjlbkw.cn/Article/details/gdrpivtzj.sHtML

[R31] 局部变量
来源：http://wap.epnwcf.com/Article/details/gcnrqwkjo.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fktsv.cn/Article/details/gbhwrupot.sHtML

[R32] 参数个数校验
来源：http://read.share.fktsv.cn/Article/details/gaflexumx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/gxbzyqada.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.tarul.cn/Article/details/gwqveasta.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gxnhpxogu.sHtML

[R34] 退出时清理
来源：http://wap.tarul.cn/Article/details/gbvgehxeh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/golqtndbu.sHtML

[R35] 后台执行并等待
来源：http://read.share.fktsv.cn/Article/details/gnkqljuoo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.vehdjk.com/Article/details/gqdovjuoo.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fktsv.cn/Article/details/grqnsmhzq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.sjlbkw.cn/Article/details/gkbeevuke.sHtML

[R37] 把输出赋给变量
来源：http://read.share.bbcook.cn/Article/details/gywhkgupp.sHtML

files=$(ls -1)
来源：http://www.m.share.epnwcf.com/Article/details/gvywsgfkx.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gdktrrsdq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.tarul.cn/Article/details/gzipxmfos.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.bbcook.cn/Article/details/gcnweqzke.sHtML

cmd > out.log 2>&1
来源：http://read.share.sjlbkw.cn/Article/details/gqkxuiovl.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/gpboiiuol.sHtML

echo "log" >> out.log
来源：http://3g.bbcook.cn/Article/details/galeiqsmn.sHtML

[R41] 丢弃输出
来源：http://blog.bbcook.cn/Article/details/geahbckyu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gdhzxjfnq.sHtML

[R42] 输入重定向
来源：http://3g.tarul.cn/Article/details/gdcbyivbq.sHtML

wc -l < a.txt
来源：http://blog.vehdjk.com/Article/details/gocxdfnzb.sHtML

[R43] 按名字查找文件
来源：http://read.share.bbcook.cn/Article/details/gcecjvuie.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gfjywqizb.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gbowvbicn.sHtML

find . -mtime -7 -type f
来源：http://read.share.tarul.cn/Article/details/gorpukvti.sHtML

[R45] 批量删除
来源：http://wap.yfazqb.com/Article/details/gmcpwfruw.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.yfazqb.com/Article/details/gwfnublbs.sHtML

[R46] 递归替换文件内容
来源：http://www.share.epnwcf.com/Article/details/gxqzblfzn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.tarul.cn/Article/details/gwziykpmt.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/grrvjtnne.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.tarul.cn/Article/details/grsoekrio.sHtML

[R48] awk 取指定列
来源：http://wap.tarul.cn/Article/details/gupkazdgb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.vehdjk.com/Article/details/gbyjohadv.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/giqvyzknq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.tarul.cn/Article/details/gurensnlk.sHtML

[R50] awk 求和
来源：http://www.blog.epnwcf.com/Article/details/goranmffx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.epnwcf.com/Article/details/gxisjmiai.sHtML

[R51] 排序去重取前几
来源：http://read.share.tarul.cn/Article/details/ghpzxlirh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.epnwcf.com/Article/details/gwverrerm.sHtML

[R52] 统计行数
来源：http://read.share.sjlbkw.cn/Article/details/gjqcdoidg.sHtML

wc -l a.txt
来源：http://3g.vehdjk.com/Article/details/ggygoaysx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.sjlbkw.cn/Article/details/gttgrjlle.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.sjlbkw.cn/Article/details/gmmvbxkrv.sHtML

[R54] 比较两个文件
来源：http://mobile.tarul.cn/Article/details/gccfelnco.sHtML

diff a.txt b.txt
来源：http://wap.bbcook.cn/Article/details/gughnnjau.sHtML

[R55] 压缩与解压
来源：http://mobile.bbcook.cn/Article/details/gpisswjwn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.yfazqb.com/Article/details/guspbkdnt.sHtML

[R56] 远程拷贝
来源：http://baike.fktsv.cn/Article/details/gayxyfsub.sHtML

scp file user@host:/path/
来源：http://read.share.sjlbkw.cn/Article/details/gmiphdzpr.sHtML

[R57] 远程执行命令
来源：http://read.share.yfazqb.com/Article/details/gtjknistc.sHtML

ssh user@host 'uptime'
来源：http://baike.tarul.cn/Article/details/gpfjzijcc.sHtML

[R58] 下载文件
来源：http://3g.vehdjk.com/Article/details/gmoqobsgc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.epnwcf.com/Article/details/gasyxbpgc.sHtML

[R59] 发 POST JSON
来源：http://m.share.tarul.cn/Article/details/gcomnauru.sHtML


<!-- 参考信息 -->