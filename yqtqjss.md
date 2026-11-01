代发 wailian999

PHP:  // 手写时间戳比较
来源：http://m.share.tarul.cn/Article/details/gviezboal.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/ghcfqhini.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/ghtsywrrj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/giwetopmf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.tarul.cn/Article/details/gkpdvlbbv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/ggkknrtlk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gmqxanock.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gmesyijbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gixnexdfb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gaojjigdp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/gzzhgkhjm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gestbprir.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/glwvptafb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.tarul.cn/Article/details/gmzojaswz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gurqkiunu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/gkanbkmng.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjubnyahw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/gtqzkonsu.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqpemhkdm.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gpqvgkxgx.sHtML

CREATE TABLE users (
来源：http://wap.bbcook.cn/Article/details/ghieiaroj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gxotmybyx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.vehdjk.com/Article/details/gkkgxnihk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.epnwcf.com/Article/details/gfljidpkd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gfbdaqgof.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gonataxky.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.vehdjk.com/Article/details/gbqyyagif.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gyhluvdcq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gfeakmqti.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gqotkhxvo.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gkhhxebpv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.bbcook.cn/Article/details/gwmymhdcf.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gsjwocvvw.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gjrbjvgca.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gpmmnbvyf.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/gpcfeajjw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gzmmazsfg.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gzgxevbtp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/gdwqsbmey.sHtML

[Q06] 删除列
来源：http://read.share.tarul.cn/Article/details/gjmhuyirr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/gdfvhjyna.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/gbnazvbdm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.vehdjk.com/Article/details/guvpfamrs.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/giyjwfgtp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gyhdvnhjw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfovgubw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gjrtwiipf.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gkvhodchd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gxdlvzgjg.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/ghbccygyi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gynyfpdrp.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gokmwvlpk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gzpbishpi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/giwgqqsig.sHtML

[Q13] 忽略重复插入
来源：http://mobile.yfazqb.com/Article/details/gnquutyhv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fktsv.cn/Article/details/gltjuewkk.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gjaosccym.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gootdrqse.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/ggllldlxe.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gwuyhxaxu.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gfenszsfw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gyglivrpw.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/gbdwhfgsy.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gcvoseays.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gdllhqukt.sHtML

[Q18] 模糊匹配
来源：http://baike.fktsv.cn/Article/details/ggfdqwhlf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.bbcook.cn/Article/details/gnpkiuugg.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gbagnwudr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gpuikankr.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gsmszoeis.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gsptrqwjy.sHtML

[Q21] 空值判断
来源：http://baike.bbcook.cn/Article/details/gokcgqeqn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gqeebhcpy.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gajcgdgko.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.tarul.cn/Article/details/geddsrxlg.sHtML

[Q23] 分页
来源：http://www.m.share.yfazqb.com/Article/details/gtlyvmgen.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gbgepctjt.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/ghqkkfmig.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/grxpgvbkw.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gcvhopesh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/ggsiddrjz.sHtML

[Q26] 计数
来源：http://wap.sjlbkw.cn/Article/details/gavoaphko.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gphzzazjj.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/gzjriitiw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/gqicqdnbo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzboslkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.tarul.cn/Article/details/gkzbzdrii.sHtML

[Q29] 最大最小值
来源：http://www.share.yfazqb.com/Article/details/gwqulffeg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gghorqbjn.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gnkzcpaqb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gogkhuksr.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gvdkwzszj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gasmdvmyi.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gypdisyee.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gkoerymrg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.tarul.cn/Article/details/gdyodkcdk.sHtML

[Q33] 多列分组
来源：http://mobile.vehdjk.com/Article/details/gyetgvpny.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gtxjkhvqi.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gjskizyks.sHtML

SELECT * FROM (
来源：http://3g.vehdjk.com/Article/details/glymwabah.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.vehdjk.com/Article/details/gtvdumted.sHtML

) t WHERE rn = 1;
来源：http://m.share.sjlbkw.cn/Article/details/gafyhoqde.sHtML

[Q35] 内连接
来源：http://m.share.sjlbkw.cn/Article/details/gqhskavba.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gozizbess.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gcbfmztor.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gkmkklqsb.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gubhvzvcj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/gayfcrevd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gbzqqsorb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gghamqagy.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/golkfzkps.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gnpnbjrpn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fktsv.cn/Article/details/ggubdisjz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gghvfscul.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gxiluhxmr.sHtML

[Q41] 多表连接
来源：http://mobile.tarul.cn/Article/details/gleoitakg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.vehdjk.com/Article/details/gdnvqknxd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.sjlbkw.cn/Article/details/gwdrghvkn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.epnwcf.com/Article/details/gpmfuzwmr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gqqfphkur.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/gmofjuvif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gkcuvdmcp.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/gzadjsefm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gzhdywjhi.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gptxhzytq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gwbnovaid.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.yfazqb.com/Article/details/gdlhshysk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.sjlbkw.cn/Article/details/gplvaappk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/gfxbaqggl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gzxzmcdht.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gnihnjfbh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.bbcook.cn/Article/details/gdhpzjbld.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gjobtfjmo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/grvyeorqb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gkwnvfssy.sHtML

[Q49] 更新单行
来源：http://blog.fktsv.cn/Article/details/gkjvobcxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gtuduhvls.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/gorajfkvp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gnycbipbm.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/gjiozyftv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gfysfcgzg.sHtML

[Q52] 删除指定行
来源：http://read.share.sjlbkw.cn/Article/details/gsopmwufj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/ghkzyiece.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gddegechu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/gnfuptdnf.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gzsmudreq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gmtyuuslp.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gyjktdnfh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.vehdjk.com/Article/details/gswltfxpf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gsktnqowr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gtlixklfp.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gnkpxcgdr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.tarul.cn/Article/details/gxjmiymju.sHtML

[Q58] 累计求和
来源：http://3g.bbcook.cn/Article/details/ggrkvkmji.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/ghnxqctdi.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/gyyxyatuy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gtdkbdkgr.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/gejwiaqpe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.bbcook.cn/Article/details/gpxasdtnq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fktsv.cn/Article/details/gdhsvdqzx.sHtML

[Q61] 移动平均
来源：http://m.share.yfazqb.com/Article/details/gogjweqfj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.tarul.cn/Article/details/grdoqysli.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gbvypiznz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gexmokred.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gorremotc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/gnozmyjzx.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gwybvfufc.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/ggfxggpqx.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/goplwonap.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gbsxzrage.sHtML

[Q66] 行锁查询
来源：http://3g.tarul.cn/Article/details/gvigekrky.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gaxoaleiz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gjundfjwa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.sjlbkw.cn/Article/details/govyogqlg.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gxvpjhfrc.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gcnwvihqv.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gwkklyyws.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fktsv.cn/Article/details/gxwztqrho.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.vehdjk.com/Article/details/gyksaabkx.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/gftuuekvh.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/guljhsxwf.sHtML

[Q71] 查看建表语句
来源：http://blog.yfazqb.com/Article/details/gbfgalohb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.sjlbkw.cn/Article/details/gzgmxixtl.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gmvtntirm.sHtML

SHOW INDEX FROM users;
来源：http://3g.yfazqb.com/Article/details/gjzkmwahh.sHtML

[Q73] 查看表状态
来源：http://baike.tarul.cn/Article/details/gwuawiigt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/guskrnoqk.sHtML

[Q74] 强制使用索引
来源：http://baike.sjlbkw.cn/Article/details/gzyrpixhf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gkvwmkncj.sHtML

[Q75] 日期格式化
来源：http://wap.yfazqb.com/Article/details/ggylbzlak.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gudeobjvv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.epnwcf.com/Article/details/gmvncmbbd.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/ggnbsavtx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.sjlbkw.cn/Article/details/gqshinylo.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gsqsxuihj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.vehdjk.com/Article/details/ggxtaimxu.sHtML

[Q78] 当前时间
来源：http://www.blog.epnwcf.com/Article/details/gxvlyorie.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gddbuccno.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gimzjarpw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gxxjaaxvl.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gsfdldkiu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gcfitarvf.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gfmgmgawy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gcdjdcszi.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.bbcook.cn/Article/details/gufxgdbjb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gpjzcftjd.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/guyhigxqy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gepkppdny.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gwqpwxavw.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gpjmxoyau.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gppepbdxz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gsvejuflh.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gkwpyqbcv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/grdfarpid.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.yfazqb.com/Article/details/grfnjshgr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.yfazqb.com/Article/details/gfuliizzx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gyydyzksi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.epnwcf.com/Article/details/gwzdosnor.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.bbcook.cn/Article/details/gysdlmkky.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/ggmbahgeo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.vehdjk.com/Article/details/ghzhidqzz.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gndgikwnn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/ggtzkybdw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gefdfhtym.sHtML

R. Bash 专题
来源：http://3g.bbcook.cn/Article/details/gjreacdeo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/glfhylqxd.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gpwcqurjk.sHtML

#!/usr/bin/env bash
来源：http://baike.fktsv.cn/Article/details/gylpcizhq.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/gnptrgglm.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/grervnyoa.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/grevsvgyw.sHtML

[R03] 只读变量
来源：http://www.m.share.tarul.cn/Article/details/ghpteadzg.sHtML

readonly PI=3.14
来源：http://baike.bbcook.cn/Article/details/gdyxoksza.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gjyamxxbd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gboosekok.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/glqbwtgyt.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gdhegbxva.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gfzxhgnhl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gpvxjtduv.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gquprafsw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.bbcook.cn/Article/details/gfwdjeagt.sHtML

[R08] 数值比较
来源：http://wap.yfazqb.com/Article/details/gfasdsjdg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.tarul.cn/Article/details/gqpyofnzj.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gywjktmjo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.bbcook.cn/Article/details/gcetbpbch.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gqdujnagg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/ghxattioo.sHtML

[R11] case 多分支
来源：http://wap.yfazqb.com/Article/details/gufypcqmk.sHtML

case "$1" in
来源：http://wap.epnwcf.com/Article/details/gnkhfcwlu.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gmqffirer.sHtML

stop)  echo "停止" ;;
来源：http://blog.yfazqb.com/Article/details/gvudhinob.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.yfazqb.com/Article/details/gbisitqhd.sHtML

