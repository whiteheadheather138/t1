代发 wailian999

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gygdfqfld.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gowcicami.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.vehdjk.com/Article/details/gannxypna.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gbvpjliuc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/goadmzitp.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/gthhqefzh.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gfzbnjkcj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gvpdladcj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gdoprgcbi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gdmleiwxx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gnlyojwqh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.yfazqb.com/Article/details/gditixwdj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gowtuptzi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gntfdygbx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcsxfnkf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/grvibpuxt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gckkywpyd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gtzazoawu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gcmedmnbs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/guzohckrw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/gpyfxhdfs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.yfazqb.com/Article/details/gqpjzqjct.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.epnwcf.com/Article/details/gdtadihvl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/ggircbkui.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnsmlxboz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gnldjzizf.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gadfoghiz.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gibvdzoln.sHtML

CREATE TABLE users (
来源：http://www.blog.bbcook.cn/Article/details/gxzqgxizq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/gnzfpsacb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gblyigwnj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gmwwrhxip.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/gwexfpren.sHtML

);
来源：http://baike.tarul.cn/Article/details/guksqkwmt.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gkqsyzqsu.sHtML

CREATE TABLE orders (
来源：http://m.share.vehdjk.com/Article/details/gepzdedcr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gwvxspkvh.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gyaiuimiz.sHtML

amount DECIMAL(10, 2),
来源：http://wap.epnwcf.com/Article/details/gdkvtgwbr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gxyibvohj.sHtML

);
来源：http://blog.vehdjk.com/Article/details/graozmegz.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gfamemdfc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/goebklezz.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/giumzwyxl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.bbcook.cn/Article/details/gcdheawda.sHtML

[Q05] 重命名列
来源：http://wap.epnwcf.com/Article/details/gjouvhdxk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/ghbzcocjv.sHtML

[Q06] 删除列
来源：http://blog.sjlbkw.cn/Article/details/gozswlvjz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gyvkztggf.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/gkivccqhi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gatpsgqxt.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/gxkgzryaj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/guauznuzc.sHtML

[Q09] 创建唯一索引
来源：http://baike.tarul.cn/Article/details/gbqyxovud.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gmvduwdad.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gagaxyjzw.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gwrpyzmqc.sHtML

[Q11] 一次插入多行
来源：http://www.share.sjlbkw.cn/Article/details/gsplkwmrt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.vehdjk.com/Article/details/gfbgfmaza.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fktsv.cn/Article/details/gvbbgqmsx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gvzqnqtbi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/grhhscxxu.sHtML

[Q13] 忽略重复插入
来源：http://read.share.yfazqb.com/Article/details/gaajdlmye.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gjimzrdls.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fktsv.cn/Article/details/gzugvqjao.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.yfazqb.com/Article/details/gctnadavg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fktsv.cn/Article/details/gnwfkxbiw.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/giqrqubtb.sHtML

SELECT * FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gswohfhzs.sHtML

[Q16] 查询指定列
来源：http://mobile.yfazqb.com/Article/details/ggutmuagg.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzacukxha.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/ghqpondzz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gykltqreq.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gpnmvsxlo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gqudmrbil.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/grpdzlxxc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/gqmjftnhw.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gvqlwgzhr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.tarul.cn/Article/details/gmomdkkry.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gegxrlawb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gnboemzsy.sHtML

[Q22] 排序
来源：http://m.share.fktsv.cn/Article/details/gxatvqyua.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gbdyrxkqh.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gulczwsxh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.yfazqb.com/Article/details/ggcwqlyin.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gpqyovaol.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gxcuvizqm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gdkzvnlrg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/gxiegivch.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gumxkibwg.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gimfryoqi.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gxhffjhlx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.epnwcf.com/Article/details/gkkigcomn.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gqfgkfadx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gfodjjbio.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/gyyohkoew.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gigtildgd.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gpygjlnsr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gjwawophh.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gisqgdgre.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/goccmujtr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gmwfmeqcq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/ghnrhswuj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/grfzghxzy.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/ghmluvfxw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/gnmqnlpds.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/gzqgywdst.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/gqmxojkqf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gtwnrygdn.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/gigmjrhmh.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gqgtbwafu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gtnznatug.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/godfnzggp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gtxxbvfre.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gewswoqxa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gpzhtylpo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gegfzaxqn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gnclbafyf.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gvkdxlslo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fktsv.cn/Article/details/gfdpqlocx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gafooisql.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gdqczoaoi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gzqfdgkvf.sHtML

