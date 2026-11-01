代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gusyferqe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/gqvcjnfdt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gdqnixiys.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gvbizwbbq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gnhomszfl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/gfeitptpx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.vehdjk.com/Article/details/gdfnzbzsv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gjjljwhfg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gveqshqkv.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/gnshhmitu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gwzznupvp.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gjqmrwujg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gjnaksqhn.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/geubrssvu.sHtML

[P07] 防抖与节流
来源：http://baike.fktsv.cn/Article/details/gconbfufu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gwytqapom.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gssnczxkf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.sjlbkw.cn/Article/details/gtuotusqz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/glnbhedxy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/goycydzxc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.vehdjk.com/Article/details/gflftktzg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.yfazqb.com/Article/details/gggbdwzla.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gtczgedbq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/gioymwzpg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgzkyhnn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.bbcook.cn/Article/details/ghxxevzxf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/gojbtbnsg.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gmamoyeog.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.epnwcf.com/Article/details/grkhbrvgo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.fktsv.cn/Article/details/gkmikgshl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fktsv.cn/Article/details/gfsroloyo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gzdzgikes.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gyhrhmwoh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/ggijhgpdi.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glhwxlhfa.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gnhhkuhzy.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/gcvnhybxr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gnbvnezqb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.yfazqb.com/Article/details/gfygjrncq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.vehdjk.com/Article/details/gsujuaroz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/grmkybpxn.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gjjsupqdv.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gcxysiwtr.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gmfhbmrpt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gpmdofchv.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gwpizptru.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gzjrdnmgm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.yfazqb.com/Article/details/gutghfnaq.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gboufviyj.sHtML

[Q03] 增加列
来源：http://www.blog.yfazqb.com/Article/details/grgotvrya.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gnicdoaov.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/giadtupvj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.vehdjk.com/Article/details/gqelwlwhr.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gfxfzyaps.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.epnwcf.com/Article/details/gqhidgard.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gbadtvesr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.epnwcf.com/Article/details/ghmhbgtre.sHtML

[Q07] 删除表
来源：http://www.share.tarul.cn/Article/details/gievzwfzo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gkociiqzs.sHtML

[Q08] 创建普通索引
来源：http://mobile.fktsv.cn/Article/details/gbizasrei.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gfsqfcizw.sHtML

[Q09] 创建唯一索引
来源：http://read.share.bbcook.cn/Article/details/gupttbqrr.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gstqwkokj.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gxcgtgdhh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gmnuuasfs.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.bbcook.cn/Article/details/gpohycait.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gjlyzgbkj.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/govuwmsvl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gvzhfehbf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/gkrivsvll.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/gbisrgybs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gwcawacqv.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gedjebtjv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gyzmwqvnt.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.yfazqb.com/Article/details/gqmfjnras.sHtML

[Q15] 查询全部
来源：http://read.share.epnwcf.com/Article/details/gizinyuep.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gczkkwkhj.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/ggokrchag.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gotoxgcyk.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/ghslhyvbb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gmugfyguy.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gkxjrycol.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gazwyhctu.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gitdmzuwa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gjoemwwlb.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/gojvobgkp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/gpzsebihm.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gktfiuqqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/gfobavieo.sHtML

[Q22] 排序
来源：http://www.m.share.fktsv.cn/Article/details/goqpetecq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gjzneulyw.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gcshptcrk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gplnvtegz.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gbybmzutc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gpfjxdxad.sHtML

[Q25] 只取前 N 条
来源：http://read.share.yfazqb.com/Article/details/gujphqwgm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.sjlbkw.cn/Article/details/gaoxhuxnp.sHtML

[Q26] 计数
来源：http://m.share.yfazqb.com/Article/details/gctejghtp.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/gdudumnvz.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/glxrzyobm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/gsnawdqzy.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gedsjrbxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gpfzsbvho.sHtML

[Q29] 最大最小值
来源：http://www.share.fktsv.cn/Article/details/gnnbrerfs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gaydxbjtz.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gfsjpjsxn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gjpmemmwk.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gmwilnmyk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.sjlbkw.cn/Article/details/gctswuobm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.tarul.cn/Article/details/gmurgslun.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gdoclpxrb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gbwcrhaia.sHtML

[Q33] 多列分组
来源：http://www.m.share.epnwcf.com/Article/details/gehcstenv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gfnqrtjli.sHtML

[Q34] 每组取第一条
来源：http://wap.vehdjk.com/Article/details/gqtdriopl.sHtML

