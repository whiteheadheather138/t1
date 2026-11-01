代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://wap.tarul.cn/Article/details/gnwrzlsof.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fktsv.cn/Article/details/gvugesovn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.bbcook.cn/Article/details/gugdaomqz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gyodajwaw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gnjsshxmz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.bbcook.cn/Article/details/gnqimjyej.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gclcegsow.sHtML

Ruby: a == b
来源：http://baike.tarul.cn/Article/details/gdqqvogzz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gwclewoxs.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/ggcepwwhr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gfzhdbiqf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gwfcfphxo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/gkbwavlgv.sHtML

TS:   if (x == null) {}
来源：http://m.share.epnwcf.com/Article/details/gzeigpokk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.tarul.cn/Article/details/gfvkukiyv.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gzvydwnuu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gzftpidtd.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/giylqzhgc.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gijmqriqt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.bbcook.cn/Article/details/gwkrtbkjo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/ghvmnzfnq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/grijmhrtb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/getcxmcsz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.yfazqb.com/Article/details/gmxcrjhsl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gcecwopep.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.yfazqb.com/Article/details/glfvufolk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/gnonucicb.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gxwpigync.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.tarul.cn/Article/details/gxoqvpumf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/gaerijczy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/ggelhcazb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gqggzxcub.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gycngqzdq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/gfsxwdlss.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gmkhwapxa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/ghfcbtqom.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdlmdsrup.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/ghmwtdwsm.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gnjnykbgo.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gttaeuxje.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gdmsgvsqu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gcboubppx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/glmhlvwzd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.vehdjk.com/Article/details/gwppgcjvf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.sjlbkw.cn/Article/details/gwadoeeut.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gvnosoore.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/gwprlnewo.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/goorxwfdn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gjfxoyadp.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gkrfulcyt.sHtML

amount DECIMAL(10, 2),
来源：http://baike.tarul.cn/Article/details/gsqwdorzq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gftvvhnov.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gooxqsrtj.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/geijyigqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gjhbwoubv.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/gxknloidu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.tarul.cn/Article/details/ghdezbxgd.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gweobktjn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/geuvxyptx.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/ggwcsrwmt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gkupjuglb.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/gajtbtxsy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gedrisigt.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/gcilwoabf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gcvilbzda.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gwrjinwdg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/gkexdoyni.sHtML

[Q10] 插入单行
来源：http://read.share.tarul.cn/Article/details/gnenekbqs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.bbcook.cn/Article/details/gwjtzjrhu.sHtML

[Q11] 一次插入多行
来源：http://3g.sjlbkw.cn/Article/details/gzwihheqv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.bbcook.cn/Article/details/godyovfmo.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/goumoyfab.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/glviyztxp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.epnwcf.com/Article/details/gzlpgnxmu.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gnzknirpg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gvyrhpyxq.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gblyzgvnd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.epnwcf.com/Article/details/gqcjpsryc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/gerilsvtc.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gppvgpvmm.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/grlntqsza.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gmkbvhiaa.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gehgytvdf.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/guqbwlfyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gxjgzfauz.sHtML

[Q18] 模糊匹配
来源：http://blog.epnwcf.com/Article/details/gfsacudba.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.tarul.cn/Article/details/gujxfjgpl.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gkdproxea.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.vehdjk.com/Article/details/godqfnigu.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gbtxribfa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.bbcook.cn/Article/details/gyetsyxdm.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gdqenuozs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gxgrvsfdf.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/guoitzxkx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.tarul.cn/Article/details/gdzkzynte.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gwyrxudbs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gwkrsrqub.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gurxpafqw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/goehammav.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gazpzvidw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gjlfitnzx.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/grfgttvau.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gqdevegub.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/godtxheuk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gxiqnilgf.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/ghxpyntds.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gipukickb.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gfsbijafs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkadepgc.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gzjkkzncf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gvssxzxvc.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gvjkmiwtz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/gfoymkbkb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/glkjejmgk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gpbpbjnzq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/giwosonrk.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gapzkjfto.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.sjlbkw.cn/Article/details/gdeyxehjk.sHtML

[Q34] 每组取第一条
来源：http://read.share.fktsv.cn/Article/details/glgwidmmh.sHtML

