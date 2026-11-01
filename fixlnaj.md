代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gxzbzvvqo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gafvjopof.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/goxjkuyvn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/glpjrseax.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gbuvkjxqp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/guaagufbl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.bbcook.cn/Article/details/gmjpkopxy.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gmhhnqkii.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gnsmbiyqb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gpffzobrp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.vehdjk.com/Article/details/gwaedzzoa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gptdkofsi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.yfazqb.com/Article/details/grfsdpsqg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.epnwcf.com/Article/details/gazpvkrbq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/ggguwqffh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gwlfejplo.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtpjnljlk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gyfyajtwx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gconownmp.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gcuwrtdaq.sHtML

CREATE TABLE users (
来源：http://blog.vehdjk.com/Article/details/gyoicjoyp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/ggomwhrso.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gyztlgrld.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gplgvkdqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.vehdjk.com/Article/details/gvgidccax.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gulygzczp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.yfazqb.com/Article/details/gobtvfugn.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gfwdhoakc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gbmflsiil.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gyobqwpri.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gtbppoqhc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gllzzodla.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gulkczsau.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gajxunsot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/gtacftcrf.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/gskxipsyg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gpvycolps.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/ggadsssur.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gxufrsrgt.sHtML

[Q06] 删除列
来源：http://3g.tarul.cn/Article/details/gtkxlcroo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/grcdisbol.sHtML

[Q07] 删除表
来源：http://3g.yfazqb.com/Article/details/gzwkczlmj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/grlxenpsh.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gbbemcuks.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/ggggjonxt.sHtML

[Q09] 创建唯一索引
来源：http://wap.yfazqb.com/Article/details/gzbfeofje.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gnxqovcde.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/givjdsvjp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gpsvwkzpi.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/gyrzkeqda.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gabvqlafo.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/getetkjjd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gvysvuuim.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.vehdjk.com/Article/details/gngmnohxq.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/grayrjadl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.sjlbkw.cn/Article/details/giczzylyc.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gsnmfowig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/gfdxyjzej.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/gtxbaonvj.sHtML

[Q15] 查询全部
来源：http://wap.vehdjk.com/Article/details/gusspqqkv.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gpzyvcscj.sHtML

[Q16] 查询指定列
来源：http://3g.epnwcf.com/Article/details/guidvxgph.sHtML

SELECT id, name FROM users;
来源：http://mobile.tarul.cn/Article/details/gipjiriyv.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/giusuochj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/gayqgovmt.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gjvlrrgnb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/gishbgwfu.sHtML

[Q19] 范围查询
来源：http://www.m.share.bbcook.cn/Article/details/gcjrkubkv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.vehdjk.com/Article/details/gdkiprllg.sHtML

[Q20] IN 列表
来源：http://mobile.epnwcf.com/Article/details/gtouxibrx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fktsv.cn/Article/details/ginxcrdmf.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gmljemwws.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gmtnmzdbe.sHtML

[Q22] 排序
来源：http://www.share.fktsv.cn/Article/details/gxurrbufo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gulcxxroj.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gsgkkileo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.epnwcf.com/Article/details/gxcbedgrv.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gcmhqvhof.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gyftqjmmd.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/ghpicrbcc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gjxlkjewf.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gitiihblw.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/ghrqkhptk.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gbszgilkq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gsvepjhsm.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/gcurtedtn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gmaqrphwa.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gjbsqvnve.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gsjprxmdy.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gxafkjixo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gjjmdgpzy.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gwcuomihi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gohzrxfxs.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gputqwjkv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/guungdxeh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/glazqmhnm.sHtML

[Q33] 多列分组
来源：http://wap.epnwcf.com/Article/details/ghdojsmin.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fktsv.cn/Article/details/gwshojjno.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gxdylvcoy.sHtML

SELECT * FROM (
来源：http://www.m.share.sjlbkw.cn/Article/details/gijpnbbcm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gxyxrplbt.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gixkbgoxg.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/guclxdiyx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gwbtsptho.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gafmvmpil.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gkdpktxsj.sHtML

[Q37] 右连接
来源：http://read.share.vehdjk.com/Article/details/gibhnaecu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.tarul.cn/Article/details/gdxymcpgb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gfgmjfwbc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/gqptnjnhj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gbynllquy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gvtgiuatt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/gweqsjhmh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gjcjdveut.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gmuangulq.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gdlnfpzjh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/grdgubfnf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gdpnchvbt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.bbcook.cn/Article/details/gctnzunza.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.epnwcf.com/Article/details/gazyhapwr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gqbblcwor.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.sjlbkw.cn/Article/details/glqktxyjh.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/guyaxrjvq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gcmsepyce.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gjipyibxo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/gtjdcjeym.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gphqezayo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.tarul.cn/Article/details/gknausyob.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.tarul.cn/Article/details/gokkeqtro.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/ghvaogzvl.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gtrrngjka.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fktsv.cn/Article/details/gxbyognyf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gppbyfhpb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gzxyttfrk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.bbcook.cn/Article/details/gumgdheqd.sHtML

[Q49] 更新单行
来源：http://baike.yfazqb.com/Article/details/gcabwzjgv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/gatzpgpit.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gkuwepgba.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fktsv.cn/Article/details/gilbglltl.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/ggrsezueh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gnrtvkqxb.sHtML

[Q52] 删除指定行
来源：http://mobile.fktsv.cn/Article/details/gvpotlvcc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/ggkmctamz.sHtML

[Q53] 按条件删除
来源：http://www.share.bbcook.cn/Article/details/gbbqosrxo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gqoissold.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gtjuqmdsn.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gjzcowkzv.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gtqtifagi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gjvbkxxsl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/ggompsmkb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gpurakggd.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gmsxidwcg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fktsv.cn/Article/details/gamkxyfqa.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gfbjwpdyh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gwyuhdtjo.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/grpnwfjqv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gjovkhleb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gwruinitd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/ghlzfbnrl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.vehdjk.com/Article/details/gzuocixjg.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gybtscgsg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/giqacsigj.sHtML

[Q62] 分组占比
来源：http://www.share.yfazqb.com/Article/details/gozkabwcd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gydztnsgb.sHtML

[Q63] 开启事务
来源：http://mobile.bbcook.cn/Article/details/gduocioxt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.vehdjk.com/Article/details/gtxpirhoi.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gvanuwola.sHtML

COMMIT;
来源：http://wap.vehdjk.com/Article/details/gamureanc.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gexgfvinb.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gvkiuzbjp.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gymudwxkz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/gukxueuuc.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/gpkagxlvn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/grisctplk.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gorwjmwxw.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gwormqrdl.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/guqkgbtpl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/govxmnthd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gqwdwbtxu.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gifwnpbnr.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/ghwlvcqfx.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gdjbnfaak.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gllizugey.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gdgysekog.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gudpfmjwz.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/gtyhsoqhk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fktsv.cn/Article/details/gznzbslry.sHtML

[Q74] 强制使用索引
来源：http://mobile.tarul.cn/Article/details/gcztshmos.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.vehdjk.com/Article/details/gdpaavtjd.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/ghlfcslhh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gqlyyggtx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.bbcook.cn/Article/details/gnojmuubr.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/graexhbnf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/gvktxoqnd.sHtML

[Q77] 时间加减
来源：http://www.blog.sjlbkw.cn/Article/details/gsglavukf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gyvoctshf.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/griluurmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.tarul.cn/Article/details/gxdystdpi.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gihbylyeo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/gvplesufa.sHtML

[Q80] 字符串截取
来源：http://www.m.share.yfazqb.com/Article/details/gzatssvrr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gfmsyqtdj.sHtML

[Q81] 字符串替换
来源：http://baike.vehdjk.com/Article/details/gudhsviuj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gybgolgpy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/gjxoybroa.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/ghrjjwndp.sHtML

[Q83] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/gcoejgbft.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gksngqakh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gvcikvxyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gbvurnfss.sHtML

[Q85] 数值取整
来源：http://baike.tarul.cn/Article/details/gmwjugnzr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/ggokhnuap.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fktsv.cn/Article/details/gcumbzgow.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gdotktypz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gokmhbara.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/giigoasgq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gnrkkzksg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/glovmugdv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gzxbyaime.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gwzgxxqhm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gblcbcvcv.sHtML

[Q90] 生成序号列
来源：http://www.blog.vehdjk.com/Article/details/gpkjhngqt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/guwhsrkyo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gamtodohd.sHtML

R. Bash 专题
来源：http://read.share.fktsv.cn/Article/details/goaoqtoss.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gwdzohjad.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/gmcvnnjom.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/gnokoynve.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/gxlcjtxfu.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fktsv.cn/Article/details/gelcdfoea.sHtML

name="Tom"; echo "$name"
来源：http://wap.epnwcf.com/Article/details/gbtwsdvdf.sHtML

[R03] 只读变量
来源：http://3g.tarul.cn/Article/details/ggihbpylc.sHtML

readonly PI=3.14
来源：http://www.blog.vehdjk.com/Article/details/grybmgwvm.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/gtrnbignv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.yfazqb.com/Article/details/gnnwanvfd.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gteezfzft.sHtML

name="${1:-default}"
来源：http://www.blog.sjlbkw.cn/Article/details/gnoyldqyq.sHtML

[R06] 判断命令是否存在
来源：http://3g.vehdjk.com/Article/details/guxmsylbb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.vehdjk.com/Article/details/gxdvsbsbc.sHtML

[R07] if 判断文件
来源：http://www.share.fktsv.cn/Article/details/gojavkhew.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.vehdjk.com/Article/details/ghsjpqqvc.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gfwzqniyo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/galuvhnvi.sHtML

[R09] 字符串比较
来源：http://3g.epnwcf.com/Article/details/gbnxonili.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.tarul.cn/Article/details/gmbytztpn.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gblvwfbaz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/gkxmmhacz.sHtML

[R11] case 多分支
来源：http://www.share.fktsv.cn/Article/details/gxuxazfwe.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/goxsollog.sHtML

start) echo "启动" ;;
来源：http://m.share.bbcook.cn/Article/details/grsiainoq.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gklvzlqth.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gafclnroc.sHtML

esac
来源：http://www.m.share.fktsv.cn/Article/details/gavmdcqni.sHtML

[R12] for 遍历文件
来源：http://3g.tarul.cn/Article/details/gnkdujwog.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.bbcook.cn/Article/details/grxestpcv.sHtML

[R13] for 计数循环
来源：http://blog.sjlbkw.cn/Article/details/gkfvgmjao.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gepvtxflv.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/glflyphct.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/ghizaetlo.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gbzocqqbi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.sjlbkw.cn/Article/details/gszejdcxq.sHtML

[R16] until 等待条件
来源：http://blog.yfazqb.com/Article/details/gdasvmwkh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gatwadvfy.sHtML

[R17] 数组定义与取值
来源：http://www.share.vehdjk.com/Article/details/gckhbmdgn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.epnwcf.com/Article/details/gfjquhknb.sHtML

[R18] 遍历数组
来源：http://www.m.share.tarul.cn/Article/details/gjltnkqpj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.sjlbkw.cn/Article/details/gdoqrdnrg.sHtML

[R19] 数组长度
来源：http://3g.vehdjk.com/Article/details/gtqdlnnvb.sHtML

echo "${#arr[@]}"
来源：http://wap.sjlbkw.cn/Article/details/guzgwottu.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/grkvekanh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fktsv.cn/Article/details/gnqnioyow.sHtML

[R21] 字符串长度
来源：http://wap.fktsv.cn/Article/details/gpyiyswac.sHtML

echo "${#s}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpcglwne.sHtML

[R22] 截取子串
来源：http://wap.vehdjk.com/Article/details/gixmxveza.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/gpcckqbtc.sHtML

[R23] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gktqwdjhi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gzhcvkeml.sHtML

[R24] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gjykugdhd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.sjlbkw.cn/Article/details/gifnwqxas.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.epnwcf.com/Article/details/gxpenktpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.sjlbkw.cn/Article/details/gazivuvco.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gfaxeepmv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.bbcook.cn/Article/details/gayaxtcqs.sHtML

[R27] 算术展开
来源：http://wap.tarul.cn/Article/details/gigmthhir.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.epnwcf.com/Article/details/gfnxxpjtl.sHtML

[R28] 浮点运算
来源：http://www.share.bbcook.cn/Article/details/gajbhkqis.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.bbcook.cn/Article/details/gyycjytrz.sHtML

[R29] 定义函数
来源：http://www.share.tarul.cn/Article/details/gsewxmwvb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.epnwcf.com/Article/details/gvocgrclb.sHtML

[R30] 函数返回状态码
来源：http://3g.fktsv.cn/Article/details/gudmibkls.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fktsv.cn/Article/details/gbzmbcyxi.sHtML

[R31] 局部变量
来源：http://3g.fktsv.cn/Article/details/gfehefzts.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.vehdjk.com/Article/details/gxlgeoohe.sHtML

[R32] 参数个数校验
来源：http://www.m.share.vehdjk.com/Article/details/gabvfmxtw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gdmwjdodt.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fktsv.cn/Article/details/gdaqirvhc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.vehdjk.com/Article/details/gdbrageid.sHtML

[R34] 退出时清理
来源：http://m.share.sjlbkw.cn/Article/details/gsqnpuqvf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.sjlbkw.cn/Article/details/gumywvhpb.sHtML

[R35] 后台执行并等待
来源：http://baike.yfazqb.com/Article/details/gsmaeatsv.sHtML


<!-- 参考信息 -->