代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.tarul.cn/Article/details/gmpntgxcy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gevczozzy.sHtML

[Q13] 忽略重复插入
来源：http://www.share.bbcook.cn/Article/details/gzlktbotz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gvwybtecs.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/glxqiusqg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/ggiowcdjs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gftssnrxh.sHtML

[Q15] 查询全部
来源：http://m.share.tarul.cn/Article/details/gfabkabxl.sHtML

SELECT * FROM users;
来源：http://mobile.yfazqb.com/Article/details/gevgzllfk.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gdzfkrtci.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gfbiundhy.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/garmrhgot.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gaggqsxez.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gzcerzrdc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/gvbgfwmzi.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gqaqwyxgl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/genlkcbas.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gyxtpytzl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/ghxnzbcng.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/ghguenvwz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/gdaknwmsv.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gkvmzomhy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gsjflcdda.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gwnzlhang.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gakipkmca.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gqkdrqooi.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gzxlmhuka.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gcuoexpzj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gxnyfizbn.sHtML

[Q26] 计数
来源：http://wap.fktsv.cn/Article/details/gzmejqcff.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gqetbdcgf.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gzrzozqeb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gtbkaytgu.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/grqrwoaue.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gzyitaygt.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/ggiqjozzn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gfndihutz.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gteknvamc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gbkigulov.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gdurqcezw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gqogvgwki.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gtvjdrijx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/glhkwjmmk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.yfazqb.com/Article/details/guuzqcdwl.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/gjjbjyoof.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/gwnvyemiq.sHtML

[Q34] 每组取第一条
来源：http://mobile.epnwcf.com/Article/details/gwjcogpbt.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gzaffxhjm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/gyzmyuxqz.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gfyfyghvy.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gbeebmfll.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gybvvsbkk.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gbgkekyii.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gcizncodj.sHtML

[Q37] 右连接
来源：http://www.blog.tarul.cn/Article/details/gfbozmdch.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.yfazqb.com/Article/details/gulnbsvoz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.bbcook.cn/Article/details/geagtvndp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/gknnfsxnc.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/goozzjlag.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gotzorlac.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gqkxbggrw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gtfinmqdp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/gefiaicvo.sHtML

[Q41] 多表连接
来源：http://read.share.fktsv.cn/Article/details/gcaswnpuh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.epnwcf.com/Article/details/gnogmqxwx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gvppwhsdq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.sjlbkw.cn/Article/details/gvsaierka.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/gjqxduiuk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.bbcook.cn/Article/details/gthirykmw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.sjlbkw.cn/Article/details/gmtykztzf.sHtML

[Q43] 标量子查询
来源：http://www.share.fktsv.cn/Article/details/gbwvkakij.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.sjlbkw.cn/Article/details/gakftpfrr.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gshoqbgbt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaelbzzfb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.yfazqb.com/Article/details/gelpfjxcb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gtehihrtf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/gwxeaigxp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gkcouyrgy.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gjnudddzw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gyhqqqnsm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.tarul.cn/Article/details/gdtktbkjd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/goaohaezy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gvxmymiza.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gloggswnu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gwgdfsleu.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/goevxjbax.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gsyohedzh.sHtML

[Q51] 用子查询更新
来源：http://3g.vehdjk.com/Article/details/ghbcrnfxa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/glsyufkpq.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/gbyinzqlc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gdmhsdzsr.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gizebvzax.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/ghkipgwkt.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gsyqdesiq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/gzfebawio.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gsxvgxvvn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.vehdjk.com/Article/details/giuooboqt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.bbcook.cn/Article/details/gasmvzurn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gphqvzgaf.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/ggmhymbem.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gsozinybk.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gxlbkytou.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/grwfbfobr.sHtML

[Q59] 分组内累计
来源：http://read.share.vehdjk.com/Article/details/gnhqieobz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gohoqnxwj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gvyyzquti.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gcwtzmkus.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gpuqxfikq.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/ghdujemxf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gotxurjhx.sHtML

