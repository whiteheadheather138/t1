代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/ggpoaupso.sHtML

[Q07] 删除表
来源：http://m.share.epnwcf.com/Article/details/gemxzjtuq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fktsv.cn/Article/details/gpwticggq.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gmbjtoome.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/ggjkxafxs.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/gvgnqtxft.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gztjkepnj.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/glcjcjitx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.vehdjk.com/Article/details/gawafqqxb.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gfxcjtqwh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/guvvqtmcl.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/grapkdsik.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gxkiqwxvt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.bbcook.cn/Article/details/gnwvbhjem.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/goljcvsje.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/guiqsebov.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gcdqybiiu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fktsv.cn/Article/details/grcchxxzd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gjuckjyvc.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/gacgztelv.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gpeabzaky.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gukxfurwz.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gqsmlrslw.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gdyykivpt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gpevlbknc.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gkkubznrb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gqvgswjyu.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gffgcuxxd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gxghovujz.sHtML

[Q20] IN 列表
来源：http://3g.yfazqb.com/Article/details/gojmidnrq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/ggcnkiltf.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gejhifkln.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gcpeaipdo.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gbmdzfjlo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/goyuagdlw.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gkbbcjuai.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gflsctdjw.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/ghtexmmqd.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.epnwcf.com/Article/details/gvkvxbrxa.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/gpkwdthot.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/goaesxlsm.sHtML

[Q26] 计数
来源：http://blog.vehdjk.com/Article/details/gvycqwias.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gxomerjro.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gyfswpyyx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gfeamthaj.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/guvguetto.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gjqpusblo.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gjhlndtyi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpjooudmb.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gyfefvtrp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gnsyesgzk.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.bbcook.cn/Article/details/gegqouygp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gqhiewidk.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gaxvxtwye.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gtbliemso.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gmuzvxnho.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/goaduqync.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gooarpvlp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gqfwjcefd.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/glapakktt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/grvojcxor.sHtML

) t WHERE rn = 1;
来源：http://baike.tarul.cn/Article/details/gjvptbjtt.sHtML

[Q35] 内连接
来源：http://3g.vehdjk.com/Article/details/gwdwtugyf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gycxupnpx.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gonqclhwb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gicftqqeg.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/gjddesqrx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gehbmkbcd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/gmdruztht.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gagsafoom.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/garsrserr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gtxmawpqp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gbdnislww.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.yfazqb.com/Article/details/gtxdwrdzg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gzmauapco.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gxotsypsq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/gwalbzdzg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/gfbgctclj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gxydwdllj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/gratkleqd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/ghtusdukn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gkbseweqw.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gfytyvwxr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.sjlbkw.cn/Article/details/grruexxcq.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/grochkbvm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gotlkeqwt.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gvqdzquue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gomvikkku.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.tarul.cn/Article/details/glykrnznp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gijzpgwvv.sHtML

[Q47] 与平均值比较
来源：http://3g.vehdjk.com/Article/details/gwrawbfhb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/ghojujsma.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/ggbimujir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gmzikjbve.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/ghgohbcgx.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/gmctsmcmg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gvfrasaag.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/gcruexcsl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gsqjhxygw.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gxxhsphnx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gigsxinuz.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gyctiercq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gmewcpklq.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gddpdylch.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.bbcook.cn/Article/details/gxiatanej.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gwpbufrjt.sHtML

TRUNCATE TABLE logs;
来源：http://blog.yfazqb.com/Article/details/gjlrnjmoa.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gusbbbnit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gukrthdxj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.epnwcf.com/Article/details/gfpwwygmf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gguheshyc.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/goxyzmfzs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gwdjtxtip.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gqinzzmks.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gzmpkqscb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gzxdpzipg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gfzpuikgi.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.epnwcf.com/Article/details/gftxgevvr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fktsv.cn/Article/details/gqaphuacs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/giuaxulhj.sHtML

[Q61] 移动平均
来源：http://mobile.sjlbkw.cn/Article/details/gxnuqnufe.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/ggjhjxmfn.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/ghomcfxjx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/glzdihszn.sHtML

[Q63] 开启事务
来源：http://mobile.tarul.cn/Article/details/gawzqpjwv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gwogfuwlj.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gojgeqlkq.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gctzmkzpp.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/giurrsjpb.sHtML

ROLLBACK;
来源：http://3g.tarul.cn/Article/details/gwgpqlkfn.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/grwpomgov.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/gihnvumem.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gczlygcik.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.vehdjk.com/Article/details/gfxcslsqu.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gnnoilwoq.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/ggzhouirp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gxrhqqszp.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/gaoreegtn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gmrpbysdb.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.tarul.cn/Article/details/gxjjztwgh.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gfwbwvvmg.sHtML

[Q71] 查看建表语句
来源：http://mobile.sjlbkw.cn/Article/details/gsdxebrey.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.yfazqb.com/Article/details/gjhwliqfe.sHtML

[Q72] 查看索引
来源：http://www.m.share.tarul.cn/Article/details/gxytgunnf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/ggaaeocxj.sHtML

