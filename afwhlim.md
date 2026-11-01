代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.epnwcf.com/Article/details/gqntpdrfd.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gvugfdcvi.sHtML

[P07] 防抖与节流
来源：http://www.blog.yfazqb.com/Article/details/gmghownat.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gvkjeflte.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.vehdjk.com/Article/details/gupeukjeg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gdijmcult.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gonrwzvsb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/godaeibhh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/guvooshjv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.yfazqb.com/Article/details/gdblcbvcg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fktsv.cn/Article/details/gmtmpveps.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.epnwcf.com/Article/details/gjyymxnxh.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gexhmivfp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/ghzqvqnrr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.tarul.cn/Article/details/gdsozhlbb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.tarul.cn/Article/details/ggzxgffzg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.yfazqb.com/Article/details/gjfqnaiuq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/gjyugeruk.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gxpmiitms.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gmwrqbzjz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gdpkngygd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/goypwzbku.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/giphaowez.sHtML

[Q01] 创建表
来源：http://m.share.tarul.cn/Article/details/gpbiyxjpb.sHtML

CREATE TABLE users (
来源：http://www.m.share.tarul.cn/Article/details/gxocpbyem.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gonnaelek.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gyvasxdix.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/gtmgqsady.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/ggqhzvbkj.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gwnyvypsh.sHtML

[Q02] 创建带外键的表
来源：http://wap.vehdjk.com/Article/details/gitqjrrex.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/gcvgtcqbp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.tarul.cn/Article/details/gzyokwtlz.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gmmvzurfd.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.yfazqb.com/Article/details/gqccbncet.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gxzaqutty.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gxzkeonnb.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/gokvfsfyy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gxxbvaemp.sHtML

[Q04] 修改列类型
来源：http://mobile.epnwcf.com/Article/details/gfddpdtlc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fktsv.cn/Article/details/gjqtcaksr.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/glgdllikx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gbstnpvjd.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gimmjemjl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fktsv.cn/Article/details/gccxllmwl.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/gamvtgdyk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.sjlbkw.cn/Article/details/gchyjgvsr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/goypabjxf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gckkrrbdi.sHtML

[Q09] 创建唯一索引
来源：http://read.share.tarul.cn/Article/details/golefywwj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.epnwcf.com/Article/details/gjniduizq.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gkrqyuubs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gyfhklqon.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gmznlrmwn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/glgwgwrhx.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gywmhmfjs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.bbcook.cn/Article/details/gcvjygxbh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gpkvoauyq.sHtML

[Q13] 忽略重复插入
来源：http://www.share.vehdjk.com/Article/details/gerxrnmfu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/gghtshten.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.yfazqb.com/Article/details/gwslqacus.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgnofdfj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/gthbycqee.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/ggfwwanah.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gslnsxhlc.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/ggyqntsez.sHtML

SELECT id, name FROM users;
来源：http://wap.epnwcf.com/Article/details/gcsudmtpi.sHtML

[Q17] 条件查询
来源：http://www.m.share.tarul.cn/Article/details/gouepsrgs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gbojczcpi.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gyougkrhc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fktsv.cn/Article/details/gfrfecziz.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gsyiznlsx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gqpjqttmm.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gssuhlpsz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gysbpnmdt.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/gdnvynyif.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gpzhjcghe.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gstuvcfov.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gzmtbnrfc.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/gpqajqjrx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/ghsvzdxbg.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gfindmuml.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gkxdgbxhv.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gpjhgptqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gtepiyaek.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gblejziki.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/guithsqgg.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/grofynvpc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/gkyzffoly.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gbgstrjxq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/guotzmsuo.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/gejuypahc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gnzetrywb.sHtML

[Q30] 分组统计
来源：http://www.share.fktsv.cn/Article/details/gpbsfinpo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gavmmwcos.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gzcapltey.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.sjlbkw.cn/Article/details/gitfojpcg.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/geyuwporn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gxtganarz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/ggblyvded.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/gfjekeciq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gguxtzuhb.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gwhheovmd.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/gdugmfhwf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/gtpznmcuu.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/gmxbelduz.sHtML

[Q35] 内连接
来源：http://mobile.epnwcf.com/Article/details/gimsmddbk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gpogerbet.sHtML

[Q36] 左连接
来源：http://mobile.yfazqb.com/Article/details/gbbskrmae.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gpdjtguie.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gmlgzsopi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gtlebonsi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/ggtuedfpd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gflubjslc.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gpitlhybz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/goawtxmjh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.vehdjk.com/Article/details/glygreijm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gekyxdpro.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gsmwykski.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gdclytwwy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/goewgzwpf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gdeosixcx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/gshgwyliu.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gmjhgseet.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gkqshbbjs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.vehdjk.com/Article/details/gacofbklp.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/gyfcaosxf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gwgsyrosa.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gxuzwubnz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.bbcook.cn/Article/details/gzdlyjgjk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gigvxxfnh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.vehdjk.com/Article/details/gvivwixha.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gitscterm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gotyggmys.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gvwsajlgp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gcxliuexj.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/grqeznofa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gieoxwhtc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gwpneywut.sHtML

[Q49] 更新单行
来源：http://3g.epnwcf.com/Article/details/gabdqmbyr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gxozkvfto.sHtML

[Q50] 批量更新
来源：http://www.m.share.sjlbkw.cn/Article/details/geidwsivk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/grqoljjdt.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gyvyqrvmi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gfbdbdumx.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gygdsnymh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gdgsvkabg.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gupkcgpgg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gghjojrdr.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gdslenbev.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gzlfxombh.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.epnwcf.com/Article/details/gawuhzuny.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gjlykreqw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.epnwcf.com/Article/details/gszqoykkz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.yfazqb.com/Article/details/gytxvevjd.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/ghsvkxutx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/gyjtpbuuz.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gvmmszpsv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gqjuetism.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/gzabxxibs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gjrjuthgd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gehhetueu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gprplhhzt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gvyxeiwci.sHtML

[Q61] 移动平均
来源：http://www.m.share.epnwcf.com/Article/details/gboitontx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gtenvrzba.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gkucbjkvj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gzvitxxky.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/guwqemqtx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/ghhmxqxig.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/gnguhydao.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gnkhysmtv.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gldzyvxqz.sHtML

ROLLBACK;
来源：http://www.blog.sjlbkw.cn/Article/details/gnngmaaui.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gqxriwzyx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/gsyukezyz.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/givjrfiws.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gbbxzzywv.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gfcalghmu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gmmphntju.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fktsv.cn/Article/details/gsjndvpws.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gpyjxurnc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gejqtrvjt.sHtML

[Q70] 更新统计信息
来源：http://read.share.vehdjk.com/Article/details/gcwcfeows.sHtML

ANALYZE TABLE users;
来源：http://wap.tarul.cn/Article/details/gdicddwal.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gkqrhhukz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.bbcook.cn/Article/details/gscemxzob.sHtML

[Q72] 查看索引
来源：http://read.share.tarul.cn/Article/details/ghzvzzbvo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gputertjy.sHtML

[Q73] 查看表状态
来源：http://www.share.vehdjk.com/Article/details/gjgbvjnjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gajtoqocb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fktsv.cn/Article/details/gofhjffcz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gvqcrxinb.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gkmatpemt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gijxftqus.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gngbloxqg.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gswfhhxbo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.bbcook.cn/Article/details/glpmovfud.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gcyoknpwq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/glxwfxonx.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/gbxdanlcy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.bbcook.cn/Article/details/gwmcjzluh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gmeuowlnw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gepmgrvsa.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gbifwkkys.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gfezwhlmj.sHtML

[Q81] 字符串替换
来源：http://m.share.sjlbkw.cn/Article/details/gbmyrntet.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.tarul.cn/Article/details/gofgtshho.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/govsylacu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gqjcxgynk.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gaybevfew.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gajzxcrdo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fktsv.cn/Article/details/grtjpvxfb.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gujfyknex.sHtML

[Q85] 数值取整
来源：http://m.share.tarul.cn/Article/details/gmoxqshqv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/ggoxpxoqi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gioigndos.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/gqknpvwfa.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.epnwcf.com/Article/details/gcdqjophs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gusuifjbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gpwelsche.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/gvmopiifm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gawobdjsj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gsoddgqwx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/gnmrbehvj.sHtML

[Q90] 生成序号列
来源：http://mobile.bbcook.cn/Article/details/gjghbewbk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gkiavcudo.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqmrghngq.sHtML

R. Bash 专题
来源：http://m.share.vehdjk.com/Article/details/guiulyvul.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gdowltbyh.sHtML

[R01] shebang 与严格模式
来源：http://3g.yfazqb.com/Article/details/gtzpdcfhh.sHtML

#!/usr/bin/env bash
来源：http://3g.vehdjk.com/Article/details/gkawskebf.sHtML

set -euo pipefail
来源：http://read.share.vehdjk.com/Article/details/gghyxxdsz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/gwzvjguet.sHtML

name="Tom"; echo "$name"
来源：http://mobile.sjlbkw.cn/Article/details/gjullclxf.sHtML

[R03] 只读变量
来源：http://3g.fktsv.cn/Article/details/gpragtacd.sHtML

readonly PI=3.14
来源：http://3g.sjlbkw.cn/Article/details/gxsbmbdtq.sHtML

[R04] 位置参数
来源：http://read.share.tarul.cn/Article/details/gsrqzzhbq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/gaxfbindx.sHtML

[R05] 参数默认值
来源：http://baike.vehdjk.com/Article/details/gnwmrzxdj.sHtML

name="${1:-default}"
来源：http://www.m.share.bbcook.cn/Article/details/gkjvaapim.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/ghzqzboce.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gjiiqutha.sHtML

[R07] if 判断文件
来源：http://www.m.share.vehdjk.com/Article/details/glkbwiiqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.vehdjk.com/Article/details/gdgzepxsk.sHtML

[R08] 数值比较
来源：http://mobile.bbcook.cn/Article/details/gcrvlxmvt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fktsv.cn/Article/details/grpeirqpz.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/gmyzqkeoh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/gxzpwlfzk.sHtML

[R10] 正则匹配
来源：http://mobile.yfazqb.com/Article/details/gypjsympc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gasnygofe.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/gwazkxjbk.sHtML

case "$1" in
来源：http://m.share.bbcook.cn/Article/details/gerzsisor.sHtML

start) echo "启动" ;;
来源：http://3g.vehdjk.com/Article/details/gjljlavib.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gmwovlcrp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gzdewhsnn.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gxuwmroai.sHtML

