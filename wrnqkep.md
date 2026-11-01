代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/gzgobyflq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gjelrrbao.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/ggzqtwrrs.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.yfazqb.com/Article/details/gyilgaplb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.fktsv.cn/Article/details/gmclnnrfp.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gypoaphxs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/gsueuaujr.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/geueepkdd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gvovkpszn.sHtML

C#:   if (x is null) {}
来源：http://read.share.bbcook.cn/Article/details/gatijdvca.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gskgkuanl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/gvqkdlkvw.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gursjsbro.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gjrfdubgb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gwxtobjcg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gvzbbzknl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.bbcook.cn/Article/details/gclskvfjw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.sjlbkw.cn/Article/details/ggxfcdwyo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/ghjsbvnre.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/gimffbuhf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.sjlbkw.cn/Article/details/gqbwqvvcm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gxmsvjxrp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gmbepvxnc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/gypudburn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gjlonkitv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.tarul.cn/Article/details/gsrpwybsm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gkadccitd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gkoofxuad.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gprrirnlm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gzgkooylc.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxjmyyfqh.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/gkrnvdyzg.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/gvkddbuth.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gviapmons.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/gkccbpljj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/gjbmasfzo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/glhzxhxhx.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gopfxjadb.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gmahyvzwz.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gfiqllpkb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gixuvvidy.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gurwnpsat.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/grcamqzck.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.epnwcf.com/Article/details/gvyqkqfnu.sHtML

);
来源：http://wap.tarul.cn/Article/details/gwvlaexzq.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/gzmbmaspx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.yfazqb.com/Article/details/gteuisoih.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/giqijfsuy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gmvubbptc.sHtML

[Q05] 重命名列
来源：http://www.m.share.yfazqb.com/Article/details/geeqarkjq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.bbcook.cn/Article/details/gxxmtryau.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gvhsaftsb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gkagrtavp.sHtML

[Q07] 删除表
来源：http://www.m.share.vehdjk.com/Article/details/gbnxrnjjy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.epnwcf.com/Article/details/gtrsxrdfz.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/ggboveplu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/geifgjcjy.sHtML

[Q09] 创建唯一索引
来源：http://mobile.vehdjk.com/Article/details/gyrswyybh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gamxonxvg.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/gwbrdswpo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/grwykszrz.sHtML

[Q11] 一次插入多行
来源：http://read.share.yfazqb.com/Article/details/goyngezul.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gnukdbljd.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/glcwsfoxb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gzcvlyksn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gldupcwwt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/geiuepylc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/gucwqvlpd.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.yfazqb.com/Article/details/gvknsvuix.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/gahyxirxx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.epnwcf.com/Article/details/gkwziscjn.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gmptkitxr.sHtML

SELECT * FROM users;
来源：http://blog.tarul.cn/Article/details/gwgwxobzb.sHtML

[Q16] 查询指定列
来源：http://mobile.yfazqb.com/Article/details/gefhatbmk.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/gwdiceleo.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gyomkalpy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.yfazqb.com/Article/details/gnoaahvfw.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/gnwathrmn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gcoophxrb.sHtML

[Q19] 范围查询
来源：http://www.blog.tarul.cn/Article/details/gnmtvcilz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gscqzglhv.sHtML

[Q20] IN 列表
来源：http://m.share.yfazqb.com/Article/details/gqoytlrsg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fktsv.cn/Article/details/gwqpxoucs.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gpahofqfy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gwgpftplh.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/gqpeqtjxm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/gutvdthtj.sHtML

[Q23] 分页
来源：http://baike.yfazqb.com/Article/details/gbjbqhcph.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/grrnuqxfc.sHtML

[Q24] 去重
来源：http://www.share.sjlbkw.cn/Article/details/gpjedrszg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/gviwfemsq.sHtML

[Q25] 只取前 N 条
来源：http://wap.epnwcf.com/Article/details/golbggwwx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gazjrkqez.sHtML

