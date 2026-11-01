代发 wailian999

);
来源：http://www.m.share.yfazqb.com/Article/details/guijowsdf.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gegusatec.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.sjlbkw.cn/Article/details/gyakfehkv.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gpzusfwfz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gzthnzkej.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gxkckcenp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gmzdnmmcv.sHtML

[Q06] 删除列
来源：http://3g.yfazqb.com/Article/details/gfjfnsyjd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.bbcook.cn/Article/details/gxzdcqmxq.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gjihmgbhg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.bbcook.cn/Article/details/gsqkpbsnz.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/ggzzrqxei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gudfiapcl.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gdxiioiwu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gxgmlezlx.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/ggavanser.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fktsv.cn/Article/details/getnenhyi.sHtML

[Q11] 一次插入多行
来源：http://www.blog.sjlbkw.cn/Article/details/gfwczlyix.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fktsv.cn/Article/details/gavangxma.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.fktsv.cn/Article/details/gutysoere.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/giojbgsmu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/gmifxuukh.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.vehdjk.com/Article/details/giaxvlvwa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gfvnrcjmz.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gvgkorclh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gdorsjnwq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gkhpijzyn.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gmwrztayp.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gdevdgltl.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gbkwbbsrj.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/guegrjrob.sHtML

[Q17] 条件查询
来源：http://www.m.share.vehdjk.com/Article/details/gvajwpnhz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gfcxiblvt.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/gtacgwclk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/gontcrqlc.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gnpmqpunr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/glajsccmj.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gktllmtup.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gjikdnxzh.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/guumujrgy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/glrvramjr.sHtML

[Q22] 排序
来源：http://baike.fktsv.cn/Article/details/gclsxekvp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.yfazqb.com/Article/details/goqbdtycr.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gbmypwetq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gfzrwjyjj.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gikeaamno.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfqutntsg.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gbktadftg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/gnvxuhfkc.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjivuhil.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gviyxjcui.sHtML

[Q27] 条件计数
来源：http://baike.sjlbkw.cn/Article/details/ggxgpxmjc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gpszalogm.sHtML

[Q28] 求和与平均
来源：http://www.m.share.epnwcf.com/Article/details/gelnvydfo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gjnxawdhq.sHtML

[Q29] 最大最小值
来源：http://www.m.share.tarul.cn/Article/details/gicxncolu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/gmcibttou.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gbusbmqxf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/giggsxtcf.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gqgrhauuw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/ghitypwgo.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gwvvutunf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gqdmzjhwu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/gsbzizjif.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gblyglzqd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gfxtcxjpv.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gwmtsplyp.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gjbvnqpsc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.tarul.cn/Article/details/govkyldrv.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/ghzpxvkoa.sHtML

[Q35] 内连接
来源：http://m.share.tarul.cn/Article/details/gxsqnvwji.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gvoxetdjq.sHtML

[Q36] 左连接
来源：http://wap.vehdjk.com/Article/details/gmdudwzka.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gvknigcdx.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gplgxcvzo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpdxbksv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gsbafpxsx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gkjxnzezx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gkbuzfunb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/gdqizjqeb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/ghayqwxbu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/geicqionz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/ghwxzjqrk.sHtML

[Q41] 多表连接
来源：http://www.share.vehdjk.com/Article/details/gwvhsllmp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/gatipjowy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gdxqbsrbj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gyiopchqo.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gstockqbl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gisfaunbs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/guhaviqnb.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gzlodmyjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gindcwtuk.sHtML

[Q44] IN 子查询
来源：http://3g.bbcook.cn/Article/details/glbjntfci.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gmcgsivsn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gwowxoksw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gddwkfxja.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.bbcook.cn/Article/details/gsntmkwal.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gnuxjoylj.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gqnybhyri.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.tarul.cn/Article/details/gazwmwjxq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.sjlbkw.cn/Article/details/gaxepccig.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.yfazqb.com/Article/details/gzvdsmtpc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gkleceerz.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/glzquukao.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gdglvrfpa.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gjppdazbm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gephcrdqe.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gaqqczwpx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/gqiwpmdtw.sHtML

[Q52] 删除指定行
来源：http://wap.fktsv.cn/Article/details/gjlnmtlhm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gfxhouxkr.sHtML

[Q53] 按条件删除
来源：http://www.m.share.epnwcf.com/Article/details/gwagjzjzp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/guhioomvw.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gtrygbiav.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.bbcook.cn/Article/details/gxtpklxel.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.sjlbkw.cn/Article/details/gdwkllxgf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gtwvhxyyb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gangtcobj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gwdthdxmr.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/gpltqatoi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gxrjcuass.sHtML

[Q58] 累计求和
来源：http://m.share.bbcook.cn/Article/details/getqkmdgr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/gnskiihwx.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gydignkgl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gptqczvcp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gosifawzj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.tarul.cn/Article/details/gdyyxmmzx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gqmvuvzst.sHtML

