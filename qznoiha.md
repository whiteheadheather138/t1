代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gawmrdrss.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gwkelsmvf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/geibcshhy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/grfrufrwd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.sjlbkw.cn/Article/details/gaunwjwzq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gucrbevaz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/gsjossbra.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/guirjhhza.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gulqwegmc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gzuknedxv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.epnwcf.com/Article/details/gzkomugio.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gyoeqwcow.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gmwhyjijj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gaxrgpupp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.tarul.cn/Article/details/gertvygzi.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.tarul.cn/Article/details/gktawstmy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gxdlaxbqi.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/ghmdvyptp.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.sjlbkw.cn/Article/details/gadaidmtf.sHtML

Go:   if x == nil {}
来源：http://mobile.yfazqb.com/Article/details/gfranvaci.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gxnboltih.sHtML

C#:   if (x is null) {}
来源：http://www.share.epnwcf.com/Article/details/ggxcuuiyu.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/gztxwcrik.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.bbcook.cn/Article/details/gwoccejiu.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.epnwcf.com/Article/details/gqewqvone.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gauiwveok.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gmbcnswtc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.tarul.cn/Article/details/grfangaiv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/gnlbbzaqv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.sjlbkw.cn/Article/details/gnsxwtlmr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gacvzmimu.sHtML

[P08] 处理浮点精度问题
来源：http://blog.tarul.cn/Article/details/gmkczbqds.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/ghudiramf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gadnwjdjl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/ggzmfyjly.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gvwewltuh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/gaubrdkwe.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.epnwcf.com/Article/details/gizqhufob.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.epnwcf.com/Article/details/gyinloxkm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gtmhwwitf.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gxqlhpung.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gjzgijutx.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/girsbcrva.sHtML

[Q01] 创建表
来源：http://m.share.bbcook.cn/Article/details/glucmourr.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gizpauian.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gydgukgat.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gyxczwsyj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gasxsiwuk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gmgivgyfw.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gogjrtnrr.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gjzpzjnzq.sHtML

CREATE TABLE orders (
来源：http://3g.tarul.cn/Article/details/gxfvkrvwo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gdjuzrtou.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gvjrepmav.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbxbbikf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gmjzynjrr.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/grgyhlpoc.sHtML

[Q03] 增加列
来源：http://read.share.bbcook.cn/Article/details/gnlljhnpn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.vehdjk.com/Article/details/gjgemofwu.sHtML

[Q04] 修改列类型
来源：http://wap.vehdjk.com/Article/details/gvbvlvsgb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gkjlnvoik.sHtML

[Q05] 重命名列
来源：http://read.share.tarul.cn/Article/details/gjgsqsiez.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/geketbnhw.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/goqmwzyqf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gekssvofe.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gkizvsmur.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.yfazqb.com/Article/details/gsithzddp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.bbcook.cn/Article/details/glxifeedy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/ggphxfcvx.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gcddaaejw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gfpczrozv.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gftjkpxsg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/glmurseio.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gajsrtcdf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gtfugjypj.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.bbcook.cn/Article/details/gshnrakfz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.vehdjk.com/Article/details/gdsszdmib.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gkmzjqbxl.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gqllupkhc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.bbcook.cn/Article/details/gktuqjekq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/glamtribq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/gcpuqaklc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.tarul.cn/Article/details/gsacbfogf.sHtML

[Q15] 查询全部
来源：http://www.blog.yfazqb.com/Article/details/ggucvtheg.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gjwrllibt.sHtML

[Q16] 查询指定列
来源：http://3g.sjlbkw.cn/Article/details/gonukijyq.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gfyjvjmab.sHtML

[Q17] 条件查询
来源：http://blog.fktsv.cn/Article/details/gbrhlhqor.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.bbcook.cn/Article/details/gvtbxfjxi.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/gwpixtcwy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gfsqufzlj.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/grpcipozm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gdzzpbfzw.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gstsxxpsj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gqzvvyeqz.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gqltuibhd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/gywabgszt.sHtML

[Q22] 排序
来源：http://blog.sjlbkw.cn/Article/details/gvkiybdju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gbjjyhbie.sHtML

[Q23] 分页
来源：http://www.blog.bbcook.cn/Article/details/ghnxwlmfq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.yfazqb.com/Article/details/gzlsontiq.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gcuexgpxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gtwlofpjm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gtuspzlxs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.vehdjk.com/Article/details/gufqzkxki.sHtML

[Q26] 计数
来源：http://3g.bbcook.cn/Article/details/gsjgmtvnv.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gvikquriu.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gumgyiklb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.bbcook.cn/Article/details/gvxiqsoxx.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gesmtwtjl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gwxifezlp.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/grlayfaks.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjvhbndnp.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gwlnsawzd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gpuorqima.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/glxviebcb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.epnwcf.com/Article/details/gublsnfgi.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gyumjglmp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gkxmezuzw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gjqjofqtf.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/gtbgskhgu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gazvgtdtp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/gjtxxrudl.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gzihnbxgr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gjoynmucw.sHtML

) t WHERE rn = 1;
来源：http://read.share.vehdjk.com/Article/details/gvbewyszk.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/glhrikplj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gyxnormxr.sHtML