SELECT * FROM (
来源：http://mobile.sjlbkw.cn/Article/details/gdnvixglk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/gghruycdj.sHtML

) t WHERE rn = 1;
来源：http://3g.epnwcf.com/Article/details/getlnstek.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/ghknzauas.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gyjhxgkrt.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gfzcrmzxo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gkfvujfoi.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gxdfrlupo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gzkjwubzo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.vehdjk.com/Article/details/gfmmlepag.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.yfazqb.com/Article/details/gfxouebjj.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gssoxgiyd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtdoxnhq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/gbsqavzdi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fktsv.cn/Article/details/gebyafrqv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gatndcoyz.sHtML

[Q41] 多表连接
来源：http://wap.tarul.cn/Article/details/gudtvruwt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gualymqvu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fktsv.cn/Article/details/gazqdigiu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gdmojhwia.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.bbcook.cn/Article/details/govclnhvl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gtsxwloje.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gewrrflze.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/gspzoxbdc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gafvvojvd.sHtML

[Q44] IN 子查询
来源：http://m.share.bbcook.cn/Article/details/grtxohryz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.epnwcf.com/Article/details/gwstsvumn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gidbajire.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gvadewlrf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.sjlbkw.cn/Article/details/gywqeqgeo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gawezcqua.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gefdxnfve.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/gtkskgilx.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.tarul.cn/Article/details/gzqyabakk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/gcvanlnja.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.sjlbkw.cn/Article/details/gdtwtiegg.sHtML

[Q49] 更新单行
来源：http://read.share.fktsv.cn/Article/details/ghxprobli.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gbqgygvwf.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/gijiupggs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gxmecakjb.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/gkpslxoja.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gbfdzhmrm.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gyiugcvcn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gwwbxhdjx.sHtML

[Q53] 按条件删除
来源：http://wap.yfazqb.com/Article/details/gepcmdmbx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gvgwrqapb.sHtML

[Q54] 清空表
来源：http://blog.epnwcf.com/Article/details/gakhwhatu.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gfrldreir.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gojhkvtww.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gkfioowow.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/ghvgcghds.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gfmbvhwpk.sHtML

[Q57] 行号
来源：http://read.share.yfazqb.com/Article/details/grpuznkpa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gkfrdlbhj.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gugyqhgyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gkoukoblk.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gvdprpxzr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gunzsudok.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gpshhimtj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gsdcddmmc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/govbliheu.sHtML

[Q61] 移动平均
来源：http://www.share.vehdjk.com/Article/details/gucbqncxy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gtpztbcok.sHtML

[Q62] 分组占比
来源：http://baike.fktsv.cn/Article/details/gerfqvroq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gnhlptrgc.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/gbtydudet.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gomyphbtm.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gplpmsana.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gihfyrtvm.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gjuqffeeg.sHtML

ROLLBACK;
来源：http://baike.fktsv.cn/Article/details/gruydhhzx.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gcnwoebae.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/gdckzttxl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gvtrrhebm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gcpvsojwc.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gpkwtdrmn.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gwyubhboi.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gjjxfgiub.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gfacwtztg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/gllsieodw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gdzkoispm.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gtlgaeula.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/galohwmjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gikzwopze.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gbxfbfigh.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gpgwlddim.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/goxsznukb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/gxtbemuuj.sHtML

[Q74] 强制使用索引
来源：http://www.blog.bbcook.cn/Article/details/gelxoaadd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.bbcook.cn/Article/details/gxejhdyuv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.epnwcf.com/Article/details/gbptngmxj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/ghingfaed.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.yfazqb.com/Article/details/gujfyrfqp.sHtML

[Q76] 按天统计
来源：http://www.m.share.vehdjk.com/Article/details/gxymiulhy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gpdtajsxn.sHtML

[Q77] 时间加减
来源：http://www.m.share.fktsv.cn/Article/details/gyqfhivgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.tarul.cn/Article/details/gxbjsyzle.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gxxomzwuk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/grnvwodzz.sHtML

[Q79] 字符串拼接
来源：http://3g.sjlbkw.cn/Article/details/gafvkipbv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gyokboxfg.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/gjuljjskm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gpbvjgits.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gfkvvehls.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnzbphixc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.epnwcf.com/Article/details/gettsbqyh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gstfjdmnz.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gntwdxgce.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/ggsiinhwm.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gaibpnpkm.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gaifhrqjs.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gtuklxmqw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.yfazqb.com/Article/details/gxsbdgmak.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gnjpwqazs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/gtoyzdjyp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gecxpvdzz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.tarul.cn/Article/details/ghsippjlv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.bbcook.cn/Article/details/ghkojcfwx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.tarul.cn/Article/details/gqlibrxng.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gfnjuocek.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gbzzogfyf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gljfqmjgt.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gbacqgtqj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/gcvywuqbm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbnzokisi.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/gkyarlimy.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gsihijyog.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/grgrhbbiy.sHtML

