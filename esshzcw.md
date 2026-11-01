代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gdelijytd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gfbqfnbmp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gxmurfqrr.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gxchapqmj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/gwczhipja.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gvtodnidd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gyumobhya.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gxmkokzse.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gscryopaq.sHtML

TS:   if (x == null) {}
来源：http://blog.fktsv.cn/Article/details/gwznymudd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gwwxnyfhy.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gtbwrhwne.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/gbpbuzrbw.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gopuhpleq.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/ghetamujj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gmsduwjyo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/guamoqlza.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/ggflijosw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/ghmhxbjvk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gpnmwffwp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gkipqgdkr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.epnwcf.com/Article/details/grdhrrxoq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gnkzbgjrh.sHtML

[P08] 处理浮点精度问题
来源：http://baike.sjlbkw.cn/Article/details/gcakglaxr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gojmqmbyb.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.vehdjk.com/Article/details/ghzdeotpd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.bbcook.cn/Article/details/gvlnklqnx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.epnwcf.com/Article/details/gxbxezdii.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/gipkyorlj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/gpmmomxes.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gasmljycd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/glpirpvlz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gshhmcemz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.vehdjk.com/Article/details/gnwakftmf.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ghivtqkej.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gjuaksnoy.sHtML

CREATE TABLE users (
来源：http://www.m.share.vehdjk.com/Article/details/gkpquwuni.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/ghofwvneq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gwnnanbcv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/glldjypim.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gcqtnjpbc.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gutsejulj.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gfusvrwtv.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gaevkyhwm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/ginzjcatn.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gzamvfewz.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gdhzkuiip.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gyddggvel.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/ggtfdicpp.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/glddlcfvs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.tarul.cn/Article/details/gsgjlibcs.sHtML

[Q04] 修改列类型
来源：http://www.blog.epnwcf.com/Article/details/gxjtogfif.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/goqdenjef.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gzjmdoukq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.yfazqb.com/Article/details/gnthgehge.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gybmqsoii.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gnopusest.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gpybhchcf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gizogxouc.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gapilwngv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/ghnioopsz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gpjsflukh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gflgytbfd.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gbvxjkzzn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fktsv.cn/Article/details/gwmfegrti.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gzosjgtxl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gxagjpeic.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gkhxzjgai.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gjhcsdzhi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gxjvapluq.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/godwdjrwf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gslqkoinx.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/gnztbdvyb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gczamfhwc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.bbcook.cn/Article/details/gnvwvrimy.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gmclxilhn.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/gvladqznd.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gfhfxirvp.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gtalspmqq.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gluykpzba.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.yfazqb.com/Article/details/grixdtuvu.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/grfjulamo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gsnmaqxce.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gdyhyfxzw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.epnwcf.com/Article/details/gswybpdmn.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gabycxvej.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkizwhqf.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gdicqoceg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gsiurpdln.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gxncptwyv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gpjurnkiu.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/ghmzsgnmo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/giceuymtx.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gqeabhaqa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gihgiwumk.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fktsv.cn/Article/details/gdqwnrpmz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gskvmkyuq.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gmrgiqyke.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/gkxdgjtrx.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gljnbuzbd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gftkakfab.sHtML

[Q28] 求和与平均
来源：http://baike.tarul.cn/Article/details/gubqlpttl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gpacqoflr.sHtML

[Q29] 最大最小值
来源：http://blog.bbcook.cn/Article/details/geefoxghe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gnwghknvz.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gdcqjqwwl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gfozjxtsp.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gzubufcpt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gvesgbnwc.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.yfazqb.com/Article/details/gjxrbjryc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/glohrwwbu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gsfhbhlmn.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gfcnorpul.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gkqcamneq.sHtML

[Q34] 每组取第一条
来源：http://3g.epnwcf.com/Article/details/gpcynqtay.sHtML

SELECT * FROM (
来源：http://m.share.epnwcf.com/Article/details/gjjjsggtc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/govxcxdil.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gwbjxwufg.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gjoejnwcd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gfitrybmp.sHtML

[Q36] 左连接
来源：http://m.share.tarul.cn/Article/details/gimwuawms.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gggquvkzp.sHtML

[Q37] 右连接
来源：http://www.share.sjlbkw.cn/Article/details/ggtrqrjpx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/guclgwhxh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gyxynfdvh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gxhdtbojr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/ghlknisay.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.sjlbkw.cn/Article/details/gpeodugwc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.bbcook.cn/Article/details/grfkwquws.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gtwsdtzcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gmlgwekkr.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gytibffng.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gdguwnhdl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/goaexnvzk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/gstlibdwb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gejlxydge.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.tarul.cn/Article/details/ggrqpeaad.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fktsv.cn/Article/details/gykmzdnho.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gcjmzniez.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/grvefiwyq.sHtML

[Q44] IN 子查询
来源：http://3g.epnwcf.com/Article/details/gykjwegrk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/gstnolucx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/grhjnafvp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gemwoepvn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/glxavyqwz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/guwebajic.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gsuhqyepm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/geyibabtf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gqpiozqit.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gxwmofevq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.epnwcf.com/Article/details/girbllhiy.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/gphellggu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fktsv.cn/Article/details/gpzfcgedg.sHtML

[Q50] 批量更新
来源：http://www.share.yfazqb.com/Article/details/guylgxhyu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gztyntcyb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/geochrpbi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gfnudzfrf.sHtML

[Q52] 删除指定行
来源：http://mobile.bbcook.cn/Article/details/gtyzqmugo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gyttjccgx.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gouscvhhn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gvpjxyypw.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gdoswxbrx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gogiddhxm.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gjikbycri.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/giadmgbzl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gigwpfscp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/ghqsnvlub.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gxlcjqmvd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gaennbccb.sHtML

[Q58] 累计求和
来源：http://baike.bbcook.cn/Article/details/gxtivvmvb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gqlzscxut.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/gvzndsafi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gnbdmpjqd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gxyvpapsa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.sjlbkw.cn/Article/details/gsubhndqq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gflbzweqh.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gmdqlriep.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gygqwwskh.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/ginjqlmho.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gzzrssfhl.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gvncdzplr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/ghqeeuyds.sHtML

[Q64] 提交事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gpagcmwfe.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gpbusclco.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fktsv.cn/Article/details/gnjuidwih.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gasnivcjs.sHtML

[Q66] 行锁查询
来源：http://blog.vehdjk.com/Article/details/gvwbjjxtp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.tarul.cn/Article/details/gkpngumhd.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/ginedtbov.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gnghhygpt.sHtML

[Q68] 保存点
来源：http://m.share.sjlbkw.cn/Article/details/gxhnhneko.sHtML

SAVEPOINT sp1;
来源：http://www.share.epnwcf.com/Article/details/gkuthufqs.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gdvsnsvel.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/geqlzfaty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.bbcook.cn/Article/details/gmfcaahio.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gcsnskgqg.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/gmdgdemqt.sHtML

[Q71] 查看建表语句
来源：http://m.share.epnwcf.com/Article/details/gkkvhhcfm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.yfazqb.com/Article/details/gfajshmcv.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gbflgudvw.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gxutadszn.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/goyuqjtpx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gtruffcpf.sHtML

[Q74] 强制使用索引
来源：http://www.share.fktsv.cn/Article/details/gnjqxehlu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gvvidgcoq.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gntyiicbr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gesmsidxu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.sjlbkw.cn/Article/details/gnqvzmlea.sHtML

[Q76] 按天统计
来源：http://m.share.sjlbkw.cn/Article/details/gddgvifkt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/ggmecwsco.sHtML

[Q77] 时间加减
来源：http://read.share.bbcook.cn/Article/details/gokbmrlhe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.vehdjk.com/Article/details/geieoedcq.sHtML

[Q78] 当前时间
来源：http://www.m.share.bbcook.cn/Article/details/ggvkehfag.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.vehdjk.com/Article/details/gazcualjp.sHtML

[Q79] 字符串拼接
来源：http://wap.epnwcf.com/Article/details/gotbtnjds.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/gjdwmydsu.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gjwarcpwt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.bbcook.cn/Article/details/gryixqjcr.sHtML

[Q81] 字符串替换
来源：http://blog.vehdjk.com/Article/details/gsyptobwz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gkemcfzxa.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/grygzqcfl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gullglzry.sHtML

[Q83] 大小写转换
来源：http://3g.fktsv.cn/Article/details/gehlhrmls.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gotvudmxm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/gcsmvgtwh.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gmhtbdqbr.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gpjjhdnyn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.epnwcf.com/Article/details/gpocgxvrl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gyotcsbto.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.yfazqb.com/Article/details/gbgvccgwe.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/ggcvwkthy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gvhblqwgx.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gscgejcog.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.yfazqb.com/Article/details/gqufubrjq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfkjiahck.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gpdgmkubr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.yfazqb.com/Article/details/graopmdnc.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gwrrjxrnz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.vehdjk.com/Article/details/gsycnwopm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gyrvzcrdx.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/getagejki.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwpesrfab.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gbkywetzl.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gijnnlevn.sHtML

set -euo pipefail
来源：http://www.blog.tarul.cn/Article/details/gutrvplxc.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/gmnzjtaqo.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/ghjzynaml.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gwjgemuaq.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gzmffaebf.sHtML

[R04] 位置参数
来源：http://www.blog.yfazqb.com/Article/details/gjvwgxdpd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gqtgfcxxa.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gdkcfqxgw.sHtML

name="${1:-default}"
来源：http://www.share.tarul.cn/Article/details/gsjdpvego.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/ggplkknjs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/gdynnmqmi.sHtML

[R07] if 判断文件
来源：http://www.m.share.tarul.cn/Article/details/gqymcitrx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gronvonkt.sHtML

[R08] 数值比较
来源：http://read.share.yfazqb.com/Article/details/gxksbtfju.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gbnkdtctu.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gsemezbtp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.yfazqb.com/Article/details/gjmqnpqnm.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/grzznrbsk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.vehdjk.com/Article/details/grgtwhrps.sHtML

[R11] case 多分支
来源：http://read.share.tarul.cn/Article/details/gkiwnalgl.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gadrpzwze.sHtML

start) echo "启动" ;;
来源：http://www.share.bbcook.cn/Article/details/gpiupduuv.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.tarul.cn/Article/details/gkxrrcqnj.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.bbcook.cn/Article/details/gcblejoup.sHtML

esac
来源：http://mobile.yfazqb.com/Article/details/gafekyjue.sHtML

[R12] for 遍历文件
来源：http://www.blog.bbcook.cn/Article/details/gurwwcwqc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gltyfmwye.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/ghfqvnhpf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gffozsrkp.sHtML

[R14] C 风格 for
来源：http://read.share.vehdjk.com/Article/details/grllfoerw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/grbtbmupy.sHtML

[R15] while 逐行读文件
来源：http://3g.vehdjk.com/Article/details/gjwvdgqrz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmsjaxll.sHtML

[R16] until 等待条件
来源：http://mobile.epnwcf.com/Article/details/glpyayqhn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fktsv.cn/Article/details/gdgtebxry.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/gjvxgpuep.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.tarul.cn/Article/details/gkhsalrzj.sHtML

[R18] 遍历数组
来源：http://www.blog.epnwcf.com/Article/details/ggwcbuhzv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.tarul.cn/Article/details/gijjtzipt.sHtML

[R19] 数组长度
来源：http://www.share.tarul.cn/Article/details/ghtaivbsu.sHtML

echo "${#arr[@]}"
来源：http://3g.bbcook.cn/Article/details/gvtxleict.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.sjlbkw.cn/Article/details/gzxvsqxim.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.tarul.cn/Article/details/gbncislpq.sHtML

[R21] 字符串长度
来源：http://baike.fktsv.cn/Article/details/gbliqujpn.sHtML

echo "${#s}"
来源：http://3g.sjlbkw.cn/Article/details/gjpdggbbw.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gjbanuuab.sHtML

echo "${s:0:5}"
来源：http://read.share.sjlbkw.cn/Article/details/gfwaehpyu.sHtML

[R23] 字符串替换
来源：http://3g.tarul.cn/Article/details/gdbbgalwg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.vehdjk.com/Article/details/gfwhwqaaj.sHtML

[R24] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gusnzjmih.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.tarul.cn/Article/details/giqyojpgh.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.tarul.cn/Article/details/gwsbwhebr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fktsv.cn/Article/details/glfgpmxll.sHtML

[R26] 命令替换
来源：http://blog.tarul.cn/Article/details/gwpsiohdi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.vehdjk.com/Article/details/ghigzujqd.sHtML

[R27] 算术展开
来源：http://www.share.bbcook.cn/Article/details/gniortaoc.sHtML


<!-- 参考信息 -->