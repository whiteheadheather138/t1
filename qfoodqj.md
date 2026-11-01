代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/ggbxpatvc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gvefuqpme.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.tarul.cn/Article/details/gsbhuegvl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gmthrqifw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gpsnwlbtz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.yfazqb.com/Article/details/goazhnice.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gikvymuhe.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/guwtexpnh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gacayhpfg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gymtkeomm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gitvlgyyn.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gxvhwxvwi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gwgelxoqc.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/goddejisr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gcmkagyhu.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gfhkbffhm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gkrxhmxfw.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gygzrzcyi.sHtML

[P07] 防抖与节流
来源：http://www.m.share.tarul.cn/Article/details/glwoprtyz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/grvwmclig.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.tarul.cn/Article/details/goyncrqxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gqkotndei.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gdblonagh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gfimeagyf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.tarul.cn/Article/details/gnkjakkkp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.bbcook.cn/Article/details/gzdflcxar.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gglkbhrrq.sHtML

[P08] 处理浮点精度问题
来源：http://3g.epnwcf.com/Article/details/gsvzxlasw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.bbcook.cn/Article/details/gzylxwtzo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gegzzkrmp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/goznmbmmu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gkwpuyrhs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/geynffwfc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gjncehlxw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/gjzfwpilo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.sjlbkw.cn/Article/details/gwpnlwlxp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gsgyyxbzc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.sjlbkw.cn/Article/details/gtugneqsv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxzhuifax.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gdxelrqpv.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gspcqzedh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gfuisdgnk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gsmsegcwt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fktsv.cn/Article/details/gzbebovxd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/gbzgsjgco.sHtML

);
来源：http://blog.epnwcf.com/Article/details/gdcnbxrjg.sHtML

[Q02] 创建带外键的表
来源：http://blog.vehdjk.com/Article/details/gredrnokz.sHtML

CREATE TABLE orders (
来源：http://3g.epnwcf.com/Article/details/gknontuqo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/geqgabdmd.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gaqnafbct.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/grbogytsb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gdrcoorhg.sHtML

);
来源：http://baike.epnwcf.com/Article/details/golwaasyi.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gqduuhkkx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.bbcook.cn/Article/details/govnkqmii.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/greygfyvx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/ghawfkarl.sHtML

[Q05] 重命名列
来源：http://www.share.yfazqb.com/Article/details/gnbzijpuv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/ggzmstiot.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gsfditybj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/grdnwseyk.sHtML

[Q07] 删除表
来源：http://baike.yfazqb.com/Article/details/gbihgbdsm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gsqkagqgj.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gqsxtjfwf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gdzpundgc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.yfazqb.com/Article/details/grknbskta.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gtfxodbms.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gedsawjzi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gohpafyix.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gizfwyqkb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/grbyccidq.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fktsv.cn/Article/details/gsemcbtdu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.yfazqb.com/Article/details/gaiywjcjq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gzupuotva.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/ggneyzdfh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gvqslemqq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.bbcook.cn/Article/details/gjllduxkc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gdzniidnr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.yfazqb.com/Article/details/gkujkubye.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gxtbbyora.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/grtcqjpif.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gsiawjisb.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gxfmetyqn.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gkyumorpr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.tarul.cn/Article/details/gyqbqmlmv.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gfuszsktp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/gvontmywf.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gofhcrexl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gnywwavoh.sHtML

[Q20] IN 列表
来源：http://www.share.sjlbkw.cn/Article/details/gecnxtlau.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.bbcook.cn/Article/details/gdgokxsts.sHtML

[Q21] 空值判断
来源：http://mobile.bbcook.cn/Article/details/guhwkzlyu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/gambebhbs.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gckihmbbs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.bbcook.cn/Article/details/gpdoginfk.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/globuznui.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.tarul.cn/Article/details/ghlcemuzr.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gonuauzio.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gctgpoayj.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/geeepomht.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/ggjhzdsva.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gimypfewu.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.bbcook.cn/Article/details/gjaudesgp.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gemsfyeyk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.sjlbkw.cn/Article/details/grmguexwf.sHtML

[Q28] 求和与平均
来源：http://read.share.sjlbkw.cn/Article/details/gfpmwfkrl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fktsv.cn/Article/details/glncmicsp.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gdbpzbrgu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gplrfloig.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gfpmqwufh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gjpmoqhnj.sHtML

[Q31] 分组后过滤
来源：http://m.share.yfazqb.com/Article/details/gfymeifla.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gdggegyzc.sHtML

[Q32] 分组拼接字符串
来源：http://baike.sjlbkw.cn/Article/details/gnutujlbl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gpfmbpmmc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/gaeynprik.sHtML

