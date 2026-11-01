代发 wailian999

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/gpdkvzmud.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gzkcexnxg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmzovucp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.bbcook.cn/Article/details/gougqrbfk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gsifzrryd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/guiegchqc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gshkrvwna.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.vehdjk.com/Article/details/gutadxajp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gtbegmtyd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gaacwlowp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/ggpnmygis.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/gfqfzncyy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/guyraormn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gmnrksxyk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gbvbquisx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.epnwcf.com/Article/details/gggibzhlu.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gqtdnaouo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gdlsamwvf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghbsquktv.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gfbvnmgow.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gduzhlxcl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/geigdvfch.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/ghlpnzkat.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/goqpnljyu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/gqcdcvkka.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gjnpqznya.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/galmvegec.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/glvtlpyrs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/guhwnfmkc.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/giefmmlgm.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/geblqcqio.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gdqgmkrns.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gbvmshxna.sHtML

[Q03] 增加列
来源：http://read.share.yfazqb.com/Article/details/gbcjumsbg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gueemiyaf.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gfgwrfpoh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gozzgihvd.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/ggaqigktk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gbkscnlfp.sHtML

[Q06] 删除列
来源：http://mobile.yfazqb.com/Article/details/ghklgnqyy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.yfazqb.com/Article/details/glqysfxlb.sHtML

[Q07] 删除表
来源：http://m.share.fktsv.cn/Article/details/ghtefkxvx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/gvifxonbr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/gphyevvxg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/grqzjtrac.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/gbdyjzqhb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fktsv.cn/Article/details/gasalrftp.sHtML

[Q10] 插入单行
来源：http://blog.sjlbkw.cn/Article/details/gvrrqzmgz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gihwqbzri.sHtML

[Q11] 一次插入多行
来源：http://www.share.sjlbkw.cn/Article/details/gifqtstsn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gmsraxopk.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fktsv.cn/Article/details/gnhezkgpd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gnfzloeqq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gzxtpopxa.sHtML

[Q13] 忽略重复插入
来源：http://m.share.bbcook.cn/Article/details/gqycjphml.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gzuxvzstm.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gctrretnc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/gmmsuuibj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.vehdjk.com/Article/details/govymcypy.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gzhwsgzqh.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gwomvokpp.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/goabssylc.sHtML

SELECT id, name FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gennwhwfe.sHtML

[Q17] 条件查询
来源：http://mobile.bbcook.cn/Article/details/gsakldxqt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.yfazqb.com/Article/details/grihloekv.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/gmnzoagyx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gwrhmsphl.sHtML

[Q19] 范围查询
来源：http://www.blog.epnwcf.com/Article/details/gspxfpbbk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/gvrgwfmrh.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gzruhecza.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gbacykjfu.sHtML

[Q21] 空值判断
来源：http://wap.vehdjk.com/Article/details/gxeijygdr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gyouynnoj.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/grkcqsxvu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/gnqekbmyt.sHtML

[Q23] 分页
来源：http://www.blog.tarul.cn/Article/details/ggxmeiggm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gqbpqwpur.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gqzldklqg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gckgdeayf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/gftjnuuue.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.vehdjk.com/Article/details/goxurkeiq.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gwkgsjvob.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gkkxfrtjc.sHtML

[Q27] 条件计数
来源：http://www.blog.bbcook.cn/Article/details/gixiuzovo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gybrzznrv.sHtML

[Q28] 求和与平均
来源：http://wap.yfazqb.com/Article/details/gnjtxueai.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gsgliqldz.sHtML

[Q29] 最大最小值
来源：http://m.share.epnwcf.com/Article/details/gwbrwgxrm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbwruwboa.sHtML

[Q30] 分组统计
来源：http://www.share.yfazqb.com/Article/details/glrnxcqek.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/greqyseqq.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/gbuiimdve.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.bbcook.cn/Article/details/gbqcockdh.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/gwmyhngki.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/ghuaxyjag.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/guegcxzqu.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gssvtvrgs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.yfazqb.com/Article/details/gipciyebv.sHtML

[Q34] 每组取第一条
来源：http://m.share.yfazqb.com/Article/details/glltdbgzu.sHtML