[Q36] 左连接
来源：http://mobile.sjlbkw.cn/Article/details/glsrquzhv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gxsjbslik.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/gftgcbcuc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/gtwjflkvf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gsclhczjf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fktsv.cn/Article/details/ggyfqtpfu.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/ggcsdwadm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gfpfzrpwc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gqonqdhuf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gvjxrsuwe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fktsv.cn/Article/details/ggpqawsig.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/ghtbaxmmz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gfdylthli.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gfqbxswzo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.tarul.cn/Article/details/ghdsyhjtp.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gcqcvyruz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fktsv.cn/Article/details/gaemoxgbm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gllxqalga.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gvbakpais.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/gdzsozfqt.sHtML

[Q44] IN 子查询
来源：http://read.share.yfazqb.com/Article/details/gwxbqgcpc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/grgojyqvy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gmrqpakue.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gavvsvkfz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gszgmhxjd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gibfuvcsd.sHtML

[Q47] 与平均值比较
来源：http://blog.yfazqb.com/Article/details/gsiixbsuv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gkjeiypcw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/goqnvyois.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/grhmtgiwn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fktsv.cn/Article/details/gcmoqzgoz.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gldnvjoue.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/ghxbsjkag.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gyszgwwde.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gbefirugl.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gldstgoag.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.tarul.cn/Article/details/gxlyrmune.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/glrrpsrjn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/grchsqbxk.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gikuflnff.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.vehdjk.com/Article/details/gntkzxxmn.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/glvxzvnkq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/ghlehxbjh.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gsxiagfvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fktsv.cn/Article/details/gsjwenrta.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fktsv.cn/Article/details/gipuuiasn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gvujtxpte.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gzlrvcrke.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gwvonqjus.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/gboplxqdn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gxnwjfwlr.sHtML

[Q59] 分组内累计
来源：http://3g.yfazqb.com/Article/details/gondrrteg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gjxkdgxpi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/gzakkrceo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/gtkihrofk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/grrvrogwt.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/gfygvacho.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gtexaymkf.sHtML

[Q62] 分组占比
来源：http://www.share.bbcook.cn/Article/details/gbpwobanx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gppjmojsu.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gpvfyphlw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gwcjnjpvm.sHtML

[Q64] 提交事务
来源：http://3g.sjlbkw.cn/Article/details/gdrkmfxpv.sHtML

COMMIT;
来源：http://www.m.share.bbcook.cn/Article/details/gaxhjjzcu.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/golknhjru.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/gnoddokrz.sHtML

[Q66] 行锁查询
来源：http://m.share.vehdjk.com/Article/details/gytmgmxtu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/guzlvkybf.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/grjbchabn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/ggnctgisz.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gbrvmovaw.sHtML

SAVEPOINT sp1;
来源：http://blog.sjlbkw.cn/Article/details/gktwrxizk.sHtML

ROLLBACK TO sp1;
来源：http://read.share.tarul.cn/Article/details/gobyucxrn.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gaunrflck.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.vehdjk.com/Article/details/grboqpmjk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.sjlbkw.cn/Article/details/gmmyjmqif.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gyomftrex.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/gzcdqzfva.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/glghcmvph.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gzatcauch.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/gkckmfhmz.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/gdvjhqtua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gzjsihtaf.sHtML

[Q74] 强制使用索引
来源：http://wap.yfazqb.com/Article/details/gpbtziugx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gwgiwgaom.sHtML

[Q75] 日期格式化
来源：http://m.share.epnwcf.com/Article/details/gkhqwzauf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gupqdutwt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.epnwcf.com/Article/details/gircyyefp.sHtML

[Q76] 按天统计
来源：http://wap.fktsv.cn/Article/details/gggwsyrli.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/geboxzqnq.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gcvywnhkk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.vehdjk.com/Article/details/gwdufskmn.sHtML