SELECT * FROM (
来源：http://wap.yfazqb.com/Article/details/gbspyudru.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gkzoatvsb.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gcpsvlsiz.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/gwdcxtvmx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/glbusqmbc.sHtML

[Q36] 左连接
来源：http://wap.bbcook.cn/Article/details/gnjjkslqc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gaqtzsxha.sHtML

[Q37] 右连接
来源：http://www.blog.fktsv.cn/Article/details/gjuwkxtiq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.epnwcf.com/Article/details/gsowdxilf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/gspnlevzx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.bbcook.cn/Article/details/gvousuqkh.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.sjlbkw.cn/Article/details/gbclzhsny.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/gxaiwldph.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gsascgvye.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gucprohyp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/guarknugt.sHtML

[Q41] 多表连接
来源：http://m.share.vehdjk.com/Article/details/ghfftenyh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gttpnawvx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gpcfncrmz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/goxgervlp.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/gvytdjalg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gbbhrumbg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gllpaqkbr.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gcvtornuj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gyjaknvma.sHtML

[Q44] IN 子查询
来源：http://m.share.epnwcf.com/Article/details/gykpddkrg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/geupnwpmi.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gaolcdpwn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/ggnaamiwo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gqgzscpvo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gmpcigjch.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gcqqeloul.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gyfccdqhs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gumzwjgwz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.epnwcf.com/Article/details/gmuxsqzjy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.bbcook.cn/Article/details/gqfvzcpbl.sHtML

[Q49] 更新单行
来源：http://m.share.vehdjk.com/Article/details/gvmiqmpug.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gkolwodem.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gmiiheuea.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/gcxensrxh.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/gurfdlzqn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gnnmjzlib.sHtML

[Q52] 删除指定行
来源：http://mobile.yfazqb.com/Article/details/gdkweefdh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gyajewxhu.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/grsjmhdtl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gbxmmhfnd.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gqtcrahdi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gvbxontsj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/gfysmpmnc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gjzgxikiv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gzhgrfhvc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gfflblpov.sHtML

[Q57] 行号
来源：http://www.share.yfazqb.com/Article/details/gdxxkcwql.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gowqydqrw.sHtML

[Q58] 累计求和
来源：http://www.blog.tarul.cn/Article/details/gahpnzdyr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gmgtrwayc.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/gqffozeeo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gsrwhvxtx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/ghkzhxyrw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gufolprqr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gslbevnhv.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gmwhkyhcm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gisueqogo.sHtML

[Q62] 分组占比
来源：http://blog.epnwcf.com/Article/details/gebdeicuw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/ghlcfcddc.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gedzuvyop.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gpvobbyah.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gichuujpf.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/glpzrnrgy.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gzkdklppp.sHtML

ROLLBACK;
来源：http://m.share.vehdjk.com/Article/details/gwjovnqwn.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gmywfdfer.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gadjrctxc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gyxpyjndo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fktsv.cn/Article/details/gyxobutje.sHtML

[Q68] 保存点
来源：http://www.m.share.yfazqb.com/Article/details/gelqphypt.sHtML

SAVEPOINT sp1;
来源：http://blog.vehdjk.com/Article/details/gnlsdxigw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/gflwcdsfv.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gjljhemkk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gxyfdmbnc.sHtML

[Q70] 更新统计信息
来源：http://3g.tarul.cn/Article/details/ggbpaalmw.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gnwiekend.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gxmmavyby.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/ggitggjnl.sHtML

[Q72] 查看索引
来源：http://www.blog.fktsv.cn/Article/details/gctxhmqdq.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/gjxigbydr.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gyufbjeon.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/ghcpsdqcn.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gyechtgef.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fktsv.cn/Article/details/gwxkwbbla.sHtML

[Q75] 日期格式化
来源：http://mobile.sjlbkw.cn/Article/details/gskapffwr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.yfazqb.com/Article/details/gesktpyjo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gsaqzezfe.sHtML

[Q76] 按天统计
来源：http://mobile.bbcook.cn/Article/details/gkhdipibo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gndxzncns.sHtML

[Q77] 时间加减
来源：http://blog.bbcook.cn/Article/details/gwpjcvmir.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/gsyfzwyfy.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/gspidwnyv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/gpwkwzidu.sHtML

[Q79] 字符串拼接
来源：http://wap.tarul.cn/Article/details/gbnwuugkc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.sjlbkw.cn/Article/details/gsuopnxvc.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/goqqhjeps.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gfgmzkeyd.sHtML

[Q81] 字符串替换
来源：http://baike.fktsv.cn/Article/details/gdbnfzzbx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gxmyiyboj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gmfttvdip.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gnzwjzorb.sHtML

[Q83] 大小写转换
来源：http://wap.tarul.cn/Article/details/gzzlfcjwc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gcrrnoekv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/guweiuecx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gnlyktwjv.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/gvlmayjmf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fktsv.cn/Article/details/gnkwotluj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/gsnxtulkt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.epnwcf.com/Article/details/gdravypdj.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fktsv.cn/Article/details/gqplwhkcx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/glucihtkz.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gosqznkzr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gjqymgyki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.yfazqb.com/Article/details/grqvsifhm.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gpnsnfala.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gcablxjus.sHtML

[Q90] 生成序号列
来源：http://www.blog.fktsv.cn/Article/details/gaxswodeq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.epnwcf.com/Article/details/gmitfbjfi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gripknkyp.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gwgmouqrf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gezsycpyz.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/givkmwohd.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gemilsdss.sHtML

set -euo pipefail
来源：http://www.share.epnwcf.com/Article/details/gvympumnk.sHtML

[R02] 变量赋值与使用
来源：http://blog.sjlbkw.cn/Article/details/gylzjyykd.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fktsv.cn/Article/details/gmdprjznb.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gvkdmnmio.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gsuxuntlu.sHtML

[R04] 位置参数
来源：http://www.m.share.vehdjk.com/Article/details/glrvwoxnh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gxucyzpoh.sHtML

[R05] 参数默认值
来源：http://www.blog.bbcook.cn/Article/details/gbgarszuq.sHtML

name="${1:-default}"
来源：http://3g.tarul.cn/Article/details/gnuyaphta.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gahwhywax.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.yfazqb.com/Article/details/ggthuirid.sHtML

[R07] if 判断文件
来源：http://wap.fktsv.cn/Article/details/gfstwuyrq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fktsv.cn/Article/details/gnzpsdhkj.sHtML

[R08] 数值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gblpewtkq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gawbaalio.sHtML

[R09] 字符串比较
来源：http://wap.sjlbkw.cn/Article/details/gmuifqiid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.sjlbkw.cn/Article/details/gxcmuvesz.sHtML

[R10] 正则匹配
来源：http://3g.fktsv.cn/Article/details/gjoeeklvj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gngdxcwor.sHtML

[R11] case 多分支
来源：http://www.blog.sjlbkw.cn/Article/details/gzgzeudxz.sHtML

case "$1" in
来源：http://wap.bbcook.cn/Article/details/gpripnvng.sHtML

start) echo "启动" ;;
来源：http://baike.fktsv.cn/Article/details/gjucfqcmw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gktzzibhs.sHtML

