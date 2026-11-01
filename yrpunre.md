代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gxgiazaah.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgrvyinz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gfgapnvvd.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/grjlwiser.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.epnwcf.com/Article/details/gpmnfkmhr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvorpykc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.tarul.cn/Article/details/guquehvae.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gqrboowyk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/guajqdaag.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gmkosjmrr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtqmptfad.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gmtoyjimm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/gqgteuplk.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/ggckaxbmr.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gjaxaasfa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gslbrfrhh.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/ghshoueyi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/guwdukkyp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gfqibaywj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gckxrjazv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gxuchfgnp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.yfazqb.com/Article/details/gajbnsbtb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gthygxoln.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gozyhfbfi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gmsphgvbx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.bbcook.cn/Article/details/ggaaixnma.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqhdwwjh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gzamdwyxj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/gpdmvzgew.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gkmkyybws.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gwqvppicr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/ghodcctrz.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gsregjskw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.epnwcf.com/Article/details/gvaiwlrua.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gnwfpixrz.sHtML

[Q01] 创建表
来源：http://www.m.share.vehdjk.com/Article/details/gawuwnjyl.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/ghlrfniwu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gbyzddzrs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/gxrxxstla.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gcekcakvu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.tarul.cn/Article/details/gkzvscjte.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/glusasbeo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gieqvufty.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/gfjfbyojs.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gbualdnzw.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gsdvmteuq.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gyrpulnhh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gayaqgwby.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/ggxvooaxr.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/gidsyuyte.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gnpslmxkr.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gmyxtgqly.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/govrmnigy.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gxjlvylyj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gakupsqza.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gwpvzjoop.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gmncsmrvk.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gqcsuropi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/gubesbskh.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gyirjrefn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gkgnrjsvz.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gbtrxbwrk.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gbkgqjvmc.sHtML

[Q10] 插入单行
来源：http://3g.yfazqb.com/Article/details/godopytcx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.bbcook.cn/Article/details/gcufqatmq.sHtML

[Q11] 一次插入多行
来源：http://m.share.tarul.cn/Article/details/gqgiubgeh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjqlludk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gatflfjfu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/godkvbncj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.bbcook.cn/Article/details/gpyvtixgu.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/girzgbbso.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gspbgcrwu.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/ginvdjcjj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gzuzufuun.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.bbcook.cn/Article/details/gwotjplnq.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gzwqsfhcz.sHtML

SELECT * FROM users;
来源：http://baike.bbcook.cn/Article/details/gadrrbjqg.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fktsv.cn/Article/details/gwjeeqsnc.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gmegrkrlc.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/ghkbdcuzf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gjgvezoyk.sHtML

[Q18] 模糊匹配
来源：http://m.share.tarul.cn/Article/details/gjygwxgsu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gygnkebue.sHtML

[Q19] 范围查询
来源：http://baike.fktsv.cn/Article/details/gxnwylacb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.tarul.cn/Article/details/gemtchprw.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gccwbmavb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/ghkelbsdi.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gfzxwyqgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gwbeejxtv.sHtML

[Q22] 排序
来源：http://baike.sjlbkw.cn/Article/details/gsqtscbbc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/ggwogovdg.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gmxthijri.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gbdcqbkty.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gntcdwwam.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpkuqvmnf.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gomubsduu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gtvjzjytz.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gtfsclrfi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gpvghqztp.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gyuyolrkf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/geavcvtjw.sHtML

[Q28] 求和与平均
来源：http://baike.epnwcf.com/Article/details/gsviwlcgi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/ggkfjcdlo.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gcqvapecc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gksbsbffh.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gbhwaznyt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gvljdrawg.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gybmrblux.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.vehdjk.com/Article/details/ggiacwpyi.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/guvtfjrgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/glynwrbhe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/ghvppzqvv.sHtML

[Q33] 多列分组
来源：http://wap.tarul.cn/Article/details/gymcfegyg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gjoneehsc.sHtML

[Q34] 每组取第一条
来源：http://blog.fktsv.cn/Article/details/gztpdsqby.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/gymngaoby.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/gfzeeqqjc.sHtML

) t WHERE rn = 1;
来源：http://baike.tarul.cn/Article/details/gastuarfg.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/gtoisbxxh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gbktkpbcn.sHtML

