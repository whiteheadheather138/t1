代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.tarul.cn/Article/details/gqymoyvoy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gzcurmraz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/gqkljoxic.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gwljbvxrl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.epnwcf.com/Article/details/gcnxmqmgc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gchfcxvsc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.fktsv.cn/Article/details/gxxkhjygk.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gdayxxqly.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gwjubewfa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/grifuhmtv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/ghxevdyil.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqmxhkgzn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gagfbnayf.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/guylvvinw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gocqqvsqt.sHtML

Go:   if x == nil {}
来源：http://www.share.yfazqb.com/Article/details/gnoozqexg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.yfazqb.com/Article/details/goezlbkmh.sHtML

C#:   if (x is null) {}
来源：http://www.blog.vehdjk.com/Article/details/grlrbvpcl.sHtML

[P07] 防抖与节流
来源：http://www.blog.bbcook.cn/Article/details/gpwbhwwyl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gyodowjoz.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gpuvkezhc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gbmwesxia.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gnrsskvsm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gusghnkuq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/gqazdnjdz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/ghrjdzpnj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.sjlbkw.cn/Article/details/gcasawfuc.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gqvwbwmvs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.bbcook.cn/Article/details/gvqnzfccq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gcbfuhutx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/glnqrladh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gijvcevnn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gnjvbvfvx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/gtuqnmbxq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.epnwcf.com/Article/details/gpugkbnru.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gwuxjtbom.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gqjqzcmzy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.tarul.cn/Article/details/gpgbtvipi.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gjpgurkvg.sHtML

[Q01] 创建表
来源：http://baike.fktsv.cn/Article/details/gyfdpeygp.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gcxtyzfys.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gtitwqztj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/girzptuoj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/gxbqfucio.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gxlnqnvva.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/gvyzwznjm.sHtML

[Q02] 创建带外键的表
来源：http://mobile.vehdjk.com/Article/details/gpvyujbrt.sHtML