[R12] for 遍历文件
来源：http://wap.yfazqb.com/Article/details/gwclhstvk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/golqndpaq.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gzyviddss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gziuzgtus.sHtML

[R14] C 风格 for
来源：http://read.share.vehdjk.com/Article/details/gsdzqremh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gznzedakb.sHtML

[R15] while 逐行读文件
来源：http://blog.tarul.cn/Article/details/glqtzmcse.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.yfazqb.com/Article/details/gbizdpcuv.sHtML

[R16] until 等待条件
来源：http://3g.yfazqb.com/Article/details/glesrsdev.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.epnwcf.com/Article/details/gkscivfmi.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gssxartds.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.yfazqb.com/Article/details/gqmvnvfio.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/gzyawolas.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gaqycjybl.sHtML

[R19] 数组长度
来源：http://www.share.vehdjk.com/Article/details/ggltqlmiq.sHtML

echo "${#arr[@]}"
来源：http://www.blog.bbcook.cn/Article/details/gajyrjfvy.sHtML

[R20] 关联数组（字典）
来源：http://blog.sjlbkw.cn/Article/details/gjmjzqjvy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.epnwcf.com/Article/details/gnkayqxhw.sHtML

[R21] 字符串长度
来源：http://www.m.share.yfazqb.com/Article/details/gbnslvbdn.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gffkncvbx.sHtML

