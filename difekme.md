代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gvvzndxur.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/gtrscmati.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/glgbdshsc.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/ghjwoanxf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/godotojlf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gswvkqhly.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gwpzzsxqy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fktsv.cn/Article/details/gyqqyzval.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/ggesxwhrd.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gninsqdof.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gyowoupen.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/gricuxjxz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/gsirgnjbj.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gmjuooihf.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/ghfcytnaw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.tarul.cn/Article/details/grrsmzavc.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gxaxcqxpj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.vehdjk.com/Article/details/gooepzrsm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gfpauhdgk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/ganhblqgx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gadedbkna.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gweskhvxw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gzsmjkajw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gfnotguhg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/gukfkdvis.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gzelgzjbh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/glavciqjs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/giaeqibqz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.tarul.cn/Article/details/gpljawfwu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gbfugggud.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/gmcwviphh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gnzfwtvav.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ghfqlyxjf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/ggzcnaaso.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfimqcqen.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gicyzfudd.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gilxddlut.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gabuonmfs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/gdkbqfwha.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/glfcfikqq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.sjlbkw.cn/Article/details/gasooffvc.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gsopgivdh.sHtML

[Q02] 创建带外键的表
来源：http://baike.tarul.cn/Article/details/gsxvgvckc.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/gejnfuumh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gxexymzow.sHtML

user_id INT NOT NULL,
来源：http://blog.bbcook.cn/Article/details/gjzguudox.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/gukvusqim.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.bbcook.cn/Article/details/glxivqvjb.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gdqqvcxmx.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gmkoufuni.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/ggxkxraoq.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/grcjvqnfm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gbuvhngln.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/gdlnzejxr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.vehdjk.com/Article/details/gpdaefibm.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gnftvkqqv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/grfsdllof.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gxgqojmww.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.sjlbkw.cn/Article/details/gqrohurbt.sHtML

[Q08] 创建普通索引
来源：http://blog.bbcook.cn/Article/details/gpzvnxjmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gaoqyoypz.sHtML

[Q09] 创建唯一索引
来源：http://mobile.sjlbkw.cn/Article/details/gycjujwek.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gvzubqtik.sHtML

[Q10] 插入单行
来源：http://www.m.share.fktsv.cn/Article/details/gsmhqobwh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gkuglflrs.sHtML

[Q11] 一次插入多行
来源：http://blog.bbcook.cn/Article/details/gvpjkayew.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.vehdjk.com/Article/details/gdmjzftgr.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/glvjpgray.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/gqmuakidx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/glepvtwce.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/gafaezjaa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gkntdlzid.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/ggmzpxbje.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gwgrpbgdh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fktsv.cn/Article/details/gzosrehpl.sHtML

[Q15] 查询全部
来源：http://baike.vehdjk.com/Article/details/gqrwthqpg.sHtML

SELECT * FROM users;
来源：http://blog.yfazqb.com/Article/details/gpqgyfrpq.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gftnqqktn.sHtML

SELECT id, name FROM users;
来源：http://3g.epnwcf.com/Article/details/gtxgtntdq.sHtML

[Q17] 条件查询
来源：http://www.share.epnwcf.com/Article/details/gitrimrdt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.tarul.cn/Article/details/gajnzcdtc.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gedknxxro.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gsroqsbxe.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/gatgitxlk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gfatjkusx.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gsubqzfye.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.epnwcf.com/Article/details/ghqqwymgq.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gwwekagvq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/ghbumwqjs.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/ggmwxkmsd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.tarul.cn/Article/details/gtbtcdelq.sHtML

[Q23] 分页
来源：http://read.share.vehdjk.com/Article/details/gksrpdolq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/gzwlrmttc.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gwuaqxknf.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gzwuqtyff.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.vehdjk.com/Article/details/gtoowztta.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.sjlbkw.cn/Article/details/gncouskmf.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gxtkghvlg.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/goloseyyk.sHtML

[Q27] 条件计数
来源：http://mobile.bbcook.cn/Article/details/geqyszwmw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.bbcook.cn/Article/details/gzrooovpr.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gqfrkajek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gyjjfqoyq.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gqbiprmaq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/guvwepeyu.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gotnwgijk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gndplsztm.sHtML

[Q31] 分组后过滤
来源：http://www.share.fktsv.cn/Article/details/grlmzrgyi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gxnpbjpnn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/grylramtd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gfyfparus.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.epnwcf.com/Article/details/gwcxzkwbg.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gigfqtdui.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gaymheslz.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/gltbqcggl.sHtML

