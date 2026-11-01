代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gjmjlwkqt.sHtML

C#:   if (x is null) {}
来源：http://wap.yfazqb.com/Article/details/gytrfpjdn.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/gskqpecbj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.tarul.cn/Article/details/gmfcoouak.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gvngrhkln.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gmmvaihwc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gcxokhhzh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gcjxccdzl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.bbcook.cn/Article/details/grhtljnyd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.bbcook.cn/Article/details/gwlzqzeem.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/glegrxnwc.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/guyjbmpyh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/gexmepsve.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/gboqnfhbt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.vehdjk.com/Article/details/goydncaty.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/gnerlcvvg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/gvzvdcgtv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gacjulhrh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.epnwcf.com/Article/details/gjsmhwqig.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.sjlbkw.cn/Article/details/gjszjlxuk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gaimjrfke.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.epnwcf.com/Article/details/gnzodcjxq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gawguqykd.sHtML

[Q01] 创建表
来源：http://www.share.bbcook.cn/Article/details/gcjnzzjvz.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gpxbptarw.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gzyrqgrnz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.tarul.cn/Article/details/gtlbmvexq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gysgbzqrp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gwnmrjcvk.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/grqzgjddi.sHtML

[Q02] 创建带外键的表
来源：http://3g.epnwcf.com/Article/details/gnemzcstj.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gkibmqati.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gxidjhaoq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gzggibara.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gwfflmirj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.tarul.cn/Article/details/gsyyjqtwr.sHtML

);
来源：http://3g.yfazqb.com/Article/details/gzbznfajn.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gwzyqpxsq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gajdajqna.sHtML

[Q04] 修改列类型
来源：http://read.share.epnwcf.com/Article/details/gcbafazim.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fktsv.cn/Article/details/ggabwzlcn.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/ggrgukzer.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gfnsahuoo.sHtML

[Q06] 删除列
来源：http://m.share.bbcook.cn/Article/details/griqrpfsy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gfgoqzojd.sHtML

[Q07] 删除表
来源：http://www.share.epnwcf.com/Article/details/ghcesvvra.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/giaodwhhr.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/giwbtbjuf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gvioocgxz.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/gmxansczn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/glkfxsoeu.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/giqdrqhxo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gteboyaax.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gmzaeegjq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gxheynfpi.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fktsv.cn/Article/details/gdkvtqbpd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.tarul.cn/Article/details/grqrgrjoo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.tarul.cn/Article/details/gkavzngtb.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gnxjwiqpv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gjdqiaijk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gohadmrxo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.sjlbkw.cn/Article/details/gbggwclku.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gldmherzs.sHtML

[Q15] 查询全部
来源：http://baike.yfazqb.com/Article/details/guwoyfflo.sHtML

SELECT * FROM users;
来源：http://read.share.yfazqb.com/Article/details/gskgqdehc.sHtML

[Q16] 查询指定列
来源：http://baike.epnwcf.com/Article/details/ghoakuehb.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/giqbckrgb.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/gbivtkxbg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/gdwvtyohb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gztljtlxt.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/gynswblze.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/gleqetwoh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gzeirumpu.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gwqnrcuvx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/gnebruobi.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/ghnmnipxp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/grbcijzkl.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/gketflbmu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fktsv.cn/Article/details/gkuuoscbt.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gmgwqhwdd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gbrovpehx.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gxsvmrunj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/grimzuvtq.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gghtglsym.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gsicavqcr.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/ghgbfvgog.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gddexrcet.sHtML

[Q27] 条件计数
来源：http://www.m.share.fktsv.cn/Article/details/gwagvgstz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvvgfgcts.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gzhlplcal.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gcrbzznlu.sHtML

[Q29] 最大最小值
来源：http://wap.bbcook.cn/Article/details/gfgpepiox.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gmrpsctbl.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/gvzrdvtmd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gfeoeqtps.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/gajqgaevj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/glzxowjpk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.sjlbkw.cn/Article/details/gefrwmovg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gamglhyto.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gyrrlybea.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/golakldov.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/gdznmmvtx.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gfbsckoif.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gemtsyxid.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.sjlbkw.cn/Article/details/gjnkvhzsc.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gstmmdetq.sHtML

[Q35] 内连接
来源：http://www.share.yfazqb.com/Article/details/gzkdfhwpp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/grpbhejrp.sHtML

