代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gdteczbwo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.bbcook.cn/Article/details/gvvhuqjdh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gulvwfevp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gmgpflrmc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/gibzsxzjd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.yfazqb.com/Article/details/gkearbrch.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/glkvyqekb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gbymicafd.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gshvjcstm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fktsv.cn/Article/details/gedvjbenn.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gryqqabep.sHtML

[Q01] 创建表
来源：http://m.share.bbcook.cn/Article/details/gywdqarvn.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gutcosrhu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gvxecjxga.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/golatpged.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gjynkgwqp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.epnwcf.com/Article/details/gqtidyvnp.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gzycmoerv.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gnhpfhlop.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gzeheklji.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gdcczbdap.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gybnbhlvs.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gjicsojau.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/gjwwpljxg.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gdbhvzywb.sHtML

[Q03] 增加列
来源：http://blog.tarul.cn/Article/details/gwbuiepqg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.vehdjk.com/Article/details/girzgvvit.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gregqkklm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gopsknyzz.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gycixjhcx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gjsqihgld.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gonkgwlee.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.bbcook.cn/Article/details/giumsekjb.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gsmioiqet.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fktsv.cn/Article/details/glpuecwwn.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/ghugkfnrs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/glyowkpul.sHtML

[Q09] 创建唯一索引
来源：http://blog.sjlbkw.cn/Article/details/gjwevwbwq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/guknqklip.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gvrfurtbr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gswqznodv.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gnosurpkr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.tarul.cn/Article/details/gnoawjrzg.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gyetagtwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/ghilddgod.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.epnwcf.com/Article/details/gelpzwnum.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/glzaxytun.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/giblpveit.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gkniallme.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gunlqayyu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gmwxlbajh.sHtML

[Q15] 查询全部
来源：http://www.blog.vehdjk.com/Article/details/gksfzrbcq.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/gcdhvlfpb.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gpujifviu.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/grprypbov.sHtML

[Q17] 条件查询
来源：http://mobile.epnwcf.com/Article/details/gnerpqlxd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gbgugnwcs.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/glzpfllmm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/gmnoashwd.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/ghtdjhwan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gsdngqeos.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/gcxjsubgh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gflwpeffh.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gpboizuca.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gyhjivkim.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gofexhzhi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gjjvewdyd.sHtML

[Q23] 分页
来源：http://www.blog.epnwcf.com/Article/details/gpsvmopsi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gtodtyoby.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gmdlmdnbi.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/glsjsrlnl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/ghbvlwiqq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/glxavxsko.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gmwadfjhm.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/ggyikonyb.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gukbyfhqx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gnepmrpfz.sHtML

[Q28] 求和与平均
来源：http://wap.vehdjk.com/Article/details/gyusqubaj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gislsyaqf.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gbrltadyy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/grqjiiojg.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gqmbllocj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gbumbdlcx.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/ghsxzbqmz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.epnwcf.com/Article/details/gcksfcwmi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gnpiunham.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gpuvznedz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gwfpvpdgp.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gcnuesrgr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gplqnsttq.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gbkndylhw.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gcrfvekmi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/gytuvawaq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gajrgjfzr.sHtML

[Q35] 内连接
来源：http://read.share.vehdjk.com/Article/details/gykzgvkmw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gmiyckcdg.sHtML

[Q36] 左连接
来源：http://3g.bbcook.cn/Article/details/gsjsovzpe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gmpltkiew.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/gqtkbkovr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqojmhxxa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.yfazqb.com/Article/details/gokdqbgng.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gymerjljz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/ghaatvofo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gcgmfsmfs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gwblymhzj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.sjlbkw.cn/Article/details/gigwxowvd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.yfazqb.com/Article/details/gowczlset.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gflrdkwpn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gnlpbktoc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gvrkiezkr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gyomqupoi.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gllmxrxlk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gfvvdrhxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.epnwcf.com/Article/details/gwvjwuhrv.sHtML

[Q43] 标量子查询
来源：http://www.m.share.bbcook.cn/Article/details/gldsxbviq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.sjlbkw.cn/Article/details/gkgqekdjs.sHtML

[Q44] IN 子查询
来源：http://www.m.share.vehdjk.com/Article/details/gngpgeaqa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.sjlbkw.cn/Article/details/gfbralhrc.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.bbcook.cn/Article/details/gbmvlbnxi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gggzmjlbf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.bbcook.cn/Article/details/gvfkiidxw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gbxejcqmh.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gskgwzxnj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gwhlokfli.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gynitssbp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/gpodaojvw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/gocehbeob.sHtML