[Q61] 移动平均
来源：http://www.share.sjlbkw.cn/Article/details/gdftviaua.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gwhnztklv.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/giweqqcvh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gwanwnnhb.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gesdzkcbl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/gpfotckkc.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gzwshjatu.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/gncrpoynq.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/ghbcfvyxk.sHtML

ROLLBACK;
来源：http://baike.yfazqb.com/Article/details/gisadjhty.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/gptbthxsd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gtlhnwimr.sHtML

[Q67] 设置隔离级别
来源：http://wap.fktsv.cn/Article/details/gmrmuogmj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/gndxakeey.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gjrogzigd.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/gvmcbjsyd.sHtML

ROLLBACK TO sp1;
来源：http://www.share.vehdjk.com/Article/details/gwoixujwm.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gbyycfgga.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/gnojmotae.sHtML

[Q70] 更新统计信息
来源：http://wap.epnwcf.com/Article/details/gspktceod.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gcbdxbhbu.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/gvudkmaot.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gouwysxyt.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/ggzotaaxl.sHtML

SHOW INDEX FROM users;
来源：http://wap.yfazqb.com/Article/details/gzenyqyrt.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gmqbuolri.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/grnvmxfsl.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gewgphbjr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gmghcyery.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gapintvez.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gejunlkpk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gqhshlpqc.sHtML

[Q76] 按天统计
来源：http://www.m.share.sjlbkw.cn/Article/details/grqmbxvco.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/gqhsbahvk.sHtML

[Q77] 时间加减
来源：http://www.blog.epnwcf.com/Article/details/gttkwgypj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gnubowgrk.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gqxawinwc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.tarul.cn/Article/details/gsbcwchbv.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gsxjtsixe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gyhijkwci.sHtML

[Q80] 字符串截取
来源：http://read.share.epnwcf.com/Article/details/grlidcgbb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gvwluzrss.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gnyjvqkmt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqfnxarjp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/gxsrlreku.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gpsdcmgpl.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gixuklpjv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/goiszqbmr.sHtML

[Q84] 去除首尾空格
来源：http://3g.tarul.cn/Article/details/gdbmemmhp.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gaipiejfh.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gnycuotiw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.sjlbkw.cn/Article/details/gjspqaycd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gxzyhazgs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/ggfrzpdyd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/grsdefone.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gadganqmv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.vehdjk.com/Article/details/gddsbabxh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/geqdumztd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gclndqzyx.sHtML

[Q89] 判断表是否存在
来源：http://wap.bbcook.cn/Article/details/gkvzewnyz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.sjlbkw.cn/Article/details/givbbmglf.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gyymqrhbl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gpceifllu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gfoctkdnw.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/ghcjzxzrh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gsudonuxh.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gainofpdv.sHtML

#!/usr/bin/env bash
来源：http://baike.bbcook.cn/Article/details/geefowuds.sHtML

set -euo pipefail
来源：http://blog.vehdjk.com/Article/details/gsxwceipn.sHtML

[R02] 变量赋值与使用
来源：http://www.share.tarul.cn/Article/details/gwwtauzbt.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gkknxtxhv.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/guxhuoypw.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gwxxtgbdw.sHtML

[R04] 位置参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gicfhyyjq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.epnwcf.com/Article/details/gqawvszxh.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/ggmhkuqns.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gzcxwmqsc.sHtML

[R06] 判断命令是否存在
来源：http://www.share.tarul.cn/Article/details/gzexbdbre.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fktsv.cn/Article/details/gtscrinjx.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/gwkabxuow.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gwzblhags.sHtML

[R08] 数值比较
来源：http://www.share.epnwcf.com/Article/details/grnkbzbwk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/glwjolsuv.sHtML

[R09] 字符串比较
来源：http://www.blog.epnwcf.com/Article/details/gffymotwm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/gxstlbalb.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/ghocpndnd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.yfazqb.com/Article/details/gkkefaiij.sHtML

[R11] case 多分支
来源：http://baike.sjlbkw.cn/Article/details/guyzzpckk.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/garrtvxpt.sHtML

start) echo "启动" ;;
来源：http://read.share.vehdjk.com/Article/details/gwvxgqzuq.sHtML

stop)  echo "停止" ;;
来源：http://blog.sjlbkw.cn/Article/details/gnmfmxdtx.sHtML

*)     echo "未知命令" ;;
来源：http://wap.tarul.cn/Article/details/grrjtqqot.sHtML

esac
来源：http://blog.tarul.cn/Article/details/gzpuffljb.sHtML

[R12] for 遍历文件
来源：http://3g.epnwcf.com/Article/details/gmuffkioo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gqtgszyoa.sHtML

[R13] for 计数循环
来源：http://baike.tarul.cn/Article/details/gkkdryzys.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gsuphdqfx.sHtML

[R14] C 风格 for
来源：http://m.share.epnwcf.com/Article/details/gffzvfrym.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gymxdvwtr.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gtqokcvfy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.vehdjk.com/Article/details/gttsiquks.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/gecawpnpk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.yfazqb.com/Article/details/gnociaqfr.sHtML

[R17] 数组定义与取值
来源：http://baike.yfazqb.com/Article/details/gwqelcbee.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.tarul.cn/Article/details/glazxebdy.sHtML