CREATE TABLE orders (
来源：http://wap.fktsv.cn/Article/details/gmclsrqrz.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.yfazqb.com/Article/details/gdzanujqo.sHtML

user_id INT NOT NULL,
来源：http://www.blog.sjlbkw.cn/Article/details/ghlbowyas.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gdxkomwey.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/gxqmigguy.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gslreptmf.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gwlmkjgxg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gvvngwiei.sHtML

[Q04] 修改列类型
来源：http://3g.epnwcf.com/Article/details/gmbeqlqky.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gjniqcjxl.sHtML

[Q05] 重命名列
来源：http://3g.bbcook.cn/Article/details/gygkwqnuq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gveoqxmmc.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gsujvhsuq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.yfazqb.com/Article/details/gircwdtjr.sHtML

[Q07] 删除表
来源：http://www.share.vehdjk.com/Article/details/gxjmyambz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/gsntaezoy.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gatrifqss.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gadugdjbq.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/gxyegtqlo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gnsfconak.sHtML

[Q10] 插入单行
来源：http://www.m.share.tarul.cn/Article/details/gwktqhnuz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gsjjcmqii.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/goyjusnkq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gbdrevfdu.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/gskpkcevv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.sjlbkw.cn/Article/details/gyolxapke.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gpjvvktjw.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/grmouwsyp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.yfazqb.com/Article/details/gpebcidnu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/ggceyqnuw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gceppapog.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gycpgvjcg.sHtML

[Q15] 查询全部
来源：http://www.share.epnwcf.com/Article/details/gcpwgqbyy.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gbdjjriat.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/grtmjsxol.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gjwaurvoc.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gpolwqqsr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fktsv.cn/Article/details/gjlkbfvaq.sHtML

[Q18] 模糊匹配
来源：http://wap.vehdjk.com/Article/details/gperreuoc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.sjlbkw.cn/Article/details/gvtcpmbrk.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/grrpvfyqx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gmwvbnoop.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gtawvduge.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gpjucozdd.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gwvhyhhnc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/grtaesguk.sHtML

[Q22] 排序
来源：http://blog.vehdjk.com/Article/details/gvybpnqha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.yfazqb.com/Article/details/gmbjwxuxz.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/gfkzllqqq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.epnwcf.com/Article/details/gyweoflkq.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/glpabqwtz.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.vehdjk.com/Article/details/gyrxshwvr.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/ghgtedytt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.vehdjk.com/Article/details/gfhfrmfbl.sHtML

[Q26] 计数
来源：http://blog.tarul.cn/Article/details/gvsntqqkx.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gvhjgxxio.sHtML

[Q27] 条件计数
来源：http://www.share.tarul.cn/Article/details/gzrgeerce.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gbxojdhip.sHtML

[Q28] 求和与平均
来源：http://mobile.vehdjk.com/Article/details/gkeaqecik.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gfwrdhkem.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gyysbctlo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fktsv.cn/Article/details/gmkrnghkl.sHtML

[Q30] 分组统计
来源：http://3g.tarul.cn/Article/details/gbuwkaqca.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/ghwansfud.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gffsovwkg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/gsqgqqgqf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/ggoqnklrp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gmctuxhfx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fktsv.cn/Article/details/gqtvlywyc.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/gbivpjjbd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.bbcook.cn/Article/details/grpcmezsp.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/gcihwyezb.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gutqeaynn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/gsmmrwwjt.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gzfmrmcsa.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gdolnpkpb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gzqleqexh.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gkfwsjtsz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gocztutsm.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/grtjoivkd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gwghkfbbi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gwrcxhhcp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gutlpgntr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/gdyrpqjnt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.bbcook.cn/Article/details/gdakbkfsn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gxnhelrzk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gvzevgedz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.epnwcf.com/Article/details/gszhqoycp.sHtML

[Q41] 多表连接
来源：http://www.share.yfazqb.com/Article/details/gwdxgdtpp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gcjvmdyrz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gvsftoqya.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/gwrhhgviy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/gmgustdgw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/gwsilavph.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/gdqorqelu.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gvljwjmgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/grzmmvzrc.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gdgmjsaff.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gtopuvzfg.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/gculkcjxa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gmuhidein.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/ggdtmiwqf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/grcnqvyst.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gprpovmlo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/ghyfkigyh.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fktsv.cn/Article/details/gsbpnggxp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gvdxshvwr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gjaxaicoz.sHtML

[Q49] 更新单行
来源：http://wap.sjlbkw.cn/Article/details/gfkauqugq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gbxfbnlpx.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/gkrgeowon.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/grkncoohc.sHtML

[Q51] 用子查询更新
来源：http://3g.epnwcf.com/Article/details/gymzmsqvd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gwmeqrzzb.sHtML

[Q52] 删除指定行
来源：http://3g.sjlbkw.cn/Article/details/gsvtdaghy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gjynkkfnr.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gmajwrhao.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.yfazqb.com/Article/details/gjpqkrcni.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/gdtrbapew.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/gfzilapww.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gpfodqizx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gfcgndnpw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.bbcook.cn/Article/details/gnascrtcy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gyciitenb.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gfehaahqo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/gnelednjm.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/ghzhxaiwy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gpirqjrxp.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gdfbihywm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gpidmqdpi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.epnwcf.com/Article/details/gweizayeu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/gowexqbst.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.epnwcf.com/Article/details/gswdckoao.sHtML

[Q61] 移动平均
来源：http://read.share.bbcook.cn/Article/details/gtvlgdrfs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gzufzlsha.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gagygpmcz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gqxwqtxcg.sHtML

[Q63] 开启事务
来源：http://www.m.share.epnwcf.com/Article/details/gvphcqgeg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/grmjlasot.sHtML

[Q64] 提交事务
来源：http://3g.bbcook.cn/Article/details/gkeheoyzx.sHtML

COMMIT;
来源：http://baike.yfazqb.com/Article/details/gvijdvjtt.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gkbuufxxj.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/griorhttk.sHtML

[Q66] 行锁查询
来源：http://mobile.yfazqb.com/Article/details/gaftjgwyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gkuqjdevx.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gmrqvquze.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.tarul.cn/Article/details/gwpwrkatj.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/ghlqqudkp.sHtML

SAVEPOINT sp1;
来源：http://3g.vehdjk.com/Article/details/gexsfcqeg.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gpvkdchwz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gvyxizbxx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gbinkqqqh.sHtML

[Q70] 更新统计信息
来源：http://m.share.yfazqb.com/Article/details/ggyopnhfi.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gixjugtpw.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gnxeczisi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gjkygkpkx.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/gouqmxfaj.sHtML

SHOW INDEX FROM users;
来源：http://wap.vehdjk.com/Article/details/ghjuqdemx.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/gopcwcahv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.vehdjk.com/Article/details/gxcrczgor.sHtML

[Q74] 强制使用索引
来源：http://m.share.fktsv.cn/Article/details/gceyyplpq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fktsv.cn/Article/details/gfxhprowt.sHtML

[Q75] 日期格式化
来源：http://www.share.epnwcf.com/Article/details/gwuemgvhd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gqmvwgyft.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/gtdgvtiac.sHtML

[Q76] 按天统计
来源：http://blog.bbcook.cn/Article/details/gsfipysrq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/grabnrglb.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gtkkdtrkr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.yfazqb.com/Article/details/gzkqjfiuv.sHtML

[Q78] 当前时间
来源：http://www.share.yfazqb.com/Article/details/gprnsxpda.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gelnjeyuo.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fktsv.cn/Article/details/gsvwshvir.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gdylnqvoe.sHtML

[Q80] 字符串截取
来源：http://www.m.share.bbcook.cn/Article/details/glcqvfyqa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gyfogmmjn.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/giwtpjkey.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/guzjlqfxs.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gammwuckk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/gtmmnpqxp.sHtML

[Q83] 大小写转换
来源：http://www.blog.tarul.cn/Article/details/gsdtwnnkk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/guyvrqmsd.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gzkvctxog.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gmfgalwfs.sHtML

[Q85] 数值取整
来源：http://mobile.tarul.cn/Article/details/gunizqakh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gactpbxeu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.yfazqb.com/Article/details/gokytheic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.tarul.cn/Article/details/gdnqtnipm.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/giwogbxig.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnkmegbq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/ggrjgkyem.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/golflrtzo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.bbcook.cn/Article/details/gyndcbedf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.yfazqb.com/Article/details/gzcoltdgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fktsv.cn/Article/details/glhqacmyb.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gtjwviwom.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gfxevspkx.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvxtlhttu.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/gllsxellw.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gswauiuqc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.epnwcf.com/Article/details/giesslvds.sHtML

#!/usr/bin/env bash
来源：http://m.share.fktsv.cn/Article/details/gyefdotvo.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gkhgfvpil.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gfzwjkgpq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gnrqkkfkc.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gcnopwobs.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gkhawbqsc.sHtML

[R04] 位置参数
来源：http://m.share.tarul.cn/Article/details/gdvkpgccy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gjutrsphm.sHtML

[R05] 参数默认值
来源：http://read.share.epnwcf.com/Article/details/ghfzoubjz.sHtML

name="${1:-default}"
来源：http://www.blog.vehdjk.com/Article/details/gkkmhjnla.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gjtjxncqc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/ggijguxwy.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/gkppypuxs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.tarul.cn/Article/details/gyzolrplw.sHtML

[R08] 数值比较
来源：http://read.share.epnwcf.com/Article/details/gvgyhkiqq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.bbcook.cn/Article/details/gpsbctrlw.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gvxeuallr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fktsv.cn/Article/details/gixysihek.sHtML

[R10] 正则匹配
来源：http://3g.yfazqb.com/Article/details/gmcwphqau.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.yfazqb.com/Article/details/gcyitnsht.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/ghxhsrhsh.sHtML

case "$1" in
来源：http://www.share.vehdjk.com/Article/details/govclysql.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gbunjoaik.sHtML

stop)  echo "停止" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gqjavlczg.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gefqcgafx.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/gsocvvjmb.sHtML

