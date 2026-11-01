代发 wailian999

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gnvugjnzd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gsljslhqw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gfbpzymav.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.epnwcf.com/Article/details/gmzlfqqex.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.sjlbkw.cn/Article/details/gfnldknox.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.bbcook.cn/Article/details/ghjdalibs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gkjmnvrsc.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/grcxvnbsk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gimfwaqoy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/grbexhpvp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/gpxfbvilc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gouyrulql.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gvgqipspa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/gblojanef.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/gfaycmuty.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gnazqvlra.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gqrpstznj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gjxfbvlyz.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gprovznwc.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdajscle.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/ggtpfrtwh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gbrdurvit.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/giwzcxagm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.bbcook.cn/Article/details/ghkycpzbx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.sjlbkw.cn/Article/details/ggpgsisxg.sHtML

);
来源：http://wap.tarul.cn/Article/details/gtpqqrqco.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gmyxrseyc.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gqufrvrme.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/grfdxdjpr.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/glwbijihv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gxyfshsto.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fktsv.cn/Article/details/gpvliowqz.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/ghivosjuk.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gqwoyppgu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gdjfhdoup.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/garezxqdu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/gqxyxzomt.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/ghzlxqqij.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gimibvezz.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/glvzpykim.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.sjlbkw.cn/Article/details/gltpaummp.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/glhnjvqit.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gpzyyytvm.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gtvumgkda.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gelmxntlg.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gbhwxwtym.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gyjpfgjtg.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gvmacwter.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gprbnopay.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/ggnuvskqn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.tarul.cn/Article/details/gbeavutyd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.yfazqb.com/Article/details/gxteqdbje.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/ghydsqtan.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/goybcncmc.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gezzwmsna.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gbtiynocz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/geilbqyte.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/grphnwesc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gnwzxiquf.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gswrcivzd.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfipeqeuv.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gjhlfbole.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gmyjreuec.sHtML

[Q17] 条件查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gypfghtyg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/glztpdtym.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gxuxjuurf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/gbpgdxrez.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/gbpednahk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gfspjhtjr.sHtML

[Q20] IN 列表
来源：http://baike.vehdjk.com/Article/details/gauiaxgxt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gjnvxqyjv.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gzuwwvbav.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/gqgnefvzr.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/gpuznunvn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gkdcvllwq.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/gptrdtmlk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gzmgygjbu.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gmxlkvifn.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.bbcook.cn/Article/details/gaaauntwj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/gpbmmepla.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.bbcook.cn/Article/details/glauwfgri.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gvrqeegsd.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggfvpdfft.sHtML

[Q27] 条件计数
来源：http://blog.bbcook.cn/Article/details/gamjjpvhk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gvknwsfxu.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/gbofrwppv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/goltekiyk.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/guhsitvop.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gvsightij.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/glcneihzo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gumjbxyrl.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/grpojalxc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gavhyihop.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gxzgbykrv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gaassjqxl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gfzhedadu.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/gerifmvtk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.epnwcf.com/Article/details/gxkjdyrsf.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gylbbazqw.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/gltqpypuv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.bbcook.cn/Article/details/gflunadqp.sHtML

) t WHERE rn = 1;
来源：http://wap.vehdjk.com/Article/details/gpobmtush.sHtML

[Q35] 内连接
来源：http://www.share.tarul.cn/Article/details/gdaipzftx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.bbcook.cn/Article/details/ghrrlnvkn.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/gjxfqagyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gjtogrjqa.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gwaxioiri.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gmfueghjb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/ghnkywjmk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gjrmcktzu.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gjkzyinfw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.yfazqb.com/Article/details/gbzcjebxa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/grefugtrw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gucmgakfv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.tarul.cn/Article/details/gnemtefue.sHtML

[Q41] 多表连接
来源：http://3g.fktsv.cn/Article/details/gcybdqvng.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gmircciih.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gtkncqdwh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/guvwjpfrb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gpnqvhvnn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gnrkxyuxg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gfdxaywrv.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gyhzzfeqi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gbzaipafg.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/gcyzondlo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gsvzkbqzo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gyllpynsw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gqjvpnfli.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.vehdjk.com/Article/details/glpywdrgl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gtcgljfzt.sHtML

