代发 wailian999

================================================================================
来源：http://blog.fktsv.cn/Article/details/gewbiouly.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gilwfxdbl.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdfpyojxx.sHtML

[Q01] 创建表
来源：http://3g.fktsv.cn/Article/details/gsxlxivfx.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gonpbaskq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gxsvwistv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gyeenphmg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gxlzndfiw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gkdpqrgoy.sHtML

);
来源：http://www.share.sjlbkw.cn/Article/details/gyuegvbcv.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gthvtpbjy.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gsfmxnnry.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gnzelxbar.sHtML

user_id INT NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gcugzxumh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gdlcptbkx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/ggzrcrqht.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gefxjmkde.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gtskgupbi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gmsunvltr.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gxaguosfv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.epnwcf.com/Article/details/gxnyfauez.sHtML

[Q05] 重命名列
来源：http://www.blog.fktsv.cn/Article/details/gpbsdhsjv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gyvveipto.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gcxyscvyw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.epnwcf.com/Article/details/gkwrvkibe.sHtML

[Q07] 删除表
来源：http://www.blog.epnwcf.com/Article/details/gnrezgfvf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/getnqnxyu.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/grumbvchz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/grkrbdgge.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/glsmttejp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gwiccfsmg.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gwppputuu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.bbcook.cn/Article/details/gkagjxjri.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/gokkiaqup.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/gvepomrrc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gnrsmjhpu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.vehdjk.com/Article/details/gpbojajtg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.epnwcf.com/Article/details/gxwffbkbf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gwjokruux.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gdkwwemno.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/geilwuges.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gziuciiwn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.yfazqb.com/Article/details/gbpsdklhn.sHtML

[Q15] 查询全部
来源：http://www.m.share.epnwcf.com/Article/details/ggujlaarh.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gqyehrvdx.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gaddgzous.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gzwsarrgg.sHtML

[Q17] 条件查询
来源：http://mobile.fktsv.cn/Article/details/gvldrulam.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.sjlbkw.cn/Article/details/gsynbrnmq.sHtML

[Q18] 模糊匹配
来源：http://read.share.fktsv.cn/Article/details/gwnlpsazu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/glgswlxxa.sHtML

[Q19] 范围查询
来源：http://mobile.yfazqb.com/Article/details/ggnftmpct.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.bbcook.cn/Article/details/gtajgjgdt.sHtML

[Q20] IN 列表
来源：http://www.share.fktsv.cn/Article/details/gaqyxeheh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/gzzbnubzj.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/ggwraucmw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.vehdjk.com/Article/details/ggdtknyts.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/gapzpcrak.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gstacthcz.sHtML

[Q23] 分页
来源：http://blog.epnwcf.com/Article/details/gphzkghxp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/goximptxz.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/ggtjuxcet.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gakequbmv.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gycxwfsxp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.sjlbkw.cn/Article/details/glbwmpkzv.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gckemmjdo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/grlajnhem.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gctavkffg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gghostren.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gitwofudw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gcvayqadf.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gpgbekyfx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gzlsuuvzt.sHtML

[Q30] 分组统计
来源：http://www.blog.tarul.cn/Article/details/gtdxyloav.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gbztuckyo.sHtML

[Q31] 分组后过滤
来源：http://blog.vehdjk.com/Article/details/gkncsjumr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/gzjwoadli.sHtML

[Q32] 分组拼接字符串
来源：http://blog.bbcook.cn/Article/details/gncqmlsxh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/ghibvnvil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gglsiqnuv.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/gkmbwjhqx.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.yfazqb.com/Article/details/giwwptcby.sHtML

[Q34] 每组取第一条
来源：http://read.share.yfazqb.com/Article/details/gosfroftx.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gqqbhwzzd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/ghigrptvz.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/gtntmfpqj.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gomyisgan.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gjqvybefm.sHtML

[Q36] 左连接
来源：http://www.share.yfazqb.com/Article/details/gfzqtqpru.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gxwqaakyq.sHtML

[Q37] 右连接
来源：http://m.share.fktsv.cn/Article/details/gwhmwpvkp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.vehdjk.com/Article/details/gyhrcotoo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.sjlbkw.cn/Article/details/gqtdxirhv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/gclgghdzk.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.tarul.cn/Article/details/gwweampds.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.sjlbkw.cn/Article/details/gihvqpxgy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.vehdjk.com/Article/details/glijrydal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gvkkwuden.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gofebgsqh.sHtML

[Q41] 多表连接
来源：http://read.share.epnwcf.com/Article/details/gvlkywgci.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gpsopoffs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gggybmnkg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gaskpzjiw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/gtpulzcok.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/guuqpvmvu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/guglxeyqm.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gbolgtjmq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gevhvltwt.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gkpxhdbko.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/gqdwuvxuj.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/gswoseaes.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/ghcuhwvrh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.tarul.cn/Article/details/glsqbtcxx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gcxakrpmi.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gisbetndd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.tarul.cn/Article/details/gyruqimlw.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/gbwfdyanw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gplxotfrs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gkkwwerdh.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gbsueossu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gbfzlvpse.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gxtjufhgc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.tarul.cn/Article/details/gvrufgfgu.sHtML

