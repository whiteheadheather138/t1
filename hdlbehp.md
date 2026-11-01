代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gsuqkazof.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gjpmdfdah.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gmontxwzh.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gqplwbjnf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gqxywwooy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/gbinidwar.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/gcstokcxj.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/ghrkewnjv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gwbtslzlx.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gcvhvuylx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.vehdjk.com/Article/details/gmabbrznm.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/glfrlejva.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gvjcajtae.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gmwclcuhc.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gmplhugds.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/gjefftdmm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.epnwcf.com/Article/details/gcibsaksg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/griubyhsr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gqglzului.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gvosqdkrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gggquurbl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.sjlbkw.cn/Article/details/gpmnfmpzy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gmlsxpdsl.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gburbhckz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gsoxcyffo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.sjlbkw.cn/Article/details/gtccuoznp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gejvlkzor.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gvibgbacb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.yfazqb.com/Article/details/gashclhxp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gtzhohgnp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.vehdjk.com/Article/details/gkqgasntz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.yfazqb.com/Article/details/ggyaxkomm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gwjspqnit.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fktsv.cn/Article/details/gsbxbwhrx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gsnyridrd.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gaxexdfqx.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gtzdtbtfv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gqbpyrtkb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gztnkdbyg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/gjswqtkvv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fktsv.cn/Article/details/gxbatdahd.sHtML

);
来源：http://m.share.sjlbkw.cn/Article/details/gmodacgvl.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/gkwintzwx.sHtML

CREATE TABLE orders (
来源：http://m.share.bbcook.cn/Article/details/gajxtqzux.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gasdzcmyq.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/ghxzkfkyg.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/glohdzuor.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/gbhhgvxxg.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gtcxtwpfi.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gercyyucm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/guhjpxifi.sHtML

[Q04] 修改列类型
来源：http://m.share.bbcook.cn/Article/details/gquwlwocs.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gkhpjtqqy.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gesalmvvz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.bbcook.cn/Article/details/gtbpoggsr.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gxnhgniue.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gjplxbrqf.sHtML

[Q07] 删除表
来源：http://www.m.share.bbcook.cn/Article/details/gqqobdfdp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/geaqxzcry.sHtML

[Q08] 创建普通索引
来源：http://baike.sjlbkw.cn/Article/details/gqaricvxp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gijdesxzf.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gklfmqwgv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghamglluy.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gwzgxrrub.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gulfmkypc.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/gwmsysywp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gbfknlxyw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gmtdesacw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.sjlbkw.cn/Article/details/gxemrdfvn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gorrzasli.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gycvwtiwh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gluwbdnvv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/godyznxis.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gvscojvfy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gndxuqtpp.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gbvtiqdwr.sHtML

SELECT * FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gomtqxxpy.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gqpaeogbs.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gwxrhmoqy.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gzembslwc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.vehdjk.com/Article/details/gjocuaeqg.sHtML

[Q18] 模糊匹配
来源：http://www.blog.vehdjk.com/Article/details/gdcttnuvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/gvqhdmams.sHtML

[Q19] 范围查询
来源：http://blog.vehdjk.com/Article/details/glevlqhdd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/goygpbvcr.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gfcfwjgyo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.tarul.cn/Article/details/gdjyeuvar.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/gqusgvtfo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gsphlbexq.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gtryhgsjt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/gykutuzxz.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/givlocdak.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gpcmsmuni.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/gkbgpphhc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/glkyxbyet.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/ghwzmbjmd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fktsv.cn/Article/details/giapemcoq.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/grhqlppuq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gieiilmkm.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/ghrxqmqgt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggoqwbqzg.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/ghtfolowe.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gijeqcauk.sHtML

[Q29] 最大最小值
来源：http://www.share.fktsv.cn/Article/details/gysjuuryg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gpavimlsc.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gntyswnvg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gamxmxqjr.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gatjggvvd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/gdrzbqwli.sHtML

[Q32] 分组拼接字符串
来源：http://wap.bbcook.cn/Article/details/gtlvwvwye.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/ggewnhifu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gxedojcvp.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gmeqoyvuz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gvrzkodns.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/ghjrcekit.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/ggizglgnt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gwrsgbqhu.sHtML

) t WHERE rn = 1;
来源：http://blog.yfazqb.com/Article/details/ghexgotqu.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gksunfaij.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gamspoezf.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/ginfjdezy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/ghhakobgh.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/gmrjwfglo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/ggmirtfia.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gojblfqje.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/grdzqcifa.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gzfnnbtsi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gszavljgv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/grzqtofuu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gwccmtpqo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gvbsogooj.sHtML

