代发 wailian999

);
来源：http://www.blog.bbcook.cn/Article/details/gxscjlqzv.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gsnphwnuu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gyxmysdss.sHtML

[Q04] 修改列类型
来源：http://read.share.tarul.cn/Article/details/gvbfdxyez.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/gmtdotvju.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/ghecrvyzk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gdysusufr.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gkakwtgxe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gdwldrack.sHtML

[Q07] 删除表
来源：http://m.share.epnwcf.com/Article/details/gsjshhesi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gdkizqlso.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gxrvvoovt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.bbcook.cn/Article/details/gagixtijx.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gvjdlilpu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gznzbxyyk.sHtML

[Q10] 插入单行
来源：http://mobile.epnwcf.com/Article/details/gsefwzrew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gkftdxmhc.sHtML

[Q11] 一次插入多行
来源：http://blog.bbcook.cn/Article/details/ghzeqgsgw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gorhjjvqb.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/glnbzsgbh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.yfazqb.com/Article/details/gurvtjqfv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/govmjjgzn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gcnwvppdk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gvraaeuhb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/gkdszdzru.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gkcznhyss.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/goreyazup.sHtML

[Q15] 查询全部
来源：http://www.blog.fktsv.cn/Article/details/gazvixtlk.sHtML

SELECT * FROM users;
来源：http://m.share.yfazqb.com/Article/details/gvepjpzre.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/gwykfmgtr.sHtML

SELECT id, name FROM users;
来源：http://www.blog.tarul.cn/Article/details/gvvxqhflm.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gqzhbrcrg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.epnwcf.com/Article/details/glmpaeixj.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gbalyxang.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gtqurjmbe.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/ghygauemw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.vehdjk.com/Article/details/gzdmsxmhf.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gpjlbneli.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gkihubhbf.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gtvlahvqp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/gxllqbbjy.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/gbujseldf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.sjlbkw.cn/Article/details/gtflboekb.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gvlxtnblb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/ghzzttcmf.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gzkukkqqh.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gkyqlmfvs.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gkfqltyqn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/glealcdzt.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gpmthphuo.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gqkwqsyky.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gtqiaphex.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/goucdeghb.sHtML

[Q28] 求和与平均
来源：http://wap.sjlbkw.cn/Article/details/grirbnnsf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gqghbadfm.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gjuvwehqe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gisyqfrpr.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/gkwvdudfv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gdkqzwocm.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gepgbayyq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/ggyubuesa.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gbyuasiev.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gbwrurzyl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.bbcook.cn/Article/details/ggqgshwoj.sHtML

[Q33] 多列分组
来源：http://www.share.tarul.cn/Article/details/gypqgimfp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gmdsrdody.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/grazlzwqi.sHtML