[Q51] 用子查询更新
来源：http://mobile.bbcook.cn/Article/details/gudphfwrl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gtibuejya.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gblmdrqjd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gtnlihpdh.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gunejjomu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gdyfecfqh.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gbujwtzkh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/gogknfuuc.sHtML

[Q55] 排名（并列占位）
来源：http://blog.vehdjk.com/Article/details/gsdapyddm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.tarul.cn/Article/details/gnojnjnma.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.epnwcf.com/Article/details/ghhwudkql.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gyivznpfq.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/gymrokluy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fktsv.cn/Article/details/gmyfkvddk.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/grwlrqvgx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/geqgluxbo.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/gpkhuixzy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/glhfgijsg.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gmegefzsu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gmzboyvno.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gformcibi.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gypssbkld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gdwhmxtvn.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/goujcexcu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gyzagobyg.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/guscbfafi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gwacglyda.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gsypheizf.sHtML

COMMIT;
来源：http://blog.fktsv.cn/Article/details/gagmxevqu.sHtML

[Q65] 回滚事务
来源：http://baike.vehdjk.com/Article/details/gityzadyz.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gjwukafao.sHtML

[Q66] 行锁查询
来源：http://blog.fktsv.cn/Article/details/gjjbkibev.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gvjmjpydx.sHtML

[Q67] 设置隔离级别
来源：http://baike.tarul.cn/Article/details/gpybmjayg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/gdzgtozyd.sHtML

[Q68] 保存点
来源：http://www.share.bbcook.cn/Article/details/gwdbrkyic.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gcabadoax.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gpnexfemx.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gqzwhkbsn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gzspcmchg.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gjghpbjpc.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gomnbrmim.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/gkluzhguw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gouxmlkly.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gldwkallj.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/gupqcmmcl.sHtML

[Q73] 查看表状态
来源：http://www.blog.yfazqb.com/Article/details/gebhdjshy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gpaopboep.sHtML

[Q74] 强制使用索引
来源：http://blog.epnwcf.com/Article/details/gbdiijazh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.vehdjk.com/Article/details/gxupjofzz.sHtML

[Q75] 日期格式化
来源：http://blog.epnwcf.com/Article/details/gdlivqhyr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/grkgmormy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gqmqtrtpd.sHtML

[Q76] 按天统计
来源：http://www.blog.fktsv.cn/Article/details/gtbsgphsh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gedxodqsz.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gvifoyeih.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gzndlwmiw.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gphuvuuey.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/gttcspxna.sHtML

[Q79] 字符串拼接
来源：http://mobile.epnwcf.com/Article/details/gstkfxrqa.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gwxqfcpmm.sHtML

[Q80] 字符串截取
来源：http://www.blog.epnwcf.com/Article/details/ggbtouswv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gjvtpiwkq.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gyzubatpz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/gxljwnmiv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/ginrpwyew.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/govtsvzlc.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gejbfxezb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gjoonwehb.sHtML

[Q84] 去除首尾空格
来源：http://baike.yfazqb.com/Article/details/gqomxuuqj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gbvsayzjd.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gdrgyefwl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/ghnkvuhjf.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/goqgpkyps.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/gjpeitfjo.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gcrbtszbw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gxpoxqyyu.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gxelkwhkk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gmqvvbrck.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gplqyjdzx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/ggmarioeh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.yfazqb.com/Article/details/gmflkjsyv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gajddzkax.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.bbcook.cn/Article/details/gxjzdplwl.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gznoegyxk.sHtML

R. Bash 专题
来源：http://mobile.bbcook.cn/Article/details/gamcxinxn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gjjoxkqfn.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gccgsryen.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsiwmala.sHtML

set -euo pipefail
来源：http://wap.fktsv.cn/Article/details/ghyksqiji.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/giabxsmxv.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/grlrvsoaa.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gvmdpfzcb.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gqlintaqa.sHtML

[R04] 位置参数
来源：http://mobile.tarul.cn/Article/details/gtmvzrumi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/gqeumrnal.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gzqlaznvd.sHtML

name="${1:-default}"
来源：http://wap.sjlbkw.cn/Article/details/gjzedlspn.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gaujdvpyu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/grewfmjqm.sHtML

[R07] if 判断文件
来源：http://3g.sjlbkw.cn/Article/details/geirnzwpt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/gqbbgtpwi.sHtML

[R08] 数值比较
来源：http://baike.epnwcf.com/Article/details/gjaproyhm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gyzgyojuf.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/gvbffsjbo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gqnikbgfx.sHtML

[R10] 正则匹配
来源：http://mobile.tarul.cn/Article/details/gohdvdsyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/ghkormkrm.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gzmttslfe.sHtML