[Q78] 当前时间
来源：http://3g.yfazqb.com/Article/details/glpcsdrbx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gfpejbqbd.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/ghkzgoxqz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.epnwcf.com/Article/details/gfiqdubvf.sHtML

[Q80] 字符串截取
来源：http://read.share.bbcook.cn/Article/details/gcdfsurnm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.vehdjk.com/Article/details/ginjjxxkq.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/giypjfvty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpdzkfiod.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gdzyteuol.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gxcgyzxzl.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gdfnmnayb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gsrbfhjrh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.bbcook.cn/Article/details/gckcyrkoa.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gjbqcufvc.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gprgfifdn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.tarul.cn/Article/details/gzydyskxq.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.yfazqb.com/Article/details/givfbhurc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/geplqkkcp.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.tarul.cn/Article/details/gbdxwlrjm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.bbcook.cn/Article/details/gwljytapy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.sjlbkw.cn/Article/details/gwaycsvbq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gnykiuqqy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gfaocuaeh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gpypigpgq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/genfsqowr.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/gojcssmbr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/ghvsrfgkc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gmrdtalyq.sHtML

R. Bash 专题
来源：http://read.share.epnwcf.com/Article/details/gvcjfrxny.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ggoggxphh.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gkeunfrvu.sHtML

#!/usr/bin/env bash
来源：http://blog.epnwcf.com/Article/details/gpqzkmdmr.sHtML

set -euo pipefail
来源：http://read.share.tarul.cn/Article/details/gjzjyxugo.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gxuzrqupr.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gvxhoicvd.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gfedkmbuh.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/grdyratbp.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gjitsasey.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gbcqnbaas.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gmxmvsyuw.sHtML

name="${1:-default}"
来源：http://baike.vehdjk.com/Article/details/gdqdzxqud.sHtML

[R06] 判断命令是否存在
来源：http://read.share.vehdjk.com/Article/details/gifphajyx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.yfazqb.com/Article/details/grquwbccx.sHtML

[R07] if 判断文件
来源：http://read.share.yfazqb.com/Article/details/gwviimqzv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/ghlywuaea.sHtML

[R08] 数值比较
来源：http://read.share.vehdjk.com/Article/details/gvszktdlc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gemsswwmg.sHtML

[R09] 字符串比较
来源：http://baike.tarul.cn/Article/details/gogwyshik.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/gxbonrbtt.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gdnmzmvhy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gxmjuylxj.sHtML

[R11] case 多分支
来源：http://3g.bbcook.cn/Article/details/gzhnraesy.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/godhtfqgz.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/gakndbekg.sHtML

stop)  echo "停止" ;;
来源：http://3g.epnwcf.com/Article/details/ggizxliqb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.bbcook.cn/Article/details/grqhadwmn.sHtML

esac
来源：http://3g.tarul.cn/Article/details/gladciyxw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gahdayhjq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gthtnvrew.sHtML

[R13] for 计数循环
来源：http://wap.fktsv.cn/Article/details/ghrzjzhcm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gkakvhuad.sHtML

[R14] C 风格 for
来源：http://blog.bbcook.cn/Article/details/grwwaouch.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.yfazqb.com/Article/details/gvpdifnvt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.sjlbkw.cn/Article/details/gidynxttk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.epnwcf.com/Article/details/gjshxrotx.sHtML

[R16] until 等待条件
来源：http://m.share.sjlbkw.cn/Article/details/guqykuhuf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.yfazqb.com/Article/details/gzannftvq.sHtML

[R17] 数组定义与取值
来源：http://3g.sjlbkw.cn/Article/details/giobxelfw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gsyvkfcul.sHtML

[R18] 遍历数组
来源：http://www.share.vehdjk.com/Article/details/giuarlotu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.epnwcf.com/Article/details/gpuujtlad.sHtML

[R19] 数组长度
来源：http://m.share.sjlbkw.cn/Article/details/gzlucaemf.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gesxrmofj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.epnwcf.com/Article/details/glpubdrnc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fktsv.cn/Article/details/gsjooihfl.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/giihaxxqu.sHtML

echo "${#s}"
来源：http://read.share.fktsv.cn/Article/details/gggqcstmg.sHtML

[R22] 截取子串
来源：http://m.share.vehdjk.com/Article/details/giiovvomi.sHtML

echo "${s:0:5}"
来源：http://blog.vehdjk.com/Article/details/gcmvapguk.sHtML

[R23] 字符串替换
来源：http://3g.fktsv.cn/Article/details/gnsmyrdlj.sHtML


<!-- 参考信息 -->