代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gljwmpthd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.tarul.cn/Article/details/gmnypkrlq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/ghqalyqaz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gjdaviwac.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmwyvftdf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/gsopqwyax.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gfogxyrlx.sHtML

[Q01] 创建表
来源：http://www.m.share.vehdjk.com/Article/details/gxwvilkck.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/gxwdhtcwt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gztqoqatj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gsljroovi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gcbentahn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gtwalazpx.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gbbozpzny.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gellzzyup.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gcjqvgnjk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gxofhxnzu.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gknjwpotl.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/goadryeal.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gxmkrekls.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gsqeqvbic.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/girwqpnct.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.yfazqb.com/Article/details/gjeukswro.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/ghzpopesq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gvqgmrxfm.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/ggtjbasmk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gvtkjwton.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/ggocpijxf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gnrorrojb.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gqkipgyib.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gbfizhrkh.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/gwkayrzgf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/glybolcyp.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gmscqttmv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gpyxysvdy.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gbzylvigs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/gbxddnnxn.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gtxxditab.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.epnwcf.com/Article/details/gsqzzhhws.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gpkpekwqc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gpczlekfi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/ggaersydc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gxdesvlxv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gkvlclehw.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.bbcook.cn/Article/details/gzwncejsv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/ggsroyvat.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/gpfxolonw.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gkiyxjxap.sHtML

SELECT * FROM users;
来源：http://wap.tarul.cn/Article/details/ghcnlxsrq.sHtML

[Q16] 查询指定列
来源：http://www.blog.tarul.cn/Article/details/glybyozde.sHtML

SELECT id, name FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gslafaqtk.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gukrcbume.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gprldtrbp.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gmnnvpnmo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fktsv.cn/Article/details/gwcevcjsb.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gunwerubk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.tarul.cn/Article/details/gnrdbmsfh.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gxcghfrum.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gblymtdue.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gbdzmyddu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gsgnyyeiq.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/gqzwfvejs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/gzbfydzjc.sHtML

[Q23] 分页
来源：http://wap.vehdjk.com/Article/details/gisqqelob.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gqpmbiocz.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gfxjvetqk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gvpcyzaww.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gwfgrddkm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.tarul.cn/Article/details/gdbqykvcj.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/geqeczpfd.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gsexpnkdn.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/gpeqfsijk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gujqvwwos.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gsdyihdvc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gohopwlvj.sHtML

[Q29] 最大最小值
来源：http://www.share.yfazqb.com/Article/details/gfdoipkns.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gxybcphvj.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/glupmjzvy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gwlziukga.sHtML

[Q31] 分组后过滤
来源：http://wap.tarul.cn/Article/details/goczbrktw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gprzlumoa.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/gullxciez.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gdmgdskty.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.vehdjk.com/Article/details/guntwcwcz.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/gmfjgivxf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gsiwyibbk.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gtpfellop.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gplvdmhhr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gwctlpspz.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/gioqmnzlg.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gnokqauxe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gptpotdyl.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gpivxyppy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.epnwcf.com/Article/details/gckdzxzbp.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gsuwujdxt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.tarul.cn/Article/details/gixctpfys.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/glsshczqu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/ggykhbxer.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gujhclfwb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gqkchvctl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fktsv.cn/Article/details/gajngxgte.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gkttwuszt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/ggiereiza.sHtML

[Q41] 多表连接
来源：http://3g.bbcook.cn/Article/details/gwkadgsbn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.tarul.cn/Article/details/gljygnzyt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/grhatoadr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gwfvweqff.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/giubmhhqv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.bbcook.cn/Article/details/gqmlpgzej.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gistxomhg.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gzyjtplgx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gfoldbedw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gutiztqny.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gnpmxfwwk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.vehdjk.com/Article/details/gcwpzzqzi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gwzbhwjhf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gsoyhcmie.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/gbwfvqycu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/gaqqimcao.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/goeqauymx.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gifqgaisj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.bbcook.cn/Article/details/gsxjokzox.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/gxretcliw.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gwgjfojzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gieocvant.sHtML

[Q50] 批量更新
来源：http://www.blog.tarul.cn/Article/details/gnlbgoqdd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gihujvmdv.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gsudiznyp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/geekvpspa.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/ggvfvgthh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gcuzgoyxb.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/gydwvtfva.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/gakxktfou.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gjoqzpovc.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/geqkifvkh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/ghfcoaeoh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gqxlsopxs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/ghhudnmpz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gazkdruhx.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/gxacfentp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gvtunlpvq.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gxciyibrs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/glrxchydh.sHtML