[R22] 截取子串
来源：http://wap.sjlbkw.cn/Article/details/gyckgmsij.sHtML

echo "${s:0:5}"
来源：http://blog.epnwcf.com/Article/details/gbdyxtjlf.sHtML

[R23] 字符串替换
来源：http://www.blog.sjlbkw.cn/Article/details/glygycgzd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.sjlbkw.cn/Article/details/gtwflforj.sHtML

[R24] 大小写转换
来源：http://m.share.tarul.cn/Article/details/gokqmpzfo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.sjlbkw.cn/Article/details/gzdiajfri.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.sjlbkw.cn/Article/details/glkwxpkup.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.bbcook.cn/Article/details/gqminsucd.sHtML

[R26] 命令替换
来源：http://read.share.bbcook.cn/Article/details/gujpnvuvz.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.yfazqb.com/Article/details/gbsjgfnlg.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gystriwvy.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.vehdjk.com/Article/details/gmqipzpdv.sHtML

[R28] 浮点运算
来源：http://3g.bbcook.cn/Article/details/gyakipksx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.bbcook.cn/Article/details/gjqiupvvi.sHtML

[R29] 定义函数
来源：http://www.share.epnwcf.com/Article/details/gzjutesnd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fktsv.cn/Article/details/glwsfdlly.sHtML

[R30] 函数返回状态码
来源：http://baike.yfazqb.com/Article/details/gbziycohy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.sjlbkw.cn/Article/details/gwzdejbdv.sHtML

[R31] 局部变量
来源：http://m.share.yfazqb.com/Article/details/gviztkvlx.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.vehdjk.com/Article/details/gnmpdiimn.sHtML

[R32] 参数个数校验
来源：http://www.m.share.bbcook.cn/Article/details/grrlkwvun.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.yfazqb.com/Article/details/gayepxynk.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fktsv.cn/Article/details/garsszqrc.sHtML


<!-- 参考信息 -->