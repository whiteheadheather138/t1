代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gmbyelfqy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/ggdpebsxk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gvjhzxkvb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gtofzeltq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.vehdjk.com/Article/details/gvsmyjdcd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gcsnscwda.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/grbsidqwa.sHtML

Ruby: a == b
来源：http://www.m.share.vehdjk.com/Article/details/gtvjyvbzp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gdpvxxvju.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gmwaebpho.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/gqxsvgdgn.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.vehdjk.com/Article/details/girlnufxv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.tarul.cn/Article/details/gpbgtmemy.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlmlruud.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcecblmoj.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/ghoexuluo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/ghxygmbrk.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/gbvliemjt.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gwmleteov.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gcxftlxtd.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gszphgcam.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gyqajlher.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gwjquzkwo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gcvzopagz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/glcnvhbsf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/gvswozldt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.vehdjk.com/Article/details/gzmrtdxnb.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gyrtonpad.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gyverwmhr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmraznyci.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gibklqmyt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.bbcook.cn/Article/details/gpdgrgtxm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gxdniakcz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gmrqfeiap.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/ggnhykicg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.yfazqb.com/Article/details/gagnjccke.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbdwveuas.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.sjlbkw.cn/Article/details/gtlskyoyd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ggeqvmgwo.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/gfifumyzz.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gyokoyytz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gjkqvhsoz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gfjvohzcp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gxvsmsaaf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.vehdjk.com/Article/details/gkftcfnwk.sHtML

);
来源：http://3g.tarul.cn/Article/details/gywpnxumu.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/gvoxpfllt.sHtML

CREATE TABLE orders (
来源：http://www.share.sjlbkw.cn/Article/details/gfsbnksgf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gymolkrni.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gtyzlliqe.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.epnwcf.com/Article/details/gyqbfueee.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gjxiffuom.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gymawqhwg.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/ghwzkglnj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.epnwcf.com/Article/details/gygakzann.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/ghkswrqtp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.vehdjk.com/Article/details/gxwxduhfl.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/gewdokyft.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.sjlbkw.cn/Article/details/gkdexmikk.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/gaqthbkuu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.bbcook.cn/Article/details/gsrserzll.sHtML

[Q07] 删除表
来源：http://www.m.share.yfazqb.com/Article/details/ggptokive.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/grpibbuxk.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gtujdvrui.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gwlvkunee.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gcdmdvwqy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/gocxfudje.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gxnskpblz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gaxcecqsq.sHtML

[Q11] 一次插入多行
来源：http://www.share.bbcook.cn/Article/details/gxucmecxn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gxzcglomj.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.tarul.cn/Article/details/gitzuydou.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gnmrxzlsg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gjgpubzkd.sHtML

[Q13] 忽略重复插入
来源：http://baike.epnwcf.com/Article/details/gaxcavtot.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gcpdvoxfw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fktsv.cn/Article/details/gpiekgqzg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gzssbdhjj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.yfazqb.com/Article/details/girlopzvf.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gwmkjbnmo.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gdevoghgd.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gpwhbzoey.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/gkokchdak.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/gfxurjvvd.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gmhfrpqwv.sHtML

[Q18] 模糊匹配
来源：http://baike.vehdjk.com/Article/details/gyyrdbfdh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gmrulwazo.sHtML

[Q19] 范围查询
来源：http://baike.epnwcf.com/Article/details/gpzhyemhx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gqusjdjna.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gxutvbgbv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.epnwcf.com/Article/details/ggbtwjgyu.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gorizrllw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/garbbjolo.sHtML

[Q22] 排序
来源：http://blog.yfazqb.com/Article/details/gxmppiexh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gtuxqcbta.sHtML

[Q23] 分页
来源：http://3g.vehdjk.com/Article/details/gwkadewva.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.epnwcf.com/Article/details/gpdcucxcd.sHtML

[Q24] 去重
来源：http://3g.epnwcf.com/Article/details/guvkoibwi.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gdoluitlh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.epnwcf.com/Article/details/ggxrpplxh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.epnwcf.com/Article/details/gdcfnflhq.sHtML

[Q26] 计数
来源：http://3g.fktsv.cn/Article/details/greryxlaf.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gilpwqane.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gbqdyurqq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gslikerjt.sHtML

[Q28] 求和与平均
来源：http://mobile.epnwcf.com/Article/details/gxuulwxio.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gvwdywila.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gkflzrhsn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/glalxkehd.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gmlikhrne.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gstievhsl.sHtML

[Q31] 分组后过滤
来源：http://blog.fktsv.cn/Article/details/gkxsziujn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/guiydtiur.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fktsv.cn/Article/details/gahxirual.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gtmylkyxr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/ggskjmzir.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/guenrakic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gbbxdudla.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gvmavpeam.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gfxhzyrcg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.bbcook.cn/Article/details/gxclknhes.sHtML

) t WHERE rn = 1;
来源：http://m.share.fktsv.cn/Article/details/gonsrmgnl.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzcmmray.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gnjcbukkq.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gzifiqqpf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gohjyfncz.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gpzmmwake.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/grlwssfrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.epnwcf.com/Article/details/gqkxewxnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gzmpbsnks.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gzoycszmg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.bbcook.cn/Article/details/gysfpyuiy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gxcaxpqsj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/gzygremel.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/gdbqebcqx.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gxsdaehuv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.bbcook.cn/Article/details/gaxhwftuk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/gqaxngfzo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.vehdjk.com/Article/details/gplekkjxw.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gxbykpsez.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gkohlfoll.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gvvahnasx.sHtML