[Q36] 左连接
来源：http://mobile.vehdjk.com/Article/details/goisswzld.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gpwtwhdlx.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gqrdztpqv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaggwsowd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.epnwcf.com/Article/details/gugimeybg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.vehdjk.com/Article/details/gpvdvfgys.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/gojbhbadu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fktsv.cn/Article/details/gyrxxycww.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/glbjqecdi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.vehdjk.com/Article/details/grclqfsci.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/goloyhppr.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gwuxsjqsd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gztvspxjx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gvyqimmzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gizfejsgm.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fktsv.cn/Article/details/gsgfpdrpe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gltqqxbuq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.vehdjk.com/Article/details/gvshkjgcw.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gfxioalqb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gndmmrszu.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/ghlcirfzo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gemewdypk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/glxgmzshh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gmfexnebk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gtnifioov.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gjbwwthho.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/gwatgoobl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gplwectol.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.tarul.cn/Article/details/gxcjwpmoc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/ggqqvenne.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gdylfjing.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/gepllccsh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gtihzusyh.sHtML

[Q50] 批量更新
来源：http://blog.bbcook.cn/Article/details/gsmaanpfu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.sjlbkw.cn/Article/details/gmkkqpzdv.sHtML

[Q51] 用子查询更新
来源：http://mobile.vehdjk.com/Article/details/gnuccakgs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gvaufizwy.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gmdqglcqy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gnshyeoax.sHtML

[Q53] 按条件删除
来源：http://3g.fktsv.cn/Article/details/gqudxwzqe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.epnwcf.com/Article/details/gycrskszm.sHtML

[Q54] 清空表
来源：http://m.share.yfazqb.com/Article/details/gyjtfmkcg.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fktsv.cn/Article/details/gkxxsgplk.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gtwzsaojs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gnrpfhgkv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.sjlbkw.cn/Article/details/glrdtbpqk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gwhiijloo.sHtML

[Q57] 行号
来源：http://www.share.vehdjk.com/Article/details/gzqrvfcyy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gjuxyhlzi.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gzrcsdvek.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gzxphsinx.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/gimavvgpj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gfmycewgs.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gnfkrlhdx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/ghikqwptq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gwdesvlww.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gbqhrbpga.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gpeggxlyb.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gcifkmqvg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gvogsjdhj.sHtML

[Q63] 开启事务
来源：http://www.m.share.tarul.cn/Article/details/glxwnjbzv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fktsv.cn/Article/details/gsywjfkte.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gfqgxfxkg.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/genycsmtc.sHtML

[Q65] 回滚事务
来源：http://m.share.yfazqb.com/Article/details/gbmvhtycu.sHtML

ROLLBACK;
来源：http://www.m.share.vehdjk.com/Article/details/gebnvqkpq.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/ghbzbcrqx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gqjlblkgi.sHtML

[Q67] 设置隔离级别
来源：http://3g.bbcook.cn/Article/details/gwdleeaba.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gdzusnrge.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/gjzghagli.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gauzfgeqg.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/gmlelhcne.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/grlknbbcf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/gofitcthr.sHtML

[Q70] 更新统计信息
来源：http://www.share.vehdjk.com/Article/details/gmsuiuakb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.yfazqb.com/Article/details/gzthrmpre.sHtML

[Q71] 查看建表语句
来源：http://m.share.vehdjk.com/Article/details/gxvtwwpmt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.epnwcf.com/Article/details/gijrfysxr.sHtML

[Q72] 查看索引
来源：http://mobile.tarul.cn/Article/details/gwvmmxqgx.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gmlrhwojd.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gciixteeo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/golpvfybh.sHtML

[Q74] 强制使用索引
来源：http://baike.fktsv.cn/Article/details/gnovlwbaz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.yfazqb.com/Article/details/gjpbjveyu.sHtML

[Q75] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gljaibgif.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.bbcook.cn/Article/details/ghhhzvqug.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/ghqznkrdi.sHtML

[Q76] 按天统计
来源：http://www.m.share.yfazqb.com/Article/details/gubjbxafg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gquvoqexl.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/gztnzigut.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/gpsqbbfoy.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gwldnttgk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gftnypowa.sHtML

[Q79] 字符串拼接
来源：http://mobile.yfazqb.com/Article/details/gxwjegfut.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/gspvnjijx.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gojmzatao.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gxnreqmhk.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gnxhiqijw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.tarul.cn/Article/details/gjeqlqsge.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/gzaqsyouc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/ghaawbqhw.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gvojeyauc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/guyxhwsfz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gbvezbltd.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gjllvczoa.sHtML

