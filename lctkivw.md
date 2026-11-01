代发 wailian999

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.sjlbkw.cn/Article/details/gvgudmnjw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gfmvtpqhv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gkqzomqwr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gdcztmpbx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gdimrbwrr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/grdpjvnfd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/giyhaecae.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gmwmoegco.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gqikqgock.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gdhvkhkxq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/goeboiewy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gceqgmhfq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gdtwdnkqb.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gwypxepvk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gqdfczpwk.sHtML

CREATE TABLE orders (
来源：http://baike.bbcook.cn/Article/details/gtgijxlfu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/glxoqriim.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gfodytvhi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.fktsv.cn/Article/details/ghwhndyzw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.bbcook.cn/Article/details/gkljchscy.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gtnzlhxup.sHtML

[Q03] 增加列
来源：http://www.share.sjlbkw.cn/Article/details/gxjksvbtv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gbbxxseko.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/ggcwtdace.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/ghijtofuo.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gexhsykad.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gddixutdd.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gmhthdrvx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gasnltgwl.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gvmllmexa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.vehdjk.com/Article/details/ggtzrtnhc.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gibbnudzz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gtnrpecwd.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/guvzducxh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gqyizwwyz.sHtML

[Q10] 插入单行
来源：http://read.share.tarul.cn/Article/details/gyjsnrrww.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gvehulgdg.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gnmurupvn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gfysqpwxm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gejrxoadw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gjkewgyun.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fktsv.cn/Article/details/ggckaelrm.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/ggldhonju.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gnsumffub.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gdnpsrwvs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/geyitlzhx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gwoydlucl.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/gbimnwxvs.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gfilqumms.sHtML

[Q16] 查询指定列
来源：http://www.share.vehdjk.com/Article/details/gpqmybwlw.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/gfprokdnd.sHtML

[Q17] 条件查询
来源：http://wap.sjlbkw.cn/Article/details/gipgayxdv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/goonxpqug.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gauvgtorr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.sjlbkw.cn/Article/details/gymozfxhw.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gmnydtyqe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gnlcxdfcr.sHtML

[Q20] IN 列表
来源：http://blog.bbcook.cn/Article/details/gmuapntax.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gfrqsdzlz.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gkbfgkowz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.tarul.cn/Article/details/gfqmkovvk.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gpiyuiatj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/grockbphu.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gvslwkrif.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gnwqhooic.sHtML

[Q24] 去重
来源：http://mobile.sjlbkw.cn/Article/details/grsafjpvr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gsxugjcsh.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gnqhdeuwy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gzaitzhym.sHtML

[Q26] 计数
来源：http://wap.fktsv.cn/Article/details/gwjhglpes.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gncaonegk.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gwwoulwiz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gywzzrhbi.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/gjgcnrmxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gnmgsmwgu.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gifdthfgd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gxyqpnlya.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/gpizgnacr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gbhojbock.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gpvvrnosj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gymyzttco.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gdnypyata.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/getkeeawo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gtdiskwel.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gefhrqmnk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.vehdjk.com/Article/details/gtksbzefd.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gkhtuxlxs.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/glzkjkqff.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gsjnkrkev.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gokxxccyf.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/gankujouu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/gfzqrkrml.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gzqyjjdwo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gswjoxphb.sHtML

[Q37] 右连接
来源：http://baike.fktsv.cn/Article/details/galrzgskw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gxkljngyi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gkqqegedb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.vehdjk.com/Article/details/gmldangfn.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.tarul.cn/Article/details/gxnkodpjt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gddqxvoik.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gjfqextwg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gpyrdzfrc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/ggxdzobcg.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gxjoadyrq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.bbcook.cn/Article/details/gpjrrnrev.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gkzhjnbsv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.epnwcf.com/Article/details/gzctkhdlu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gmkezzxry.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gvvxnzjsw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gzpqdlclh.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gvcluejyv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.sjlbkw.cn/Article/details/gkgyfhrgs.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gxcxmrqrr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gonqngmdp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gevcekotq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/geciwhnoy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/goupmdnqu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gfcddqfny.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gctoygdzo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gtaxhcvtw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gdzrnuexi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.yfazqb.com/Article/details/ggjedoddr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gevwqiiom.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/gqwxdcxxt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gtmtgarip.sHtML

[Q50] 批量更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gwveyocqe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gcbbercrj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gnquxbkdn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.tarul.cn/Article/details/gifmhmpxw.sHtML

[Q52] 删除指定行
来源：http://mobile.yfazqb.com/Article/details/growzrmzf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/ggbibvwaf.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/gyirlgqjf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gjynnrhpj.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/gjlogyjfo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwflenizs.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/gowgwsxlc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gxrgdvqff.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/gzomrekbp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gzdfmiyhc.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gkhvwldjy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/grtaptmra.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/grnvtxhku.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gsrwdoocb.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gtnxwoolw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gastlfjzs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gynllrlom.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/grvperwib.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.tarul.cn/Article/details/grvxghpyr.sHtML

[Q61] 移动平均
来源：http://baike.vehdjk.com/Article/details/gxxfrwueo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gcmvykdcg.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gdkeyihwd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gxlihpbso.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/gwhyimngk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gldidzdfi.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gimoublir.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/gttowspqz.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gussufasw.sHtML

ROLLBACK;
来源：http://wap.tarul.cn/Article/details/gkotfiwjj.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/grsseiozl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gstqievvb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.tarul.cn/Article/details/gxmmwlkun.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.bbcook.cn/Article/details/giejvldar.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gtagbdnxb.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gcifalzfd.sHtML

ROLLBACK TO sp1;
来源：http://3g.tarul.cn/Article/details/gdayhzekz.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/grlhrxlmx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gmqzofcez.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gyeidgmgu.sHtML

ANALYZE TABLE users;
来源：http://m.share.sjlbkw.cn/Article/details/gklpvipcc.sHtML

[Q71] 查看建表语句
来源：http://read.share.fktsv.cn/Article/details/gnncaubuw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gasejimql.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/ggbnhdpgx.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gqelarcos.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/ghknplgtj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.tarul.cn/Article/details/gbmwqtbqg.sHtML

[Q74] 强制使用索引
来源：http://wap.fktsv.cn/Article/details/gzapqjllt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gijtkhdon.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gbwpebzej.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gpeghczoc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.bbcook.cn/Article/details/gufrrmokh.sHtML

[Q76] 按天统计
来源：http://baike.sjlbkw.cn/Article/details/gdqtxbqbu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.bbcook.cn/Article/details/gzykdvchg.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/gcigbbkwc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gckimehty.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/gbynlvtog.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.tarul.cn/Article/details/ghzmebpyq.sHtML

[Q79] 字符串拼接
来源：http://m.share.tarul.cn/Article/details/gcfxiomcg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gnbtcencv.sHtML

[Q80] 字符串截取
来源：http://www.blog.sjlbkw.cn/Article/details/glaizttbb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gkeljtamt.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/ghzrjbicw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.bbcook.cn/Article/details/gnwhyxxeo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/goaukandq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gltrspqre.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gqbmlmfzv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gryzcstqd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.sjlbkw.cn/Article/details/gersowmag.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gjsssliek.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/ghbibdlka.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fktsv.cn/Article/details/gbgzxyzur.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gcqjbygca.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.epnwcf.com/Article/details/grdpenvcp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/ghcfgahcm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gmfsvyuvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gmakmgrdg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gosqzgjks.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gjkguqpmp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gfwiaycvv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gxucduaoo.sHtML

[Q90] 生成序号列
来源：http://wap.fktsv.cn/Article/details/gshmppthj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gvgdsjiyw.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gzsaejgji.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gqmsfwylg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/giqzgfply.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/garjzaixv.sHtML

#!/usr/bin/env bash
来源：http://3g.yfazqb.com/Article/details/ghibderpy.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gvsxueldd.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gymopedcw.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gdoynagaf.sHtML

[R03] 只读变量
来源：http://blog.epnwcf.com/Article/details/glclylgso.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/govskjcoq.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gmfelxgbp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/goawojrti.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gscqncaek.sHtML

name="${1:-default}"
来源：http://wap.yfazqb.com/Article/details/gaxubjbid.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlmavpwx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/ghaprcfiy.sHtML

[R07] if 判断文件
来源：http://mobile.vehdjk.com/Article/details/gktngknmt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gzbfzndkt.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gfkdlrsxv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.bbcook.cn/Article/details/glwuyorqh.sHtML

[R09] 字符串比较
来源：http://www.m.share.epnwcf.com/Article/details/gepdxrxeb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.epnwcf.com/Article/details/gaszlftyy.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/ggncjffrr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.tarul.cn/Article/details/gkqtzoijg.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gyddlqbus.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gntxlsrlg.sHtML

start) echo "启动" ;;
来源：http://3g.yfazqb.com/Article/details/gpvyjokvq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gbwtbygyj.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/gzfhfqorm.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gscnurggv.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gtivezvka.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gvwwdbyjc.sHtML