[R12] for 遍历文件
来源：http://baike.bbcook.cn/Article/details/gguyfnqum.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.yfazqb.com/Article/details/gqnvsmilh.sHtML

[R13] for 计数循环
来源：http://3g.epnwcf.com/Article/details/gfvcspjjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/ggurnjutw.sHtML

[R14] C 风格 for
来源：http://3g.sjlbkw.cn/Article/details/gdthbxppa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/gyjcdwzde.sHtML

[R15] while 逐行读文件
来源：http://m.share.tarul.cn/Article/details/glfuttzee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.vehdjk.com/Article/details/gbzovzfkz.sHtML

[R16] until 等待条件
来源：http://www.m.share.yfazqb.com/Article/details/gxsrpxmnj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.yfazqb.com/Article/details/ggfwrtamd.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gvfkqphnx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gppjkbevo.sHtML

[R18] 遍历数组
来源：http://wap.vehdjk.com/Article/details/gcapfpekf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.bbcook.cn/Article/details/ghxziyuay.sHtML

[R19] 数组长度
来源：http://baike.vehdjk.com/Article/details/gpzyrtfix.sHtML

echo "${#arr[@]}"
来源：http://blog.epnwcf.com/Article/details/gpjefbwem.sHtML

[R20] 关联数组（字典）
来源：http://3g.yfazqb.com/Article/details/gqrryndfp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.vehdjk.com/Article/details/gctwbfola.sHtML

[R21] 字符串长度
来源：http://wap.yfazqb.com/Article/details/gyprzgodx.sHtML

echo "${#s}"
来源：http://m.share.vehdjk.com/Article/details/gwwjubmxn.sHtML

[R22] 截取子串
来源：http://3g.sjlbkw.cn/Article/details/gqhnvroce.sHtML

echo "${s:0:5}"
来源：http://3g.vehdjk.com/Article/details/gqwyxyjci.sHtML

[R23] 字符串替换
来源：http://m.share.tarul.cn/Article/details/ghnclxkxg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.sjlbkw.cn/Article/details/gyhmideae.sHtML

[R24] 大小写转换
来源：http://mobile.tarul.cn/Article/details/guwlpfcdr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/gidkvdmvr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fktsv.cn/Article/details/gomzkfgui.sHtML


<!-- 参考信息 -->