#!/usr/bin/env bash
来源：http://read.share.fktsv.cn/Article/details/gmfdmkgix.sHtML

set -euo pipefail
来源：http://read.share.bbcook.cn/Article/details/gpvzkhuyf.sHtML

[R02] 变量赋值与使用
来源：http://read.share.sjlbkw.cn/Article/details/gqnvadndy.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.epnwcf.com/Article/details/guuyvihpd.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gtwyfpkzj.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/ggbydpkek.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/gfxilcbkk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gcncjaztk.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/grbjacrzk.sHtML

name="${1:-default}"
来源：http://read.share.bbcook.cn/Article/details/gtktnfdsr.sHtML

[R06] 判断命令是否存在
来源：http://baike.tarul.cn/Article/details/giehrpnxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.tarul.cn/Article/details/gesydoiiq.sHtML

[R07] if 判断文件
来源：http://www.blog.sjlbkw.cn/Article/details/gdkotcjzz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.sjlbkw.cn/Article/details/giqovkojq.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gcbzvnysn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.vehdjk.com/Article/details/gglinemmy.sHtML

[R09] 字符串比较
来源：http://blog.sjlbkw.cn/Article/details/gejcnuqpt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fktsv.cn/Article/details/gohrfvzed.sHtML

[R10] 正则匹配
来源：http://read.share.sjlbkw.cn/Article/details/gtyaiqcia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fktsv.cn/Article/details/gaxhrooag.sHtML

[R11] case 多分支
来源：http://www.share.bbcook.cn/Article/details/gvvfmraus.sHtML

case "$1" in
来源：http://www.share.bbcook.cn/Article/details/gkydermnq.sHtML

start) echo "启动" ;;
来源：http://m.share.epnwcf.com/Article/details/gbqtgwybf.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/goyghtapg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.vehdjk.com/Article/details/gxfxilzmd.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gzpwjeyjh.sHtML

[R12] for 遍历文件
来源：http://blog.tarul.cn/Article/details/gmcnanwul.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gzgmasedo.sHtML

[R13] for 计数循环
来源：http://www.m.share.bbcook.cn/Article/details/gogjputrs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fktsv.cn/Article/details/gbolynndd.sHtML

[R14] C 风格 for
来源：http://read.share.epnwcf.com/Article/details/goeoswodo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.vehdjk.com/Article/details/gpvqywzla.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gxurtembc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/gikleabsh.sHtML

[R16] until 等待条件
来源：http://www.share.sjlbkw.cn/Article/details/gbcxyywjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/gluxfwgei.sHtML

[R17] 数组定义与取值
来源：http://wap.vehdjk.com/Article/details/ghnbwzfof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.vehdjk.com/Article/details/gqrqnnhuz.sHtML

[R18] 遍历数组
来源：http://read.share.tarul.cn/Article/details/gwcizkwwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gjbfyfzst.sHtML

[R19] 数组长度
来源：http://read.share.fktsv.cn/Article/details/gwsqgkwfe.sHtML

echo "${#arr[@]}"
来源：http://www.share.fktsv.cn/Article/details/gkgnsgfcg.sHtML

[R20] 关联数组（字典）
来源：http://www.share.tarul.cn/Article/details/gactjtlsr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.vehdjk.com/Article/details/gsdczhhtm.sHtML

[R21] 字符串长度
来源：http://www.m.share.tarul.cn/Article/details/gxydwdleo.sHtML

echo "${#s}"
来源：http://mobile.vehdjk.com/Article/details/guphnhjez.sHtML

[R22] 截取子串
来源：http://mobile.bbcook.cn/Article/details/gpvnijrew.sHtML

echo "${s:0:5}"
来源：http://baike.epnwcf.com/Article/details/gnyassakq.sHtML

[R23] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gtgjmczds.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fktsv.cn/Article/details/gvvqymirx.sHtML

[R24] 大小写转换
来源：http://www.blog.vehdjk.com/Article/details/gcdxatshw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.bbcook.cn/Article/details/grxgwlyji.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.yfazqb.com/Article/details/gvixiyhcq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.yfazqb.com/Article/details/guxlzjgqs.sHtML

[R26] 命令替换
来源：http://wap.tarul.cn/Article/details/giymebyhp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.bbcook.cn/Article/details/gmhqgfsxl.sHtML

[R27] 算术展开
来源：http://www.m.share.tarul.cn/Article/details/gxsvwerwx.sHtML


<!-- 参考信息 -->