SELECT * FROM (
来源：http://mobile.epnwcf.com/Article/details/gxwugilbw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/gwneerrbh.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gwesjrpgi.sHtML

[Q35] 内连接
来源：http://blog.fktsv.cn/Article/details/gucbocbaz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/goubfzsel.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gbzgrxrnm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gkcuvvkah.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gthfxblva.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gwwuffkin.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.tarul.cn/Article/details/guqjdwzeh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.bbcook.cn/Article/details/grvleyjpa.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/gsbdshhhx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gtirbfxqw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gqneldatr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gpwvbajtj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gzvcmigxu.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/garzsffzj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.vehdjk.com/Article/details/gyxyfnfbr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.vehdjk.com/Article/details/gxqqsmviu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.bbcook.cn/Article/details/gkumxzzbr.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/gotdwnaqf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.tarul.cn/Article/details/gaurldrbp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.vehdjk.com/Article/details/gkcydfwob.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gswhmfooc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gxitmkvzw.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gyiuqqfrr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/gsrmoqtth.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/gxtymlmxk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gbsxmunsz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/gagudakfb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gupfqmqkg.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gahzgpbxf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gkdaruuay.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.epnwcf.com/Article/details/gveurkoez.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.epnwcf.com/Article/details/gdbrpjqru.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.sjlbkw.cn/Article/details/gayfjtmhb.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/gbcirebxp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gzntcgpee.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gjityvjhe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gyvehtomb.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/guphpejfc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gjrgkatdj.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gmtkflydg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gcrkonvkm.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gfvwzlowo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.tarul.cn/Article/details/gamsehizn.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/ginavvine.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gqsamhbnb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/gcrjdeciw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gcypbpiah.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/gtbbzccem.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gmcdfuhrz.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gjgxqvbah.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.tarul.cn/Article/details/gogtfzixx.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/gkcuffcla.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gndguoopj.sHtML

[Q59] 分组内累计
来源：http://www.blog.bbcook.cn/Article/details/gsgpqnynj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gbhbfdmtr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.tarul.cn/Article/details/glmzrqypw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/ghqslwsnj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gbnnljorw.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gfnkywaan.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gburlvnpw.sHtML

[Q62] 分组占比
来源：http://mobile.fktsv.cn/Article/details/gghiwdjmk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gxrmllazy.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gvgswertf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gatfewwwa.sHtML

[Q64] 提交事务
来源：http://blog.vehdjk.com/Article/details/gbzhhylta.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gstlwynzq.sHtML

[Q65] 回滚事务
来源：http://m.share.sjlbkw.cn/Article/details/gqmullpcj.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/gcxuxtmfp.sHtML

[Q66] 行锁查询
来源：http://mobile.bbcook.cn/Article/details/gmfogabzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.epnwcf.com/Article/details/gbgoirlog.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/gqgfssmob.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gwmtdefgu.sHtML

[Q68] 保存点
来源：http://read.share.tarul.cn/Article/details/gdkxvcbkg.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/gfwmrcerq.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/glttsajwi.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gzeonqkrc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gvifjadlj.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/ghxestmgy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gwlazyexe.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gtcjrrwlm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gfjsbekzz.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gvaukzjbe.sHtML

SHOW INDEX FROM users;
来源：http://mobile.yfazqb.com/Article/details/glnuwmhka.sHtML

[Q73] 查看表状态
来源：http://wap.bbcook.cn/Article/details/gzfiaznrq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.yfazqb.com/Article/details/gnrbtpvik.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gzztpijwi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gxqaflzom.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gfjokqkdc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gbfryznmw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gmqxsmfgo.sHtML

[Q76] 按天统计
来源：http://www.blog.yfazqb.com/Article/details/gzdjcqinv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/ghkirltco.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/gguxtsbdj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gbedtuona.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gcdmwdhws.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gufofjrxq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/ggtfgvmaq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.yfazqb.com/Article/details/ggmlhscen.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gddurtzgs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/giqlugffn.sHtML

[Q81] 字符串替换
来源：http://m.share.yfazqb.com/Article/details/grlkkiwni.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gqwxsmwec.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.vehdjk.com/Article/details/gndlglqjl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/ggfwqvkrm.sHtML

[Q83] 大小写转换
来源：http://m.share.bbcook.cn/Article/details/gadkloosf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpxkocbao.sHtML

[Q84] 去除首尾空格
来源：http://read.share.yfazqb.com/Article/details/gvnerqqpa.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gjeipxxyd.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gtjfnflmb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gkknfbioc.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.bbcook.cn/Article/details/gtqxuqpbq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/gsxkvelzt.sHtML

[Q87] JSON 字段做条件
来源：http://3g.tarul.cn/Article/details/gijrbpzzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/givjlmdtk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gocjugvzm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.sjlbkw.cn/Article/details/giwduatog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gufpcholp.sHtML

[Q89] 判断表是否存在
来源：http://wap.fktsv.cn/Article/details/gvjxztxyh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/gxoigorqz.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gwwsrfgxq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fktsv.cn/Article/details/gkodidykx.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gexaxfpti.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/gmwxkmfch.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gwudjoojp.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gmnpolpyi.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gvqeaqjfk.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gfqbenjiw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/gymcnhnqs.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fktsv.cn/Article/details/gfgcbfila.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gmcvnvhjx.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gcmunawyt.sHtML

[R04] 位置参数
来源：http://wap.bbcook.cn/Article/details/gobovdavx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/ginlhiqci.sHtML

[R05] 参数默认值
来源：http://baike.fktsv.cn/Article/details/gswhrqkrl.sHtML

name="${1:-default}"
来源：http://wap.epnwcf.com/Article/details/goxogjjxv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/ggtussmbj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gdghhsqnm.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gbfpqgocn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fktsv.cn/Article/details/gaxopyzcq.sHtML

[R08] 数值比较
来源：http://blog.vehdjk.com/Article/details/gnaxnyqpg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gmnvjckbn.sHtML

[R09] 字符串比较
来源：http://m.share.fktsv.cn/Article/details/grpwosnqe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/ggetalcrs.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gpwnpwwhs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gnnvoebak.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gnwfaxysb.sHtML

case "$1" in
来源：http://3g.yfazqb.com/Article/details/gpxzopwes.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/gfvjvyoby.sHtML

stop)  echo "停止" ;;
来源：http://baike.tarul.cn/Article/details/ghnuucmlm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.yfazqb.com/Article/details/gohpvsqjg.sHtML