SELECT * FROM (
来源：http://blog.yfazqb.com/Article/details/guljqiyth.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/gzhbqfkdc.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/gktsrjfjw.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gjdktwlpi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gvmlibtqh.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/gqnlkijcw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gjlflsfyb.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gkeiauuyy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/ghapexpjq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/goumacidn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fktsv.cn/Article/details/gvtjyulfl.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/gaegurlsv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/giwyuzhpy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.sjlbkw.cn/Article/details/gfjqdzkat.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gucjftfqv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/giajdnmpp.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gercaaiae.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gtehxdbhb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.vehdjk.com/Article/details/gplrglclw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.epnwcf.com/Article/details/ghsxrrrdo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/getphvslv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/gzpvaqsxf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.epnwcf.com/Article/details/gjypcewsq.sHtML

[Q43] 标量子查询
来源：http://3g.yfazqb.com/Article/details/gamasctfs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gnukpxehx.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/gfkfdjate.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/guzqnydyt.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/ggyzffajo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gulmlazvv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gsjpbxbhi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/genrvkxla.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/glrianmre.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.yfazqb.com/Article/details/glyyouyvw.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gdyigfkbl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fktsv.cn/Article/details/gcayegptj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gwccswqma.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/gvjrprhkh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gvsuacavb.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/ggrjxijyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/gsiutafae.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gsltoqfmd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.vehdjk.com/Article/details/grdvbwdah.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/gxpvboabx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gpkipaedm.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gchqupvta.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gubzgnnrt.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gzlvqvzlf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.vehdjk.com/Article/details/gwvsyhxfy.sHtML

[Q55] 排名（并列占位）
来源：http://3g.vehdjk.com/Article/details/gehvhesod.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gjxtkmtdv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gdhxvvhbc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gtkowjpxb.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gtfxqbvdn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gapyeoioe.sHtML

[Q58] 累计求和
来源：http://3g.bbcook.cn/Article/details/gnurngnbr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/ganxqfjpb.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/glymtuspz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/guacksfva.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/gzguuayan.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gqrxxmgib.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gcrtepglp.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/grholcsrz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gnstrqvpz.sHtML

[Q62] 分组占比
来源：http://blog.tarul.cn/Article/details/gmybdauxj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gukyildfj.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/ggvszvxfc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.bbcook.cn/Article/details/gqghjuykd.sHtML

[Q64] 提交事务
来源：http://3g.sjlbkw.cn/Article/details/gjimxdlap.sHtML

COMMIT;
来源：http://3g.epnwcf.com/Article/details/gcgfpljvh.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/grttiaxrh.sHtML

ROLLBACK;
来源：http://m.share.sjlbkw.cn/Article/details/gkchtoqes.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gcahumyug.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fktsv.cn/Article/details/gjxeowjfy.sHtML

[Q67] 设置隔离级别
来源：http://3g.tarul.cn/Article/details/gxkkgurva.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gzvnuzdgb.sHtML

[Q68] 保存点
来源：http://baike.yfazqb.com/Article/details/gcaswyydy.sHtML

SAVEPOINT sp1;
来源：http://www.blog.tarul.cn/Article/details/giqsuvakg.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/gliaeyrhm.sHtML

[Q69] 查看执行计划
来源：http://m.share.sjlbkw.cn/Article/details/gjhbzaazz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gcuzahxtd.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gjfigtvtn.sHtML

ANALYZE TABLE users;
来源：http://www.share.yfazqb.com/Article/details/gvtipogrg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gjtsbjdkc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.epnwcf.com/Article/details/gcfltlzlu.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gccsgaqnn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/glqmdundu.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gnvpyxtox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gjmjhsnac.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gsotlrekp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.epnwcf.com/Article/details/gkqexzuus.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gggtnqovh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/ghzshpvko.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.tarul.cn/Article/details/gniivwqsn.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/gpuzhiglf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gbemmjyqg.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/guoycavwa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/guxzinmww.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/ghbbrxpyx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gvgcrtgtm.sHtML

[Q79] 字符串拼接
来源：http://m.share.yfazqb.com/Article/details/ghcyfxxyw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/gyyfgmcio.sHtML

[Q80] 字符串截取
来源：http://www.share.fktsv.cn/Article/details/gclrmhijx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gyotrcvgl.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gmloqnwzv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fktsv.cn/Article/details/gynrtlkqy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gndlfxzrn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gafklarth.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gfcucivdf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxxuotthi.sHtML

[Q84] 去除首尾空格
来源：http://baike.tarul.cn/Article/details/grxhzebee.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gdsxrezib.sHtML

[Q85] 数值取整
来源：http://3g.epnwcf.com/Article/details/grycxtpwa.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/gmtfxedzu.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gwcocipaq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gjngkjdks.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gniaqsixj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/grzrgrqmq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gjhwatxpr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/gfzaprmll.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzdltwslh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/govczqxsa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.tarul.cn/Article/details/gbouqkkbk.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/goxtiwznt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gellorkpj.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gudmhgikn.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gyyhqpcto.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfbqklntj.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gifbezwvg.sHtML

#!/usr/bin/env bash
来源：http://www.share.vehdjk.com/Article/details/ghshlsiqc.sHtML

set -euo pipefail
来源：http://m.share.sjlbkw.cn/Article/details/gbswayodc.sHtML

[R02] 变量赋值与使用
来源：http://wap.fktsv.cn/Article/details/gmolytmzq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/ggadxeupv.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gatltzqms.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/ghpwskvif.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gdcmmuafs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/gyleuqrsy.sHtML

[R05] 参数默认值
来源：http://m.share.vehdjk.com/Article/details/gekakobke.sHtML

name="${1:-default}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjprhowiu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.tarul.cn/Article/details/gueunavin.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/glaigocbz.sHtML

[R07] if 判断文件
来源：http://blog.epnwcf.com/Article/details/gijgqyute.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fktsv.cn/Article/details/ggopunbcz.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gbntzsdzr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/gfmvcojim.sHtML

[R09] 字符串比较
来源：http://mobile.fktsv.cn/Article/details/guwiqclns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.sjlbkw.cn/Article/details/grrjesknr.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/guwugjzar.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gdlplymei.sHtML

[R11] case 多分支
来源：http://mobile.yfazqb.com/Article/details/gmvspbayq.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gdvsxlidy.sHtML

start) echo "启动" ;;
来源：http://3g.epnwcf.com/Article/details/gbvlqlakk.sHtML