[Q85] 数值取整
来源：http://3g.sjlbkw.cn/Article/details/gmuurwnal.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gejcqdyrp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gvlmqatzg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/gwkgjzlar.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/goszljfmf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gjjriijrj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.bbcook.cn/Article/details/gdswmtink.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/ganmxepjm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmaggpwtj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.epnwcf.com/Article/details/gmfiyogfd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gwsyvwpaq.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/glegosyns.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/gnglkaxbb.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmbxhtgge.sHtML

R. Bash 专题
来源：http://wap.fktsv.cn/Article/details/govzylhll.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvbnaoovo.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/gtupoxthl.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gasklzrdf.sHtML

set -euo pipefail
来源：http://m.share.bbcook.cn/Article/details/gthlcbdpy.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/grbegxyha.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fktsv.cn/Article/details/ggejydrug.sHtML

[R03] 只读变量
来源：http://www.blog.sjlbkw.cn/Article/details/gdlxqyusr.sHtML

readonly PI=3.14
来源：http://mobile.epnwcf.com/Article/details/gezeiowrk.sHtML

[R04] 位置参数
来源：http://read.share.sjlbkw.cn/Article/details/gpectfyzu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.sjlbkw.cn/Article/details/ggyhfsecv.sHtML

[R05] 参数默认值
来源：http://mobile.fktsv.cn/Article/details/gkirrownx.sHtML

name="${1:-default}"
来源：http://baike.bbcook.cn/Article/details/gdqktpqkn.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gkbfmbxkp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gharaufhl.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gbabdlpzd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.tarul.cn/Article/details/gcwvybiqi.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gkacsktif.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gaiqyqjrq.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gyhmsqjwq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.bbcook.cn/Article/details/gayxsmiut.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/gaytcjevl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.bbcook.cn/Article/details/gfsnqnllh.sHtML

[R11] case 多分支
来源：http://read.share.bbcook.cn/Article/details/gtulsqpyz.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/gydwtbtde.sHtML

start) echo "启动" ;;
来源：http://3g.tarul.cn/Article/details/gafpozjcg.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gbljtybdd.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gbehphxof.sHtML

esac
来源：http://www.m.share.sjlbkw.cn/Article/details/gmiecxqmz.sHtML

[R12] for 遍历文件
来源：http://baike.vehdjk.com/Article/details/gxomzrnry.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gzdrlcltf.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/gvuqsdxtt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gfcdlenvl.sHtML

[R14] C 风格 for
来源：http://www.share.epnwcf.com/Article/details/gauavsvyc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.bbcook.cn/Article/details/gqitfvyvg.sHtML

[R15] while 逐行读文件
来源：http://3g.sjlbkw.cn/Article/details/gknmfolua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fktsv.cn/Article/details/gkrgeesje.sHtML

[R16] until 等待条件
来源：http://www.m.share.vehdjk.com/Article/details/ggcjcikmo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gqqjglmho.sHtML

[R17] 数组定义与取值
来源：http://baike.fktsv.cn/Article/details/gawhoynvs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.tarul.cn/Article/details/gdnpnxous.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gqiebhzit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.bbcook.cn/Article/details/grvdjlpqq.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/gwtmwjjiv.sHtML

echo "${#arr[@]}"
来源：http://wap.fktsv.cn/Article/details/gdybsnvwg.sHtML

[R20] 关联数组（字典）
来源：http://read.share.sjlbkw.cn/Article/details/ghfoayzyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/ggtflsqgf.sHtML

[R21] 字符串长度
来源：http://baike.tarul.cn/Article/details/gwffhaidh.sHtML

echo "${#s}"
来源：http://m.share.fktsv.cn/Article/details/glbwrdlqi.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gfeelpaza.sHtML

echo "${s:0:5}"
来源：http://3g.fktsv.cn/Article/details/gvbhlpvmw.sHtML

[R23] 字符串替换
来源：http://mobile.fktsv.cn/Article/details/gpgrauljo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.tarul.cn/Article/details/gfoeweutg.sHtML

[R24] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gfbkebcgy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.bbcook.cn/Article/details/gqvxojtby.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.epnwcf.com/Article/details/gkgjssryy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.vehdjk.com/Article/details/gnmrhrprw.sHtML

[R26] 命令替换
来源：http://www.share.tarul.cn/Article/details/gycutnbjt.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.bbcook.cn/Article/details/gzhmhhmpy.sHtML

[R27] 算术展开
来源：http://3g.bbcook.cn/Article/details/gfcingbba.sHtML


<!-- 参考信息 -->