[Q47] 与平均值比较
来源：http://www.share.fktsv.cn/Article/details/gkjxszisc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gofzdbusf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gqcckqane.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.sjlbkw.cn/Article/details/gjbffzjlc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.yfazqb.com/Article/details/ghfqiduxx.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gtfvkisep.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/glmtmqofa.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gnyhynryj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/guqoyctep.sHtML

[Q51] 用子查询更新
来源：http://www.blog.tarul.cn/Article/details/gcssbzosn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gambywoaw.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gfpkxacdr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gsmqtwdil.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gzusqcmuh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fktsv.cn/Article/details/gaswypiir.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gfmfhfgey.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.epnwcf.com/Article/details/gwezgxnry.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.yfazqb.com/Article/details/gydaqpjwf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/gmuqobocq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fktsv.cn/Article/details/gnrsrytcc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gngpzmvod.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gautughwe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.epnwcf.com/Article/details/gebjcszlw.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gcqkxtkxd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ggaywflgw.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/ggooaxxyb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gdrmcdrmr.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gpxevriyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gwdwbhlbf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gwrsygfdj.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gvgakcdbp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gckknmwhu.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gvoupxhjs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gxbtnmjcw.sHtML

[Q63] 开启事务
来源：http://baike.bbcook.cn/Article/details/guwfztate.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.epnwcf.com/Article/details/ggjqwnntt.sHtML

[Q64] 提交事务
来源：http://blog.sjlbkw.cn/Article/details/gupxntabj.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gdqmzgwlw.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gssfvzadm.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gijkrcvqu.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gnefznojg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gtshvavok.sHtML

[Q67] 设置隔离级别
来源：http://mobile.epnwcf.com/Article/details/gtjmmyobs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.tarul.cn/Article/details/gfgsifxmm.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gsyvdtiem.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gtdnxenky.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gitkdqsno.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/ggjozcjgu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gwgrpdkxs.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/gilzgbito.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gghkvnijd.sHtML

[Q71] 查看建表语句
来源：http://m.share.fktsv.cn/Article/details/gnzibexmi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.vehdjk.com/Article/details/gilgbkyyl.sHtML

[Q72] 查看索引
来源：http://m.share.sjlbkw.cn/Article/details/genkfrwrv.sHtML

SHOW INDEX FROM users;
来源：http://baike.yfazqb.com/Article/details/gdlxhacrf.sHtML

[Q73] 查看表状态
来源：http://www.share.bbcook.cn/Article/details/giekyavck.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gfpofjaxd.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/gjmjbnfhs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.tarul.cn/Article/details/gybifimcs.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gorzhpwhq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gpswgiwks.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gucnbqjse.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/goomqrtoe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.yfazqb.com/Article/details/gwzupccce.sHtML

[Q77] 时间加减
来源：http://mobile.fktsv.cn/Article/details/gsivoieds.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gwsigvyit.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gmdgjkcnu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gxpdxuedb.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gfliiytjd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/givanfkzd.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gzbfzwccd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/ggfvnrctr.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gbwwpmlcy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.epnwcf.com/Article/details/guihtmvdz.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gvehbanxn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gfjrarvvc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gzhtubmdc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gectvfsys.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.vehdjk.com/Article/details/gwcjefkkt.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gjwxqkabb.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/gyymfzfgf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.vehdjk.com/Article/details/gcgznbstz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.yfazqb.com/Article/details/gqfppkkrw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.sjlbkw.cn/Article/details/gtmeokbho.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gbmozzlwm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.epnwcf.com/Article/details/gdwumwlre.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/gjurhhpft.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gtjtnfexl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/grwszujwd.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/ghxyvjxzw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.bbcook.cn/Article/details/gmzdocuyl.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gtnouhbjl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gmwfzkdyb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbohffomf.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gaqiaqegg.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/giusgkjcv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.sjlbkw.cn/Article/details/grrcvgegx.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/grhdfxluc.sHtML

set -euo pipefail
来源：http://read.share.fktsv.cn/Article/details/gfvwpxpze.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gewyfridx.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gjzfrxfis.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/giwjvyzbh.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gfjtgoewv.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gozxcbbbq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.bbcook.cn/Article/details/gffckppon.sHtML

[R05] 参数默认值
来源：http://www.blog.fktsv.cn/Article/details/gxswxbmvl.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gvuqqneab.sHtML

