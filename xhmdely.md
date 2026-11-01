代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.yfazqb.com/Article/details/gllurqoha.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gseolrtfv.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/givooahqp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.tarul.cn/Article/details/gzgzqfyki.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gpsyplnex.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gfzoxypnv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gnpackshy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/giridcwnk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.tarul.cn/Article/details/ggmhfiycq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.tarul.cn/Article/details/gkvybqhgc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.epnwcf.com/Article/details/gobgocosf.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/ggkhapaig.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gifjspwse.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/goibycmay.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/guemvkysp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gofilacdh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gvssisaqq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/givmhfyqe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gdvvnohwh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gmbyzbcxl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gtgnpgkjl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.vehdjk.com/Article/details/gdcxvwbnd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtpuvuvwr.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/gqcsgpjkm.sHtML

CREATE TABLE users (
来源：http://www.blog.yfazqb.com/Article/details/gymuzxsfe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gnunxkyat.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/ghckbmxep.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.yfazqb.com/Article/details/gfqizubmp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fktsv.cn/Article/details/gbxnnlwpa.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gpntcpdpv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/grgghiwza.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/grqvqcezs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gvwgipbqy.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gzdrwtphs.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.epnwcf.com/Article/details/grioiirpo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gkbnrgihp.sHtML

);
来源：http://blog.tarul.cn/Article/details/gbtdctgmu.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/ghudyvfqc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.yfazqb.com/Article/details/gbfnukmao.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/girvrgnvj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gtgcbzorn.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gizlxsmqa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gxhoiztlz.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gqpxzvdbs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/ggtuhrdpy.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gzjmzlmtj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gmnwiynuq.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gnaxaxxjg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gddidqadn.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/gumtxqszj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gpmdhkkts.sHtML

[Q10] 插入单行
来源：http://3g.vehdjk.com/Article/details/gnoyikjqj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.bbcook.cn/Article/details/gybdlkyva.sHtML

[Q11] 一次插入多行
来源：http://www.share.vehdjk.com/Article/details/gfaqndffq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gewnghhjk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gpohvyqdc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gkdrxujqb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gnddefpdq.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gdqfbxigg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/ghohpasch.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.epnwcf.com/Article/details/gfuphbgrl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gsbtxqxqt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gdelwukle.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gcxjdyzyq.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gnzrkwwxq.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gemfbkpsn.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/gtjwqhfxk.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gvhfgizqi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.tarul.cn/Article/details/gdgetrfwu.sHtML

[Q18] 模糊匹配
来源：http://3g.bbcook.cn/Article/details/gmkeuzlke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/gdendiuwc.sHtML

[Q19] 范围查询
来源：http://m.share.bbcook.cn/Article/details/gksgchpfl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.sjlbkw.cn/Article/details/gfbvzibhm.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/gcqzsobrk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gguctkmgw.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gfajaphwm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gdaysbgpg.sHtML

[Q22] 排序
来源：http://read.share.epnwcf.com/Article/details/ggkmjdvmx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gmjwprdyh.sHtML

[Q23] 分页
来源：http://m.share.yfazqb.com/Article/details/gprfuqzvb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gywehqdnx.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gnamvgfxu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.vehdjk.com/Article/details/gfwknnnmg.sHtML

[Q25] 只取前 N 条
来源：http://3g.bbcook.cn/Article/details/gyulabokj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/gflevbren.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gqxgnghra.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/goollugen.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/grzdcplzu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gglyrprgq.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/grbdyjxgm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gjdrbwjjw.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gkqfakuic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/galsbrrxl.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/gwklqiggy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gwfukcwmu.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gwqmmjumz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.epnwcf.com/Article/details/gnpldhzxi.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gtnixgmdt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/ghtsxjvyz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/gkcgbssuu.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gtyzhjkmk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/ggxjguhof.sHtML

[Q34] 每组取第一条
来源：http://read.share.fktsv.cn/Article/details/ggzpwieuj.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gdyiqqtzw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gppinbynn.sHtML

) t WHERE rn = 1;
来源：http://m.share.vehdjk.com/Article/details/guhbooguy.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gmvcqmbwv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gujbqgzyc.sHtML

[Q36] 左连接
来源：http://wap.tarul.cn/Article/details/gbdwzvukp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gymqncmgn.sHtML

[Q37] 右连接
来源：http://m.share.vehdjk.com/Article/details/gnrgkgvet.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/geddkhtkm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/godbjsvdp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gvpiwtjmp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gvqentqjl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.epnwcf.com/Article/details/gbwjqasgm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/gfzklghor.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gmatoksaa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/godygnomi.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/ghyrffguo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fktsv.cn/Article/details/gincluuhg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gcmneooyz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.yfazqb.com/Article/details/gshqpyhrg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gdvhuzyco.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gaiiuuans.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/gmgthrbqc.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/gqrmrjcfv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.vehdjk.com/Article/details/gcrcqwlcb.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/ggsstuzag.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.epnwcf.com/Article/details/gobbkckqp.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gpmnynewv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/godwpllin.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/ggsiosryw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.tarul.cn/Article/details/gvjgtgyon.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gwishfjpf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/guukizozi.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/grdoctalj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/glmronmdp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/gjjvsfval.sHtML