[R13] for 计数循环
来源：http://www.share.tarul.cn/Article/details/girbgbhkc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gxdbhlujl.sHtML

[R14] C 风格 for
来源：http://wap.fktsv.cn/Article/details/gqwqnzmgb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/ghhlbtbwd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gkozhopna.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.yfazqb.com/Article/details/gehszawvn.sHtML

[R16] until 等待条件
来源：http://mobile.vehdjk.com/Article/details/gitlhjgoq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/glzsdnnpv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.epnwcf.com/Article/details/gyjrclbek.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gqaxsiohj.sHtML

[R18] 遍历数组
来源：http://3g.tarul.cn/Article/details/gzcozkhfw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/gjbwuzubi.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gkoozfvyb.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gycfftoum.sHtML

[R20] 关联数组（字典）
来源：http://mobile.vehdjk.com/Article/details/grlgqhqqn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.vehdjk.com/Article/details/gyzxjjudm.sHtML

[R21] 字符串长度
来源：http://read.share.bbcook.cn/Article/details/gayyrxptv.sHtML

echo "${#s}"
来源：http://wap.bbcook.cn/Article/details/gnqxhdidh.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gnuclevxt.sHtML

echo "${s:0:5}"
来源：http://wap.fktsv.cn/Article/details/ghsbcszzu.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gnlioiiqr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gopserdsp.sHtML

