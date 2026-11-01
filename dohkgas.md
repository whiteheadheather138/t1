代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.sjlbkw.cn/Article/details/gnjrdumya.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/goyhllxzk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gkmdfzlzs.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gidcivqlg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/girospuyo.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gxcdfdcfx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/ghrowoluf.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gjdekmifm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gdyjhjrjm.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gnpsrtxql.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gsofpbqwg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/ghzfpxpzx.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gbqylkgcs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gtiajwhfu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gdhcgwack.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/ghcfoxuyd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gdbjcwtge.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gfqnxqenm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.tarul.cn/Article/details/gvvdrkkfd.sHtML

[P08] 处理浮点精度问题
来源：http://3g.vehdjk.com/Article/details/gzqseimnt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gymcnkfpf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/ggbrzyybi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.epnwcf.com/Article/details/gaftlcvbv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gnntcidou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.sjlbkw.cn/Article/details/glbjgzkba.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gdiuouzji.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.bbcook.cn/Article/details/gvhbkreou.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gjwcrmnvq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfingecqk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gdfopmekv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsmxwmvgc.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gsxyffuae.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gnmemvots.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gkxrzwsee.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gpklzggyn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.yfazqb.com/Article/details/gitgwmgwq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/ghhipalon.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gybhzjwwm.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fktsv.cn/Article/details/gkjgkhfox.sHtML