[Q26] 计数
来源：http://wap.vehdjk.com/Article/details/gwpmstuda.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grfzvnrpn.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/ggvqkaojv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/gvzxffwlt.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gdsfbyxrv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gcmnbrkrc.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gowlusinb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/ghecolfrb.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gyhzyobuv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/gtwsdpjaz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gurcfxvgm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/gicwfakxi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/glvzlsajv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/githlixzc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/guzxnmrcy.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gvjmmdzit.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.epnwcf.com/Article/details/gbyuwqgyn.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gqoqgzdga.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gftecfiiq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/gtfafvvix.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gisunpdul.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gkjlcpgbf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gyrwipmyz.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gtvkcgedg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/glpiabioc.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gbqggqihj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.sjlbkw.cn/Article/details/gnupztsab.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.epnwcf.com/Article/details/gwzlxskpx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gebxzibit.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gyjrqjfcw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gnqyosild.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gjkjuzbca.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gshbkopyh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/gzuilziuc.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gmnoethvq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/gscrujyzv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gyegdlsue.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gxwhyeozm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/ghuizzmzu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gfcxnnama.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gghruulzb.sHtML

[Q43] 标量子查询
来源：http://baike.tarul.cn/Article/details/gueguberr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gkufztcop.sHtML

[Q44] IN 子查询
来源：http://3g.sjlbkw.cn/Article/details/gtszyichr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.yfazqb.com/Article/details/gllcnkwzs.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.yfazqb.com/Article/details/gwkauowyz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.tarul.cn/Article/details/gzncfayls.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.sjlbkw.cn/Article/details/gjkjkxvjz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gcrsiluga.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gwuyzapxd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/giwghzaet.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gytcvbpar.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.bbcook.cn/Article/details/gipudedqa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gzwdhqwkb.sHtML

[Q49] 更新单行
来源：http://wap.tarul.cn/Article/details/gucgjsjrf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/guvkffjnn.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/goxpwsnrg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gtpjtbmis.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gnjqvvcyk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gocgefrsv.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gfuouwime.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/genxvcdub.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gspouqhpm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgdydkvz.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gelpptlpb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.yfazqb.com/Article/details/glzsbamre.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.tarul.cn/Article/details/gfnygimmd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gzjfeiglx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.epnwcf.com/Article/details/ggxjmxpng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.tarul.cn/Article/details/gigypoeay.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/ghgkezwmd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gczrfhizl.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gjeecgvsi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/geucgynhk.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gkelojfdh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gvjilaxxz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gmfrhtcwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gwrxpelwf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gbaaechen.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gaysolqzt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gjtdhfnsx.sHtML

[Q62] 分组占比
来源：http://wap.vehdjk.com/Article/details/gxjqatjjp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/grjtikcsa.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gkiihpjht.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gqybtwlnc.sHtML

[Q64] 提交事务
来源：http://baike.tarul.cn/Article/details/ghpmcnfqv.sHtML

COMMIT;
来源：http://www.m.share.bbcook.cn/Article/details/gxvzemcuf.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/ghkjkhlzu.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/guxxkirki.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/guovzrxva.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/goqaegjah.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/gzudhsloe.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gpeieeoan.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/gxadpnsxl.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/gvmmvzfmh.sHtML

ROLLBACK TO sp1;
来源：http://mobile.tarul.cn/Article/details/gfrwfytrm.sHtML

[Q69] 查看执行计划
来源：http://mobile.vehdjk.com/Article/details/gqepnqlrc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gjhsichyo.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gnemjrqxz.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gmogqfnqv.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gpvpbewcm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fktsv.cn/Article/details/gbyhefbuc.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/gzlikwiip.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fktsv.cn/Article/details/gvzshesph.sHtML

[Q73] 查看表状态
来源：http://blog.fktsv.cn/Article/details/gywxwothz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhnkvuie.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/giyogaoyz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gpzmpofky.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gtdylvfzo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.bbcook.cn/Article/details/gneuvdauq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/guwitizio.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gpsehsbpm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/gzdhlmkbm.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gpeollynd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gxsccyqae.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gtmgrtnvm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gtwtzssdp.sHtML

[Q79] 字符串拼接
来源：http://www.share.sjlbkw.cn/Article/details/gduxuwmst.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.epnwcf.com/Article/details/gcmzwaeyd.sHtML

[Q80] 字符串截取
来源：http://wap.fktsv.cn/Article/details/ggwcfmscq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gssgpofjt.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gxetsslaq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.vehdjk.com/Article/details/goqvecaiu.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.yfazqb.com/Article/details/gexznafua.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gcmmijbrm.sHtML

[Q83] 大小写转换
来源：http://blog.sjlbkw.cn/Article/details/gwhcewymb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gweokpiai.sHtML

