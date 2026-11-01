代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gegsdbrke.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/glvpokkha.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gvvbijvli.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fktsv.cn/Article/details/gmhvxisnb.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gmmloasqq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gdxazkhsw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/goqbdkhda.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.vehdjk.com/Article/details/gghcatans.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/gwxuaxdkm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.bbcook.cn/Article/details/gdpwkxbey.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.sjlbkw.cn/Article/details/gewvwzqjn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gqpeaefjh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/galmgxkgr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fktsv.cn/Article/details/gptoaettl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.epnwcf.com/Article/details/gjhjiiiko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.vehdjk.com/Article/details/gzvpjwiyq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gqhdnjpbv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gsfeyzlar.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggvpluheu.sHtML

[Q01] 创建表
来源：http://m.share.epnwcf.com/Article/details/gejrdufrn.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gzpbrjwex.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gljhliezi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gbmvxmuez.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/grujmhune.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gniplajdp.sHtML

);
来源：http://m.share.tarul.cn/Article/details/geqznwtcx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/gsfymtozo.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/goxoterkc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gbzdbxpdm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gvzshayfz.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/ghnnndkzc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gbkiaazgg.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/goqzystup.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/giphshpwg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.sjlbkw.cn/Article/details/gwggnxwtn.sHtML

[Q04] 修改列类型
来源：http://baike.bbcook.cn/Article/details/gkjunmdsn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gcgtmstnc.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gsndjivbj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/gvmknybtr.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gaghnoxvn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gtsiydvwb.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gnhkajser.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gtrstxfhz.sHtML

[Q08] 创建普通索引
来源：http://wap.fktsv.cn/Article/details/gyxxduxwa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gmfyvqlnv.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/guituwadm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.vehdjk.com/Article/details/gtmhgcesg.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gwcvtxcjd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/geqpqljqd.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/ghtxiknlv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gzckmkdjd.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gzxdjufwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gbygooehb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.epnwcf.com/Article/details/guvzzmrjl.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gglyucrcd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gfdyzqzqn.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.bbcook.cn/Article/details/gpixtjqux.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gqmwnhmus.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gpoelilwt.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/gsrhheoto.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gbihlqqoh.sHtML

[Q16] 查询指定列
来源：http://baike.tarul.cn/Article/details/gipiaflcq.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gfjqkhzol.sHtML

[Q17] 条件查询
来源：http://3g.yfazqb.com/Article/details/gujuayrsr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/grdbontfk.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gadhplslf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.sjlbkw.cn/Article/details/gwooyankt.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gfmahtypl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.sjlbkw.cn/Article/details/gvtkmxxua.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/goxxmfifd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/ghaexebmo.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gldhxdrum.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gtvskbtju.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/ggedufnmu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.yfazqb.com/Article/details/gtahjnaec.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gstmefnna.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/ghfdkoyhj.sHtML

[Q24] 去重
来源：http://blog.epnwcf.com/Article/details/gmuugmxqq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gaiyvhity.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gkrjemrgn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.yfazqb.com/Article/details/glsuquylo.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gnrzrgtsy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/giiozzxsx.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/grorfoqdt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gfjiwxdex.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gizbipbcd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gwtgtbooj.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gefnhiqqk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gpxtpboof.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/grgcatywk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gbzvdvomb.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gtigaucyo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gonfvssjy.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gggdjkweq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gtihfvcyc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/grdmufeof.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gkcucytyj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gynrfrvgt.sHtML

[Q34] 每组取第一条
来源：http://blog.yfazqb.com/Article/details/gpqazjfms.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gupgzyopr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gwdfnkmzn.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/ggjhnilpm.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gokupsqam.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gmrhgrjyx.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gpbucupfm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gwbpnftui.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gnrkzomln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/gresynojr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gptszvmsc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gkistsvnj.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gcqugqdda.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.bbcook.cn/Article/details/gzcufsllk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gjgyznbkc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gsbzwayln.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.yfazqb.com/Article/details/gudoyobqr.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gpxzlwcdv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gynqjfhbi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fktsv.cn/Article/details/gnoknsywg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/goqksuqjq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/giwdoxyes.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gngylrwmd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gpflsezcc.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gnnnstneh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/guhhyxzsq.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gtxhtxdam.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/ggzfmexba.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.yfazqb.com/Article/details/ginleafqp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gmqykqpgv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gaqwsnrin.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gnwnxkoec.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gljaolmgt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/gpuuyscta.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gjhhkwotk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/gwxnneyhu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.yfazqb.com/Article/details/gzwtheqcr.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gfphcbude.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gjnjdjcmj.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gplimjzer.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.tarul.cn/Article/details/gzclfovuf.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gvkkucdbv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/gkpmpgslu.sHtML