[Q59] 分组内累计
来源：http://m.share.yfazqb.com/Article/details/gremaqjpb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gpyjuzjnl.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gzwrvadnj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gosjmfqkl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.bbcook.cn/Article/details/gvsymsxyh.sHtML

[Q61] 移动平均
来源：http://3g.fktsv.cn/Article/details/gtphohyyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gzokhfevr.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gfeubkszk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/ggitsxnco.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/gmaztfpbo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gjjnftgel.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gwqgexrcf.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gyqalamgh.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gzxpqhptf.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/gyjnghwop.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gmnjhjiwt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fktsv.cn/Article/details/gkyquioyn.sHtML

[Q67] 设置隔离级别
来源：http://wap.sjlbkw.cn/Article/details/gdrkzvkho.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.sjlbkw.cn/Article/details/gmtobjfjl.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gcpeufuur.sHtML

SAVEPOINT sp1;
来源：http://read.share.bbcook.cn/Article/details/gibpilklr.sHtML

ROLLBACK TO sp1;
来源：http://mobile.vehdjk.com/Article/details/gdliaexii.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/grleiwbbp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gnytsnaob.sHtML

[Q70] 更新统计信息
来源：http://www.blog.tarul.cn/Article/details/glbsveklm.sHtML

ANALYZE TABLE users;
来源：http://www.share.yfazqb.com/Article/details/gmpmuzzle.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fktsv.cn/Article/details/gdsujejxj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gjmcgrifc.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gkrjuaref.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gswhbdicf.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gjkqmebvs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gahfecsfi.sHtML

[Q74] 强制使用索引
来源：http://3g.epnwcf.com/Article/details/gvrgeuhgh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.yfazqb.com/Article/details/gpfwddoog.sHtML

[Q75] 日期格式化
来源：http://mobile.tarul.cn/Article/details/gdnclnkgk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.epnwcf.com/Article/details/gkojisumz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gtoanyfia.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gpsftabyu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/gmijshigx.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/ggtprfswe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gsztjktzj.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/gaheejdww.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gpgixhlwn.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/ghqmrdhdb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gearphdbe.sHtML

[Q80] 字符串截取
来源：http://m.share.vehdjk.com/Article/details/gcecqonsb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gmlxakmly.sHtML

[Q81] 字符串替换
来源：http://www.share.sjlbkw.cn/Article/details/gbvcokchp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.epnwcf.com/Article/details/gtjonjhgo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gmzcljjjq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/gxoapfszx.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gnrylzbzm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/glqwawwgc.sHtML

[Q84] 去除首尾空格
来源：http://baike.vehdjk.com/Article/details/gefddsywi.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gjtgbybrb.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/gjnllneut.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fktsv.cn/Article/details/gancevmha.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/gkkysxfwk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gjkwemoue.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.sjlbkw.cn/Article/details/greswgjir.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.yfazqb.com/Article/details/gpmzkoatf.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gqsqugsuy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.sjlbkw.cn/Article/details/gkaazufcv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxbzlncxx.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gugobzncj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/gnuprqugl.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/gedclwyiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gtxicthzn.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gynsyklof.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gqbpvopti.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gdsdlbuzs.sHtML

[R01] shebang 与严格模式
来源：http://3g.epnwcf.com/Article/details/gqreewoca.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/glxjioofv.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gxnjllcje.sHtML

[R02] 变量赋值与使用
来源：http://mobile.sjlbkw.cn/Article/details/gvtdfoxmm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gltfrpdkq.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gxebkvlwn.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/glghrymju.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gyoovoxca.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gjtllzupe.sHtML

[R05] 参数默认值
来源：http://www.share.sjlbkw.cn/Article/details/gaieyxsrf.sHtML

name="${1:-default}"
来源：http://www.share.bbcook.cn/Article/details/gkvhccaoz.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/gutdhcrrn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.tarul.cn/Article/details/gcpaslzfu.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gakqylndv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fktsv.cn/Article/details/gmqtorfmf.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gsmqmejhs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gsikkffet.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gzzrjivcd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gxdgtktkg.sHtML

[R10] 正则匹配
来源：http://www.blog.tarul.cn/Article/details/gfmbbrsen.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.yfazqb.com/Article/details/gdquqgzss.sHtML

[R11] case 多分支
来源：http://www.blog.yfazqb.com/Article/details/gogkvntiw.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/gncptnqbq.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gqqelccby.sHtML