[Q84] 去除首尾空格
来源：http://www.share.epnwcf.com/Article/details/gwkzgrrqe.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fktsv.cn/Article/details/glezzlzhy.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gmuvdlpka.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gyxvfzztf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/ghepzflea.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.bbcook.cn/Article/details/gfbloqiqg.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.epnwcf.com/Article/details/gcufsngji.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fktsv.cn/Article/details/gnbozhgzq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvtaegtta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.vehdjk.com/Article/details/gojokopqh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/gmaqrjmcc.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/gfeyodgps.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.epnwcf.com/Article/details/gjjhwrpwo.sHtML

[Q90] 生成序号列
来源：http://3g.bbcook.cn/Article/details/gcgngljiu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gavxfzmtj.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/glpeqzphb.sHtML

R. Bash 专题
来源：http://www.m.share.bbcook.cn/Article/details/gcwaeukfx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goncqxwhi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gnkdoofwk.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gnyhtaxrj.sHtML

set -euo pipefail
来源：http://read.share.sjlbkw.cn/Article/details/gfjldeaen.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gexrvklnf.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/grrpgqset.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gryhkzadl.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/grgsgkswh.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gddebxjcs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.epnwcf.com/Article/details/guljlaznn.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gnhjtyvwe.sHtML

name="${1:-default}"
来源：http://www.m.share.epnwcf.com/Article/details/gflleexch.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fktsv.cn/Article/details/gbyzimejw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.yfazqb.com/Article/details/gtpnhzmot.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/glkmpdfen.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gxrxhahre.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/ginkayipy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gsluyddgx.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gytcgynrg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gkekwqvrx.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/gmtfloatt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gkfizldyk.sHtML

[R11] case 多分支
来源：http://www.m.share.vehdjk.com/Article/details/gqhgcgbwc.sHtML

case "$1" in
来源：http://m.share.bbcook.cn/Article/details/gjghkoiqd.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gsjdnzpme.sHtML

stop)  echo "停止" ;;
来源：http://3g.sjlbkw.cn/Article/details/gvhxrhbnu.sHtML

*)     echo "未知命令" ;;
来源：http://baike.tarul.cn/Article/details/gohevnbeg.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/guxqflkfe.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gtuygkidl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gseylqvny.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/guplcqswa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gressiukd.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/glgkbhymj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.yfazqb.com/Article/details/gpwpnssvj.sHtML

[R15] while 逐行读文件
来源：http://www.blog.vehdjk.com/Article/details/gxtichpzi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gfrpvupav.sHtML

[R16] until 等待条件
来源：http://read.share.bbcook.cn/Article/details/grxvblmot.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/gueroirsj.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gimwaxuxn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.sjlbkw.cn/Article/details/gbomiroru.sHtML

[R18] 遍历数组
来源：http://baike.yfazqb.com/Article/details/gnheixicl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.bbcook.cn/Article/details/gndbsonvb.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gbjzerbdh.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/geevogqhh.sHtML

[R20] 关联数组（字典）
来源：http://blog.bbcook.cn/Article/details/glerrbzsm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gqpsgrvmg.sHtML

[R21] 字符串长度
来源：http://m.share.tarul.cn/Article/details/gubddvrqs.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/golhwguka.sHtML

[R22] 截取子串
来源：http://www.share.fktsv.cn/Article/details/gxvyniqfn.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gczqzrffb.sHtML

[R23] 字符串替换
来源：http://blog.fktsv.cn/Article/details/gxjtrqset.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.sjlbkw.cn/Article/details/gypmrhujq.sHtML

[R24] 大小写转换
来源：http://baike.fktsv.cn/Article/details/gatedrtqs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fktsv.cn/Article/details/gznwkzpby.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.yfazqb.com/Article/details/genyrxnsu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gwsluyvlm.sHtML

[R26] 命令替换
来源：http://baike.fktsv.cn/Article/details/gahitefxp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.sjlbkw.cn/Article/details/gwarcaifk.sHtML

[R27] 算术展开
来源：http://read.share.tarul.cn/Article/details/glgpjpgdt.sHtML

echo $((1 + 2 * 3))
来源：http://3g.sjlbkw.cn/Article/details/gluinfnic.sHtML

[R28] 浮点运算
来源：http://read.share.sjlbkw.cn/Article/details/gpwvcphnl.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.tarul.cn/Article/details/gxlxetcgt.sHtML

[R29] 定义函数
来源：http://mobile.fktsv.cn/Article/details/gxxbvqono.sHtML


<!-- 参考信息 -->