[Q62] 分组占比
来源：http://blog.vehdjk.com/Article/details/gtrihutal.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/glrgwjfhi.sHtML

[Q63] 开启事务
来源：http://www.m.share.vehdjk.com/Article/details/gbuveftun.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gqrrdwgcs.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gnzuoxdtx.sHtML

COMMIT;
来源：http://www.m.share.yfazqb.com/Article/details/geflkqqmb.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjrpyyrl.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gqxlicfvb.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gisotfvzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.vehdjk.com/Article/details/gabkqrurx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/guresgxsx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/ghyxaonhm.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gasucudud.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/geqdpfesx.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gqmwiulkc.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gmoayuimt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsfaiwkc.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gbztxruas.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gjefnehmb.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/ggoplzvyl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gvmtwtfgb.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/gjmkutbgu.sHtML

SHOW INDEX FROM users;
来源：http://baike.vehdjk.com/Article/details/gubtxotak.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gtusfxiah.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.tarul.cn/Article/details/ghiagncbk.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gzrajfajj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gdvmnimfy.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gswdkdvwh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gqvzjgoap.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gxoqiiiqb.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gpyrifsli.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/ghztysqmh.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/glujxjxzs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gkmfiwfec.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/ggxwuegrv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gnvvsjvgu.sHtML

[Q79] 字符串拼接
来源：http://3g.vehdjk.com/Article/details/gkxngpzcq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gzvakqtpi.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gipbbeaoe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gjfwpygxf.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/geyljhyjz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfqixxbjg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/grmsvsqdh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gwtoxzkzn.sHtML

[Q83] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gtbevmdjq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gqproazvn.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/gcaomgbgh.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gnukofeui.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gkngnsfkh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gvrblcegc.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/gljkflgyo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.epnwcf.com/Article/details/gsjgrkqvb.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gcjyuxppu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gfyubcofy.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fktsv.cn/Article/details/gmcqmdloj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/gjyxvhmzq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gqxuryctx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gartjqyed.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fktsv.cn/Article/details/gpblpqkhn.sHtML

[Q90] 生成序号列
来源：http://3g.sjlbkw.cn/Article/details/gupkuzahv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.tarul.cn/Article/details/gjwssyrgr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmhetqxnp.sHtML

R. Bash 专题
来源：http://3g.yfazqb.com/Article/details/gszsaezsc.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grmgajwap.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gegurvsrl.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gpbmhihgk.sHtML

set -euo pipefail
来源：http://read.share.yfazqb.com/Article/details/gillrsavr.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gjrnkvkub.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gucxnfpzc.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gqnipfbbt.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gwznursvt.sHtML

[R04] 位置参数
来源：http://baike.bbcook.cn/Article/details/givtnxaxs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.sjlbkw.cn/Article/details/gxehcmpun.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gdwinxmzr.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/gjarugyor.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gefzcjwom.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gsczovidp.sHtML

[R07] if 判断文件
来源：http://wap.vehdjk.com/Article/details/gvfvylzwv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.sjlbkw.cn/Article/details/galpsblqk.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/gukmfnmev.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gimpmsqmg.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gapskhsif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gkkobeuxf.sHtML

[R10] 正则匹配
来源：http://www.blog.bbcook.cn/Article/details/gnqaddbeo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.sjlbkw.cn/Article/details/ghdoeqbiz.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gjmmhitrm.sHtML

case "$1" in
来源：http://m.share.yfazqb.com/Article/details/gtspamsbt.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gyxsrbkhw.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/gvipzbjas.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gsejslaxf.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gthojguex.sHtML

[R12] for 遍历文件
来源：http://m.share.sjlbkw.cn/Article/details/gxjlwfzmx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.tarul.cn/Article/details/gderormrx.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/ggtdtiaod.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.bbcook.cn/Article/details/gtofticge.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/glspegdrw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gimciqlef.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/geujqfmxn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.bbcook.cn/Article/details/gkighjqpr.sHtML

