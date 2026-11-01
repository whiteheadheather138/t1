代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/ghyalvhsz.sHtML

user_id INT NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gqfbhiynn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gcfymkgiu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.tarul.cn/Article/details/grjjpnmtw.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gvxxcntgr.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/giggtbwvf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gfztgxgmi.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/gayudviki.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.bbcook.cn/Article/details/gbfhwekgf.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gxnhmdxmt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/gtbzqgjzm.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/gfvtgsevk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gjkpjkphd.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gnrvguwql.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.vehdjk.com/Article/details/gbicdbzma.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/gpksetirp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gknkmktyl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gekyguulr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gqpsvtbds.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gwgpvygzz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gzvgcpsyx.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gfobfcamg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fktsv.cn/Article/details/guqtsknja.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/ggbjzxefx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/gvwcxmrbb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/gxjjdhcxv.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gbivtpedh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/guvdepqeg.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gjsreggob.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gqdjzbjqa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.tarul.cn/Article/details/grreifqgs.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/goedwplrv.sHtML

SELECT * FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gwjeyfoss.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gcnlnlhnu.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/gduoeiuvl.sHtML

[Q17] 条件查询
来源：http://www.share.tarul.cn/Article/details/gakcgkysh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gxcghhneh.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/ggschyyzt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/gipxcmvse.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gynjtosxv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gigoswvje.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/ghsgyzbju.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/gwkiiwcwx.sHtML

[Q21] 空值判断
来源：http://www.blog.fktsv.cn/Article/details/gkxyhyifo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/gjzrsznaj.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gfrfleafl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fktsv.cn/Article/details/gxvvqddgg.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/galcpoouo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/gkfqlkqiq.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/guiefhddi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.tarul.cn/Article/details/gygberinc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gjiyohfnb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gsvhbkggu.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/gnkmilipy.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/goflkeeag.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gxicakvwt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/glycfpxbg.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gggujclzd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gllrfceng.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gazipsgoo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/glxkvfgdv.sHtML

[Q30] 分组统计
来源：http://m.share.fktsv.cn/Article/details/gutlimrfn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gtdtydnpt.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gaflrpflx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gvsjuwbdg.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gvcvvnfxx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gculodjph.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.sjlbkw.cn/Article/details/gxgxyvqbl.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gezmyqzzb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gsxjhepnk.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gtpnfzphf.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gvwrfpzih.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.tarul.cn/Article/details/gnqstigtj.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/gemyvpkiq.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gkkqzelct.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gnycjieog.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gbhmrhbat.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gsmfbvlsy.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gkdeoqxio.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.epnwcf.com/Article/details/gasmposxh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gdlkwxyts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/glqvubsvr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gpxsqftix.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.bbcook.cn/Article/details/gvvlgwleb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/guavbmyci.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.bbcook.cn/Article/details/gyfqxcbxp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gzqjyhfvg.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gcpertrmg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.epnwcf.com/Article/details/gjgugelip.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gskgrzrfe.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gisieujmr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.sjlbkw.cn/Article/details/gsqdesdrf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fktsv.cn/Article/details/gvbrynexh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gpfssmqno.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gooyuxbie.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/ggkbnnvih.sHtML

[Q44] IN 子查询
来源：http://read.share.epnwcf.com/Article/details/gjwxroovw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/gsixnynbx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/ggnxsurkh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/goazkfkhl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/gjjxiarpz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/grnacmrwa.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/gsofjxvld.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.vehdjk.com/Article/details/gwgixoeev.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gexzhslmr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gnbkijmxl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gbuaefmkw.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gkqzlamje.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gqoscnshz.sHtML

[Q50] 批量更新
来源：http://3g.yfazqb.com/Article/details/gtzitrphh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/grhvxwpfd.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.vehdjk.com/Article/details/gaqzjfemx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gqypydkpd.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gbpyeduou.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gbutbgyqx.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gntlwindt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gdyvrukry.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gvfsnmgxa.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gcegfrsct.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gklxcbeeh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/guwwcwbhe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gmakqmfdk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/ggezrvwso.sHtML