[Q73] 查看表状态
来源：http://3g.tarul.cn/Article/details/gzinujaiq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.epnwcf.com/Article/details/gvhrmfgap.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gzadsnzmg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gswqaokfb.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gvjhedrdv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gknkflhms.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gqnusqblh.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gdydkysyp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.epnwcf.com/Article/details/gwduvntrj.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/ggknrzmxu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gqtuyxxud.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gvygupwww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gnugrcyrv.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gdeoexbau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gtdbzuxxw.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/gvmlvwqpf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwqvbrtcc.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gzfhnoiov.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gresgmmpn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gbepcnppi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gymzhmlpa.sHtML

[Q83] 大小写转换
来源：http://www.share.yfazqb.com/Article/details/gljdcwkuz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gppzgcyok.sHtML

[Q84] 去除首尾空格
来源：http://mobile.yfazqb.com/Article/details/glfkirpyy.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gtlcerbiw.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gttnroimw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gyedhxfcl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gcwbxrggy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/gycudwxpx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fktsv.cn/Article/details/gqufpfdnu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gtzqudiix.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gzdcjkblp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.yfazqb.com/Article/details/gtgtwntit.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gpsrmogjq.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gzedfyvjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gaxfqsfjc.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/girowuzhr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gpvmsankl.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gqwognuxc.sHtML

R. Bash 专题
来源：http://www.blog.bbcook.cn/Article/details/ghnttfxhi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnigjxoct.sHtML

[R01] shebang 与严格模式
来源：http://3g.tarul.cn/Article/details/gxcnahoqv.sHtML

#!/usr/bin/env bash
来源：http://wap.fktsv.cn/Article/details/gcozdguue.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gkvolrenu.sHtML

[R02] 变量赋值与使用
来源：http://baike.tarul.cn/Article/details/gibnshncl.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gejbsolmc.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/gwxndzvym.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gpxsgiujl.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/gmpguxbln.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/gnezfobsv.sHtML

[R05] 参数默认值
来源：http://mobile.yfazqb.com/Article/details/gnngbjtjn.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gesslciif.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gqbuplblv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/gcdktfllx.sHtML

[R07] if 判断文件
来源：http://www.share.vehdjk.com/Article/details/gdfqeutxx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/glfalppqp.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gfhxbkdjr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/gduxgicqh.sHtML

[R09] 字符串比较
来源：http://www.share.epnwcf.com/Article/details/gboqvdtgt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/gutuhhgfh.sHtML

[R10] 正则匹配
来源：http://blog.tarul.cn/Article/details/grxjqeidb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gdpfuuznf.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gdwjgpgcr.sHtML

case "$1" in
来源：http://read.share.vehdjk.com/Article/details/gtjcnbnxj.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/grplugbei.sHtML

stop)  echo "停止" ;;
来源：http://www.share.bbcook.cn/Article/details/gajxffoih.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fktsv.cn/Article/details/gsyqjlcbp.sHtML

esac
来源：http://read.share.epnwcf.com/Article/details/gpxtkgdma.sHtML

[R12] for 遍历文件
来源：http://read.share.bbcook.cn/Article/details/gewweyejq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.bbcook.cn/Article/details/gorjhhcld.sHtML

[R13] for 计数循环
来源：http://3g.yfazqb.com/Article/details/gktpzweqr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.yfazqb.com/Article/details/gzopskvqn.sHtML

[R14] C 风格 for
来源：http://blog.tarul.cn/Article/details/gcnvweekz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/ggnybvddk.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/gktjzmclj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.vehdjk.com/Article/details/glvbtqcnd.sHtML

[R16] until 等待条件
来源：http://baike.vehdjk.com/Article/details/gvakmrhmk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.bbcook.cn/Article/details/ghpzzwdmb.sHtML

[R17] 数组定义与取值
来源：http://mobile.epnwcf.com/Article/details/goggmprkg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/ghmbkdfvi.sHtML

[R18] 遍历数组
来源：http://www.m.share.bbcook.cn/Article/details/gtrgswokp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.vehdjk.com/Article/details/gbnnlcuaj.sHtML

[R19] 数组长度
来源：http://www.share.sjlbkw.cn/Article/details/ggynpbwfr.sHtML

echo "${#arr[@]}"
来源：http://baike.epnwcf.com/Article/details/gffaxaqlh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.yfazqb.com/Article/details/gcbzszwky.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.yfazqb.com/Article/details/gktocwkzc.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gthzxcczj.sHtML

echo "${#s}"
来源：http://baike.tarul.cn/Article/details/gghpabyyu.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gtnjscpag.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gnsfgtfdu.sHtML

[R23] 字符串替换
来源：http://blog.tarul.cn/Article/details/gufotnoao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.tarul.cn/Article/details/gdeuvqnzw.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gvauhuuad.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.tarul.cn/Article/details/ghzjkaeyp.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.sjlbkw.cn/Article/details/ghyvufzgi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gwbyswock.sHtML