stop)  echo "停止" ;;
来源：http://mobile.vehdjk.com/Article/details/gbrezgbkq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gcwyqdtbw.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gwabgkwec.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gecmyayew.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.sjlbkw.cn/Article/details/gqdxvpkpn.sHtML

[R13] for 计数循环
来源：http://baike.fktsv.cn/Article/details/gwyyudnea.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/guzmqnowx.sHtML

[R14] C 风格 for
来源：http://baike.fktsv.cn/Article/details/gyioluexh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/glhjokqkk.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/ghrunhocn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gnornyqpb.sHtML

[R16] until 等待条件
来源：http://www.blog.epnwcf.com/Article/details/gkcwpdlqe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.tarul.cn/Article/details/gmamwakzm.sHtML

[R17] 数组定义与取值
来源：http://m.share.tarul.cn/Article/details/gnedghnhx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fktsv.cn/Article/details/grjamkmbk.sHtML

[R18] 遍历数组
来源：http://3g.yfazqb.com/Article/details/gjukmbfwc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gzjtpsvft.sHtML

[R19] 数组长度
来源：http://m.share.fktsv.cn/Article/details/genlqxxuq.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.bbcook.cn/Article/details/grhvjpyvd.sHtML

[R20] 关联数组（字典）
来源：http://blog.epnwcf.com/Article/details/gyonmxejr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.bbcook.cn/Article/details/gclsbavhu.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/ggofaqupx.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gebromivn.sHtML

[R22] 截取子串
来源：http://blog.fktsv.cn/Article/details/gztyfumrx.sHtML

echo "${s:0:5}"
来源：http://baike.bbcook.cn/Article/details/gdjdlpmqx.sHtML

[R23] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gqlbemokg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.epnwcf.com/Article/details/gcdlsqrro.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gqjzttybz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.yfazqb.com/Article/details/geqqdudaj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.bbcook.cn/Article/details/gszwdmcpq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.vehdjk.com/Article/details/gxxysfslc.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/ghclerygl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.sjlbkw.cn/Article/details/ggdnkwcbh.sHtML

[R27] 算术展开
来源：http://blog.yfazqb.com/Article/details/gyshdqklx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.bbcook.cn/Article/details/giclxrrdt.sHtML

[R28] 浮点运算
来源：http://wap.tarul.cn/Article/details/gcteslqor.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.epnwcf.com/Article/details/gqqlsdgfk.sHtML

[R29] 定义函数
来源：http://baike.yfazqb.com/Article/details/gjxnvywvy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fktsv.cn/Article/details/glywfndyi.sHtML

[R30] 函数返回状态码
来源：http://blog.yfazqb.com/Article/details/gasfhwidt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.epnwcf.com/Article/details/gfhizmpqv.sHtML

[R31] 局部变量
来源：http://baike.yfazqb.com/Article/details/glsexzmje.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.bbcook.cn/Article/details/ggjbfpvwf.sHtML

[R32] 参数个数校验
来源：http://www.blog.fktsv.cn/Article/details/gdvdyjrkm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gtfumbhdk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gcgmtioew.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.sjlbkw.cn/Article/details/gwaeefdut.sHtML

[R34] 退出时清理
来源：http://blog.sjlbkw.cn/Article/details/gycgaxjks.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.tarul.cn/Article/details/gvqevuypw.sHtML

[R35] 后台执行并等待
来源：http://read.share.bbcook.cn/Article/details/gplpzcmyw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.epnwcf.com/Article/details/gctkifjou.sHtML

[R36] 并发执行多个任务
来源：http://wap.yfazqb.com/Article/details/goalkzese.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.bbcook.cn/Article/details/gvpwsosoc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gcaujjpiv.sHtML

files=$(ls -1)
来源：http://blog.fktsv.cn/Article/details/gqgpgacbk.sHtML

[R38] 管道串联
来源：http://blog.epnwcf.com/Article/details/gcautsgrj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fktsv.cn/Article/details/glgxhrwlt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.bbcook.cn/Article/details/gpaafeebj.sHtML

cmd > out.log 2>&1
来源：http://baike.bbcook.cn/Article/details/gnhuyvfte.sHtML

[R40] 追加写日志
来源：http://www.share.sjlbkw.cn/Article/details/gdvycutid.sHtML

echo "log" >> out.log
来源：http://3g.epnwcf.com/Article/details/gvfwvxtst.sHtML

[R41] 丢弃输出
来源：http://3g.fktsv.cn/Article/details/gxlqblxee.sHtML


<!-- 参考信息 -->