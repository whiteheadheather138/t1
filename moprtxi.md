代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/gjntordev.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/gjuokmvnx.sHtML

[P07] 防抖与节流
来源：http://wap.vehdjk.com/Article/details/gschyifiv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gmozpzsrn.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/ggvuppsck.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gnpcjbavm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gltsbllwo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/gjthawgdz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.epnwcf.com/Article/details/gxlqksdzf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gsmsruqgw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gfwnhyknp.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/gunplxegy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.bbcook.cn/Article/details/gdzlthhvt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gsnzujneu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gqxitriqw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gstrpfwxk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.epnwcf.com/Article/details/gooycywwm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gfhwzrakm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gghgcilyb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gfguuviqs.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ggemfmsdu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.epnwcf.com/Article/details/gfxkphdyi.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmnapaok.sHtML

[Q01] 创建表
来源：http://mobile.bbcook.cn/Article/details/gjfomuqyr.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/gfrqxozeu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gmwruixei.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gbbvjhmdx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.tarul.cn/Article/details/gsedejlkt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gkxgecosm.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gejlagzhl.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/glmjpvjfk.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/glndkfjdt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gydkgipsg.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gxkeogwqo.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gyjsxuail.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.sjlbkw.cn/Article/details/geauwshkj.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/goaizcuzj.sHtML

[Q03] 增加列
来源：http://baike.sjlbkw.cn/Article/details/grzxyafhv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/geeutfvtj.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gezpjzyrs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gawcylrlw.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/gyejddnxv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/ggkacvauz.sHtML

[Q06] 删除列
来源：http://baike.vehdjk.com/Article/details/geskccvgp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gfoilozzc.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gipjifgjl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/gigircenm.sHtML

[Q08] 创建普通索引
来源：http://3g.vehdjk.com/Article/details/gzezknize.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gxllvvhwm.sHtML

[Q09] 创建唯一索引
来源：http://blog.vehdjk.com/Article/details/gpxyhitno.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gclvzbope.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gtntjetco.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/grmajnqyb.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gjhmmbfmx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gfmndjbmm.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gcxuhvyyx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gcqfwkskw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.tarul.cn/Article/details/gauxzyhtv.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gwklcfyij.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gqxmkkzgv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/geicfujsv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.epnwcf.com/Article/details/gikocrbta.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gsfkmsixy.sHtML

[Q15] 查询全部
来源：http://blog.fktsv.cn/Article/details/gtestxbqv.sHtML

SELECT * FROM users;
来源：http://blog.vehdjk.com/Article/details/gtrzmenym.sHtML

[Q16] 查询指定列
来源：http://baike.yfazqb.com/Article/details/glsmfkfpn.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/gemcsyglj.sHtML

[Q17] 条件查询
来源：http://wap.vehdjk.com/Article/details/gvnnkxskn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gxpvjwune.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.sjlbkw.cn/Article/details/gccjwjwdm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gelrtuxqc.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gyecvtsxp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/georipwrf.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/gswityynq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gydjkuzta.sHtML

[Q21] 空值判断
来源：http://www.blog.bbcook.cn/Article/details/glpxjuffk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gpndhdtjw.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gryilqgog.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.tarul.cn/Article/details/gabnjjfey.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gnsddntcn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gpbfiivga.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gedluwten.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gcblsdmei.sHtML

[Q25] 只取前 N 条
来源：http://read.share.bbcook.cn/Article/details/gyguufcbo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.sjlbkw.cn/Article/details/giujvlpvp.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gbfcevezr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gbbhvnbuz.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gvwsagxeq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/grcnukatm.sHtML

[Q28] 求和与平均
来源：http://www.m.share.tarul.cn/Article/details/gwfaxacro.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gjdmumvey.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gvikvcmzk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gqikcksnz.sHtML

[Q30] 分组统计
来源：http://m.share.yfazqb.com/Article/details/gbupniroz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gsfpyhhcm.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/geghucfxt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gptfpmzte.sHtML

[Q32] 分组拼接字符串
来源：http://baike.vehdjk.com/Article/details/gsgdsfqgq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gujvqashl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/gzjxvcgob.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/glykvradb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/glzbrkkkj.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gtknrzuvo.sHtML

SELECT * FROM (
来源：http://wap.yfazqb.com/Article/details/gbjuhndwd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gvrqzunks.sHtML

) t WHERE rn = 1;
来源：http://3g.fktsv.cn/Article/details/gwhpcxayw.sHtML

[Q35] 内连接
来源：http://3g.fktsv.cn/Article/details/grsqybtuj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gkqrnzjoy.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gimqlukto.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gscgdzxgi.sHtML