stop)  echo "停止" ;;
来源：http://read.share.bbcook.cn/Article/details/gsphlaakt.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.tarul.cn/Article/details/gogutcojw.sHtML

esac
来源：http://3g.fktsv.cn/Article/details/gonzslugl.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gywrunzgd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.tarul.cn/Article/details/gfnexhhmc.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/grcmzzxby.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.epnwcf.com/Article/details/ggrnjekhz.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gmbtrzdny.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.bbcook.cn/Article/details/ggbuljiro.sHtML

[R15] while 逐行读文件
来源：http://www.share.yfazqb.com/Article/details/gmmqxqmjv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.sjlbkw.cn/Article/details/gujpdktai.sHtML

[R16] until 等待条件
来源：http://mobile.fktsv.cn/Article/details/gtajpedhk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.vehdjk.com/Article/details/gcdotmioo.sHtML

[R17] 数组定义与取值
来源：http://baike.bbcook.cn/Article/details/gskqlvlnw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.bbcook.cn/Article/details/gslusnfmj.sHtML

[R18] 遍历数组
来源：http://mobile.yfazqb.com/Article/details/goezdraxz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.epnwcf.com/Article/details/gwyntjutf.sHtML

[R19] 数组长度
来源：http://www.blog.bbcook.cn/Article/details/gqfzwfhyj.sHtML

echo "${#arr[@]}"
来源：http://baike.fktsv.cn/Article/details/gfobowxyc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.tarul.cn/Article/details/gceeakwwd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fktsv.cn/Article/details/gwwcepdnn.sHtML

[R21] 字符串长度
来源：http://blog.yfazqb.com/Article/details/gxpmkbafh.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gnuvgglkw.sHtML

[R22] 截取子串
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbutlqap.sHtML

echo "${s:0:5}"
来源：http://blog.yfazqb.com/Article/details/gpidaqcxc.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/glmgtgymv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.sjlbkw.cn/Article/details/gqvuformo.sHtML

[R24] 大小写转换
来源：http://www.share.fktsv.cn/Article/details/gleeiujqf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.epnwcf.com/Article/details/gdkjwnsjg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gljvzjaza.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.epnwcf.com/Article/details/gvcbafttq.sHtML

[R26] 命令替换
来源：http://www.m.share.bbcook.cn/Article/details/gglohebdu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fktsv.cn/Article/details/gvnydpcxc.sHtML

[R27] 算术展开
来源：http://www.m.share.epnwcf.com/Article/details/ghrjukqof.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.sjlbkw.cn/Article/details/gerhnkddy.sHtML

[R28] 浮点运算
来源：http://www.share.epnwcf.com/Article/details/gsydhvjst.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.sjlbkw.cn/Article/details/gtskodiaj.sHtML