esac
来源：http://mobile.bbcook.cn/Article/details/gvsmzfwal.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gnosfdshj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gotgrgiwl.sHtML

[R13] for 计数循环
来源：http://wap.bbcook.cn/Article/details/gnfmvcbfl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gnpxhrjge.sHtML

[R14] C 风格 for
来源：http://wap.vehdjk.com/Article/details/gxtgyirjz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gvtrodmsh.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fktsv.cn/Article/details/guvolmwat.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.yfazqb.com/Article/details/gtzzmtnvw.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gakuhhqyp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.vehdjk.com/Article/details/ghmghgenr.sHtML

[R17] 数组定义与取值
来源：http://www.blog.bbcook.cn/Article/details/gqvlwyvaf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.bbcook.cn/Article/details/gnjododxx.sHtML

[R18] 遍历数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gexbmogxa.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.sjlbkw.cn/Article/details/gaqcjmzdw.sHtML

[R19] 数组长度
来源：http://blog.bbcook.cn/Article/details/glixacqpx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.epnwcf.com/Article/details/ghhkzzwdj.sHtML

[R20] 关联数组（字典）
来源：http://wap.fktsv.cn/Article/details/gjwppepqf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.yfazqb.com/Article/details/gfhhcgeng.sHtML

[R21] 字符串长度
来源：http://www.share.bbcook.cn/Article/details/gfdvwpytp.sHtML