[Q36] 左连接
来源：http://wap.fktsv.cn/Article/details/gwgfkuqta.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gtqjduhky.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gypcdxato.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.vehdjk.com/Article/details/gqvtdshai.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.epnwcf.com/Article/details/gdhyjibsy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.tarul.cn/Article/details/gamfewqjz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/gozsexbvo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gsluelwgw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gwyhijgdx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gfpbtegqe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gkzgxnkgf.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gqwpnywea.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.vehdjk.com/Article/details/gurliafhs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gqqztuasz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/ggwewsfgs.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/guamiebsj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/geojsbxaa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gwfezpsmo.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gadvtdyke.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/grumyppnh.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gsisqnjro.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gqgltqnsb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gvpymejiu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gfecyroql.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.bbcook.cn/Article/details/gaznsurlr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gtlvydsxb.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/ghcpnkkde.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/gfobjmucx.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/gybuywier.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.vehdjk.com/Article/details/glkuhwwqo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/gylexmhzu.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/gibvsmyei.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gvsppbkdo.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gqqqhvctz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gttjudfbw.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gixbzlilg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.yfazqb.com/Article/details/gtuljdbir.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gzyhhhiwv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gpyxoypku.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gvxhzzzhl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gcwgskyng.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gwyytvutc.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/ggthtpram.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gkujsyepq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.tarul.cn/Article/details/gulbhpsyu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/grhhxivel.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.tarul.cn/Article/details/gwyeqxrvj.sHtML

[Q57] 行号
来源：http://wap.vehdjk.com/Article/details/grutgruwu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gkvtvobio.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gefsfxiyn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gnusjqddo.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gjtyawngu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gattslmbp.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gtfisskkn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.vehdjk.com/Article/details/gtcfjkndu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gvdzymxsz.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gyhafbjey.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gjmanzawg.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/ggrndvibr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gvrfergmi.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gluyxsyiz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.sjlbkw.cn/Article/details/gcdylkfnh.sHtML

[Q64] 提交事务
来源：http://baike.fktsv.cn/Article/details/goyrosfmb.sHtML

COMMIT;
来源：http://wap.fktsv.cn/Article/details/gpetfduiw.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gfwjzcdzb.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/ginmyxykg.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gqbvtrjun.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gdruadsic.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.yfazqb.com/Article/details/gltkqybvd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gtgaowvsj.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gdpcdeujg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.yfazqb.com/Article/details/gdrvcuces.sHtML

ROLLBACK TO sp1;
来源：http://m.share.tarul.cn/Article/details/gjffarlbs.sHtML

[Q69] 查看执行计划
来源：http://www.share.sjlbkw.cn/Article/details/ghpeyaxfq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/gokofpthm.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gqislrddz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fktsv.cn/Article/details/gircxllya.sHtML

[Q71] 查看建表语句
来源：http://baike.yfazqb.com/Article/details/grhcfuxcq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gggxftlvt.sHtML

[Q72] 查看索引
来源：http://www.share.bbcook.cn/Article/details/gvljiznet.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/ggodtyayx.sHtML

[Q73] 查看表状态
来源：http://www.blog.vehdjk.com/Article/details/gfyktokvf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/gnirlbtmb.sHtML

[Q74] 强制使用索引
来源：http://baike.yfazqb.com/Article/details/gicopycah.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/gpmrbeuia.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gsibwlufh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gvtwgswcj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gmhzsemix.sHtML

[Q76] 按天统计
来源：http://blog.tarul.cn/Article/details/gbksntwez.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gljhoxuuz.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/ghjttkyrs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/glopssogz.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gyaidtvbf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gytbehmpl.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gubwxladt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.sjlbkw.cn/Article/details/gguywdjvr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/gpgischtv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.vehdjk.com/Article/details/gquogerlf.sHtML

[Q81] 字符串替换
来源：http://m.share.epnwcf.com/Article/details/gacvcibsl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/gqpeehgvs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.yfazqb.com/Article/details/gteceipwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.tarul.cn/Article/details/gjxtszgus.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gfmhfuimn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.tarul.cn/Article/details/gbbtuwxuj.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/gwmqjairr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gyuuybkvq.sHtML

[Q85] 数值取整
来源：http://m.share.epnwcf.com/Article/details/gnzbqvmqn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.tarul.cn/Article/details/garqvgukb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gdwteiqxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gofxyynfy.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.yfazqb.com/Article/details/gssqkjfxg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.bbcook.cn/Article/details/gxagypkfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gtneyyqkb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.bbcook.cn/Article/details/gpziswsnl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gtkmsbzny.sHtML

[Q89] 判断表是否存在
来源：http://www.share.sjlbkw.cn/Article/details/gqjtvyxnh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gjxamwngv.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/gxuzzfgpl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.epnwcf.com/Article/details/grzirzwmm.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gycgbaols.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gfqckhvnn.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gcuwqcxvv.sHtML

[R01] shebang 与严格模式
来源：http://baike.vehdjk.com/Article/details/gjqtsybwa.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gtdcqrtxh.sHtML

