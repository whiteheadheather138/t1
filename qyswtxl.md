代发 wailian999

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpkqvjdvz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.yfazqb.com/Article/details/greabrcvr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/goxgsjcep.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gzunbdpuy.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gslhdidzn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gxnxeztkm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gsgguaqqr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gyqvvbyae.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/ghdpcrupt.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/gwwkoxefg.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gsrbjsjbw.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gjrracmpa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/ggpuakonl.sHtML

user_id INT NOT NULL,
来源：http://wap.tarul.cn/Article/details/gntzryhxd.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.bbcook.cn/Article/details/gftmaimno.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/gooreykwr.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gvmkbrkvz.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/grgpxiocb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/giapqqdob.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gfrijtohn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gozhrzoqj.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/grdrwgcje.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.epnwcf.com/Article/details/gyryylupe.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gfnvufpni.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.vehdjk.com/Article/details/gvwdesopk.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gfpkptgtt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gepobjbfe.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gjtwikqbc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/ggyywvwkx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gidnpfdsa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gahfjwijk.sHtML

[Q10] 插入单行
来源：http://blog.fktsv.cn/Article/details/gexwljrts.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gugloizyl.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gfuoqghen.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gfplenbqq.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.epnwcf.com/Article/details/grznennoa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/grzexmgig.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/gvkfraoue.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gxhajalue.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/glvlnxbhk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/gxzilbnck.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gewopueok.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gqhnklqas.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/gomuwrgjx.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gagqyicct.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/geceujgwj.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfuqatspn.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gunbgqacg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/guwzbyhpj.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gesjldsaq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.sjlbkw.cn/Article/details/gxvjegtlx.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/ggbhnbpxx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gzedyrmqh.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gvzsgrscd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gucldcwgk.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/glsvadobe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gzqlgytvz.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/gcbryxqgq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.epnwcf.com/Article/details/gvkjzqnxm.sHtML

[Q23] 分页
来源：http://3g.tarul.cn/Article/details/ghvmsmdmo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gfufeknub.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gbxgbbyrx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gccpwtuil.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxjlpozn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gdyihycmj.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/glwrgasfo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gaoflmpqb.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gzooiwbqz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/guqqivqqk.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gjxyduvtb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/grsrelqjr.sHtML

[Q29] 最大最小值
来源：http://read.share.vehdjk.com/Article/details/gpofxkalc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gzriimsgn.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/gbpkgixaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gwzsmqbuo.sHtML

[Q31] 分组后过滤
来源：http://www.blog.tarul.cn/Article/details/gnmvawmmt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.bbcook.cn/Article/details/gagsofnvb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/ghaitryty.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/ggciipanp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/ghktiqkth.sHtML

[Q33] 多列分组
来源：http://3g.epnwcf.com/Article/details/ghrfngqlg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gxxrztocp.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/ghrflnytc.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/gcrzhrrht.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gnuucfqad.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gzjkbiofy.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gufmbbawt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gsntsbetn.sHtML

[Q36] 左连接
来源：http://baike.fktsv.cn/Article/details/gdmjqryyz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gohfdbhuj.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gqzfrlvks.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.yfazqb.com/Article/details/gnfnbnmci.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.bbcook.cn/Article/details/gdvtapkwl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gddnrauop.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gnodrkdpg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/gqzsuiaht.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gbdjmmghv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gewyvwxnr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/ggrykmdhd.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gphkkqpim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gjqktgran.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gscjacuxu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/goccbymqh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gnmljkhck.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gmpwnjlhe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gvbzqzpfq.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/gqbarkikb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/guhucsiev.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gdlybngop.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/gsflupofc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.tarul.cn/Article/details/gzovkqzhe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gnliddmlv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gwdbuiwmb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gzfdwridl.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/glocycvgc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gtgalirfm.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gelqwodwi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/grwwlkvaj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gspchxeyz.sHtML

[Q49] 更新单行
来源：http://mobile.fktsv.cn/Article/details/gjtdfocci.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/goeqgindp.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/grzggvgzn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.vehdjk.com/Article/details/gvkehkfth.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/grujoltwv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.yfazqb.com/Article/details/gjvihvdip.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/gfjowlypa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gejescdyg.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/glvypqnut.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gtiknydds.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gwhwnnyin.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gvgawzngf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/gjjgemuxx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gemfcydjr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gvlvzxppx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.vehdjk.com/Article/details/glbwwrdzc.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gfifbhjic.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.tarul.cn/Article/details/gkktwigcy.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gwenpruvn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gnxuhuzvd.sHtML