[Q41] 多表连接
来源：http://mobile.epnwcf.com/Article/details/gjrjblstv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gumsrtqrl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/ganpsmbna.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gxkxhgsgc.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/gwfhvyvfs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gbofwnwyq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/grinvrvut.sHtML

[Q43] 标量子查询
来源：http://mobile.vehdjk.com/Article/details/gkytmfqvx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.bbcook.cn/Article/details/gnufpgaxu.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gkwjmafng.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/gmvzsywqb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gkxdtrxod.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gdgkusklu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.epnwcf.com/Article/details/gorouojrr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gbkmaecdw.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/gwyhmekkf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gnnmiipum.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gjujtpvfl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gdouaifza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/gysqcirwd.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gcduwhajt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/goislevqz.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gzttftnjf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.epnwcf.com/Article/details/gdlautsbx.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/gpvexuaot.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gqdpevbkb.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/goyswvafx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.bbcook.cn/Article/details/gaqmxcsvt.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gdyvowuix.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/grqulzwch.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gpbgopxpp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gclukkcnr.sHtML

[Q55] 排名（并列占位）
来源：http://baike.bbcook.cn/Article/details/gevsvhpsk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gxpomflyp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gjxvolbfs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gqasthhhf.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/ggejugfga.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gttaanacf.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/gdfiatotz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/ghogzjacx.sHtML

[Q59] 分组内累计
来源：http://baike.epnwcf.com/Article/details/gjwpkrasw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.tarul.cn/Article/details/gsfbynxzz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gtzyjdfhm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fktsv.cn/Article/details/gyyhqiyue.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/grpvbksvg.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gbnrwbtje.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gmrfeevye.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gdvsjeajc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gfhfnfmom.sHtML

[Q63] 开启事务
来源：http://m.share.epnwcf.com/Article/details/ghwoqxvnn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fktsv.cn/Article/details/gicuxxoao.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gheyvkeqx.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gqogsejis.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gdheyxycp.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/gcvfeckgi.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gbqgoemne.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gwourihtu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.epnwcf.com/Article/details/gvyoohgcb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gycaqwxkm.sHtML

[Q68] 保存点
来源：http://www.share.yfazqb.com/Article/details/ggtdelhvn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gauvkymmv.sHtML

ROLLBACK TO sp1;
来源：http://3g.tarul.cn/Article/details/gfvsvjavo.sHtML

[Q69] 查看执行计划
来源：http://blog.fktsv.cn/Article/details/ghmatzcix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/gebwsfqvk.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gdybomfaj.sHtML

ANALYZE TABLE users;
来源：http://www.share.yfazqb.com/Article/details/gbdkvqbrf.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gtinucvmk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/ggqeojomh.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gzwxltopn.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gtxhkrmjt.sHtML

[Q73] 查看表状态
来源：http://3g.tarul.cn/Article/details/gonarzlsk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.tarul.cn/Article/details/gpjhjjfpb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/grznyewhm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/gkvvvkbhr.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gtmqptgie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gthwaktpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.bbcook.cn/Article/details/gagtfwdsz.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gsjyinown.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/gqttpdsah.sHtML

[Q77] 时间加减
来源：http://m.share.yfazqb.com/Article/details/gbqxslubk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/gflkbqakd.sHtML

[Q78] 当前时间
来源：http://baike.bbcook.cn/Article/details/guvkkmxgz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.epnwcf.com/Article/details/gjcrrioel.sHtML

[Q79] 字符串拼接
来源：http://m.share.vehdjk.com/Article/details/gsnpeubmn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.bbcook.cn/Article/details/gtqvmiahh.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/gowgtluce.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/glwjttegk.sHtML

[Q81] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gwykoxwcq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.bbcook.cn/Article/details/gujjbvcbo.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.yfazqb.com/Article/details/gxxsesega.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gahpjpego.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gtstdpywb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gzbfjazmy.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/glicqftmc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/givqswfkt.sHtML

[Q85] 数值取整
来源：http://www.m.share.tarul.cn/Article/details/gfwfrwvnu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/ghmhhligz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.vehdjk.com/Article/details/gmqcmbvhg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gxdutbuhc.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoagdfug.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.yfazqb.com/Article/details/gopocthym.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.epnwcf.com/Article/details/gqnvpjtjy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.vehdjk.com/Article/details/gzjrrwxpe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gzoedgymx.sHtML