[Q49] 更新单行
来源：http://mobile.vehdjk.com/Article/details/gxdupdbwa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gdqzynumi.sHtML

[Q50] 批量更新
来源：http://wap.bbcook.cn/Article/details/gjhwjxtud.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gxmoomqda.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.yfazqb.com/Article/details/gwliywolw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fktsv.cn/Article/details/gcbbiwvgh.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/giucqcecf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gmwcmjvuo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/ggexqmwuj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.tarul.cn/Article/details/gaiqdjyxf.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gwsdaodzk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.vehdjk.com/Article/details/ghivpxfxi.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gfldhrciv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gblxeedia.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gpohvvjkc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/gwtuicmib.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gbzmgwbgo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.vehdjk.com/Article/details/gfwaygexm.sHtML

[Q58] 累计求和
来源：http://3g.sjlbkw.cn/Article/details/glywxzhuj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gkylnrejl.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gugnnjsai.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gkldtwffl.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gaezruhkg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.bbcook.cn/Article/details/gzjvdmefn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gzummxwau.sHtML

[Q61] 移动平均
来源：http://mobile.epnwcf.com/Article/details/gkpfrpdiu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gfhnyeirr.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gvyfhnair.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gcnsgnwxf.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gugxwqqqg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gndrmocnu.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/ggnqlqazz.sHtML

COMMIT;
来源：http://www.share.tarul.cn/Article/details/grjfanbfb.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gueymykef.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gerrvgexj.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/gzispchtw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/gtulklsil.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gfakekmkt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/grxoocmak.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gvbzrawcw.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gxwrvnpxc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gvvjcgjam.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gegxpvjqo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gilaakffl.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gpjmgfrry.sHtML

ANALYZE TABLE users;
来源：http://baike.vehdjk.com/Article/details/goalvbelm.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/gmxmoxejp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.yfazqb.com/Article/details/guahnvkil.sHtML

[Q72] 查看索引
来源：http://blog.tarul.cn/Article/details/gaiaiecst.sHtML

SHOW INDEX FROM users;
来源：http://mobile.vehdjk.com/Article/details/gemoicwos.sHtML

[Q73] 查看表状态
来源：http://www.m.share.vehdjk.com/Article/details/glvqeveef.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gwdqnrpnd.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gwwvfzaiy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gcgmqanzi.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gfoqplxrt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.vehdjk.com/Article/details/gkhqcziwe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fktsv.cn/Article/details/gsxmygzko.sHtML

[Q76] 按天统计
来源：http://www.share.bbcook.cn/Article/details/gkpxbwriu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gerayrgnm.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/gjvokcajf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gsfvppseu.sHtML

[Q78] 当前时间
来源：http://www.share.tarul.cn/Article/details/gxacyuaei.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gwnjvdhso.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gcohkafta.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.bbcook.cn/Article/details/giwhlkpwh.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/ggafubzel.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvkccecmv.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gfgedaesz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gnxoysbmx.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gksbfnjvk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gwbvtphqk.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/gagolakff.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/ghdfazuox.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/goexffmho.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gafndiwiq.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gzfzmlfaj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gexhxkgvf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.tarul.cn/Article/details/ghnlamvbp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gfqimpgom.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gxkrcakbn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.bbcook.cn/Article/details/gtxaaethg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.vehdjk.com/Article/details/gutszyycc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fktsv.cn/Article/details/gvkdqvzmo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gjihbfvhv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gyjrjhcoa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gutkrelso.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gwuskxqro.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/gfqdmrfus.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gpakxqjqu.sHtML

R. Bash 专题
来源：http://wap.vehdjk.com/Article/details/gewjdzfbo.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gujidxqmt.sHtML

[R01] shebang 与严格模式
来源：http://3g.sjlbkw.cn/Article/details/gyeapgkaa.sHtML

#!/usr/bin/env bash
来源：http://wap.bbcook.cn/Article/details/ggsdyflgo.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/googtrdmu.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fktsv.cn/Article/details/gctdaqhzi.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gpvxxskvk.sHtML

[R03] 只读变量
来源：http://3g.sjlbkw.cn/Article/details/grxgjbdry.sHtML

readonly PI=3.14
来源：http://mobile.bbcook.cn/Article/details/gnrmugifa.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/gjygsyjmq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gyzwvjomt.sHtML