[Q37] 右连接
来源：http://read.share.tarul.cn/Article/details/gsaquebrw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gswakyira.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gttspiujd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fktsv.cn/Article/details/gatzjezwv.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/gbbiiqlor.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.tarul.cn/Article/details/gqfehutiu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.epnwcf.com/Article/details/gbvpgvhkn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gpbhsuoew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gqylkwprr.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gsvulxavo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fktsv.cn/Article/details/gtwrqyuxg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/ghejkhomj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.vehdjk.com/Article/details/glxclvpze.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/gzfeyphrq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/gquitzebx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gdemxkjhf.sHtML

[Q43] 标量子查询
来源：http://www.share.bbcook.cn/Article/details/gftukcejt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gmmsydscg.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gsqfxzqxm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fktsv.cn/Article/details/gizopkdka.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gjjnkybdz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/grxfqyggm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gjnuddhye.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.sjlbkw.cn/Article/details/gtunbloca.sHtML

[Q47] 与平均值比较
来源：http://read.share.fktsv.cn/Article/details/gyfzcenuw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/grxwsxptv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.vehdjk.com/Article/details/grlqxmzyt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/guhccmxtx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.bbcook.cn/Article/details/giuqpbncq.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gdihzrfga.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gfykfrqhl.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/gzosrapyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gbbefopun.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gprvhyvyr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.tarul.cn/Article/details/ghuiyxpkd.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/ghwrgmhck.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gazdopbnt.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gupnsmyqi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gredzkkwg.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gsvveyjyo.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gnybktbem.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/gppnxivbe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gexchdqsl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gkekcjlca.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.tarul.cn/Article/details/guklempiv.sHtML

[Q57] 行号
来源：http://wap.tarul.cn/Article/details/gegetcyho.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gxbtvtame.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gtyafcuau.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gxgpicwet.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gasydmymd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gwbfxlfdh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gmzuwpbak.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fktsv.cn/Article/details/gijfqhsaw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/guealptnc.sHtML

[Q61] 移动平均
来源：http://baike.sjlbkw.cn/Article/details/ghxxermaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gbzpltsof.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gvibedmmc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gkttwfhqq.sHtML

[Q63] 开启事务
来源：http://m.share.vehdjk.com/Article/details/gzmqouzfc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gwnyfvuos.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gtrtzpzhp.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gzlhiietw.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/gjvqhpgol.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/gkcgovryy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/gmfmrhpta.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.vehdjk.com/Article/details/ggdymlhvd.sHtML

[Q67] 设置隔离级别
来源：http://3g.epnwcf.com/Article/details/getykauqo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gotfddgmr.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gtuxhbhjm.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gnbtjtdza.sHtML

ROLLBACK TO sp1;
来源：http://m.share.yfazqb.com/Article/details/gnbpatzom.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/giinzgfpo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gpmgrrjfw.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gdrziatsl.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gbhfiuuac.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/gribofebf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.epnwcf.com/Article/details/gxywsmkee.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/gfnetxsgv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gxzsqskpp.sHtML

[Q73] 查看表状态
来源：http://3g.bbcook.cn/Article/details/gchpaqudo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fktsv.cn/Article/details/glxxltnfq.sHtML

[Q74] 强制使用索引
来源：http://wap.tarul.cn/Article/details/gvdbhvnra.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gmflgdqeb.sHtML

[Q75] 日期格式化
来源：http://www.blog.vehdjk.com/Article/details/gkrhyutcs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gxcxgdssc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gqrukxvus.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/gresnwall.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/gocuxxtpr.sHtML

[Q77] 时间加减
来源：http://www.m.share.tarul.cn/Article/details/gjxgrtuff.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/gqkwxtwdk.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gdugxvqjf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gmhhkvaky.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gncdgihvc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fktsv.cn/Article/details/gfyhbjgnf.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gufsarqwt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/ggyzkdsra.sHtML

[Q81] 字符串替换
来源：http://www.blog.vehdjk.com/Article/details/gwhsihuxj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.bbcook.cn/Article/details/gweptfwfe.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.bbcook.cn/Article/details/gcmjolvlp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gavztfyum.sHtML

[Q83] 大小写转换
来源：http://m.share.vehdjk.com/Article/details/gzqmsjlwo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/genxwxdxl.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fktsv.cn/Article/details/gourafwry.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gfkfkgqfq.sHtML

[Q85] 数值取整
来源：http://www.share.epnwcf.com/Article/details/gvkosdiyz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gvcxpqlxe.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.sjlbkw.cn/Article/details/goanaquzg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/gxurqkyxy.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gmpvsbzmg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gxsycdgfy.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gbnbleuyg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/grctaypru.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/guokmgjvx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.yfazqb.com/Article/details/gxjyjtjfq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fktsv.cn/Article/details/gargqstwj.sHtML

[Q90] 生成序号列
来源：http://mobile.tarul.cn/Article/details/gvnitkbcw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fktsv.cn/Article/details/ggiouusfr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbeehnrtd.sHtML

R. Bash 专题
来源：http://mobile.fktsv.cn/Article/details/gthfktfet.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ggkgghgnr.sHtML