set -euo pipefail
来源：http://3g.bbcook.cn/Article/details/gpgotuvsx.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gjeyshaqu.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gewehzchw.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/guxcnukpz.sHtML

readonly PI=3.14
来源：http://www.share.epnwcf.com/Article/details/gquwyihnk.sHtML

[R04] 位置参数
来源：http://mobile.epnwcf.com/Article/details/gdscelugu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.yfazqb.com/Article/details/gaudufafc.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gvdtlocpy.sHtML

name="${1:-default}"
来源：http://wap.epnwcf.com/Article/details/gpthqasiq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.sjlbkw.cn/Article/details/gztoiqzic.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/guxdfqubw.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gmslvglux.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gjubdstux.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gpxjibjgw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gmfqikvcq.sHtML

[R09] 字符串比较
来源：http://m.share.sjlbkw.cn/Article/details/gadfsieno.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fktsv.cn/Article/details/gqdpcasiu.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/govbbybdx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gfofrvmdu.sHtML

[R11] case 多分支
来源：http://m.share.bbcook.cn/Article/details/gqlfykvuh.sHtML

case "$1" in
来源：http://m.share.bbcook.cn/Article/details/gpekelzpg.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gygtlcfqh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.epnwcf.com/Article/details/ghyaepjsq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.yfazqb.com/Article/details/grzuduuys.sHtML

esac
来源：http://read.share.tarul.cn/Article/details/gsitfgdgp.sHtML

[R12] for 遍历文件
来源：http://mobile.sjlbkw.cn/Article/details/gitpzkgww.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gtrstisrj.sHtML

[R13] for 计数循环
来源：http://3g.sjlbkw.cn/Article/details/gzzarnhfx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.bbcook.cn/Article/details/gfkvryrmv.sHtML

[R14] C 风格 for
来源：http://read.share.sjlbkw.cn/Article/details/gpldrgnjx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fktsv.cn/Article/details/gdkhpppkx.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gszjswyqi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gtibbhnni.sHtML

[R16] until 等待条件
来源：http://www.blog.fktsv.cn/Article/details/gavkitxwk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gasdbbxsn.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gbmweicae.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.epnwcf.com/Article/details/gtjkvvuua.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gxojxdrzy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.yfazqb.com/Article/details/gylsxkyzf.sHtML

[R19] 数组长度
来源：http://baike.tarul.cn/Article/details/goxngyphg.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gzgeshhvu.sHtML

[R20] 关联数组（字典）
来源：http://m.share.tarul.cn/Article/details/gmwxkkjvl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.sjlbkw.cn/Article/details/gobtupikz.sHtML

[R21] 字符串长度
来源：http://baike.vehdjk.com/Article/details/greqtjuek.sHtML

echo "${#s}"
来源：http://www.blog.sjlbkw.cn/Article/details/gszuvzbvm.sHtML

[R22] 截取子串
来源：http://www.blog.sjlbkw.cn/Article/details/gvfcienld.sHtML

echo "${s:0:5}"
来源：http://3g.bbcook.cn/Article/details/gkalkewow.sHtML

[R23] 字符串替换
来源：http://read.share.epnwcf.com/Article/details/gnwgnhksl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fktsv.cn/Article/details/gtsjxnubs.sHtML

[R24] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gerscrign.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.sjlbkw.cn/Article/details/giltjwwwt.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.sjlbkw.cn/Article/details/gfclnubuw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.bbcook.cn/Article/details/gisfjlbqd.sHtML

[R26] 命令替换
来源：http://www.m.share.vehdjk.com/Article/details/gvsreupyi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.epnwcf.com/Article/details/gqdusdguf.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/gzjtioirp.sHtML

echo $((1 + 2 * 3))
来源：http://blog.bbcook.cn/Article/details/gmukhxris.sHtML

[R28] 浮点运算
来源：http://www.m.share.epnwcf.com/Article/details/ghwpcqgml.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.sjlbkw.cn/Article/details/gnzvejtlc.sHtML

[R29] 定义函数
来源：http://m.share.sjlbkw.cn/Article/details/gqcpqwtqc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.yfazqb.com/Article/details/gzijggdyq.sHtML

[R30] 函数返回状态码
来源：http://wap.yfazqb.com/Article/details/gwiapqeks.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.sjlbkw.cn/Article/details/ggfsiamwa.sHtML

[R31] 局部变量
来源：http://read.share.sjlbkw.cn/Article/details/gycgngyon.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.vehdjk.com/Article/details/gsdhrnozk.sHtML

[R32] 参数个数校验
来源：http://3g.fktsv.cn/Article/details/girifuhrt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.sjlbkw.cn/Article/details/gvvbwlaje.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.epnwcf.com/Article/details/gujllwjtm.sHtML


<!-- 参考信息 -->