[Q57] 行号
来源：http://wap.vehdjk.com/Article/details/grccjluko.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/gzqmpyyyl.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gxzzstiqf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.epnwcf.com/Article/details/ghciuletq.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/geszwqngl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gaedgntut.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gqgbmhegi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fktsv.cn/Article/details/gjobdycxk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gbwgljwac.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/giwfovvdp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gsquntkgi.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gttaqwgvm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gzfmukfxn.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gknfzduad.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gsihjqxnk.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gcpmtrfzg.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/gajfkzumo.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gdpplwfiy.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gyrcqgxuu.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/guhuvacjw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/grfzwwcoc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/gzylugqyc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.epnwcf.com/Article/details/gujsppvyz.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gwfirihri.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gmtpsvlnk.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gvrryvieo.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gqvkwfdns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gpnzoqqhd.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gqsyzqsfi.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gjhjvqwta.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/glmevpkqq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.tarul.cn/Article/details/gavqdbaak.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/ghxwzktrk.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gwsjraukw.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gcskvgyga.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/giusgcupg.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/gphmrlucx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gtwqlpnyg.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/grrxtnbxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gaegycpmy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gxgypjcjl.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/glgryujak.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gjseuecod.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/gzwicckat.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.epnwcf.com/Article/details/gukmsaabs.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/giprymjqi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gfpjgtwix.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gsnatpnzz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gzyposief.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gbsycwtiw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gxjmxbnbr.sHtML

[Q81] 字符串替换
来源：http://blog.tarul.cn/Article/details/grnoipsnl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gheukxoeo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/glgeayctv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gwcpctcbc.sHtML

[Q83] 大小写转换
来源：http://www.share.bbcook.cn/Article/details/goyhuscqm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/ghedzhmrl.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fktsv.cn/Article/details/gweeyzxbd.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gpbvapfop.sHtML

[Q85] 数值取整
来源：http://blog.yfazqb.com/Article/details/gqfmmxxnj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gsedxvfoo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/giyvxfnwf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.vehdjk.com/Article/details/ggidlthfw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fktsv.cn/Article/details/gkiwyxesg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.tarul.cn/Article/details/gvdbthzqp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gdqgylsue.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.yfazqb.com/Article/details/gpjzyicpr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gerdlbtur.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gyobkloua.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gisxhvtpk.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gofizcqcq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/gbirvvmjb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcidwkqjo.sHtML

R. Bash 专题
来源：http://read.share.yfazqb.com/Article/details/gfyiqebda.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gcjbvnmwp.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gxoysdkul.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/gidraytqu.sHtML

set -euo pipefail
来源：http://m.share.fktsv.cn/Article/details/gvnvbgjej.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gdibccbjj.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gbehfoxyp.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gkhmpmmqc.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gzpnhtuaf.sHtML

[R04] 位置参数
来源：http://mobile.bbcook.cn/Article/details/gbqfatvaa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.vehdjk.com/Article/details/glzvbyssi.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gjkqriqok.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gixzxmaig.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/ghzqucirh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/ganvriert.sHtML

[R07] if 判断文件
来源：http://3g.tarul.cn/Article/details/gapekzkve.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.epnwcf.com/Article/details/gqrmotunx.sHtML

[R08] 数值比较
来源：http://m.share.epnwcf.com/Article/details/gzhskmcuf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.sjlbkw.cn/Article/details/geylxywwh.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/gotqafjjm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gmgphbceq.sHtML

[R10] 正则匹配
来源：http://www.share.bbcook.cn/Article/details/gkapffjni.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gmzjskjcm.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gbrggoznb.sHtML

case "$1" in
来源：http://www.share.tarul.cn/Article/details/gssbbikkt.sHtML

start) echo "启动" ;;
来源：http://blog.tarul.cn/Article/details/gdpxccgse.sHtML

stop)  echo "停止" ;;
来源：http://m.share.tarul.cn/Article/details/gkpbullub.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/giciitdho.sHtML

esac
来源：http://3g.bbcook.cn/Article/details/gdvjdfwjk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbwkgzsv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gmkwqucad.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gpxuvpnpx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.epnwcf.com/Article/details/gwumpwbnw.sHtML

[R14] C 风格 for
来源：http://blog.vehdjk.com/Article/details/gbyteedcg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gezldhmwe.sHtML

[R15] while 逐行读文件
来源：http://baike.tarul.cn/Article/details/gwsqdnwfq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fktsv.cn/Article/details/gbvagwoqf.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gnqoheygm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gqvglpdaw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gjhbrktlg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gvolhqpvi.sHtML

[R18] 遍历数组
来源：http://www.blog.sjlbkw.cn/Article/details/gvmwitxcr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gmvyktazy.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/gspoqgwdc.sHtML

echo "${#arr[@]}"
来源：http://read.share.tarul.cn/Article/details/gwgnzffiy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.yfazqb.com/Article/details/gilwbecrt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gkhwlxutp.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gyozsjact.sHtML

echo "${#s}"
来源：http://read.share.sjlbkw.cn/Article/details/gwrguncqd.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gollorowe.sHtML

