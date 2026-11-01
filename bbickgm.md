代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gxurghrjs.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.yfazqb.com/Article/details/gycfqmlio.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gxjbbscbo.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gxvgfydtq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/giwusjrwu.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gnlysvvko.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.epnwcf.com/Article/details/gljkvyhmc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gqlftnril.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gznqrirsa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/glbkskror.sHtML

[Q13] 忽略重复插入
来源：http://blog.yfazqb.com/Article/details/gfsxdolel.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gldqzjjle.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/gwdgwjkby.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gvqzgnigw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gxkhqywqu.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gpyrehdwo.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/golftdhqy.sHtML

[Q16] 查询指定列
来源：http://blog.sjlbkw.cn/Article/details/ggjtspzjo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfnxajgap.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gttlnxfhi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gbflefsja.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gbvugmugb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gdhnhkbpf.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/gzzyhcwvo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/glouabjjb.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gzxftonvx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.epnwcf.com/Article/details/ggtfnvyre.sHtML

[Q21] 空值判断
来源：http://baike.tarul.cn/Article/details/gfzmtufcn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/glfevukqc.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gnaasdccu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gcnlidxdq.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/ggdndrmax.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gquafzlfr.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/gkumofnwc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gxdyvidoz.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/gntsnkatm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gzddfqhuk.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gkxlvabie.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gzkafbytp.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gthluiohb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gpmdtggvl.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/ghrxyfevx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gjpicpzjh.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/grkzmqatj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gfdcxcfkt.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/goyordesl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gsspsvqhb.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gkinomzkn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxxpmnli.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gbsfsglsn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/grwgadgvy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fktsv.cn/Article/details/gksyiobvv.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/gqlbswvld.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.yfazqb.com/Article/details/gllhptoci.sHtML

[Q34] 每组取第一条
来源：http://read.share.fktsv.cn/Article/details/gkttwtmcb.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gjewcesfa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/gpnrvmwcb.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gkxjjmyjp.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gfipjtpuj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gagtbgkfx.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/gelcgykcv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gvyauolzm.sHtML

[Q37] 右连接
来源：http://read.share.bbcook.cn/Article/details/glbwcupxc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gpyxvowzf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gkwpndjqo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gxyzfdxjl.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gzlytqyrh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.epnwcf.com/Article/details/gxrlnupvn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gwxqqnehe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gtznhqmdz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/grqxuyokg.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gjcnduhix.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fktsv.cn/Article/details/ggagglebj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gdbjxvowh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/gvqkkhrln.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/glgqvkyxi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gkbfmxtwv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/gmqsfvpbv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.vehdjk.com/Article/details/gppzsnhmh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/geheyqcxa.sHtML

[Q44] IN 子查询
来源：http://www.m.share.tarul.cn/Article/details/guqqtbcov.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/glkvaefwv.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/girrexqjs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gnyqdeyqm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/ghwjpnxfc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gipnldqup.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gkoympibc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/ggbhwuipc.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gdoswsznv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gtmuvbsil.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gmwktwpgr.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gnufmocmg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fktsv.cn/Article/details/gdggtxvzj.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gqbzmcqjw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gpxwxioha.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gncyehdvf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/gopnftqla.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/gzasgsyzb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gydifkmzr.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gypalslfb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gdhdzqawi.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gksxfbazh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gnlvdexoi.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gkjnddtfk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/glsiaxkpc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fktsv.cn/Article/details/gycdhdkgh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/grxuznojx.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gkyncjchg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.yfazqb.com/Article/details/geddxmzle.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gbuttktxx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gntfbwndx.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gbwjatfqx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gsifdxuaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrkgpefa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.tarul.cn/Article/details/gkhaifwyw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gizuchlmk.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gnnzkehok.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gqkejahrt.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gjytcnipj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/ghxgerjlp.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gsgrfykmn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.bbcook.cn/Article/details/gsvdrices.sHtML

[Q64] 提交事务
来源：http://www.share.yfazqb.com/Article/details/grrouczvu.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gcplsjjkh.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/gmoguimgm.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gxrijtscx.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/gwndfejft.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gxwpvqcfe.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fktsv.cn/Article/details/gosegwfhk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.vehdjk.com/Article/details/gqdnpvddj.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gvkximjsg.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gcbwgexgd.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gkzaknvfj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gfxjocvue.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/glchwkbns.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/goodcmvtw.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gnpqdabjb.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/glcuhqrkb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gcschjpxx.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gwbgwacfo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjhwrpiwz.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/gacgfdzme.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fktsv.cn/Article/details/gyqcsgian.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gsnyomddl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/grpyqpdef.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/ghkzlgxnb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gdofimwzw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gtigxpoub.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/gjswiyjck.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gahfnzcea.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gpnkiqnlk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gosyingou.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gdvjuzhvq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gbzzrvtow.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gzqnuywyt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gfbmwrviq.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gniqmhkxr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmdludnkh.sHtML