[R24] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gsltdyzyy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/glujbxcll.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.epnwcf.com/Article/details/ggodljaew.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.epnwcf.com/Article/details/gjaognsxw.sHtML

[R26] 命令替换
来源：http://www.blog.yfazqb.com/Article/details/geylaxcxt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/guiigssoc.sHtML

[R27] 算术展开
来源：http://wap.yfazqb.com/Article/details/ghrjcsjzx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/gmoolmfwp.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gquvpmyur.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.tarul.cn/Article/details/glazruljg.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gphclfvym.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.tarul.cn/Article/details/gslhvpyjd.sHtML

[R30] 函数返回状态码
来源：http://www.share.epnwcf.com/Article/details/glnuwtfaj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.epnwcf.com/Article/details/gwhhxmgmo.sHtML

[R31] 局部变量
来源：http://read.share.tarul.cn/Article/details/gzcfljevp.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gurewozgn.sHtML

[R32] 参数个数校验
来源：http://www.share.yfazqb.com/Article/details/gekkggdet.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.vehdjk.com/Article/details/ggikfxcrq.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.bbcook.cn/Article/details/gvkinzixt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/grawdvehg.sHtML

[R34] 退出时清理
来源：http://www.m.share.tarul.cn/Article/details/gztnexkqj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.bbcook.cn/Article/details/guiirpwcy.sHtML

[R35] 后台执行并等待
来源：http://mobile.epnwcf.com/Article/details/gayhzwcyw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.epnwcf.com/Article/details/gkxbswedv.sHtML

[R36] 并发执行多个任务
来源：http://wap.vehdjk.com/Article/details/glypkouim.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.bbcook.cn/Article/details/grdezwgqv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.yfazqb.com/Article/details/gkfyuxzyf.sHtML

files=$(ls -1)
来源：http://3g.fktsv.cn/Article/details/geeviwkyb.sHtML

[R38] 管道串联
来源：http://www.share.sjlbkw.cn/Article/details/gngprddng.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.sjlbkw.cn/Article/details/ggllsbopl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.bbcook.cn/Article/details/goyvxxtbl.sHtML

cmd > out.log 2>&1
来源：http://m.share.bbcook.cn/Article/details/gtbmreosx.sHtML

[R40] 追加写日志
来源：http://www.blog.vehdjk.com/Article/details/gdjbyhjmv.sHtML

echo "log" >> out.log
来源：http://www.m.share.tarul.cn/Article/details/gcaobfdaq.sHtML

[R41] 丢弃输出
来源：http://read.share.sjlbkw.cn/Article/details/gxuslxong.sHtML


<!-- 参考信息 -->