echo "${s:0:5}"
来源：http://www.blog.bbcook.cn/Article/details/gkkuxcbhn.sHtML

[R23] 字符串替换
来源：http://www.blog.epnwcf.com/Article/details/grghcjyhv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.tarul.cn/Article/details/gwlgbpirq.sHtML

[R24] 大小写转换
来源：http://www.m.share.tarul.cn/Article/details/gamdptolx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.epnwcf.com/Article/details/gyxiseypd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gzijqmeyb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fktsv.cn/Article/details/ginmwjqxj.sHtML

[R26] 命令替换
来源：http://read.share.tarul.cn/Article/details/gxsivxlox.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.yfazqb.com/Article/details/gmrjbffku.sHtML

[R27] 算术展开
来源：http://m.share.bbcook.cn/Article/details/gmsrelfvk.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.bbcook.cn/Article/details/gkxaczyof.sHtML

[R28] 浮点运算
来源：http://www.m.share.tarul.cn/Article/details/gnxdgplqp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwmpccdi.sHtML

[R29] 定义函数
来源：http://m.share.epnwcf.com/Article/details/gwkisvyuu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.epnwcf.com/Article/details/gaendrwuc.sHtML

[R30] 函数返回状态码
来源：http://3g.tarul.cn/Article/details/gaoptbeqc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.epnwcf.com/Article/details/gmwwezgqr.sHtML

[R31] 局部变量
来源：http://baike.tarul.cn/Article/details/gjquehtnd.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.epnwcf.com/Article/details/gdpkqdvoi.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/gspcovayw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gubzecfwa.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.sjlbkw.cn/Article/details/golvuxhoh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.bbcook.cn/Article/details/gqgtpiero.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gtjzkddlo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.vehdjk.com/Article/details/ghvpilkcj.sHtML

[R35] 后台执行并等待
来源：http://read.share.yfazqb.com/Article/details/gsjeoqlzs.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.sjlbkw.cn/Article/details/grpndkhle.sHtML

[R36] 并发执行多个任务
来源：http://read.share.epnwcf.com/Article/details/guficngke.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.yfazqb.com/Article/details/gmjwqwsoe.sHtML

[R37] 把输出赋给变量
来源：http://wap.tarul.cn/Article/details/gtbpkcvnd.sHtML

files=$(ls -1)
来源：http://blog.vehdjk.com/Article/details/gadzxsdpp.sHtML

[R38] 管道串联
来源：http://m.share.epnwcf.com/Article/details/gqpoopvsl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.epnwcf.com/Article/details/gukgcnjyy.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fktsv.cn/Article/details/ggbbgfrkn.sHtML

cmd > out.log 2>&1
来源：http://mobile.yfazqb.com/Article/details/gelgitrox.sHtML

[R40] 追加写日志
来源：http://mobile.epnwcf.com/Article/details/gssolrtgw.sHtML

echo "log" >> out.log
来源：http://baike.epnwcf.com/Article/details/ghoxovsle.sHtML

[R41] 丢弃输出
来源：http://blog.fktsv.cn/Article/details/gpelcwezq.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fktsv.cn/Article/details/glewftvfb.sHtML

[R42] 输入重定向
来源：http://baike.sjlbkw.cn/Article/details/ggxqamngp.sHtML

wc -l < a.txt
来源：http://wap.bbcook.cn/Article/details/gdufzqrne.sHtML

[R43] 按名字查找文件
来源：http://blog.sjlbkw.cn/Article/details/gqnimwigf.sHtML

find . -name "*.log" -type f
来源：http://wap.tarul.cn/Article/details/gwfzhicze.sHtML

[R44] 按修改时间查找
来源：http://read.share.yfazqb.com/Article/details/grwgficpo.sHtML

find . -mtime -7 -type f
来源：http://m.share.sjlbkw.cn/Article/details/gfpzgdphb.sHtML

[R45] 批量删除
来源：http://www.blog.tarul.cn/Article/details/gfscvinhq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.vehdjk.com/Article/details/gjnqznrju.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.tarul.cn/Article/details/gfydmebmr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fktsv.cn/Article/details/gtkvyoxlc.sHtML

[R47] sed 单行替换
来源：http://read.share.yfazqb.com/Article/details/gacnklubr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fktsv.cn/Article/details/gnezytxnm.sHtML

[R48] awk 取指定列
来源：http://www.share.bbcook.cn/Article/details/gmfturttg.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fktsv.cn/Article/details/gpcemwmmt.sHtML

[R49] awk 带条件
来源：http://read.share.yfazqb.com/Article/details/gzsztgrpy.sHtML


<!-- 参考信息 -->