echo "${#s}"
来源：http://baike.epnwcf.com/Article/details/gghurxply.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/gzsilvrpp.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gtxmgahpl.sHtML

[R23] 字符串替换
来源：http://www.blog.yfazqb.com/Article/details/gvcpufcpg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.bbcook.cn/Article/details/gifmyxwbw.sHtML

[R24] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gqheuzpff.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fktsv.cn/Article/details/gpfswecot.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.tarul.cn/Article/details/gwtkeyeeq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.vehdjk.com/Article/details/ggkwhsdgr.sHtML

[R26] 命令替换
来源：http://www.m.share.yfazqb.com/Article/details/gwjxgraau.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.vehdjk.com/Article/details/guhqedgzg.sHtML

[R27] 算术展开
来源：http://baike.epnwcf.com/Article/details/griylunzj.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fktsv.cn/Article/details/grkiobwne.sHtML

[R28] 浮点运算
来源：http://www.blog.epnwcf.com/Article/details/gdzqbgnle.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.epnwcf.com/Article/details/gtxeeehqo.sHtML

[R29] 定义函数
来源：http://m.share.bbcook.cn/Article/details/gpfxibqmd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.vehdjk.com/Article/details/gjuwhhwfj.sHtML

[R30] 函数返回状态码
来源：http://3g.epnwcf.com/Article/details/gxktsmrvu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.tarul.cn/Article/details/ggwhploon.sHtML

[R31] 局部变量
来源：http://3g.bbcook.cn/Article/details/gwhprmabc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.epnwcf.com/Article/details/gadegnhvd.sHtML

[R32] 参数个数校验
来源：http://baike.fktsv.cn/Article/details/gfrdkwgoj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/gsuoznjaz.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwqkcpem.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.vehdjk.com/Article/details/ghfjoxhtu.sHtML

[R34] 退出时清理
来源：http://blog.tarul.cn/Article/details/gwhdyvzft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gnflvtusf.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.tarul.cn/Article/details/gdzgilrny.sHtML


<!-- 参考信息 -->