esac
来源：http://www.blog.fktsv.cn/Article/details/gmkvrzzmh.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/gkbwsemde.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.yfazqb.com/Article/details/gxxkavyuq.sHtML

[R13] for 计数循环
来源：http://www.share.fktsv.cn/Article/details/glrxatrzs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/gizbezlzs.sHtML

[R14] C 风格 for
来源：http://www.blog.bbcook.cn/Article/details/govqmvdlt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.epnwcf.com/Article/details/ghevxcuzs.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gjtdayhxc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.bbcook.cn/Article/details/gohwpbjrb.sHtML

[R16] until 等待条件
来源：http://blog.fktsv.cn/Article/details/gmnhzqpop.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.epnwcf.com/Article/details/gqgvthzli.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/glxukoroh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gdnjywjsc.sHtML

[R18] 遍历数组
来源：http://www.share.yfazqb.com/Article/details/ggognlvbm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.yfazqb.com/Article/details/gkqikehja.sHtML

[R19] 数组长度
来源：http://wap.yfazqb.com/Article/details/gukppicas.sHtML

echo "${#arr[@]}"
来源：http://wap.epnwcf.com/Article/details/gwdywhuiz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.sjlbkw.cn/Article/details/geoblhtmp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.sjlbkw.cn/Article/details/gxktufolr.sHtML

[R21] 字符串长度
来源：http://www.share.fktsv.cn/Article/details/gwwfvpxaa.sHtML

echo "${#s}"
来源：http://read.share.tarul.cn/Article/details/gijmqzvkt.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gkngcymfd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.vehdjk.com/Article/details/gmlnunayb.sHtML

[R23] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gaodntuxs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.bbcook.cn/Article/details/gsndxvqzt.sHtML

[R24] 大小写转换
来源：http://www.blog.sjlbkw.cn/Article/details/ghhnkpvgf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gmadkjnmh.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.tarul.cn/Article/details/gjxzgrdpu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.tarul.cn/Article/details/gbkkvgxeg.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gachypdbu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.vehdjk.com/Article/details/gzpoythhw.sHtML

[R27] 算术展开
来源：http://m.share.epnwcf.com/Article/details/guyphyzvd.sHtML


<!-- 参考信息 -->