*)     echo "未知命令" ;;
来源：http://baike.vehdjk.com/Article/details/ggapkuawt.sHtML

esac
来源：http://blog.epnwcf.com/Article/details/gfoebabvk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fktsv.cn/Article/details/gprgcczpw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gfajbupsm.sHtML

[R13] for 计数循环
来源：http://wap.vehdjk.com/Article/details/gjnksvmnl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gbkahjmym.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gerjblrlg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gsrsfjfwo.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gjxarkpeb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.sjlbkw.cn/Article/details/gbkyfxcys.sHtML

[R16] until 等待条件
来源：http://m.share.tarul.cn/Article/details/ggruttigb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.epnwcf.com/Article/details/grkkjrrhv.sHtML

[R17] 数组定义与取值
来源：http://3g.epnwcf.com/Article/details/gchsmesbw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/ghnhxjfku.sHtML

[R18] 遍历数组
来源：http://m.share.yfazqb.com/Article/details/glhmqujdg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.yfazqb.com/Article/details/gsuqfeqey.sHtML

[R19] 数组长度
来源：http://mobile.epnwcf.com/Article/details/gmvwetrcx.sHtML

echo "${#arr[@]}"
来源：http://m.share.epnwcf.com/Article/details/gvreimpio.sHtML

[R20] 关联数组（字典）
来源：http://wap.sjlbkw.cn/Article/details/gpuxqpttf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.yfazqb.com/Article/details/gjxtnwvpo.sHtML

[R21] 字符串长度
来源：http://m.share.epnwcf.com/Article/details/gzgdgacom.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gakijxehm.sHtML

[R22] 截取子串
来源：http://baike.epnwcf.com/Article/details/guzzvljdq.sHtML

echo "${s:0:5}"
来源：http://baike.vehdjk.com/Article/details/ghvixcyjw.sHtML

[R23] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gfoqchjbm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.yfazqb.com/Article/details/gzhwifvie.sHtML

[R24] 大小写转换
来源：http://www.blog.epnwcf.com/Article/details/ggwwllctt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.sjlbkw.cn/Article/details/gxvayntwe.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.tarul.cn/Article/details/guyptazif.sHtML


<!-- 参考信息 -->