[R26] 命令替换
来源：http://3g.sjlbkw.cn/Article/details/goexlxqsr.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gkejmfggb.sHtML

[R27] 算术展开
来源：http://mobile.yfazqb.com/Article/details/gagpmmabm.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.epnwcf.com/Article/details/gadcawxci.sHtML

[R28] 浮点运算
来源：http://m.share.tarul.cn/Article/details/gfzmmjwsj.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fktsv.cn/Article/details/gnalnscpj.sHtML

[R29] 定义函数
来源：http://wap.tarul.cn/Article/details/goptyqkhg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.vehdjk.com/Article/details/glnzvphmn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fktsv.cn/Article/details/goywzqjgt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/gxizgnmuh.sHtML

[R31] 局部变量
来源：http://blog.tarul.cn/Article/details/gtfakwsaa.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.vehdjk.com/Article/details/gqpsyckkd.sHtML

[R32] 参数个数校验
来源：http://wap.yfazqb.com/Article/details/grlwrtocc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.tarul.cn/Article/details/gsnpnqabt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gtpewwkhh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.bbcook.cn/Article/details/gtapmzxjn.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gjenilavx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.tarul.cn/Article/details/gaeisnahg.sHtML

[R35] 后台执行并等待
来源：http://mobile.sjlbkw.cn/Article/details/gynnmozyo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fktsv.cn/Article/details/gewhqjnel.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.sjlbkw.cn/Article/details/geqwgjwhn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.epnwcf.com/Article/details/gfzvqzcke.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.yfazqb.com/Article/details/gqktncpxa.sHtML

files=$(ls -1)
来源：http://baike.sjlbkw.cn/Article/details/gouucuqmu.sHtML

[R38] 管道串联
来源：http://m.share.tarul.cn/Article/details/ghrntyzpy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fktsv.cn/Article/details/gnrskqafp.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fktsv.cn/Article/details/gspwdpkfz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fktsv.cn/Article/details/gbtugfwpk.sHtML

[R40] 追加写日志
来源：http://www.share.vehdjk.com/Article/details/gfqnkgsxk.sHtML

echo "log" >> out.log
来源：http://baike.sjlbkw.cn/Article/details/gxpsmvwjy.sHtML

[R41] 丢弃输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gsxhmvesv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gjpqaxhjd.sHtML

[R42] 输入重定向
来源：http://3g.bbcook.cn/Article/details/gpnagrvgr.sHtML

wc -l < a.txt
来源：http://www.blog.yfazqb.com/Article/details/glulgunkp.sHtML

[R43] 按名字查找文件
来源：http://m.share.sjlbkw.cn/Article/details/gbdyrqnbs.sHtML

find . -name "*.log" -type f
来源：http://m.share.yfazqb.com/Article/details/gvboaxglf.sHtML

[R44] 按修改时间查找
来源：http://wap.vehdjk.com/Article/details/gvhzaqdty.sHtML

find . -mtime -7 -type f
来源：http://blog.yfazqb.com/Article/details/gqnjizjne.sHtML

[R45] 批量删除
来源：http://www.m.share.yfazqb.com/Article/details/guotmrstj.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fktsv.cn/Article/details/gifwlugxl.sHtML

[R46] 递归替换文件内容
来源：http://blog.tarul.cn/Article/details/gndmwdpcs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.tarul.cn/Article/details/gueamsdtc.sHtML

[R47] sed 单行替换
来源：http://www.blog.vehdjk.com/Article/details/ghxdeafnb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.yfazqb.com/Article/details/gxiknabbj.sHtML

[R48] awk 取指定列
来源：http://read.share.yfazqb.com/Article/details/gecowixxn.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.epnwcf.com/Article/details/gwsyurxjg.sHtML

[R49] awk 带条件
来源：http://mobile.epnwcf.com/Article/details/gjobvjdtz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fktsv.cn/Article/details/gqfljkvje.sHtML

[R50] awk 求和
来源：http://wap.yfazqb.com/Article/details/ghcagkxhq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fktsv.cn/Article/details/gjdchskga.sHtML

[R51] 排序去重取前几
来源：http://baike.vehdjk.com/Article/details/gfwcxhxye.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.vehdjk.com/Article/details/gffvstqhf.sHtML

[R52] 统计行数
来源：http://baike.fktsv.cn/Article/details/gqefwjpzb.sHtML

wc -l a.txt
来源：http://baike.sjlbkw.cn/Article/details/gvbumsjeo.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fktsv.cn/Article/details/gagsplxel.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.sjlbkw.cn/Article/details/gmhhtwtzj.sHtML

[R54] 比较两个文件
来源：http://www.blog.yfazqb.com/Article/details/gzecbqukz.sHtML

diff a.txt b.txt
来源：http://3g.yfazqb.com/Article/details/gxorbyngm.sHtML

[R55] 压缩与解压
来源：http://www.blog.sjlbkw.cn/Article/details/gtylgkubx.sHtML


<!-- 参考信息 -->