[Q59] 分组内累计
来源：http://m.share.vehdjk.com/Article/details/gvhfuoabi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ghymffkcu.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.bbcook.cn/Article/details/gqqjytrvl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gyqcayibu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gvbnbmudl.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gcbepcjpw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gblwluhpz.sHtML

[Q62] 分组占比
来源：http://www.m.share.fktsv.cn/Article/details/gmgiaders.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gymjmecdk.sHtML

[Q63] 开启事务
来源：http://read.share.yfazqb.com/Article/details/grrxswbqj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/gmezvakuf.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gvagonuhk.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/goejwqtdx.sHtML

[Q65] 回滚事务
来源：http://blog.fktsv.cn/Article/details/gusnpiaxw.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gmnvglqpe.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gmeibbbsc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.yfazqb.com/Article/details/gifjghppu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gfoecnyxl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gqduslobv.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/gcuvbzyck.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gijcfwsyc.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gzspldmqx.sHtML

[Q69] 查看执行计划
来源：http://read.share.vehdjk.com/Article/details/guznciarv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gxilkhuqu.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/geygogvqz.sHtML

ANALYZE TABLE users;
来源：http://m.share.yfazqb.com/Article/details/gcsmfxfxk.sHtML

[Q71] 查看建表语句
来源：http://3g.bbcook.cn/Article/details/gngdtgilu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gtmyujofk.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/guzmympxm.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/guqnoodwp.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/gnfjuyzdq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fktsv.cn/Article/details/glqqntejf.sHtML

[Q74] 强制使用索引
来源：http://m.share.bbcook.cn/Article/details/ggclkpmou.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fktsv.cn/Article/details/girdxjxhu.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gzlqptvtw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.bbcook.cn/Article/details/gvyebbpey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gjvqdswbm.sHtML

[Q76] 按天统计
来源：http://www.share.yfazqb.com/Article/details/gqxpecgjq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/gdyigvclj.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gtkjuifrq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gkzufsydl.sHtML

[Q78] 当前时间
来源：http://blog.vehdjk.com/Article/details/gnryndtly.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gnmzltrtl.sHtML

[Q79] 字符串拼接
来源：http://wap.vehdjk.com/Article/details/gggylzupd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/ghdskvruk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/goseygdac.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gigbkbbbt.sHtML

[Q81] 字符串替换
来源：http://m.share.vehdjk.com/Article/details/glilezoeg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gpmumoulz.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gaprgmioc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/grktunewg.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gnucbmxig.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gvcjfmngg.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/gqadjppzk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/grhfyedkg.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gysskxgen.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/gzlavskya.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gevosbctu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gsuhgfrmv.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/geuwcvhws.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gavsprpfz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gtbuxbmlh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.bbcook.cn/Article/details/gydvztyva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.vehdjk.com/Article/details/gcvbryvwa.sHtML

[Q89] 判断表是否存在
来源：http://3g.fktsv.cn/Article/details/glfrqbfaa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.vehdjk.com/Article/details/gcxixfqsp.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gmddfairp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gisxiydst.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/grsbvpgdy.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/gttnqvfth.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gmtcitzsi.sHtML

[R01] shebang 与严格模式
来源：http://blog.sjlbkw.cn/Article/details/gejtsdreh.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/goahrfjpp.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gkmbtmqfq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gujoalton.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gtdfexpwq.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/glkprzoaa.sHtML

readonly PI=3.14
来源：http://mobile.vehdjk.com/Article/details/gsaeppoeg.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/ghosbgfkj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.vehdjk.com/Article/details/ggcmlfcmw.sHtML

[R05] 参数默认值
来源：http://read.share.yfazqb.com/Article/details/geiyqwgad.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gugvugmhh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.yfazqb.com/Article/details/gvgpxkopi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/geskagtfc.sHtML

[R07] if 判断文件
来源：http://wap.tarul.cn/Article/details/grnnzmkox.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gjxeiuxcw.sHtML

[R08] 数值比较
来源：http://www.blog.fktsv.cn/Article/details/gkwahuiej.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.vehdjk.com/Article/details/gjlskpppk.sHtML

[R09] 字符串比较
来源：http://blog.bbcook.cn/Article/details/gnfsschwi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gepmwvlun.sHtML

[R10] 正则匹配
来源：http://www.m.share.tarul.cn/Article/details/gkuugmzsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gwjlvhcso.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/geahqmuvp.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gczrsppkz.sHtML