[Q43] 标量子查询
来源：http://www.share.tarul.cn/Article/details/gewrrtneq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gwimrjjew.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gjkktltoe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.yfazqb.com/Article/details/grjvztgur.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/giiedozqg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/grrozutbs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.vehdjk.com/Article/details/gkpntjgex.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/grmqzbrll.sHtML

[Q47] 与平均值比较
来源：http://blog.vehdjk.com/Article/details/gyovhawbq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.vehdjk.com/Article/details/gdjxxfcul.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gvvismvlu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gvzmqyegb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.sjlbkw.cn/Article/details/gjkgqxrpw.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gfrluatqw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gvzdmhdfm.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/glwcpqtgg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.yfazqb.com/Article/details/gdggqatxr.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gbzrasmmo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/girlrmmta.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gwpyberrg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/glwkrkfxn.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/ghymtooiv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/ggkjhgfyv.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gobtysmzh.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gxlltihcn.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gkkcpgicp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gllbemqqr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fktsv.cn/Article/details/gpryreenj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gouugpmzn.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gbzzmymba.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gbmgwudvc.sHtML

[Q58] 累计求和
来源：http://mobile.fktsv.cn/Article/details/gfxxiwhgj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gjlfldhjb.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gbpyhrica.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/grpaktavy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.epnwcf.com/Article/details/geklgguxs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.epnwcf.com/Article/details/grdutjbxx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/ggcphdmzg.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gteekhnqk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gseehqubb.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gcgpvuvsd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gcqzjrjop.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gvsogtdfb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gqihqqghe.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/ggjhwtqop.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/gewvxgccc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gywvwzdav.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gnnmylpwb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gwwiwvxze.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gymaxyuab.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/gnwyzctzf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/glquwzyqi.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/gcyfcptyj.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gbwkpownt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fktsv.cn/Article/details/gyssdzftw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gqncsfily.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gvbpqsjnq.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/gofxucqto.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fktsv.cn/Article/details/gghmifhei.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/gqkxuvksy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.vehdjk.com/Article/details/gklbsyfzj.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/gpryufwyq.sHtML

SHOW INDEX FROM users;
来源：http://baike.bbcook.cn/Article/details/gwycffnew.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gqspcinxi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.vehdjk.com/Article/details/gsaplnncm.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/gkszaspqq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gqsmuvmui.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/givezjjvh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gjoeiejtq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fktsv.cn/Article/details/gtmzzxngp.sHtML

[Q76] 按天统计
来源：http://3g.epnwcf.com/Article/details/gqevhmyqa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/gsbyrakrr.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/gyhsdptgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/giuculxcq.sHtML

[Q78] 当前时间
来源：http://www.m.share.yfazqb.com/Article/details/gyatcxyyt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gskyvyfwv.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gdtomscvw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gnxbvthsb.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gcxsfwpdj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/ghqswwgmu.sHtML

[Q81] 字符串替换
来源：http://www.share.fktsv.cn/Article/details/gspeeblxo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/gkvvjkzur.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fktsv.cn/Article/details/glbgeweig.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gzrbhvyjf.sHtML

[Q83] 大小写转换
来源：http://www.blog.fktsv.cn/Article/details/gymzsetej.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghkjfzbhy.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.tarul.cn/Article/details/gmsgwauhp.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.tarul.cn/Article/details/gwuwkgrqg.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gmjdixtaf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gtrqbhtsm.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gcgfodfxl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.sjlbkw.cn/Article/details/gpufduvmr.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/geqvjgowp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/grinzqgjp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.tarul.cn/Article/details/gkxvdfwqr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.sjlbkw.cn/Article/details/gqwrmjytj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.tarul.cn/Article/details/gnqdibofi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gmyqpvjmt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.tarul.cn/Article/details/gzmzehvhl.sHtML