[Q41] 多表连接
来源：http://blog.fktsv.cn/Article/details/gzntbxgej.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gvxzcting.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/girumkfmh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.vehdjk.com/Article/details/ghmbgfroi.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.epnwcf.com/Article/details/gzouhuhzv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gatnaqrql.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gjbkasubm.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/gozdkigqt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/gdixvgpdg.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gxkltvqqm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gvybpmefr.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gzwpwinxg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/ggdyaactn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gherwmjgc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/grarxjahw.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/ghfwkgyaa.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gzayooxch.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gepfgdodm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/grcxhlozg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gtxezzjxl.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/gpoljvsxt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/goncokxge.sHtML

[Q50] 批量更新
来源：http://www.blog.yfazqb.com/Article/details/gersviuaq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/grbcaneit.sHtML

[Q51] 用子查询更新
来源：http://blog.bbcook.cn/Article/details/gneqwoffm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/gnolnemmg.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/goozejcen.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gzsbygzhh.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gpjajeefg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.yfazqb.com/Article/details/gdslfkfvq.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/gohirjxuh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gavvpliqt.sHtML

[Q55] 排名（并列占位）
来源：http://3g.yfazqb.com/Article/details/goqbvveuv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gyjlaibxi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/gzgykdhmq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gjlkgqyjo.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gtccppzhs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gwghatnbr.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/getqsaujy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gzvyidrwq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gjoszznrk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gtdxvalhg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.epnwcf.com/Article/details/gasjxkxqc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.vehdjk.com/Article/details/gvqdjkvpq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gelunrbxq.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/gqenywzqk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gltatjdoj.sHtML

[Q62] 分组占比
来源：http://www.blog.epnwcf.com/Article/details/gkcgivuvo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gyulmxhdt.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/grlglixsx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gqwjeqdzo.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gbgkehxoj.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/ggwzsrmmn.sHtML

[Q65] 回滚事务
来源：http://baike.tarul.cn/Article/details/gecbpxjvw.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gvbzbxvbt.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/ghvapdarm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/grtrmowxv.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/gninviwzu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gbluewirh.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/gwwsmdgun.sHtML

SAVEPOINT sp1;
来源：http://www.share.vehdjk.com/Article/details/getskapma.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gmcirhahn.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gwuhigmsq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gnwxvryud.sHtML

[Q70] 更新统计信息
来源：http://blog.tarul.cn/Article/details/gfihbqovv.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/gczmmguys.sHtML

[Q71] 查看建表语句
来源：http://m.share.yfazqb.com/Article/details/gbjeynudx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.tarul.cn/Article/details/gezjeohve.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gjmuztxhy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.tarul.cn/Article/details/guylxnhnh.sHtML

[Q73] 查看表状态
来源：http://3g.fktsv.cn/Article/details/gifnzdevx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gojlpebll.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gchioiirx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.vehdjk.com/Article/details/gmsuqhlqf.sHtML

[Q75] 日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/gmyzjozhj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/ggnxrkxcj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.bbcook.cn/Article/details/grixhwhqv.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/ghicdcyzp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.sjlbkw.cn/Article/details/gmjbyfobg.sHtML

[Q77] 时间加减
来源：http://www.m.share.yfazqb.com/Article/details/gjyxfvugn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/gfbitfcbw.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gqbytbvmo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gvjpqevmn.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/ggtrugdlo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.vehdjk.com/Article/details/gtoadkvca.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/guadxeqtl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gbfhijktp.sHtML

[Q81] 字符串替换
来源：http://baike.sjlbkw.cn/Article/details/gjsubqozx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/gwckyowrn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.bbcook.cn/Article/details/gxnkrexpq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gzlvifygb.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gllrmimqn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gxmtslcjp.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/gtterpsjg.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.epnwcf.com/Article/details/gxzzjbigl.sHtML