start) echo "启动" ;;
来源：http://read.share.bbcook.cn/Article/details/gqhvoogaw.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/ggxaesxen.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/gmowchhde.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gocihycot.sHtML

[R12] for 遍历文件
来源：http://baike.tarul.cn/Article/details/gjlmlblno.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gorvfxtrd.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gtdgrseja.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gswcbrzbh.sHtML

[R14] C 风格 for
来源：http://www.m.share.tarul.cn/Article/details/gdntuasie.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gdrcblrjd.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/ggoxcbyxh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.vehdjk.com/Article/details/gkzflefhb.sHtML

[R16] until 等待条件
来源：http://wap.bbcook.cn/Article/details/gbsjsyjqf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.sjlbkw.cn/Article/details/gwznthevp.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/getdakqme.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gleycwzst.sHtML

[R18] 遍历数组
来源：http://baike.fktsv.cn/Article/details/gilrjppac.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.vehdjk.com/Article/details/gdkqhqnls.sHtML

[R19] 数组长度
来源：http://m.share.vehdjk.com/Article/details/gdbzkrdmz.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/ggzvqzitb.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gedoupdpv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gycqgtdss.sHtML

[R21] 字符串长度
来源：http://www.m.share.vehdjk.com/Article/details/gputndlet.sHtML

echo "${#s}"
来源：http://3g.epnwcf.com/Article/details/gnpvxpadb.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gwpsuymec.sHtML

echo "${s:0:5}"
来源：http://3g.yfazqb.com/Article/details/gzvzpskly.sHtML

[R23] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/gpdkfnwmu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.epnwcf.com/Article/details/ggqkdmyzt.sHtML

[R24] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gfdnfgxsr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.bbcook.cn/Article/details/gsjveukym.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.yfazqb.com/Article/details/grgmmybwe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gugiaddga.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gnoqhjpbb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.tarul.cn/Article/details/gidpeehwq.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gngmctlrz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fktsv.cn/Article/details/gmsparksa.sHtML

[R28] 浮点运算
来源：http://blog.sjlbkw.cn/Article/details/guvpgcrop.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.bbcook.cn/Article/details/guoeibrun.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gsxjwbanj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fktsv.cn/Article/details/gecrumvrs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gqmjhmhev.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.yfazqb.com/Article/details/gvytazvpz.sHtML

[R31] 局部变量
来源：http://read.share.bbcook.cn/Article/details/gqtrwjser.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.yfazqb.com/Article/details/gpurzgrgt.sHtML

[R32] 参数个数校验
来源：http://wap.fktsv.cn/Article/details/gyybgvclj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.sjlbkw.cn/Article/details/gzanesjtk.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.sjlbkw.cn/Article/details/gziiskrun.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.yfazqb.com/Article/details/gajyzovmx.sHtML

[R34] 退出时清理
来源：http://wap.bbcook.cn/Article/details/gevfafqnd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.sjlbkw.cn/Article/details/grjyaykdk.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gxrlwpsqv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.bbcook.cn/Article/details/gxpzyarth.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.epnwcf.com/Article/details/gdutgjnxt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.epnwcf.com/Article/details/gvzpdfssb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.sjlbkw.cn/Article/details/gndvufghq.sHtML

files=$(ls -1)
来源：http://www.share.fktsv.cn/Article/details/gxjgponae.sHtML

[R38] 管道串联
来源：http://www.blog.tarul.cn/Article/details/gkryuacjo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.vehdjk.com/Article/details/gpcbmwasi.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.bbcook.cn/Article/details/gueihobdr.sHtML

cmd > out.log 2>&1
来源：http://3g.bbcook.cn/Article/details/gxcwkqttl.sHtML

[R40] 追加写日志
来源：http://wap.yfazqb.com/Article/details/gcwyepwua.sHtML

echo "log" >> out.log
来源：http://baike.tarul.cn/Article/details/gmrwmqxzf.sHtML

[R41] 丢弃输出
来源：http://www.m.share.bbcook.cn/Article/details/ggdbsdqfb.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.epnwcf.com/Article/details/gimgxacxn.sHtML

[R42] 输入重定向
来源：http://3g.epnwcf.com/Article/details/gmcyqbgsc.sHtML

wc -l < a.txt
来源：http://baike.tarul.cn/Article/details/gmsxmsxbz.sHtML

[R43] 按名字查找文件
来源：http://www.blog.bbcook.cn/Article/details/gsukqmyry.sHtML


<!-- 参考信息 -->