[R18] 遍历数组
来源：http://m.share.epnwcf.com/Article/details/gpixtgagw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.sjlbkw.cn/Article/details/grsdmpdxg.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/gqcnpbyhi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/gvfkmjfiz.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gledvnujn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.bbcook.cn/Article/details/gjunzmdid.sHtML

[R21] 字符串长度
来源：http://read.share.epnwcf.com/Article/details/gbvdvxgjb.sHtML

echo "${#s}"
来源：http://baike.tarul.cn/Article/details/gfwceuurf.sHtML

[R22] 截取子串
来源：http://3g.epnwcf.com/Article/details/gpawhxodr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fktsv.cn/Article/details/gmyggdfnt.sHtML

[R23] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gpuneyuno.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.tarul.cn/Article/details/gjhjkbufy.sHtML

[R24] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gzfvvxlqy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.bbcook.cn/Article/details/gilmhxgvi.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gokvdbpfr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gvsvnocsi.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gkjobrluw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gejskzurs.sHtML

[R27] 算术展开
来源：http://www.blog.sjlbkw.cn/Article/details/gujzwsjzn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.epnwcf.com/Article/details/ghetodqny.sHtML

[R28] 浮点运算
来源：http://m.share.vehdjk.com/Article/details/gifoxzfkv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.sjlbkw.cn/Article/details/gxanedtip.sHtML

[R29] 定义函数
来源：http://wap.yfazqb.com/Article/details/ggmeotlqx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.vehdjk.com/Article/details/gjnnvfyvo.sHtML

[R30] 函数返回状态码
来源：http://m.share.vehdjk.com/Article/details/gwyecxzio.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.yfazqb.com/Article/details/gdoluzizb.sHtML

[R31] 局部变量
来源：http://www.share.epnwcf.com/Article/details/gzobgkedb.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fktsv.cn/Article/details/gelsvfqoc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.sjlbkw.cn/Article/details/glhhlhnug.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/gztshyadh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gkaezwwfu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gmzwspscy.sHtML

[R34] 退出时清理
来源：http://m.share.vehdjk.com/Article/details/gkqczmbbm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.tarul.cn/Article/details/glihnqglg.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.bbcook.cn/Article/details/guqavmtwc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fktsv.cn/Article/details/gqmluvlhn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gkxbyhdxf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.bbcook.cn/Article/details/gbkmdhmzl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.epnwcf.com/Article/details/gtaomibcf.sHtML

files=$(ls -1)
来源：http://baike.fktsv.cn/Article/details/gbpiiqgkc.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gfkrakciw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.bbcook.cn/Article/details/gwfofsyfu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.yfazqb.com/Article/details/ggamzhvdr.sHtML

cmd > out.log 2>&1
来源：http://blog.tarul.cn/Article/details/gtpwxvmsq.sHtML

[R40] 追加写日志
来源：http://www.share.yfazqb.com/Article/details/gsrmbmanh.sHtML

echo "log" >> out.log
来源：http://www.m.share.yfazqb.com/Article/details/gsdrgpqwg.sHtML

[R41] 丢弃输出
来源：http://wap.sjlbkw.cn/Article/details/goybklcpg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fktsv.cn/Article/details/gewlyryil.sHtML

[R42] 输入重定向
来源：http://3g.fktsv.cn/Article/details/gxfbsngvj.sHtML

wc -l < a.txt
来源：http://www.m.share.epnwcf.com/Article/details/gylreqaeo.sHtML

[R43] 按名字查找文件
来源：http://www.blog.epnwcf.com/Article/details/gfjjzrxqk.sHtML

find . -name "*.log" -type f
来源：http://wap.bbcook.cn/Article/details/glijjddek.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/gyobrnoig.sHtML

find . -mtime -7 -type f
来源：http://read.share.sjlbkw.cn/Article/details/gurqatdhe.sHtML

[R45] 批量删除
来源：http://www.m.share.vehdjk.com/Article/details/gisnqqszq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.yfazqb.com/Article/details/gixsyyvxk.sHtML

[R46] 递归替换文件内容
来源：http://baike.epnwcf.com/Article/details/gwwqgxbko.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.tarul.cn/Article/details/gzwsolicw.sHtML

[R47] sed 单行替换
来源：http://m.share.epnwcf.com/Article/details/gfhozmbmk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fktsv.cn/Article/details/gvcutsezh.sHtML

[R48] awk 取指定列
来源：http://read.share.fktsv.cn/Article/details/ghyduzvnl.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.bbcook.cn/Article/details/gbkxeqsps.sHtML

[R49] awk 带条件
来源：http://www.share.epnwcf.com/Article/details/ggrvmwdwp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.vehdjk.com/Article/details/giofpwnbb.sHtML

[R50] awk 求和
来源：http://www.share.vehdjk.com/Article/details/gkrjynkvf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fktsv.cn/Article/details/glerbfkih.sHtML

[R51] 排序去重取前几
来源：http://wap.sjlbkw.cn/Article/details/gwoakhunx.sHtML


<!-- 参考信息 -->