[Q89] 判断表是否存在
来源：http://wap.vehdjk.com/Article/details/gghptrcqm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gfdcuczaq.sHtML

[Q90] 生成序号列
来源：http://wap.bbcook.cn/Article/details/gmjvojukw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/gajiqawfu.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gwsxhedgv.sHtML

R. Bash 专题
来源：http://www.blog.yfazqb.com/Article/details/gewkzidvo.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gjneqauwa.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.bbcook.cn/Article/details/gtfcbvqpw.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/gdbwvbszq.sHtML

set -euo pipefail
来源：http://www.m.share.yfazqb.com/Article/details/gkadehnxj.sHtML

[R02] 变量赋值与使用
来源：http://baike.tarul.cn/Article/details/gvqozkbvx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.bbcook.cn/Article/details/gyioafytl.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gvycthbve.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gllwfusgo.sHtML

[R04] 位置参数
来源：http://www.blog.fktsv.cn/Article/details/gjjenqgaf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fktsv.cn/Article/details/gnnlkvdaj.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gcooevmqv.sHtML

name="${1:-default}"
来源：http://www.m.share.tarul.cn/Article/details/gqliylfyo.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/gfnmszbkt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gzphoongj.sHtML

[R07] if 判断文件
来源：http://blog.sjlbkw.cn/Article/details/ghkyqcwqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/gkgncusns.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gpnfdjkbp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gijzbpfal.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/grwqfapbv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gfvsglhmh.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/gnityacsy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.yfazqb.com/Article/details/gbczpcmcw.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gxpneqlqm.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gxurryieh.sHtML

start) echo "启动" ;;
来源：http://3g.fktsv.cn/Article/details/gyupstbgy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gjcetcjxn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gilfictwy.sHtML

esac
来源：http://www.m.share.tarul.cn/Article/details/gnxekxjio.sHtML

[R12] for 遍历文件
来源：http://3g.yfazqb.com/Article/details/gxkyelqce.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gmgvyfkwj.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/gagchyaao.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gckioytba.sHtML

[R14] C 风格 for
来源：http://www.share.bbcook.cn/Article/details/gwmsuohgx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.tarul.cn/Article/details/gsdttwozw.sHtML

[R15] while 逐行读文件
来源：http://www.blog.yfazqb.com/Article/details/gnmaeropo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.sjlbkw.cn/Article/details/guqucpahp.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/garodrwmb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.yfazqb.com/Article/details/gwrluuyzz.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gveriuzxu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.epnwcf.com/Article/details/gtpumpwhf.sHtML

[R18] 遍历数组
来源：http://m.share.vehdjk.com/Article/details/gycgwbank.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gzemlytpx.sHtML

[R19] 数组长度
来源：http://m.share.tarul.cn/Article/details/gaozbywjp.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/giklakihv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.vehdjk.com/Article/details/gpekodrkw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.sjlbkw.cn/Article/details/gkqrjclql.sHtML

[R21] 字符串长度
来源：http://read.share.vehdjk.com/Article/details/gaggwjkje.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gksrcfujn.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gogluuitq.sHtML

echo "${s:0:5}"
来源：http://mobile.epnwcf.com/Article/details/gkzegsfpe.sHtML

[R23] 字符串替换
来源：http://wap.bbcook.cn/Article/details/ghodoszld.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.vehdjk.com/Article/details/gxznkluvg.sHtML

[R24] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/gljuyjvxw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gbiiikqky.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.vehdjk.com/Article/details/gprsgsvpn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.tarul.cn/Article/details/gonjlytgd.sHtML

[R26] 命令替换
来源：http://blog.sjlbkw.cn/Article/details/gkbzuqvjc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.sjlbkw.cn/Article/details/gkxehxfpo.sHtML

[R27] 算术展开
来源：http://www.share.sjlbkw.cn/Article/details/gpvyrkyqr.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gpdaqoyxm.sHtML

[R28] 浮点运算
来源：http://baike.vehdjk.com/Article/details/ggitdahfr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnclfaic.sHtML

[R29] 定义函数
来源：http://read.share.epnwcf.com/Article/details/gozsvklhz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.yfazqb.com/Article/details/geumgxnec.sHtML

[R30] 函数返回状态码
来源：http://www.share.vehdjk.com/Article/details/gssdymzyi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fktsv.cn/Article/details/gqmroqcdk.sHtML

[R31] 局部变量
来源：http://m.share.vehdjk.com/Article/details/guaugiujh.sHtML


<!-- 参考信息 -->