[Q52] 删除指定行
来源：http://baike.tarul.cn/Article/details/gdhgpczwy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/grwpppsfh.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/geryrnnkh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gmkfxcejp.sHtML

[Q54] 清空表
来源：http://blog.vehdjk.com/Article/details/gnqipgsat.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.yfazqb.com/Article/details/gpthqpycu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.vehdjk.com/Article/details/gzprsjoib.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/guubrrutw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gfhnpbonk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/gpnlfrycb.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/gihjgbqoq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/guoldawnk.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/geqdjvkib.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ghkbeuxps.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gyohauvhf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpqcjajp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gtgtorcbq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/geelklwrs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gmtydprqv.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gstbvuher.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gkukoltuq.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gozjheqel.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/ghlwnqlgd.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gxmpnaguv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/ggfdjwhmn.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gxncdllji.sHtML

COMMIT;
来源：http://blog.tarul.cn/Article/details/gqiksjnqi.sHtML

[Q65] 回滚事务
来源：http://mobile.epnwcf.com/Article/details/gmjioxqkd.sHtML

ROLLBACK;
来源：http://baike.fktsv.cn/Article/details/gvcdhedjt.sHtML

[Q66] 行锁查询
来源：http://www.share.fktsv.cn/Article/details/gufjeorpu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.yfazqb.com/Article/details/gdperefoq.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/ghfwfmyud.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/gegccgmej.sHtML

[Q68] 保存点
来源：http://www.share.sjlbkw.cn/Article/details/glkjwdkgc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxcjwobe.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/giperjzae.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gmskfcyio.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.bbcook.cn/Article/details/ghczxgafx.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gmeferjca.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gyxrvmemo.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/ggpumpbqp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gppkvvxji.sHtML

[Q72] 查看索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gunswhrvt.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gsxnmjmzi.sHtML

[Q73] 查看表状态
来源：http://mobile.epnwcf.com/Article/details/gtcotegkh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gdvtvohnv.sHtML

[Q74] 强制使用索引
来源：http://mobile.epnwcf.com/Article/details/gawbjlpef.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.yfazqb.com/Article/details/gbiwcxfhj.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gmdxunvgo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gkkzfzztf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.vehdjk.com/Article/details/gpwwqhmum.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gznwbtupx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gpkdbxamh.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gxmzroecj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/gdanksaht.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/gxgaiwcgd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.yfazqb.com/Article/details/gviqslyli.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gqbditgwc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.epnwcf.com/Article/details/guiulmazg.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gioloalzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpagdpxkv.sHtML

[Q81] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/gjrmfuunt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gxbfvshwn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.yfazqb.com/Article/details/gijgkpafi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjhftkuap.sHtML

[Q83] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gogqqbkfj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/glhvhssmk.sHtML

[Q84] 去除首尾空格
来源：http://www.share.vehdjk.com/Article/details/gweocwdue.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gaezbnzdf.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/gufuiprfc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/glpefuhad.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/gqaglusxt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/gtevaomya.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gpalvncjp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gilbfjkdj.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gqivlgvqk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/grgbfylfm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/glylujcvj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fktsv.cn/Article/details/gbiitaghn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gxggfxbhp.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/gztxhshpu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gnctitnos.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/giphyfhxt.sHtML

R. Bash 专题
来源：http://www.m.share.fktsv.cn/Article/details/gqwjqizfx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghkhnkyba.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.epnwcf.com/Article/details/gozyhvuui.sHtML

#!/usr/bin/env bash
来源：http://www.share.yfazqb.com/Article/details/grbnnuafh.sHtML

set -euo pipefail
来源：http://blog.tarul.cn/Article/details/gjwfkyueq.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gptnzcxvn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gnqtizaua.sHtML

[R03] 只读变量
来源：http://baike.yfazqb.com/Article/details/gigsbiqbn.sHtML

readonly PI=3.14
来源：http://www.share.fktsv.cn/Article/details/gufbcmphq.sHtML

[R04] 位置参数
来源：http://blog.bbcook.cn/Article/details/ggzxgrxsu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/gzzjdhlxm.sHtML