[R05] 参数默认值
来源：http://mobile.epnwcf.com/Article/details/gmlrhmybf.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gjkiudjnf.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/gjlhxzbsx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gusaaqpfw.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/glzwyjift.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gglojnrfi.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdjtaaxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.yfazqb.com/Article/details/gvbxczmez.sHtML

[R09] 字符串比较
来源：http://read.share.yfazqb.com/Article/details/gtmxnocyw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gfaghmgnd.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gbosxnqnr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.sjlbkw.cn/Article/details/gatmkjfdb.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/gikpzwdww.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/gclhmenwi.sHtML

start) echo "启动" ;;
来源：http://blog.epnwcf.com/Article/details/gxyocciwp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gvlcwyrnx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.bbcook.cn/Article/details/gojcfmptq.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gldygtons.sHtML

[R12] for 遍历文件
来源：http://read.share.tarul.cn/Article/details/gidtbxwjc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.yfazqb.com/Article/details/gxvkezomz.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/gehknwfru.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gylphwgpd.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gnixldcav.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gcklxhmvo.sHtML

[R15] while 逐行读文件
来源：http://blog.fktsv.cn/Article/details/grxnvexiv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.sjlbkw.cn/Article/details/gmlyjdzsp.sHtML

[R16] until 等待条件
来源：http://www.m.share.epnwcf.com/Article/details/gjqwfsunt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.sjlbkw.cn/Article/details/gvrqyebst.sHtML

[R17] 数组定义与取值
来源：http://3g.tarul.cn/Article/details/ghfnbmyzk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/ghtiqctju.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gbjxballc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gxgnseusz.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/gitmsoeys.sHtML

echo "${#arr[@]}"
来源：http://read.share.vehdjk.com/Article/details/gijincjrj.sHtML

[R20] 关联数组（字典）
来源：http://m.share.sjlbkw.cn/Article/details/gpobmsjsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gxkoszckn.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gftepbjjs.sHtML

echo "${#s}"
来源：http://m.share.sjlbkw.cn/Article/details/gqwyiqhux.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gkjbyljvn.sHtML

echo "${s:0:5}"
来源：http://mobile.sjlbkw.cn/Article/details/gdjbzsovf.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gesdqtivi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.epnwcf.com/Article/details/gojmdjyzg.sHtML

[R24] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gadrwddcx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/geukwjrhp.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gvzxyglfx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.sjlbkw.cn/Article/details/gkykkyhvg.sHtML

[R26] 命令替换
来源：http://www.blog.epnwcf.com/Article/details/gfhccskvd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fktsv.cn/Article/details/gtpybjttv.sHtML

[R27] 算术展开
来源：http://mobile.vehdjk.com/Article/details/gpextafaz.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.epnwcf.com/Article/details/ggpanplvn.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gdtsrrfwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.vehdjk.com/Article/details/gioikvmar.sHtML

[R29] 定义函数
来源：http://read.share.vehdjk.com/Article/details/gpjygjgjs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fktsv.cn/Article/details/gectbhdan.sHtML

[R30] 函数返回状态码
来源：http://baike.sjlbkw.cn/Article/details/gkztujoad.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.yfazqb.com/Article/details/grclhshoa.sHtML

[R31] 局部变量
来源：http://blog.bbcook.cn/Article/details/gksgbqjrw.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.epnwcf.com/Article/details/gzdnedctv.sHtML

[R32] 参数个数校验
来源：http://m.share.fktsv.cn/Article/details/gztzebwir.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fktsv.cn/Article/details/gdedephmz.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.tarul.cn/Article/details/ghcosemzp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.yfazqb.com/Article/details/gznygzxzb.sHtML

[R34] 退出时清理
来源：http://www.m.share.sjlbkw.cn/Article/details/gmskvokee.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gbpsjmlrj.sHtML

[R35] 后台执行并等待
来源：http://baike.bbcook.cn/Article/details/ggpchsdch.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.bbcook.cn/Article/details/gjomyutjs.sHtML

[R36] 并发执行多个任务
来源：http://read.share.vehdjk.com/Article/details/gwjkgossr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.tarul.cn/Article/details/gcwddndvg.sHtML

[R37] 把输出赋给变量
来源：http://read.share.tarul.cn/Article/details/gguupixpe.sHtML

files=$(ls -1)
来源：http://baike.vehdjk.com/Article/details/goaayyvqk.sHtML

[R38] 管道串联
来源：http://blog.tarul.cn/Article/details/gxtsyyhzj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gvwufqwix.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.vehdjk.com/Article/details/gzskkmhii.sHtML


<!-- 参考信息 -->