case "$1" in
来源：http://www.share.sjlbkw.cn/Article/details/gsbqgsiql.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gbnoeaofz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.tarul.cn/Article/details/gorhiyppe.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gxyiekdzi.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gsgoggeos.sHtML

[R12] for 遍历文件
来源：http://m.share.yfazqb.com/Article/details/gxoxichjp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fktsv.cn/Article/details/gyguuftgx.sHtML

[R13] for 计数循环
来源：http://www.share.bbcook.cn/Article/details/gqtjwxcsp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.sjlbkw.cn/Article/details/gzlhtutze.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gmuunznfe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.yfazqb.com/Article/details/gtrnxseud.sHtML

[R15] while 逐行读文件
来源：http://m.share.epnwcf.com/Article/details/grjphposm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.tarul.cn/Article/details/gnbwyhfmj.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gmdkitxgc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fktsv.cn/Article/details/gyxhhlcnr.sHtML

[R17] 数组定义与取值
来源：http://mobile.tarul.cn/Article/details/gsbkvokpl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.epnwcf.com/Article/details/gqcenftbd.sHtML

[R18] 遍历数组
来源：http://blog.vehdjk.com/Article/details/gvcthcmrg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.sjlbkw.cn/Article/details/ggdrgsafa.sHtML

[R19] 数组长度
来源：http://www.blog.epnwcf.com/Article/details/ghrmvqwsr.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gclxxkoeb.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/gzpqwujxq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.yfazqb.com/Article/details/gjahzkmfc.sHtML

[R21] 字符串长度
来源：http://blog.sjlbkw.cn/Article/details/ggixmltbm.sHtML

echo "${#s}"
来源：http://3g.yfazqb.com/Article/details/glglxinfr.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gtbrygjod.sHtML

echo "${s:0:5}"
来源：http://m.share.epnwcf.com/Article/details/gbdvhhcpz.sHtML

[R23] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gpivtvfut.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.tarul.cn/Article/details/gvcddwljl.sHtML

[R24] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gqengkrsh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.yfazqb.com/Article/details/gmhqqlbio.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.tarul.cn/Article/details/ghnsvzjpn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fktsv.cn/Article/details/gvnvwdcug.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gmsnpxaca.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/griycsude.sHtML

[R27] 算术展开
来源：http://www.blog.vehdjk.com/Article/details/gyknktztm.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.yfazqb.com/Article/details/gyecpyvmg.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gqkxrrocz.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.sjlbkw.cn/Article/details/gpsarqzbw.sHtML

[R29] 定义函数
来源：http://www.blog.fktsv.cn/Article/details/gwnniuack.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.sjlbkw.cn/Article/details/gjsfyhjso.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gljedeyoy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.epnwcf.com/Article/details/gbbtxkaxp.sHtML

[R31] 局部变量
来源：http://m.share.fktsv.cn/Article/details/gejhumxfq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.sjlbkw.cn/Article/details/geompnldt.sHtML

[R32] 参数个数校验
来源：http://baike.epnwcf.com/Article/details/gcgwvjegx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gdyevenhw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fktsv.cn/Article/details/gncduupfc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gbvdowano.sHtML

[R34] 退出时清理
来源：http://baike.tarul.cn/Article/details/gaeiqyhdv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.tarul.cn/Article/details/gvwfrgkxy.sHtML

[R35] 后台执行并等待
来源：http://read.share.tarul.cn/Article/details/giokfzpmk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.yfazqb.com/Article/details/golyorkpe.sHtML

[R36] 并发执行多个任务
来源：http://m.share.vehdjk.com/Article/details/gjiiaawpj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.vehdjk.com/Article/details/gpdwusali.sHtML

[R37] 把输出赋给变量
来源：http://3g.vehdjk.com/Article/details/ggugdoxgb.sHtML

files=$(ls -1)
来源：http://www.m.share.bbcook.cn/Article/details/gszwwnhnc.sHtML

[R38] 管道串联
来源：http://blog.yfazqb.com/Article/details/gptilybat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.tarul.cn/Article/details/gnjwhmxbo.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.epnwcf.com/Article/details/gkeiurnot.sHtML

cmd > out.log 2>&1
来源：http://wap.bbcook.cn/Article/details/gkqtofpsv.sHtML

[R40] 追加写日志
来源：http://www.m.share.vehdjk.com/Article/details/gqbqyowva.sHtML

echo "log" >> out.log
来源：http://mobile.bbcook.cn/Article/details/gvjccjdys.sHtML

[R41] 丢弃输出
来源：http://www.share.fktsv.cn/Article/details/gddaepxem.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fktsv.cn/Article/details/gmfdwlame.sHtML

[R42] 输入重定向
来源：http://read.share.vehdjk.com/Article/details/gffrwdicf.sHtML

wc -l < a.txt
来源：http://baike.yfazqb.com/Article/details/gwsvkhwyk.sHtML

[R43] 按名字查找文件
来源：http://wap.vehdjk.com/Article/details/gmshomqyn.sHtML


<!-- 参考信息 -->