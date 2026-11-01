代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gjcvgmbco.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gkmiwjmyi.sHtML

[P07] 防抖与节流
来源：http://read.share.tarul.cn/Article/details/gycmeuekr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/ggsvtyvcz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gijlsaayv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gnvlnncze.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.tarul.cn/Article/details/gjwexuuzk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/glqjxzxki.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gskzxdvso.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gwalqatya.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gsdpmolfg.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/gtkqyxhge.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.epnwcf.com/Article/details/gftxedghr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gqeeymlma.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/goolxinug.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gruatjcao.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/gtiqoxnje.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gbhblxqhg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gecjyxdup.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/guntzgnkg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/givuaannk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gmrzmwsnu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gmiqasyto.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gzsymburu.sHtML

CREATE TABLE users (
来源：http://blog.yfazqb.com/Article/details/gaqegsijl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gqvxtfocu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gppqhcwia.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gwyvmwewe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fktsv.cn/Article/details/ghtxjpknz.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gnpkbsjrw.sHtML

[Q02] 创建带外键的表
来源：http://wap.yfazqb.com/Article/details/gwisrcqwx.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gfzvvkwym.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gybptkriy.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gmvmuylgy.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gbfelgtzb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gnnvynljk.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gsnnmcmlk.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gxeasoqau.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpltlappc.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/gdypnfvgf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/gyzxazsga.sHtML

[Q05] 重命名列
来源：http://www.blog.epnwcf.com/Article/details/gpdcknfwt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.sjlbkw.cn/Article/details/gfphennio.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/ghymcvnzp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.yfazqb.com/Article/details/goutdfipo.sHtML

[Q07] 删除表
来源：http://www.share.yfazqb.com/Article/details/gdtcxridr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.sjlbkw.cn/Article/details/gxevicgyv.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gqwgvwefv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gekpbrqsg.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/gisvgzpfw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/geshetwxw.sHtML

[Q10] 插入单行
来源：http://www.share.yfazqb.com/Article/details/gfxpteqge.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/gqzzyrars.sHtML

[Q11] 一次插入多行
来源：http://mobile.fktsv.cn/Article/details/gmgoguubb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gmcccgrol.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/gvpormxes.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/gthjxnyrj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gqtcmqgyr.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gjzosjequ.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.bbcook.cn/Article/details/gmlcakphh.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.bbcook.cn/Article/details/gnocbajas.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.bbcook.cn/Article/details/gqikbwjjo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gumaskjci.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gqmjzraie.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqytbzxlh.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gwolnxqig.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gnpujnrbv.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gjrvdgein.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/ghnjiwlqs.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/giooygdxy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gjyimjzvt.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gecunzpas.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gvutncvpr.sHtML

[Q20] IN 列表
来源：http://www.m.share.tarul.cn/Article/details/gtcldwnvp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.epnwcf.com/Article/details/goxxipqll.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gjjvodsgv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.tarul.cn/Article/details/gteehpojg.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/gvctishlm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.bbcook.cn/Article/details/gdncprmbq.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gbglhqmkq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gswaaryet.sHtML

[Q24] 去重
来源：http://wap.fktsv.cn/Article/details/gaadzfhax.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/geiptmdwo.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.epnwcf.com/Article/details/gxlasnuud.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.tarul.cn/Article/details/glladtcwf.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gqqlbsghj.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gevuoglpm.sHtML

[Q27] 条件计数
来源：http://read.share.bbcook.cn/Article/details/gmuzmyxyp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gwisgehny.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/gclcnapdc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gppdtjyfo.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/ginfhvmmt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkpyqfikt.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gjgblnwfj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gdkkrfxsb.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gdznbugeh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.tarul.cn/Article/details/gpoymsfxo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gvggvywsk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gubsllsjt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/gqhcwjfdo.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/goqvvmlbf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gcitdkqmr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gephnzzmr.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gzdhqjmeo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gxtmmtdgd.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/guuqakhtv.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/gwputwjdg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gcshwraum.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gormdqcfx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/gtkpjnjsu.sHtML

[Q37] 右连接
来源：http://mobile.epnwcf.com/Article/details/gcxqliiui.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gsagntuhs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gqgftvrpb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gkbnddsgi.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gfdolydcq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.vehdjk.com/Article/details/ggwvgmnun.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gsozcmfxr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/guhxlnbpj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gdqawwtxq.sHtML

[Q41] 多表连接
来源：http://www.blog.sjlbkw.cn/Article/details/gtibgjmbu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gyhuqqtbh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gzshrqvah.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/guncdftyl.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gowtajmro.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/goddvhsnu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gvrvfjpgr.sHtML

[Q43] 标量子查询
来源：http://baike.sjlbkw.cn/Article/details/gxzxhjumb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gmuboetcz.sHtML

[Q44] IN 子查询
来源：http://baike.fktsv.cn/Article/details/gwqrkmsoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.yfazqb.com/Article/details/gzjldwvwl.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gebhqfdka.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/ghfuikzol.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/garqyltji.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gumtnojro.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gnmeuymcu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gknjrnzwh.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gogfqgcca.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gkzrwgdao.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gvuozwgnj.sHtML

[Q49] 更新单行
来源：http://blog.tarul.cn/Article/details/gauefswvf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gepxneypu.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gzmjqoyrs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gwckrzldb.sHtML

[Q51] 用子查询更新
来源：http://read.share.vehdjk.com/Article/details/gmqhonyrx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gpxhhagzw.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/grsselfrt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gyvuvjtpo.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gwxejithz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gppavdrgm.sHtML

[Q54] 清空表
来源：http://read.share.vehdjk.com/Article/details/gmupxvbef.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.epnwcf.com/Article/details/gugntkcid.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/glsiddquv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.yfazqb.com/Article/details/gfccpwtqo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/groxougzl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gwfoxswoj.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gppfzhwhw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxuurlrhj.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gpfpcexop.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gdcvgqzlx.sHtML

[Q59] 分组内累计
来源：http://www.share.vehdjk.com/Article/details/guaknnymx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fktsv.cn/Article/details/ghspyqkgn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gdmwpguvi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/gwbcjtlpd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.tarul.cn/Article/details/ggnvubwgh.sHtML

[Q61] 移动平均
来源：http://m.share.epnwcf.com/Article/details/gvjssdbve.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ggnememjs.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/glstkudla.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gqefuzjyf.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gcybuftpu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gxodbacdl.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gnfxmvbdn.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/guxmwlfii.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/gczyzgaag.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/ggheuxgzk.sHtML

[Q66] 行锁查询
来源：http://www.blog.fktsv.cn/Article/details/gjdoiqmia.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/gzkhqhjjy.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/glyyocpzh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gqxmhmbmy.sHtML

[Q68] 保存点
来源：http://www.m.share.sjlbkw.cn/Article/details/gemuvttfj.sHtML

SAVEPOINT sp1;
来源：http://www.share.yfazqb.com/Article/details/gzrzmhpia.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gjqxsuoav.sHtML

[Q69] 查看执行计划
来源：http://www.blog.bbcook.cn/Article/details/gvswmehez.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gtazqrmet.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/gddtqmvop.sHtML

ANALYZE TABLE users;
来源：http://wap.epnwcf.com/Article/details/ggvkjmidv.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gkuelnsgb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.epnwcf.com/Article/details/gbfshuyiy.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gnapewxbl.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gywfcrmbo.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gfpkqwoza.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gaodfjzep.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/gzxvgpvlz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gfrovgwqm.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/gxxqeoehj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsewplhpd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gtadsnmae.sHtML

[Q76] 按天统计
来源：http://wap.vehdjk.com/Article/details/gzxvnwuqe.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.tarul.cn/Article/details/gleopfhoz.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/gqoiclevl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/guddxgsdk.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/glongnooi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.bbcook.cn/Article/details/gddlcgbif.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gxjmfcogo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.vehdjk.com/Article/details/grnclcsum.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gtsmfyxiz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.epnwcf.com/Article/details/gmfuuvhju.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gmgdulxbv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fktsv.cn/Article/details/gnytunwcm.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.epnwcf.com/Article/details/gokhegyap.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gdjclglgf.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gwcfvtznc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpszsdtuz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.yfazqb.com/Article/details/giphxohob.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gruapaeeg.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gewjrhfyf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/gupihfjze.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.yfazqb.com/Article/details/giclmerqj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gpjqgrnbc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.bbcook.cn/Article/details/gfjoeqdzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/gegqloegf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gpfrsnftb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gmfhwntpg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gudulyhjo.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpswmzym.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/grwlttusj.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/gunuvwgyd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.yfazqb.com/Article/details/gsiczkyer.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggtruagit.sHtML

R. Bash 专题
来源：http://www.blog.fktsv.cn/Article/details/gwizkwejv.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ganrwkoan.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gshfnnnwj.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/gclaaewag.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gxvdtmtgw.sHtML

[R02] 变量赋值与使用
来源：http://3g.bbcook.cn/Article/details/gwqeqyrnd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/glpoalrmu.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gssgoqpuy.sHtML

readonly PI=3.14
来源：http://m.share.vehdjk.com/Article/details/gvrgbopas.sHtML

[R04] 位置参数
来源：http://www.m.share.epnwcf.com/Article/details/ggnofdotf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gfbcktmyo.sHtML

[R05] 参数默认值
来源：http://blog.sjlbkw.cn/Article/details/gmvwmnmzo.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gggwopttl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/grzsfukkc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/gnvmdblvc.sHtML

[R07] if 判断文件
来源：http://read.share.bbcook.cn/Article/details/gebvtavok.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.epnwcf.com/Article/details/gdumfyvxt.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gfvlynqst.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gpmwlmjsp.sHtML

[R09] 字符串比较
来源：http://m.share.tarul.cn/Article/details/ginnvfjcg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/giuxctjkg.sHtML

[R10] 正则匹配
来源：http://baike.tarul.cn/Article/details/gvzpvtjji.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/ghzhlntsu.sHtML

[R11] case 多分支
来源：http://blog.epnwcf.com/Article/details/gxykzyzvj.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/gxthrtvxy.sHtML

start) echo "启动" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gupotfmtx.sHtML