[R01] shebang 与严格模式
来源：http://baike.fktsv.cn/Article/details/gsteofeiv.sHtML

#!/usr/bin/env bash
来源：http://mobile.yfazqb.com/Article/details/gycokvchi.sHtML

set -euo pipefail
来源：http://www.m.share.bbcook.cn/Article/details/grsbgomlg.sHtML

[R02] 变量赋值与使用
来源：http://mobile.tarul.cn/Article/details/giztwanpg.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gxstysxwc.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/ghurhezxs.sHtML

readonly PI=3.14
来源：http://m.share.tarul.cn/Article/details/gqnpteaxu.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gdxznkeei.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gdjqykgpl.sHtML

[R05] 参数默认值
来源：http://blog.bbcook.cn/Article/details/gevgdcmhp.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gjvtcdbfx.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fktsv.cn/Article/details/gqjlhjlkg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gmtpysueq.sHtML

[R07] if 判断文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxoazgnp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gtoliyjyp.sHtML

[R08] 数值比较
来源：http://m.share.vehdjk.com/Article/details/gwuxwblrw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.yfazqb.com/Article/details/gvpssjsez.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gmlolkleq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/gtfqjoqzo.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gezqwfqud.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.vehdjk.com/Article/details/gfqxkegly.sHtML

[R11] case 多分支
来源：http://mobile.tarul.cn/Article/details/gmugmzjlj.sHtML

case "$1" in
来源：http://www.blog.vehdjk.com/Article/details/gmglkehsa.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gzeqvhlpm.sHtML

stop)  echo "停止" ;;
来源：http://m.share.yfazqb.com/Article/details/ghiiwokdt.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/guuiwegak.sHtML

esac
来源：http://mobile.epnwcf.com/Article/details/gffmnkqji.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gtyyxkbkp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gckqedhhw.sHtML

[R13] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/ggmvxfykd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/gymhgtmwc.sHtML

[R14] C 风格 for
来源：http://m.share.yfazqb.com/Article/details/gndloofqx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/guihbhmgv.sHtML

[R15] while 逐行读文件
来源：http://3g.yfazqb.com/Article/details/gnxuzvofq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gbathudji.sHtML

[R16] until 等待条件
来源：http://www.m.share.epnwcf.com/Article/details/geaklxkru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/ggfbgcloe.sHtML

[R17] 数组定义与取值
来源：http://wap.bbcook.cn/Article/details/ghsiocvbd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.bbcook.cn/Article/details/gyhctpvlm.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/garrgsyzm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.vehdjk.com/Article/details/grhsbnktx.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gwaeludyq.sHtML

echo "${#arr[@]}"
来源：http://mobile.epnwcf.com/Article/details/ggaeevogc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.epnwcf.com/Article/details/gbndrlkng.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.bbcook.cn/Article/details/gxaolxvml.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/goqfyzlkf.sHtML

echo "${#s}"
来源：http://baike.vehdjk.com/Article/details/gdzxjdjrk.sHtML

[R22] 截取子串
来源：http://baike.fktsv.cn/Article/details/gcketdnkz.sHtML

echo "${s:0:5}"
来源：http://www.share.sjlbkw.cn/Article/details/ggdakvufa.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gtabwdbvc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.tarul.cn/Article/details/ghakvmqgl.sHtML

[R24] 大小写转换
来源：http://www.m.share.vehdjk.com/Article/details/gafhlpxus.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fktsv.cn/Article/details/glkiybkqg.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.vehdjk.com/Article/details/gvouhoqmv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/guohjwjvr.sHtML

[R26] 命令替换
来源：http://read.share.vehdjk.com/Article/details/gsqbupdel.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fktsv.cn/Article/details/ggjdzcbpu.sHtML

[R27] 算术展开
来源：http://blog.fktsv.cn/Article/details/ggmmylhxb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.yfazqb.com/Article/details/gxctubxxq.sHtML

[R28] 浮点运算
来源：http://read.share.epnwcf.com/Article/details/gkanocgau.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.tarul.cn/Article/details/gleosahgj.sHtML

[R29] 定义函数
来源：http://read.share.fktsv.cn/Article/details/gkacgvztv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.epnwcf.com/Article/details/goiwwlbvi.sHtML

[R30] 函数返回状态码
来源：http://read.share.yfazqb.com/Article/details/gdubovumg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fktsv.cn/Article/details/gjikogjgg.sHtML

[R31] 局部变量
来源：http://baike.vehdjk.com/Article/details/gbquwkmdv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.tarul.cn/Article/details/guvuovduy.sHtML

[R32] 参数个数校验
来源：http://read.share.yfazqb.com/Article/details/gnbiymhde.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.yfazqb.com/Article/details/gdnjttxbq.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.yfazqb.com/Article/details/gmustnxoe.sHtML


<!-- 参考信息 -->