[R06] 判断命令是否存在
来源：http://blog.bbcook.cn/Article/details/gxcnvhfvo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.sjlbkw.cn/Article/details/gkjexvuvz.sHtML

[R07] if 判断文件
来源：http://read.share.vehdjk.com/Article/details/ggcjqpiau.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gzgxgzdrw.sHtML

[R08] 数值比较
来源：http://wap.bbcook.cn/Article/details/ghqikwngk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.tarul.cn/Article/details/gntppofft.sHtML

[R09] 字符串比较
来源：http://www.share.bbcook.cn/Article/details/gcfqreben.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gibmbsfwk.sHtML

[R10] 正则匹配
来源：http://mobile.sjlbkw.cn/Article/details/grysgxkdb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.bbcook.cn/Article/details/gjmxngssw.sHtML

[R11] case 多分支
来源：http://wap.epnwcf.com/Article/details/gypozhxic.sHtML

case "$1" in
来源：http://3g.vehdjk.com/Article/details/gzkjzimui.sHtML

start) echo "启动" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvhikqmbx.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gduaezqdd.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/glgpxwaxh.sHtML

esac
来源：http://wap.yfazqb.com/Article/details/gosabrsoe.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gvgpocfpk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.bbcook.cn/Article/details/gqqsvcone.sHtML

[R13] for 计数循环
来源：http://baike.yfazqb.com/Article/details/gwbazpael.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gcuvwzonv.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/ggvcvrckk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/genkfzwhk.sHtML

[R15] while 逐行读文件
来源：http://wap.vehdjk.com/Article/details/goucwweec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.bbcook.cn/Article/details/guiwpwlwo.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gfehmfkzt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.vehdjk.com/Article/details/gbkgrddtg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfckodsi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fktsv.cn/Article/details/golzfdlny.sHtML

[R18] 遍历数组
来源：http://www.m.share.vehdjk.com/Article/details/gsvbuaauf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gvcuamxyp.sHtML

[R19] 数组长度
来源：http://www.blog.tarul.cn/Article/details/gtsbaifnk.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gpvxjcnqn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fktsv.cn/Article/details/gljsodllv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fktsv.cn/Article/details/gpacyllug.sHtML

[R21] 字符串长度
来源：http://mobile.yfazqb.com/Article/details/gmzymkvap.sHtML

echo "${#s}"
来源：http://baike.sjlbkw.cn/Article/details/gwtonpazn.sHtML

[R22] 截取子串
来源：http://www.blog.vehdjk.com/Article/details/gjihqripv.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gtotquxzn.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gebuiizti.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/gpvitcqxg.sHtML

[R24] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gceoryxbs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/godjofcmu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.yfazqb.com/Article/details/glehlgshw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.yfazqb.com/Article/details/gawmfquqw.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gzxxkmjgx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.bbcook.cn/Article/details/gnwmecjpg.sHtML

[R27] 算术展开
来源：http://www.blog.yfazqb.com/Article/details/grqqteofx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.vehdjk.com/Article/details/gihaesbwo.sHtML

[R28] 浮点运算
来源：http://m.share.vehdjk.com/Article/details/gfcgsvqvm.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.epnwcf.com/Article/details/gstdajtic.sHtML

[R29] 定义函数
来源：http://3g.fktsv.cn/Article/details/gptlshawm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.yfazqb.com/Article/details/gmdwqkdzo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fktsv.cn/Article/details/govwfbkjg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.tarul.cn/Article/details/grtflzfyv.sHtML

[R31] 局部变量
来源：http://www.share.vehdjk.com/Article/details/gqhstubev.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.tarul.cn/Article/details/ghnhwqazo.sHtML

[R32] 参数个数校验
来源：http://www.m.share.yfazqb.com/Article/details/gdmdlrfvz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gwyollgmb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.yfazqb.com/Article/details/gwzkpzesm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.vehdjk.com/Article/details/gcuonqhpd.sHtML

[R34] 退出时清理
来源：http://www.blog.sjlbkw.cn/Article/details/gqvawcltt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fktsv.cn/Article/details/gkxjbmrqd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.epnwcf.com/Article/details/gsnpefgve.sHtML


<!-- 参考信息 -->