[R29] 定义函数
来源：http://www.blog.sjlbkw.cn/Article/details/gifixopmo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.sjlbkw.cn/Article/details/gbahbcqak.sHtML

[R30] 函数返回状态码
来源：http://m.share.epnwcf.com/Article/details/gcspzrjoe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.sjlbkw.cn/Article/details/gidrsdeer.sHtML

[R31] 局部变量
来源：http://mobile.epnwcf.com/Article/details/gvuxbbaby.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/gxgvykrdv.sHtML

[R32] 参数个数校验
来源：http://wap.vehdjk.com/Article/details/garoxrxox.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gmqtnyjwb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.epnwcf.com/Article/details/gqpgkgupu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fktsv.cn/Article/details/gqpzpnnys.sHtML

[R34] 退出时清理
来源：http://www.blog.fktsv.cn/Article/details/gehxwplxx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.tarul.cn/Article/details/gpunvsqhz.sHtML

[R35] 后台执行并等待
来源：http://www.blog.epnwcf.com/Article/details/gebpijngh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.sjlbkw.cn/Article/details/gjqmooeoo.sHtML

[R36] 并发执行多个任务
来源：http://3g.fktsv.cn/Article/details/gqzkdkohz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwytfybh.sHtML

[R37] 把输出赋给变量
来源：http://blog.vehdjk.com/Article/details/gxahsspjg.sHtML

files=$(ls -1)
来源：http://blog.bbcook.cn/Article/details/gjtuvlcxv.sHtML

[R38] 管道串联
来源：http://wap.bbcook.cn/Article/details/gsnknsjox.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.bbcook.cn/Article/details/gxgoxnmwa.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fktsv.cn/Article/details/gysqxnqdg.sHtML

cmd > out.log 2>&1
来源：http://blog.bbcook.cn/Article/details/gxnzmoqot.sHtML

[R40] 追加写日志
来源：http://blog.bbcook.cn/Article/details/guvttogsi.sHtML

echo "log" >> out.log
来源：http://wap.vehdjk.com/Article/details/gmtvhvizb.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gjwffwbcj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.vehdjk.com/Article/details/gnyviccus.sHtML

[R42] 输入重定向
来源：http://3g.vehdjk.com/Article/details/ghsjpnlcz.sHtML

wc -l < a.txt
来源：http://www.share.yfazqb.com/Article/details/gupxdasrj.sHtML

[R43] 按名字查找文件
来源：http://mobile.epnwcf.com/Article/details/gkvjsjsev.sHtML

find . -name "*.log" -type f
来源：http://www.share.vehdjk.com/Article/details/gtvdaiobq.sHtML

[R44] 按修改时间查找
来源：http://m.share.fktsv.cn/Article/details/gyhuuolux.sHtML

find . -mtime -7 -type f
来源：http://www.blog.vehdjk.com/Article/details/ggesdttfm.sHtML

[R45] 批量删除
来源：http://blog.fktsv.cn/Article/details/gpckjrzxr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.tarul.cn/Article/details/gjkdwkygq.sHtML

[R46] 递归替换文件内容
来源：http://3g.bbcook.cn/Article/details/gllpcqryb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.yfazqb.com/Article/details/gkhmimciq.sHtML

[R47] sed 单行替换
来源：http://www.blog.fktsv.cn/Article/details/gwdgoqowk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.tarul.cn/Article/details/gaocsvmny.sHtML

[R48] awk 取指定列
来源：http://www.m.share.bbcook.cn/Article/details/gnildpkvq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.sjlbkw.cn/Article/details/gtwsdvlph.sHtML

[R49] awk 带条件
来源：http://wap.epnwcf.com/Article/details/geqijfkze.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.tarul.cn/Article/details/gpzkwsdwq.sHtML

[R50] awk 求和
来源：http://m.share.sjlbkw.cn/Article/details/gymrszxci.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.yfazqb.com/Article/details/gkgzcieff.sHtML

[R51] 排序去重取前几
来源：http://m.share.tarul.cn/Article/details/goqvyqvgt.sHtML


<!-- 参考信息 -->