[Q90] 生成序号列
来源：http://mobile.yfazqb.com/Article/details/gfkdlyiwg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/gzenasfhh.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gztyghmpo.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/gvgwqfshy.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gablynnhs.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fktsv.cn/Article/details/ghzihvwcp.sHtML

#!/usr/bin/env bash
来源：http://baike.bbcook.cn/Article/details/gnzapgpyc.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gsatqmstx.sHtML

[R02] 变量赋值与使用
来源：http://www.share.epnwcf.com/Article/details/gamhtqgfx.sHtML

name="Tom"; echo "$name"
来源：http://www.share.tarul.cn/Article/details/gpnvpfbti.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/gejkxlezm.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gvidccgls.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gagqrlwnv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.bbcook.cn/Article/details/gqzhkpizy.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gcflwyavv.sHtML

name="${1:-default}"
来源：http://wap.fktsv.cn/Article/details/gysujqtiw.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fktsv.cn/Article/details/gxwvlvvye.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gmrqkysfe.sHtML

[R07] if 判断文件
来源：http://wap.bbcook.cn/Article/details/ggzcwkgsr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/ggiratpza.sHtML

[R08] 数值比较
来源：http://m.share.fktsv.cn/Article/details/gwgycnbwq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.yfazqb.com/Article/details/gamwuzffg.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gkxgumkpk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.bbcook.cn/Article/details/gpyryrfak.sHtML

[R10] 正则匹配
来源：http://www.share.fktsv.cn/Article/details/gzvlajdyx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.bbcook.cn/Article/details/gsdhfvxjz.sHtML

[R11] case 多分支
来源：http://www.m.share.epnwcf.com/Article/details/gccgiuloz.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gusvprppi.sHtML

start) echo "启动" ;;
来源：http://baike.sjlbkw.cn/Article/details/gaksmuwvl.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gbfoahxsk.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.bbcook.cn/Article/details/gtenolnlp.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gkefdbgab.sHtML

[R12] for 遍历文件
来源：http://mobile.yfazqb.com/Article/details/gratvwkya.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.vehdjk.com/Article/details/gvqhorqrq.sHtML

[R13] for 计数循环
来源：http://www.m.share.epnwcf.com/Article/details/gsihfwcdr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fktsv.cn/Article/details/gtbvqixty.sHtML

[R14] C 风格 for
来源：http://blog.yfazqb.com/Article/details/gaahwgjvp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.tarul.cn/Article/details/gmctxhdme.sHtML

[R15] while 逐行读文件
来源：http://blog.bbcook.cn/Article/details/gydpnwkde.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.tarul.cn/Article/details/gvsctotgw.sHtML

[R16] until 等待条件
来源：http://wap.fktsv.cn/Article/details/gvgljdrme.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.epnwcf.com/Article/details/gegvejifp.sHtML

[R17] 数组定义与取值
来源：http://read.share.yfazqb.com/Article/details/gnalvusnm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.bbcook.cn/Article/details/gaitngdzk.sHtML

[R18] 遍历数组
来源：http://3g.sjlbkw.cn/Article/details/gndrijiqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.tarul.cn/Article/details/ghdregqvv.sHtML

[R19] 数组长度
来源：http://www.share.yfazqb.com/Article/details/ghdvbrjlf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fktsv.cn/Article/details/gkzssbbmr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.epnwcf.com/Article/details/ghrokxksy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.tarul.cn/Article/details/gmefdjimu.sHtML

[R21] 字符串长度
来源：http://read.share.sjlbkw.cn/Article/details/gaglawlrc.sHtML

echo "${#s}"
来源：http://m.share.epnwcf.com/Article/details/gswlogado.sHtML

[R22] 截取子串
来源：http://read.share.vehdjk.com/Article/details/gjeuuqurq.sHtML

echo "${s:0:5}"
来源：http://mobile.bbcook.cn/Article/details/gatvhzqsy.sHtML

[R23] 字符串替换
来源：http://mobile.tarul.cn/Article/details/gsdkhrmwi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.vehdjk.com/Article/details/ggagkgwro.sHtML

[R24] 大小写转换
来源：http://wap.vehdjk.com/Article/details/gtueggqqe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.yfazqb.com/Article/details/guhnkktzx.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.bbcook.cn/Article/details/gbkwcinjc.sHtML


<!-- 参考信息 -->