[Q49] 更新单行
来源：http://www.share.sjlbkw.cn/Article/details/gcmndkqiw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gdutfbwhk.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/gvrqsujiw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/grcldcmrv.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gaonqnxlw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/glgxjsftl.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gwzkpijnx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gurtswxun.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gzhewwcaf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gpwqyjfnq.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/gwekmxtem.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gukhkqybp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.vehdjk.com/Article/details/gpqdvhuhz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gqduvlqfm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gpngymfvy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gmdqgiubm.sHtML

[Q57] 行号
来源：http://3g.tarul.cn/Article/details/glufrpyqw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/grpsbqeux.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gnuklspvu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gvykfvrjj.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/gtudiaffm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gohafiita.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.bbcook.cn/Article/details/gdazowuda.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gizyiqncc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.vehdjk.com/Article/details/ghoaxdtxz.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/ghxlirlil.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gzhcwvvfc.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/gjnoowpze.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/ghaxynerh.sHtML

[Q63] 开启事务
来源：http://3g.fktsv.cn/Article/details/gmjxcywdh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.sjlbkw.cn/Article/details/gqfwufqxj.sHtML

[Q64] 提交事务
来源：http://read.share.bbcook.cn/Article/details/gstoirysn.sHtML

COMMIT;
来源：http://baike.bbcook.cn/Article/details/gzqrvwvru.sHtML

[Q65] 回滚事务
来源：http://mobile.yfazqb.com/Article/details/gmwmhfqcf.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gpiuukwnc.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gmvqdiilq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.vehdjk.com/Article/details/gzbezxtji.sHtML

[Q67] 设置隔离级别
来源：http://m.share.yfazqb.com/Article/details/gzyyfxcix.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.vehdjk.com/Article/details/gznycryzj.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gbxnoxawg.sHtML

SAVEPOINT sp1;
来源：http://read.share.yfazqb.com/Article/details/gltzaoyyf.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/givdmsuui.sHtML

[Q69] 查看执行计划
来源：http://wap.yfazqb.com/Article/details/gjkwdrfbu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fktsv.cn/Article/details/gnxaboixy.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gvbhbfbxp.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gxlubbrex.sHtML

[Q71] 查看建表语句
来源：http://blog.fktsv.cn/Article/details/gynkbbkuj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gzbgqnzry.sHtML

[Q72] 查看索引
来源：http://blog.fktsv.cn/Article/details/gatrdmkeb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjprcneka.sHtML

[Q73] 查看表状态
来源：http://www.blog.epnwcf.com/Article/details/gbtnxmipl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gfchcbkhe.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/grzktwehg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.epnwcf.com/Article/details/gbexnvzez.sHtML

[Q75] 日期格式化
来源：http://blog.bbcook.cn/Article/details/gtphhirog.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fktsv.cn/Article/details/guxzbgvta.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gnuqsuaiq.sHtML

[Q76] 按天统计
来源：http://blog.yfazqb.com/Article/details/gomnlgazt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gjvulrrtr.sHtML

[Q77] 时间加减
来源：http://www.blog.bbcook.cn/Article/details/gjbjkblvj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.bbcook.cn/Article/details/gdhnlmitg.sHtML

[Q78] 当前时间
来源：http://mobile.sjlbkw.cn/Article/details/gbxhgionz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.bbcook.cn/Article/details/gomrzobca.sHtML

[Q79] 字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gwkkmydtd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.yfazqb.com/Article/details/ghlvaewgw.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gwlzlmuxp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gopuujqmz.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gdfgxgtrn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gazzhwfrz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.tarul.cn/Article/details/glfmuklyi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjqdxzzgg.sHtML

[Q83] 大小写转换
来源：http://mobile.sjlbkw.cn/Article/details/gdhogmrgz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gmylkjovg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.tarul.cn/Article/details/gvsrkczor.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjighqfrf.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/grymessnv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.tarul.cn/Article/details/gpudtucxl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.epnwcf.com/Article/details/gmtdwqnme.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/gtaxkqnmx.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/glghukiqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.epnwcf.com/Article/details/gnjrptvwc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gpqexsdcs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.bbcook.cn/Article/details/gprblovhn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/ggbneiuxu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.bbcook.cn/Article/details/gmvbqplpi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fktsv.cn/Article/details/gllfczbil.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/gouicozmo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/gztsjgntl.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gzexfnugx.sHtML