[R16] until 等待条件
来源：http://read.share.vehdjk.com/Article/details/gdacvizkm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.bbcook.cn/Article/details/gqrbyukrc.sHtML

[R17] 数组定义与取值
来源：http://www.share.yfazqb.com/Article/details/gvvvtewao.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.sjlbkw.cn/Article/details/gvghoyjbz.sHtML

[R18] 遍历数组
来源：http://www.blog.yfazqb.com/Article/details/glvikyszv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.tarul.cn/Article/details/gsgzzurdd.sHtML

[R19] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gjvxorjtg.sHtML

echo "${#arr[@]}"
来源：http://blog.fktsv.cn/Article/details/gbvvzabiw.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/gqmtlslbr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.sjlbkw.cn/Article/details/gdbqttaqa.sHtML

[R21] 字符串长度
来源：http://mobile.vehdjk.com/Article/details/gqrhnnbvm.sHtML

echo "${#s}"
来源：http://www.share.tarul.cn/Article/details/gfbgbppgk.sHtML

[R22] 截取子串
来源：http://read.share.sjlbkw.cn/Article/details/gjkxceibn.sHtML

echo "${s:0:5}"
来源：http://www.blog.vehdjk.com/Article/details/ggrgqsvjk.sHtML

[R23] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gffazsnmt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gkhdfrssg.sHtML

[R24] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gvgbktkjq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.yfazqb.com/Article/details/giwupeqcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gbawqsplr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.vehdjk.com/Article/details/gjehlwhcx.sHtML

[R26] 命令替换
来源：http://baike.yfazqb.com/Article/details/gokfrovqp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.vehdjk.com/Article/details/gqkzcmuhs.sHtML

[R27] 算术展开
来源：http://3g.epnwcf.com/Article/details/gkdpqaffz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.vehdjk.com/Article/details/gbpynbjst.sHtML

[R28] 浮点运算
来源：http://baike.bbcook.cn/Article/details/ggeyggvzo.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fktsv.cn/Article/details/glfvpxrkf.sHtML

[R29] 定义函数
来源：http://mobile.epnwcf.com/Article/details/gtcqlvoea.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.tarul.cn/Article/details/gomyavmdd.sHtML

[R30] 函数返回状态码
来源：http://3g.vehdjk.com/Article/details/gqugiofkl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.bbcook.cn/Article/details/geebnubvc.sHtML

[R31] 局部变量
来源：http://www.m.share.sjlbkw.cn/Article/details/geoxvyyis.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gvfwoziap.sHtML

[R32] 参数个数校验
来源：http://read.share.epnwcf.com/Article/details/gzhzqhqhu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.epnwcf.com/Article/details/gcuivkvxv.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.yfazqb.com/Article/details/gtpxwlndy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.epnwcf.com/Article/details/gcdkdohbu.sHtML

[R34] 退出时清理
来源：http://blog.yfazqb.com/Article/details/ggttpgypm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.sjlbkw.cn/Article/details/geihixewa.sHtML

[R35] 后台执行并等待
来源：http://www.share.fktsv.cn/Article/details/gboisffjj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.tarul.cn/Article/details/gctweeqrp.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gibbddwiv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.tarul.cn/Article/details/gugmfnxyx.sHtML

[R37] 把输出赋给变量
来源：http://baike.tarul.cn/Article/details/gtrocglkd.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gnsbkdkdp.sHtML

[R38] 管道串联
来源：http://blog.fktsv.cn/Article/details/gkckbqeba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.sjlbkw.cn/Article/details/gfjtacpmk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.vehdjk.com/Article/details/gacyahans.sHtML

cmd > out.log 2>&1
来源：http://3g.tarul.cn/Article/details/gaoqzknmq.sHtML

[R40] 追加写日志
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvoqkfcg.sHtML

echo "log" >> out.log
来源：http://baike.bbcook.cn/Article/details/gpmenebny.sHtML