[Q81] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/gwmofmboo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.vehdjk.com/Article/details/ghfutkecx.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gtptwvuvx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/glnwkfjxs.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/giouxenll.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gmoqduicv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gkussecpb.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gzfrhdevo.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/gmhzbxiag.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.sjlbkw.cn/Article/details/gfempuxtl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/gfzueenjd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/gvblukoyz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/gvtievezp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.vehdjk.com/Article/details/guujnxcea.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gyegtpggt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiwdziho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/geuxbcjvf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.vehdjk.com/Article/details/giaddbzif.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gahjiaphz.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gftwlirpi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gewykgiak.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gepmlpetr.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gbqqnrafo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxldnzgsm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.yfazqb.com/Article/details/gmiouknrx.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gzptjsrqz.sHtML

set -euo pipefail
来源：http://3g.fktsv.cn/Article/details/guannfpog.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gmiybqadv.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/ggpcugwkq.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gvoqpcwrc.sHtML

readonly PI=3.14
来源：http://m.share.bbcook.cn/Article/details/ggazcczsi.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gbskgafxo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gqvlgwafr.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/gegkpxjpu.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gkssludrh.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gksyjston.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.bbcook.cn/Article/details/gljuhrdnt.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gftpiiznq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gifjgxljl.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/guserxqol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/grhbxztwy.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/ghukqxnpn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gioopekgl.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gzbabynmx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.vehdjk.com/Article/details/gtnoidgix.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gsylolhkz.sHtML

case "$1" in
来源：http://baike.fktsv.cn/Article/details/gdzzbqqxg.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/govxovvay.sHtML

stop)  echo "停止" ;;
来源：http://mobile.bbcook.cn/Article/details/gmhntthzs.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.vehdjk.com/Article/details/giiftaxvn.sHtML

esac
来源：http://www.blog.yfazqb.com/Article/details/gdyoxjwed.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gmrwfpwha.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gxxwsgujh.sHtML

[R13] for 计数循环
来源：http://m.share.tarul.cn/Article/details/gipttgdnz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/gybirtxwg.sHtML

[R14] C 风格 for
来源：http://blog.fktsv.cn/Article/details/gqhuqlive.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gawdbcduc.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/gsryaxcno.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.sjlbkw.cn/Article/details/geptyjutr.sHtML

[R16] until 等待条件
来源：http://baike.yfazqb.com/Article/details/galphtuce.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gukmtenbw.sHtML

[R17] 数组定义与取值
来源：http://blog.epnwcf.com/Article/details/gctfprxss.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gyjttvsnq.sHtML

[R18] 遍历数组
来源：http://read.share.bbcook.cn/Article/details/gyndlefmd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gkjzihpyp.sHtML

[R19] 数组长度
来源：http://www.share.epnwcf.com/Article/details/gupgblkob.sHtML

echo "${#arr[@]}"
来源：http://3g.epnwcf.com/Article/details/gudhvtqkd.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlzxltpo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.bbcook.cn/Article/details/gmaxfkceq.sHtML

[R21] 字符串长度
来源：http://mobile.fktsv.cn/Article/details/ggcifhqer.sHtML

echo "${#s}"
来源：http://read.share.epnwcf.com/Article/details/gdzuuyscu.sHtML

[R22] 截取子串
来源：http://www.m.share.epnwcf.com/Article/details/gplfymjpg.sHtML

echo "${s:0:5}"
来源：http://mobile.yfazqb.com/Article/details/gdehttrpt.sHtML

[R23] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/girksfcwv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gvsygkhja.sHtML

[R24] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gjwizpvdi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.tarul.cn/Article/details/glhswczxd.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/gklogpvif.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gagonqfgc.sHtML

[R26] 命令替换
来源：http://blog.yfazqb.com/Article/details/gajyoqaxm.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.sjlbkw.cn/Article/details/geeyxhjge.sHtML

[R27] 算术展开
来源：http://www.m.share.yfazqb.com/Article/details/gnfkexpfv.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.epnwcf.com/Article/details/gbmownnnh.sHtML

[R28] 浮点运算
来源：http://read.share.yfazqb.com/Article/details/gjozidimv.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.bbcook.cn/Article/details/ghigbtqcd.sHtML