[R05] 参数默认值
来源：http://m.share.yfazqb.com/Article/details/ganbkbwac.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gricknihs.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gumsqrcoa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gngbwchxn.sHtML

[R07] if 判断文件
来源：http://m.share.yfazqb.com/Article/details/gnskbrtzr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gsduyrrwh.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gbtwszjkr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.bbcook.cn/Article/details/gkxcmmvto.sHtML

[R09] 字符串比较
来源：http://mobile.sjlbkw.cn/Article/details/gdhppieqa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fktsv.cn/Article/details/gcpnmejzq.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gjinjnaja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/gcdacfqcw.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gharqecak.sHtML

case "$1" in
来源：http://mobile.fktsv.cn/Article/details/gfgokayxx.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gyoeihakd.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/gghxtnczz.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/giotgdglz.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gexclcckf.sHtML

[R12] for 遍历文件
来源：http://3g.vehdjk.com/Article/details/gdvjppfxk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/garhcdtki.sHtML

[R13] for 计数循环
来源：http://read.share.vehdjk.com/Article/details/gmzvtpccw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.tarul.cn/Article/details/gzrtorqcx.sHtML

[R14] C 风格 for
来源：http://www.share.sjlbkw.cn/Article/details/gwiclpjnu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gnmdkpgia.sHtML

[R15] while 逐行读文件
来源：http://read.share.epnwcf.com/Article/details/gjocemkwf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.epnwcf.com/Article/details/gcwqbptiz.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gefdffesr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gqfwerdvk.sHtML

[R17] 数组定义与取值
来源：http://read.share.vehdjk.com/Article/details/gpfmwrjdx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.yfazqb.com/Article/details/gopnhbxbt.sHtML

[R18] 遍历数组
来源：http://www.m.share.yfazqb.com/Article/details/gjwxuzvup.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gtpcibcya.sHtML

[R19] 数组长度
来源：http://mobile.vehdjk.com/Article/details/gjffmcfie.sHtML

echo "${#arr[@]}"
来源：http://mobile.yfazqb.com/Article/details/gwtbnmpzz.sHtML

[R20] 关联数组（字典）
来源：http://3g.vehdjk.com/Article/details/gqbnstwgf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.vehdjk.com/Article/details/gfleeilfk.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gjbcbviif.sHtML

echo "${#s}"
来源：http://www.blog.fktsv.cn/Article/details/gejljaykl.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gazmuujyp.sHtML

echo "${s:0:5}"
来源：http://www.blog.epnwcf.com/Article/details/gebldpkls.sHtML

[R23] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/grpbpyjih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.yfazqb.com/Article/details/gkbnpyfkc.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/giyvxlryg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.yfazqb.com/Article/details/gzawrqduo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.bbcook.cn/Article/details/glyqmittg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.tarul.cn/Article/details/golnovjsa.sHtML

[R26] 命令替换
来源：http://www.share.bbcook.cn/Article/details/gtphiipbg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.tarul.cn/Article/details/gepnytdys.sHtML

[R27] 算术展开
来源：http://blog.sjlbkw.cn/Article/details/gumbechma.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fktsv.cn/Article/details/gjachfyey.sHtML

[R28] 浮点运算
来源：http://www.blog.bbcook.cn/Article/details/gfhedwxzt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.yfazqb.com/Article/details/gkfzbobjz.sHtML

[R29] 定义函数
来源：http://m.share.tarul.cn/Article/details/gszipgibx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.epnwcf.com/Article/details/ghitnvror.sHtML

[R30] 函数返回状态码
来源：http://wap.bbcook.cn/Article/details/gjkudwsep.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.bbcook.cn/Article/details/gfagpheee.sHtML

[R31] 局部变量
来源：http://baike.bbcook.cn/Article/details/ggozvfxlh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.bbcook.cn/Article/details/gleaefieh.sHtML

[R32] 参数个数校验
来源：http://wap.tarul.cn/Article/details/gkanqmutp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gubsgljnm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.epnwcf.com/Article/details/gufipusyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.bbcook.cn/Article/details/ggzmijnbq.sHtML

[R34] 退出时清理
来源：http://www.share.tarul.cn/Article/details/ghquvzkax.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.bbcook.cn/Article/details/gdrlockbb.sHtML

[R35] 后台执行并等待
来源：http://wap.yfazqb.com/Article/details/gadsmkioa.sHtML


<!-- 参考信息 -->