[R41] 丢弃输出
来源：http://www.blog.tarul.cn/Article/details/gtcqxuyci.sHtML

cmd >/dev/null 2>&1
来源：http://wap.tarul.cn/Article/details/gjovijbnt.sHtML

[R42] 输入重定向
来源：http://read.share.tarul.cn/Article/details/gpkgmqjan.sHtML

wc -l < a.txt
来源：http://read.share.fktsv.cn/Article/details/glbglyhxh.sHtML

[R43] 按名字查找文件
来源：http://3g.sjlbkw.cn/Article/details/gsedskkit.sHtML

find . -name "*.log" -type f
来源：http://baike.fktsv.cn/Article/details/gypklwvaa.sHtML

[R44] 按修改时间查找
来源：http://read.share.bbcook.cn/Article/details/gaqldcqor.sHtML

find . -mtime -7 -type f
来源：http://3g.vehdjk.com/Article/details/gluywicap.sHtML

[R45] 批量删除
来源：http://blog.sjlbkw.cn/Article/details/grbtsfbim.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.sjlbkw.cn/Article/details/griqoikvi.sHtML

[R46] 递归替换文件内容
来源：http://m.share.sjlbkw.cn/Article/details/gwymldand.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.sjlbkw.cn/Article/details/gjczyhzxg.sHtML

[R47] sed 单行替换
来源：http://3g.bbcook.cn/Article/details/gxamcuxjm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.bbcook.cn/Article/details/gxjjbsykh.sHtML

[R48] awk 取指定列
来源：http://mobile.epnwcf.com/Article/details/gnrwxznfg.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gkrobljhh.sHtML

[R49] awk 带条件
来源：http://read.share.sjlbkw.cn/Article/details/gtejuzikx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.yfazqb.com/Article/details/geleeouir.sHtML

[R50] awk 求和
来源：http://m.share.vehdjk.com/Article/details/gecnukoix.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.vehdjk.com/Article/details/gclquavqq.sHtML

[R51] 排序去重取前几
来源：http://read.share.epnwcf.com/Article/details/ginnhexsi.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.sjlbkw.cn/Article/details/grzsctpap.sHtML

[R52] 统计行数
来源：http://m.share.fktsv.cn/Article/details/ggldxweas.sHtML

wc -l a.txt
来源：http://wap.tarul.cn/Article/details/ggrnymezr.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.tarul.cn/Article/details/gxtbfbkrr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fktsv.cn/Article/details/gqsfixoma.sHtML

[R54] 比较两个文件
来源：http://blog.epnwcf.com/Article/details/gkirpgenh.sHtML

diff a.txt b.txt
来源：http://m.share.epnwcf.com/Article/details/gneatclvc.sHtML

[R55] 压缩与解压
来源：http://wap.tarul.cn/Article/details/gvlumseas.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.sjlbkw.cn/Article/details/ggansnkog.sHtML

[R56] 远程拷贝
来源：http://www.blog.vehdjk.com/Article/details/gessqhrha.sHtML

scp file user@host:/path/
来源：http://wap.tarul.cn/Article/details/gtbllcyea.sHtML

[R57] 远程执行命令
来源：http://blog.yfazqb.com/Article/details/grrvceuhk.sHtML

ssh user@host 'uptime'
来源：http://mobile.sjlbkw.cn/Article/details/gamgwhqhp.sHtML

[R58] 下载文件
来源：http://www.m.share.vehdjk.com/Article/details/gzqqonaas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.tarul.cn/Article/details/gcxlqzhrc.sHtML

[R59] 发 POST JSON
来源：http://mobile.vehdjk.com/Article/details/gwgtjwjuy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.epnwcf.com/Article/details/gpspszmfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.vehdjk.com/Article/details/gtgmahmqg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.bbcook.cn/Article/details/guozgadzv.sHtML

[R61] 磁盘占用
来源：http://wap.bbcook.cn/Article/details/gfytcrodo.sHtML


<!-- 参考信息 -->