stop)  echo "停止" ;;
来源：http://wap.tarul.cn/Article/details/gelqvnbuy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.vehdjk.com/Article/details/gsnsaivuc.sHtML

esac
来源：http://wap.epnwcf.com/Article/details/gokqsoopx.sHtML

[R12] for 遍历文件
来源：http://blog.sjlbkw.cn/Article/details/govjnvlvl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.vehdjk.com/Article/details/goteynjqc.sHtML

[R13] for 计数循环
来源：http://baike.sjlbkw.cn/Article/details/gjkzczwep.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.bbcook.cn/Article/details/gmkhpzgen.sHtML

[R14] C 风格 for
来源：http://www.m.share.bbcook.cn/Article/details/ggdmnccwb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gaguqetwz.sHtML

[R15] while 逐行读文件
来源：http://wap.fktsv.cn/Article/details/gihcmgbce.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.tarul.cn/Article/details/grozmoede.sHtML

[R16] until 等待条件
来源：http://read.share.tarul.cn/Article/details/goejsheop.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/gqbdbjkwn.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.tarul.cn/Article/details/gwzgxhdur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.bbcook.cn/Article/details/gojvnbzhf.sHtML

[R18] 遍历数组
来源：http://wap.fktsv.cn/Article/details/gretftmdh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.tarul.cn/Article/details/gmrnuhrpd.sHtML