[Q33] 多列分组
来源：http://3g.tarul.cn/Article/details/gtjkouqxa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gzwremrfg.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gtxhpkokr.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gmwydwotk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/ghgsymnif.sHtML

) t WHERE rn = 1;
来源：http://www.share.yfazqb.com/Article/details/glfmlqsfg.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gevtxcljg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/guothupao.sHtML

[Q36] 左连接
来源：http://www.blog.bbcook.cn/Article/details/gzgqqhevm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gjecmhner.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/gzwzrqxfs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/gmzptlxos.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gheslkvix.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/giybqhvup.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gzseywzwm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gjcgomsbw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gepeibkur.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gxnnobxug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gfkztital.sHtML

[Q41] 多表连接
来源：http://baike.epnwcf.com/Article/details/gwipwrfcr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.vehdjk.com/Article/details/gmkldxkkx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.epnwcf.com/Article/details/gqpyoztch.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.epnwcf.com/Article/details/glxwfwehq.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.yfazqb.com/Article/details/glbpebqpn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.sjlbkw.cn/Article/details/gwdeuusyg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gjyjipfiv.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gtejtuvqp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gjsufeggu.sHtML

[Q44] IN 子查询
来源：http://wap.sjlbkw.cn/Article/details/gnfxksnrr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gemcdnssi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/glxzendaw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gbcxrdzlc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.sjlbkw.cn/Article/details/gvrmsdmyd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gtefjfcke.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gzfiolppg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gyevxqrtl.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gbhicnshw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/guoqjhgbb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gteohothy.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gbqorbcaf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gihyeutvm.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gvicliarv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gjeyvitjr.sHtML

[Q51] 用子查询更新
来源：http://blog.sjlbkw.cn/Article/details/gkvtgpxit.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gucwjaisg.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gyzucuzfm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/glksplilu.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gxpojexlm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.bbcook.cn/Article/details/gzpibletg.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gjpcowwjg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/ggkqnuyok.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gedvmerbo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/gyzsduqfw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.bbcook.cn/Article/details/gqemilazg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/ghhtyomer.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gcwkaftvt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/gfaaehgdt.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gzmmubexa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gccedpknf.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/gbgihffby.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gagjgbxuk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/givxksizi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/ganleglcx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gfcoezwgl.sHtML

[Q61] 移动平均
来源：http://www.blog.vehdjk.com/Article/details/gdhuwixux.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gdqqbgqig.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gtgeinrgd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/glgqejcoo.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gtdiswwhv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gapkicmon.sHtML

[Q64] 提交事务
来源：http://baike.bbcook.cn/Article/details/gpclpqqrv.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gsionczeh.sHtML

[Q65] 回滚事务
来源：http://wap.tarul.cn/Article/details/gmtfxtyvb.sHtML

ROLLBACK;
来源：http://read.share.vehdjk.com/Article/details/gbbhmcpax.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gjrmovhlx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gzyjskxwc.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gbsaqadfs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/grlagvkus.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/giqsoctsa.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gkbyuqfnd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gwlwzfxdp.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/gemelxhye.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/grfdvgyno.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/glsfyyfhc.sHtML

ANALYZE TABLE users;
来源：http://www.blog.yfazqb.com/Article/details/gjlmkzngi.sHtML

[Q71] 查看建表语句
来源：http://3g.epnwcf.com/Article/details/gwfnyumoa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.sjlbkw.cn/Article/details/gaybmwmwn.sHtML

[Q72] 查看索引
来源：http://www.m.share.epnwcf.com/Article/details/gyrbnfqkf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxiqdgcus.sHtML

[Q73] 查看表状态
来源：http://mobile.sjlbkw.cn/Article/details/gymqknqyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.sjlbkw.cn/Article/details/gpxlhiypv.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gilhgrdea.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gahgzudnp.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/gazbyrzfe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gavsonmgz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/ghoxjascg.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gyjfxxwpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/geiyqwyuo.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gwiccsnlf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gtrfowmhq.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/ggnqhocjb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.yfazqb.com/Article/details/gbzwtkbnn.sHtML

[Q79] 字符串拼接
来源：http://www.share.fktsv.cn/Article/details/gegkialvh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/gaedahfbx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gubsjmcwd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gkeiuhmaz.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gyjmbffgf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gzkjyahen.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gpvgadhde.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gclrislxq.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gykunqneq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gjrcomnzv.sHtML