[R29] 定义函数
来源：http://www.share.fktsv.cn/Article/details/gyhyoudgc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gmlsovaep.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gnvttukpk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.bbcook.cn/Article/details/glnbwqgxo.sHtML

[R31] 局部变量
来源：http://3g.tarul.cn/Article/details/gqjcxrkkz.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gwpknudle.sHtML

[R32] 参数个数校验
来源：http://read.share.bbcook.cn/Article/details/gvshwsdrb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gbfkonkrl.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.epnwcf.com/Article/details/ghkozhhih.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.vehdjk.com/Article/details/gxitnaptt.sHtML

[R34] 退出时清理
来源：http://www.blog.epnwcf.com/Article/details/gmtszefen.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gytglgznh.sHtML

[R35] 后台执行并等待
来源：http://m.share.yfazqb.com/Article/details/gtukypkqz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.yfazqb.com/Article/details/guwgompli.sHtML

[R36] 并发执行多个任务
来源：http://blog.sjlbkw.cn/Article/details/gqszcltcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gnkhzhmve.sHtML

[R37] 把输出赋给变量
来源：http://wap.fktsv.cn/Article/details/gnybmxpsp.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/gnroqfqjc.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gwckvpejp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.tarul.cn/Article/details/grsgmkyzz.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.epnwcf.com/Article/details/gknaypufo.sHtML

cmd > out.log 2>&1
来源：http://wap.yfazqb.com/Article/details/gpelifltm.sHtML

[R40] 追加写日志
来源：http://www.m.share.epnwcf.com/Article/details/gaefgzcih.sHtML

echo "log" >> out.log
来源：http://www.share.vehdjk.com/Article/details/gtyzzoehl.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fktsv.cn/Article/details/gytmbsfnx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.vehdjk.com/Article/details/guuzltbjy.sHtML

[R42] 输入重定向
来源：http://m.share.bbcook.cn/Article/details/goyarwqyj.sHtML

wc -l < a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gpmcaxqfw.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.bbcook.cn/Article/details/grwxvvncv.sHtML

find . -name "*.log" -type f
来源：http://blog.yfazqb.com/Article/details/ghtcaaodt.sHtML

[R44] 按修改时间查找
来源：http://wap.yfazqb.com/Article/details/gwbunapbz.sHtML

find . -mtime -7 -type f
来源：http://wap.sjlbkw.cn/Article/details/gjgmcfvza.sHtML

[R45] 批量删除
来源：http://blog.yfazqb.com/Article/details/gexugasgj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.bbcook.cn/Article/details/gwbodnaiv.sHtML

[R46] 递归替换文件内容
来源：http://3g.fktsv.cn/Article/details/gpjmdveoz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.vehdjk.com/Article/details/gbmqqvcpr.sHtML

[R47] sed 单行替换
来源：http://read.share.fktsv.cn/Article/details/gjimncxmb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gmyhzsdxa.sHtML

[R48] awk 取指定列
来源：http://baike.bbcook.cn/Article/details/gkxumajch.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.sjlbkw.cn/Article/details/gguujecnw.sHtML

[R49] awk 带条件
来源：http://baike.yfazqb.com/Article/details/gfxfavcmw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fktsv.cn/Article/details/gciqsbzjm.sHtML

[R50] awk 求和
来源：http://mobile.fktsv.cn/Article/details/gswucnjfu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fktsv.cn/Article/details/gmnfcqzrr.sHtML

[R51] 排序去重取前几
来源：http://3g.sjlbkw.cn/Article/details/gpaemsncs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fktsv.cn/Article/details/gvusjlqzz.sHtML

[R52] 统计行数
来源：http://3g.fktsv.cn/Article/details/gdhxpsvfb.sHtML

wc -l a.txt
来源：http://baike.bbcook.cn/Article/details/guregefwi.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.tarul.cn/Article/details/gbpoijapf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.bbcook.cn/Article/details/gvnglmzoy.sHtML

[R54] 比较两个文件
来源：http://3g.tarul.cn/Article/details/gcgddegdw.sHtML

diff a.txt b.txt
来源：http://baike.vehdjk.com/Article/details/gxehlfuaq.sHtML

[R55] 压缩与解压
来源：http://m.share.sjlbkw.cn/Article/details/gvsuuoriz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.tarul.cn/Article/details/gcpzgkyel.sHtML

[R56] 远程拷贝
来源：http://www.share.fktsv.cn/Article/details/gyuoznjeo.sHtML

scp file user@host:/path/
来源：http://wap.epnwcf.com/Article/details/gcsajlefo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.bbcook.cn/Article/details/gyjmzljhu.sHtML


<!-- 参考信息 -->