CREATE TABLE orders (
来源：http://read.share.bbcook.cn/Article/details/geznmrzhn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gzjpwlcha.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gfncjjpbq.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/gnmukickp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.yfazqb.com/Article/details/gdylbopms.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gnshhoxfp.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gzpehjwar.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gfakgeffn.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/gqmamglnq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/geqgjhnjt.sHtML

[Q05] 重命名列
来源：http://baike.tarul.cn/Article/details/grlfgtozv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gqftpmerd.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gadvklqxt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/govnecjlv.sHtML

[Q07] 删除表
来源：http://mobile.sjlbkw.cn/Article/details/glxcmzdnu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.vehdjk.com/Article/details/gwrqjcxvw.sHtML

[Q08] 创建普通索引
来源：http://www.blog.fktsv.cn/Article/details/gzvfancnc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/glpctdbuj.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/guderauhv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/guzsaqbgo.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gzutxppjb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/ghogngpfc.sHtML

[Q11] 一次插入多行
来源：http://m.share.vehdjk.com/Article/details/gwcpgopio.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gouxbkbpc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gbtqvpdpt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/grmnbzfre.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/gvkrrgypl.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/ghskphajq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/ggzhvjzjb.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.vehdjk.com/Article/details/gctbbmvvq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.yfazqb.com/Article/details/gxyydlton.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/gzmdcaieb.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gjqufabac.sHtML

SELECT * FROM users;
来源：http://www.share.vehdjk.com/Article/details/guokjccvz.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gessmhmrp.sHtML

SELECT id, name FROM users;
来源：http://baike.fktsv.cn/Article/details/glljmbdij.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/ggsyrpzub.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.tarul.cn/Article/details/gmhtvcxun.sHtML

[Q18] 模糊匹配
来源：http://read.share.vehdjk.com/Article/details/gjsivhigz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gcxghyfes.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gxicywrse.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/ggvlnkodn.sHtML

[Q20] IN 列表
来源：http://mobile.vehdjk.com/Article/details/gugyyndvt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gonoujdiy.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gvaamnppq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gdfqgelbv.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/gfamrbrpe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/goujeydtu.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gwdrvohad.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gzoukboez.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gnfjunmts.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/ggtmrgcoz.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gtexpcjvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fktsv.cn/Article/details/gkilkwetm.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gkgympefu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gjbkvpdep.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gclsxqitu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gtoknuegq.sHtML

[Q28] 求和与平均
来源：http://www.share.yfazqb.com/Article/details/gkdilihbf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/glvmzhhss.sHtML

[Q29] 最大最小值
来源：http://blog.vehdjk.com/Article/details/gwowpwhrv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gbpxkmuai.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gtzwjlxvf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gmgyxjoxx.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gfmhewzvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gvotyxniw.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.epnwcf.com/Article/details/gfxgjbrgj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gnvskpbkv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.vehdjk.com/Article/details/gmybinvkz.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gloeksjkr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.tarul.cn/Article/details/gxwtswlfa.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gkqdoqddc.sHtML

SELECT * FROM (
来源：http://baike.tarul.cn/Article/details/gptiwnlsh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fktsv.cn/Article/details/gfiqmdipk.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/grvswpkre.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gqgmpxtet.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/grzuksvxl.sHtML

[Q36] 左连接
来源：http://baike.yfazqb.com/Article/details/gagydhify.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gvnvkryrz.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gswtgfdfv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/geluhlmfk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gfcinbver.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.vehdjk.com/Article/details/gkpmpmzwg.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/ghiuolcru.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhcpnyeq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.sjlbkw.cn/Article/details/gpbnzrzsw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gxoqzrbrc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gzafypkyz.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gmsrbpmbr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/gpfzmyuwl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.vehdjk.com/Article/details/gwwwhgcsw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gforowndn.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.tarul.cn/Article/details/gwcljhjfw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gwaoogldx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gwnoadzsf.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gsfgeabyr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gimlhhpge.sHtML

[Q44] IN 子查询
来源：http://m.share.fktsv.cn/Article/details/gzvzspubl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.tarul.cn/Article/details/gcaxlmwgd.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/gsvucnfbn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.tarul.cn/Article/details/gvskcltxi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/ggvsvhbla.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gpfnuvecx.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gedvxfgga.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gjmgtzfwl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gdikiahqe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.epnwcf.com/Article/details/gmqgfmbwd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gpksixmmb.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/gkoqjowpi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gnmdyeboi.sHtML

[Q50] 批量更新
来源：http://blog.fktsv.cn/Article/details/gzwaysuii.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gfflcrusb.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gnqxhkxdh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gslesxlmz.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gwymttjpn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gwouqlqvl.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gpfpjmifc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.vehdjk.com/Article/details/gescbtmgt.sHtML

[Q54] 清空表
来源：http://www.blog.tarul.cn/Article/details/gzfpnyypr.sHtML

TRUNCATE TABLE logs;
来源：http://wap.tarul.cn/Article/details/ghansuzrl.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gpzifubko.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gxcqexcmo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggylouakc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gdkftnkbb.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gqxqemzes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gzzmydztl.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/glmpkjclf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gkkmenuoe.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/gxkpzeelg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gzbwzynxk.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fktsv.cn/Article/details/gjxcbueuu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gekrlkmbl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/ggznmbkzz.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gjypgdvgg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gfslrvkay.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gsguvivjk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/ggjtupfzc.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/gkdydlyvr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/geqoixtww.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gtweruqhi.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/gqjdxuzks.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gtkrhekhf.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/gxdhaksdj.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gxksohzpq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.epnwcf.com/Article/details/gtrdmyvid.sHtML

[Q67] 设置隔离级别
来源：http://www.share.tarul.cn/Article/details/gmkircrur.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gyblszlyt.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/gzrdtucbb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gseuwglpw.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/grcpiqzwl.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/gcerlxwhi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/godhllxsf.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/goyhccjhn.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gxdjkjtyy.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gdsbeuhgs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/giqoexbyk.sHtML

[Q72] 查看索引
来源：http://www.share.yfazqb.com/Article/details/gsruwftkv.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/ggxqdryqi.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gwynyzupa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gyfrsvwwx.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/gsmtudmmz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gsiuovqju.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/glpjiricv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/gdnapghfc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gzpdchjxc.sHtML

[Q76] 按天统计
来源：http://wap.yfazqb.com/Article/details/gipvagfde.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/ggdifimcw.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gnmtcjeki.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gofaryucr.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gmqrgnmen.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fktsv.cn/Article/details/gfuagmpwg.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gerqrzecf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/ggmuwghfr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.tarul.cn/Article/details/gfuixkegj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/giyranyiu.sHtML

[Q81] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gqjmujfvy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gwtrivkaq.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/geeqppxmc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/gyhoffflp.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/ghqiqpzzb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gxvzkquvt.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gkgikygtb.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ggoktimbo.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/glnghewnv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gyzdfedxk.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.tarul.cn/Article/details/gfkvdmeal.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gxwquxcep.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gukidderp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fktsv.cn/Article/details/gctuhllxq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.tarul.cn/Article/details/gklxagzhi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gduyhgqke.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/ggrqagbna.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gvxqcozbd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/gymdojzpl.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gcerfqrbn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.epnwcf.com/Article/details/glrqtzzca.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfjkguait.sHtML

R. Bash 专题
来源：http://mobile.epnwcf.com/Article/details/geneglebg.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gebfhpbca.sHtML

[R01] shebang 与严格模式
来源：http://read.share.vehdjk.com/Article/details/gqrocdzwj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.epnwcf.com/Article/details/ghhdxndlj.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gblczrhab.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/grkyepybm.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/gqupwqtxq.sHtML

[R03] 只读变量
来源：http://m.share.fktsv.cn/Article/details/gsycniwkg.sHtML

readonly PI=3.14
来源：http://www.share.bbcook.cn/Article/details/gjrvbbqni.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gmjkwwosl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.bbcook.cn/Article/details/gtlpdidlw.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/grgldkvgg.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gnijgtzha.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/gbygqhchx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gjzfrvaiq.sHtML

[R07] if 判断文件
来源：http://blog.fktsv.cn/Article/details/giytuzxhw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/guqoswyqs.sHtML

[R08] 数值比较
来源：http://3g.yfazqb.com/Article/details/gseanhwhi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.epnwcf.com/Article/details/goozkdjif.sHtML

[R09] 字符串比较
来源：http://3g.bbcook.cn/Article/details/gsodcjsvf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/ghluljtgt.sHtML

[R10] 正则匹配
来源：http://mobile.bbcook.cn/Article/details/gwljtuynx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gincentye.sHtML

[R11] case 多分支
来源：http://baike.tarul.cn/Article/details/guewbpmhz.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gonhwjhcv.sHtML

start) echo "启动" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gjiuejrai.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gweesvizq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.tarul.cn/Article/details/gzmnyhapq.sHtML

esac
来源：http://www.share.fktsv.cn/Article/details/gdaownhbv.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gnmnybefa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gvpbbhhjv.sHtML

[R13] for 计数循环
来源：http://www.m.share.tarul.cn/Article/details/gavyjitct.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fktsv.cn/Article/details/gvjqaxzbh.sHtML

[R14] C 风格 for
来源：http://baike.epnwcf.com/Article/details/glqwcxfmz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.epnwcf.com/Article/details/gxynzbhpn.sHtML

[R15] while 逐行读文件
来源：http://mobile.yfazqb.com/Article/details/gdepzwerz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fktsv.cn/Article/details/govcvbmky.sHtML

[R16] until 等待条件
来源：http://m.share.fktsv.cn/Article/details/gdsliavky.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.sjlbkw.cn/Article/details/gomsqwrjt.sHtML

[R17] 数组定义与取值
来源：http://wap.tarul.cn/Article/details/gqntyfkmn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.yfazqb.com/Article/details/ggegyjwbz.sHtML

[R18] 遍历数组
来源：http://3g.fktsv.cn/Article/details/glzlncqod.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.tarul.cn/Article/details/grulqsiyi.sHtML

[R19] 数组长度
来源：http://www.share.fktsv.cn/Article/details/gssscrymf.sHtML

echo "${#arr[@]}"
来源：http://mobile.sjlbkw.cn/Article/details/gpuykagqi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.vehdjk.com/Article/details/gnxcftpmc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.bbcook.cn/Article/details/gwchmglij.sHtML

[R21] 字符串长度
来源：http://www.share.epnwcf.com/Article/details/ggnvwhglq.sHtML

echo "${#s}"
来源：http://mobile.tarul.cn/Article/details/gauhaygee.sHtML

[R22] 截取子串
来源：http://blog.epnwcf.com/Article/details/gxeymxmov.sHtML

echo "${s:0:5}"
来源：http://read.share.tarul.cn/Article/details/gzkqmdobx.sHtML

[R23] 字符串替换
来源：http://m.share.bbcook.cn/Article/details/gfbwkvwbt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fktsv.cn/Article/details/glghbzttl.sHtML

[R24] 大小写转换
来源：http://www.blog.yfazqb.com/Article/details/grqlgffnj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.vehdjk.com/Article/details/gmaticohn.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fktsv.cn/Article/details/gotidhaor.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.yfazqb.com/Article/details/gdetnatvv.sHtML

[R26] 命令替换
来源：http://read.share.sjlbkw.cn/Article/details/gerotknyj.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fktsv.cn/Article/details/gatjounqy.sHtML

[R27] 算术展开
来源：http://www.share.fktsv.cn/Article/details/gtrsfzqna.sHtML

echo $((1 + 2 * 3))
来源：http://blog.yfazqb.com/Article/details/gugzpvyjf.sHtML

[R28] 浮点运算
来源：http://3g.sjlbkw.cn/Article/details/gkmmkhyvt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.vehdjk.com/Article/details/gythkoicp.sHtML

[R29] 定义函数
来源：http://blog.fktsv.cn/Article/details/gevgsznmg.sHtML


<!-- 参考信息 -->