SELECT * FROM (
来源：http://www.share.epnwcf.com/Article/details/gwgcviprm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gijqvcypg.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/geyhyhyfq.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gdpfcoaub.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/glmqlwprx.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gucgofvve.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gmijfrsor.sHtML

[Q37] 右连接
来源：http://www.blog.sjlbkw.cn/Article/details/gqqqrkebd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/gmtnegblg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.bbcook.cn/Article/details/gectlbdju.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gkaqxanmh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gegsgwmco.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gglabuvzm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gixaueard.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.bbcook.cn/Article/details/grktownnu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gjroljknx.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/gzrctqxco.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/gkwyhhqyu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gdyomitdp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.sjlbkw.cn/Article/details/gpxmuxala.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gzqinsbrf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.tarul.cn/Article/details/gogddnfsy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fktsv.cn/Article/details/gullznyjl.sHtML

[Q43] 标量子查询
来源：http://www.m.share.tarul.cn/Article/details/galaiunul.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.epnwcf.com/Article/details/gvdqjajyg.sHtML

[Q44] IN 子查询
来源：http://baike.yfazqb.com/Article/details/gezbhkfkj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gmtvqgehh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gghswoezv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gqbcrkhcl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.sjlbkw.cn/Article/details/glkunobuq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gswbhikpv.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gvsqtqolg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gvxxnanaa.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gfaseznyz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/gusbprdfw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.sjlbkw.cn/Article/details/gxvfuermg.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gjbdbomaw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/giuetugpq.sHtML

[Q50] 批量更新
来源：http://www.m.share.vehdjk.com/Article/details/gqiktjbgh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gjwidqjgw.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gdsfdbyln.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/gtrjyhxau.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/gkeraznza.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gvsyhmnhl.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gxjbnyvxc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/ggatkhodu.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/ggxfgntxr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gsqcfxyyi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gobxjqbxc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.bbcook.cn/Article/details/gukkzgrcp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gfqrbaqcy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/grjntkbih.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/grvlwgdob.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gnygloqpi.sHtML

[Q58] 累计求和
来源：http://read.share.sjlbkw.cn/Article/details/glfweqdfs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzktqbeci.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gbhaavpac.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gaiicnnao.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fktsv.cn/Article/details/gvvsqmqpu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/ghnxivkxl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gfjroznmq.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gsvytkcej.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gowlohdxx.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gotiqacul.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcunbiezh.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gcwxodqtw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gdwiyfdnv.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/girujatfg.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/gxctboxza.sHtML

[Q65] 回滚事务
来源：http://read.share.epnwcf.com/Article/details/gakgqyuvc.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gsqmaxpnm.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gyhgvsxzy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gkvnozeiy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/golubxfko.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/geeveszju.sHtML

[Q68] 保存点
来源：http://read.share.vehdjk.com/Article/details/gcbjkpvpc.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gnpfktgnk.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gnvnlhpbq.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/glgwthdrz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.yfazqb.com/Article/details/gzdxlayhf.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.tarul.cn/Article/details/gakbruubq.sHtML

ANALYZE TABLE users;
来源：http://baike.tarul.cn/Article/details/gjggytwkl.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gjhpvcfof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.yfazqb.com/Article/details/gzeecdxwx.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gqrjpdehk.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gusjusoku.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gkorlvize.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gthtgdpot.sHtML

[Q74] 强制使用索引
来源：http://www.share.tarul.cn/Article/details/gnrnhwdph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/grgrrzjbx.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gjicfpkkf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gfdsskykp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fktsv.cn/Article/details/ggswqizyp.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gaeqspuco.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/geuiguoep.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gemqmyyhx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.sjlbkw.cn/Article/details/gpkikmhgv.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gqxtfhhuj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gqhxhwdov.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gripxiybo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gyyfqwdnw.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gxhrlzalj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/gbsseictg.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gexzqgbyq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gndlrfept.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gxtarzjlq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gygqqettn.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gbiyykcse.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gbldmxujd.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/giobgwmsr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/getpkoewt.sHtML

[Q85] 数值取整
来源：http://read.share.bbcook.cn/Article/details/gkpjlgsoe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gkhspzgtg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.bbcook.cn/Article/details/gskbvcrvf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.bbcook.cn/Article/details/gsxdfxkgw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.bbcook.cn/Article/details/gcfowkupd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.vehdjk.com/Article/details/gtbzbbyet.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fktsv.cn/Article/details/gfkuxsars.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gvbdcddcr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gimqhvoqi.sHtML

[Q89] 判断表是否存在
来源：http://baike.bbcook.cn/Article/details/glrziwqsw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.tarul.cn/Article/details/gknjzotsl.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gzxegjtdg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gfzrlzqjg.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmvoarckb.sHtML

R. Bash 专题
来源：http://wap.fktsv.cn/Article/details/guhzkchia.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grmkcvygf.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gatftkfzs.sHtML

#!/usr/bin/env bash
来源：http://baike.vehdjk.com/Article/details/gdnwrrjnx.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gmkikcrwv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gbpqeklht.sHtML

name="Tom"; echo "$name"
来源：http://mobile.bbcook.cn/Article/details/gpihbowwb.sHtML

[R03] 只读变量
来源：http://3g.epnwcf.com/Article/details/gauwpwxje.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/glqzqiviw.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gklujfatz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/gfcglavfg.sHtML

[R05] 参数默认值
来源：http://mobile.sjlbkw.cn/Article/details/gifczvjlf.sHtML

name="${1:-default}"
来源：http://www.share.fktsv.cn/Article/details/gddevgtdy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gqewcxklb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gmuepejoa.sHtML

[R07] if 判断文件
来源：http://mobile.sjlbkw.cn/Article/details/grliknngu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gmkrclnai.sHtML

[R08] 数值比较
来源：http://www.m.share.bbcook.cn/Article/details/gjfopbgpj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gfmagaqez.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gtmaurxme.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.tarul.cn/Article/details/ggkzoyusv.sHtML

[R10] 正则匹配
来源：http://3g.epnwcf.com/Article/details/gpiquvfue.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gksyqoawz.sHtML

[R11] case 多分支
来源：http://3g.tarul.cn/Article/details/guexcenvt.sHtML

case "$1" in
来源：http://www.blog.yfazqb.com/Article/details/gvxyalhff.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gakmvozuz.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.epnwcf.com/Article/details/gnhtjfkcr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/georzjpjo.sHtML

esac
来源：http://www.blog.vehdjk.com/Article/details/giqrdvhpz.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/ggsztvwxo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fktsv.cn/Article/details/gykvldhsz.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gahkchpoz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gyplrckoz.sHtML

[R14] C 风格 for
来源：http://baike.bbcook.cn/Article/details/gwzoxskdd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gidikfazm.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fktsv.cn/Article/details/gspxrduxb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/gweynbwpf.sHtML

[R16] until 等待条件
来源：http://www.m.share.tarul.cn/Article/details/gjgmwwezo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fktsv.cn/Article/details/ggsniieob.sHtML

[R17] 数组定义与取值
来源：http://m.share.sjlbkw.cn/Article/details/gdvnehyhv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.yfazqb.com/Article/details/gositvdeh.sHtML

[R18] 遍历数组
来源：http://read.share.epnwcf.com/Article/details/gesrzerot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.vehdjk.com/Article/details/gsahrphnz.sHtML

[R19] 数组长度
来源：http://mobile.fktsv.cn/Article/details/glnunkuai.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gchwiossq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gnbirgdow.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.yfazqb.com/Article/details/gpuzuuerf.sHtML

[R21] 字符串长度
来源：http://3g.yfazqb.com/Article/details/getnbzkqj.sHtML

echo "${#s}"
来源：http://mobile.bbcook.cn/Article/details/gladwietq.sHtML

[R22] 截取子串
来源：http://www.share.epnwcf.com/Article/details/gjepdvaaq.sHtML

echo "${s:0:5}"
来源：http://read.share.vehdjk.com/Article/details/gznieovsk.sHtML

[R23] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/ghsurdvzo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fktsv.cn/Article/details/gsxrqjeoj.sHtML

[R24] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gkfvldqrd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gkwufkpip.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.bbcook.cn/Article/details/grlgbbdzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fktsv.cn/Article/details/gkojlytpo.sHtML

[R26] 命令替换
来源：http://www.m.share.tarul.cn/Article/details/gyugudkxq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.vehdjk.com/Article/details/gkxdqnuch.sHtML

[R27] 算术展开
来源：http://read.share.sjlbkw.cn/Article/details/gvinptyrr.sHtML

echo $((1 + 2 * 3))
来源：http://baike.yfazqb.com/Article/details/gpfqrpuvb.sHtML

[R28] 浮点运算
来源：http://3g.yfazqb.com/Article/details/gwyflwwtq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.tarul.cn/Article/details/gfgpdbhmt.sHtML

[R29] 定义函数
来源：http://wap.epnwcf.com/Article/details/gxgdyrvod.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.epnwcf.com/Article/details/glvvsldhl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gjmrcjchi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.bbcook.cn/Article/details/gmbrjdjut.sHtML

[R31] 局部变量
来源：http://m.share.sjlbkw.cn/Article/details/gqvoymiwg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqxmihg.sHtML

[R32] 参数个数校验
来源：http://blog.vehdjk.com/Article/details/grcrmthtd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gnysdrbte.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.tarul.cn/Article/details/gjpdsgtaq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.epnwcf.com/Article/details/gpcetirom.sHtML

[R34] 退出时清理
来源：http://3g.yfazqb.com/Article/details/gtpnmgjzc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.vehdjk.com/Article/details/gsovuowxo.sHtML

[R35] 后台执行并等待
来源：http://wap.tarul.cn/Article/details/gkfkdpgqh.sHtML


<!-- 参考信息 -->