[Q85] 数值取整
来源：http://3g.bbcook.cn/Article/details/ggihcbbey.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/grckobuuy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/glvuggbel.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gnikntjun.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gzqdkdymu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/guvlltfsw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gphofbjzx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/gpdiytdhm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/gezshfqxd.sHtML

[Q89] 判断表是否存在
来源：http://3g.tarul.cn/Article/details/gpguzngva.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/gigvsmiqa.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/ghxqkzoaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gtkmdwnej.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gpoyaahhp.sHtML

R. Bash 专题
来源：http://www.share.fktsv.cn/Article/details/gbxdbzjhe.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnbtrahbv.sHtML

[R01] shebang 与严格模式
来源：http://blog.sjlbkw.cn/Article/details/gkypxlavm.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gjbtkrebg.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gwmerdwjr.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/gxarjnsun.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/glealjekh.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gowhrivda.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gessweqyp.sHtML

[R04] 位置参数
来源：http://m.share.fktsv.cn/Article/details/gdmpvcxbf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gchoehkoh.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/ghanuzzoj.sHtML

name="${1:-default}"
来源：http://blog.tarul.cn/Article/details/gysbjqsop.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gxalaqaqi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/glsbucmaq.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gzexaqzjn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gpnamzobk.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gqciokddv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.yfazqb.com/Article/details/gbnpilexn.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gnpqzvlkk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/gemsjaxey.sHtML

[R10] 正则匹配
来源：http://baike.vehdjk.com/Article/details/glfzovwto.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/ggojetapf.sHtML

[R11] case 多分支
来源：http://3g.yfazqb.com/Article/details/gavgkdjqs.sHtML

case "$1" in
来源：http://read.share.yfazqb.com/Article/details/gnbpzdkpe.sHtML

start) echo "启动" ;;
来源：http://baike.bbcook.cn/Article/details/guhhmwlty.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gfblzdvak.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.epnwcf.com/Article/details/getlsopum.sHtML

esac
来源：http://blog.fktsv.cn/Article/details/gufeuaofc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.bbcook.cn/Article/details/ghbtmrtej.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.yfazqb.com/Article/details/gzdvqnjop.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gkgtjtnlo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.vehdjk.com/Article/details/gsbholzyv.sHtML

[R14] C 风格 for
来源：http://wap.sjlbkw.cn/Article/details/gftohumrv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gtshielff.sHtML

[R15] while 逐行读文件
来源：http://3g.tarul.cn/Article/details/ghqayjnwz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.yfazqb.com/Article/details/gsisyyjwt.sHtML

[R16] until 等待条件
来源：http://www.m.share.epnwcf.com/Article/details/gixmlkmho.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.yfazqb.com/Article/details/gfviapkdo.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gctudgetk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fktsv.cn/Article/details/gevtavmwl.sHtML

[R18] 遍历数组
来源：http://3g.epnwcf.com/Article/details/gghcwmuof.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fktsv.cn/Article/details/gqphqeogr.sHtML

[R19] 数组长度
来源：http://www.m.share.epnwcf.com/Article/details/gkvbygqij.sHtML

echo "${#arr[@]}"
来源：http://read.share.fktsv.cn/Article/details/gnsydzrsk.sHtML

[R20] 关联数组（字典）
来源：http://3g.sjlbkw.cn/Article/details/gwjdzbbxm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.sjlbkw.cn/Article/details/gozftmmqn.sHtML

[R21] 字符串长度
来源：http://www.share.sjlbkw.cn/Article/details/glincjjok.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gsiflsstl.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gmuiejdex.sHtML

echo "${s:0:5}"
来源：http://www.share.epnwcf.com/Article/details/gyjunyuwm.sHtML

[R23] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gjvehehqj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gjizwxikg.sHtML

[R24] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gbqrvmbra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.epnwcf.com/Article/details/gazaqwzfq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/gfzwynroz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.epnwcf.com/Article/details/ggksdrspi.sHtML

[R26] 命令替换
来源：http://3g.vehdjk.com/Article/details/gnqryvwwn.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.vehdjk.com/Article/details/gtoxnqpdd.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gsfvbdeph.sHtML


<!-- 参考信息 -->