[Q84] 去除首尾空格
来源：http://3g.sjlbkw.cn/Article/details/gasnruwdx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjoosahtd.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/ggvyhwkda.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/guhejplix.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/gewejbxcj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gbdmvoefw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/guodzvvga.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fktsv.cn/Article/details/gzmdzoukm.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gnqwgialj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/gnvpsxmmp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.yfazqb.com/Article/details/gapnzgloh.sHtML

[Q89] 判断表是否存在
来源：http://m.share.yfazqb.com/Article/details/gcsjuyrgi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gxdbaskuw.sHtML

[Q90] 生成序号列
来源：http://mobile.fktsv.cn/Article/details/gwuqmjyns.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.vehdjk.com/Article/details/girfpqfhk.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsqrmxzzv.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/giavccgxc.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gbceyjgqc.sHtML

[R01] shebang 与严格模式
来源：http://blog.yfazqb.com/Article/details/gjtoalrvs.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gljglcdbv.sHtML

set -euo pipefail
来源：http://www.m.share.epnwcf.com/Article/details/gkrnoesps.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/ghmpozvht.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/glbaymxus.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gbyylufev.sHtML

readonly PI=3.14
来源：http://www.m.share.fktsv.cn/Article/details/gsavfgtij.sHtML

[R04] 位置参数
来源：http://mobile.fktsv.cn/Article/details/glbgbzxop.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.yfazqb.com/Article/details/ghvnllekc.sHtML

[R05] 参数默认值
来源：http://m.share.yfazqb.com/Article/details/giejjlyjo.sHtML

name="${1:-default}"
来源：http://baike.yfazqb.com/Article/details/gwpfqotnp.sHtML

[R06] 判断命令是否存在
来源：http://blog.tarul.cn/Article/details/gvwakkqho.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gmbgoofrc.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/gnfkirifn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.sjlbkw.cn/Article/details/golnjvzpa.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/gkzuxrfkt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.sjlbkw.cn/Article/details/goelyljzo.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/gwahdybbq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.bbcook.cn/Article/details/gskoltoiv.sHtML

[R10] 正则匹配
来源：http://read.share.bbcook.cn/Article/details/gzjtywvpi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gtkczlzwd.sHtML

[R11] case 多分支
来源：http://blog.sjlbkw.cn/Article/details/ggvxtsavk.sHtML

case "$1" in
来源：http://m.share.fktsv.cn/Article/details/gosmiqaxb.sHtML

start) echo "启动" ;;
来源：http://mobile.epnwcf.com/Article/details/gquwertzr.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gjgpoyxgg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.bbcook.cn/Article/details/gjuvsfdgm.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gdxvcljre.sHtML

[R12] for 遍历文件
来源：http://m.share.vehdjk.com/Article/details/giotnimhg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.yfazqb.com/Article/details/gtgrgydaw.sHtML

[R13] for 计数循环
来源：http://wap.fktsv.cn/Article/details/gaqqzblbk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.sjlbkw.cn/Article/details/gewrktezt.sHtML

[R14] C 风格 for
来源：http://mobile.bbcook.cn/Article/details/gczdrkiuo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.bbcook.cn/Article/details/gxvaiglpe.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/gzwicgskr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fktsv.cn/Article/details/gehrouzlm.sHtML

[R16] until 等待条件
来源：http://wap.tarul.cn/Article/details/gftasjilm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.bbcook.cn/Article/details/gjyykfdqg.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gndagrneh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.yfazqb.com/Article/details/gnewhfvyv.sHtML

[R18] 遍历数组
来源：http://mobile.tarul.cn/Article/details/gaicmmswc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.tarul.cn/Article/details/gwfuwcltj.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gxfjnxldf.sHtML

echo "${#arr[@]}"
来源：http://wap.tarul.cn/Article/details/gkliuiwtz.sHtML

[R20] 关联数组（字典）
来源：http://wap.yfazqb.com/Article/details/gnpkusrij.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.bbcook.cn/Article/details/gdbpobrxy.sHtML

[R21] 字符串长度
来源：http://www.share.bbcook.cn/Article/details/gcgebjfkr.sHtML

echo "${#s}"
来源：http://wap.tarul.cn/Article/details/gxivwwgtk.sHtML

[R22] 截取子串
来源：http://baike.sjlbkw.cn/Article/details/gaptclpsu.sHtML

echo "${s:0:5}"
来源：http://read.share.fktsv.cn/Article/details/gttixfwwb.sHtML

[R23] 字符串替换
来源：http://3g.tarul.cn/Article/details/gohybadzy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.bbcook.cn/Article/details/glazltook.sHtML

[R24] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gxjdwazco.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.bbcook.cn/Article/details/gwnaboevx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.vehdjk.com/Article/details/gfbvmecpc.sHtML


<!-- 参考信息 -->