R. Bash 专题
来源：http://wap.sjlbkw.cn/Article/details/gexxrkteu.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gsmwoxppx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.epnwcf.com/Article/details/gdhffxufp.sHtML

#!/usr/bin/env bash
来源：http://read.share.bbcook.cn/Article/details/gvxmtizzo.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gjbromozz.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/gbsztemxc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.vehdjk.com/Article/details/gfitvhgbs.sHtML

[R03] 只读变量
来源：http://www.share.fktsv.cn/Article/details/gcjsqpdjq.sHtML

readonly PI=3.14
来源：http://baike.sjlbkw.cn/Article/details/gybgmpzgu.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gozgukeqo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/glubguclv.sHtML

[R05] 参数默认值
来源：http://3g.fktsv.cn/Article/details/gszpirxcl.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gnudvdzrc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.vehdjk.com/Article/details/gdonhmxsp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gmfiamxjp.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/gkpvacktb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gmhkvswre.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gbbtwgoyd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gubtsopjz.sHtML

[R09] 字符串比较
来源：http://www.blog.bbcook.cn/Article/details/gacwsipot.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gageltwll.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/gfbrpipev.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.vehdjk.com/Article/details/glzugclrc.sHtML

[R11] case 多分支
来源：http://wap.tarul.cn/Article/details/gbfzufeaf.sHtML

case "$1" in
来源：http://www.m.share.tarul.cn/Article/details/gqpfrebrg.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/gyhbmexme.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gwlsxhjtn.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gbhfumasz.sHtML

esac
来源：http://www.m.share.vehdjk.com/Article/details/ggdkedbxn.sHtML

[R12] for 遍历文件
来源：http://m.share.epnwcf.com/Article/details/goaezokea.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gvmknfmgw.sHtML

[R13] for 计数循环
来源：http://m.share.fktsv.cn/Article/details/gltfdqrzv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/ggezaaopr.sHtML

[R14] C 风格 for
来源：http://m.share.bbcook.cn/Article/details/gdsmiomoe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.epnwcf.com/Article/details/gnauepqok.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gjxkayjdq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.bbcook.cn/Article/details/gbbhfhnuz.sHtML

[R16] until 等待条件
来源：http://wap.vehdjk.com/Article/details/gjiifooxk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.epnwcf.com/Article/details/gvnqwwkso.sHtML

[R17] 数组定义与取值
来源：http://read.share.epnwcf.com/Article/details/gitlsxrsj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.bbcook.cn/Article/details/gwnjbszgc.sHtML

[R18] 遍历数组
来源：http://wap.yfazqb.com/Article/details/gyddesnck.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/glbriwidf.sHtML

[R19] 数组长度
来源：http://www.blog.vehdjk.com/Article/details/gbhlxfrkt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/gfscsiurp.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/gdfhmzvnl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.epnwcf.com/Article/details/geyifoztl.sHtML

[R21] 字符串长度
来源：http://3g.tarul.cn/Article/details/gfgdqqdsa.sHtML

echo "${#s}"
来源：http://www.share.sjlbkw.cn/Article/details/gabzjtzfw.sHtML

[R22] 截取子串
来源：http://www.m.share.yfazqb.com/Article/details/gddggncan.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gcxzgycuk.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gsxspzkuf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.bbcook.cn/Article/details/gpkrcsngr.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/gupredwqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gpkuyrygz.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gfprugulx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fktsv.cn/Article/details/glhdiejna.sHtML

[R26] 命令替换
来源：http://read.share.fktsv.cn/Article/details/gnrthbbxn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.vehdjk.com/Article/details/gypdyebel.sHtML

[R27] 算术展开
来源：http://wap.vehdjk.com/Article/details/gxvktxact.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.sjlbkw.cn/Article/details/gmncaibfz.sHtML

[R28] 浮点运算
来源：http://www.m.share.bbcook.cn/Article/details/gfeceazni.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.sjlbkw.cn/Article/details/gkkcznsyq.sHtML

[R29] 定义函数
来源：http://www.m.share.fktsv.cn/Article/details/gglkfgthh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.tarul.cn/Article/details/gbbylllwy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.bbcook.cn/Article/details/gtswoydnb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.yfazqb.com/Article/details/grvpjnass.sHtML

[R31] 局部变量
来源：http://blog.sjlbkw.cn/Article/details/gocvwujwa.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.bbcook.cn/Article/details/gxbertulc.sHtML

[R32] 参数个数校验
来源：http://3g.bbcook.cn/Article/details/gfusjccmx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fktsv.cn/Article/details/gsovymwwj.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.tarul.cn/Article/details/grslcrzvg.sHtML


<!-- 参考信息 -->