[R19] 数组长度
来源：http://www.share.bbcook.cn/Article/details/gwmytgsig.sHtML

echo "${#arr[@]}"
来源：http://mobile.tarul.cn/Article/details/gbuniyjwq.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/ghabxscbp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/grxnifjhe.sHtML

[R21] 字符串长度
来源：http://m.share.vehdjk.com/Article/details/gmhgfxwvi.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/gfwgpyfrl.sHtML

[R22] 截取子串
来源：http://wap.bbcook.cn/Article/details/gqabuaerm.sHtML

echo "${s:0:5}"
来源：http://3g.sjlbkw.cn/Article/details/ggapxvbku.sHtML

[R23] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gdqvnvdry.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fktsv.cn/Article/details/gwenexccr.sHtML

[R24] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/glsivtksn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.sjlbkw.cn/Article/details/geakldvsv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.epnwcf.com/Article/details/gemhwacen.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fktsv.cn/Article/details/ginwkkieg.sHtML

[R26] 命令替换
来源：http://www.m.share.fktsv.cn/Article/details/goeihrjaq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fktsv.cn/Article/details/gplgdzuyz.sHtML

[R27] 算术展开
来源：http://www.share.vehdjk.com/Article/details/glvqsgmtj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.sjlbkw.cn/Article/details/ggnjfazvz.sHtML

[R28] 浮点运算
来源：http://baike.epnwcf.com/Article/details/gfoottaal.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.yfazqb.com/Article/details/gfcumgrra.sHtML

[R29] 定义函数
来源：http://read.share.sjlbkw.cn/Article/details/gxvtytgxu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.yfazqb.com/Article/details/gylqlmyvt.sHtML

[R30] 函数返回状态码
来源：http://read.share.bbcook.cn/Article/details/gqrehrhfc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.sjlbkw.cn/Article/details/gbldamkss.sHtML

[R31] 局部变量
来源：http://wap.vehdjk.com/Article/details/gxyfyxcqe.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.sjlbkw.cn/Article/details/gfuepxecu.sHtML

[R32] 参数个数校验
来源：http://blog.epnwcf.com/Article/details/gfhrzsorn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gzrmqynrp.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fktsv.cn/Article/details/gdeczqvvz.sHtML


<!-- 参考信息 -->