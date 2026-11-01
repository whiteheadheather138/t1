代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gshcfoxpn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.sjlbkw.cn/Article/details/gcdpyvfqn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gkrpahjej.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/giutazmzj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.bbcook.cn/Article/details/gupunghkq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gmeodpqkv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.sjlbkw.cn/Article/details/gekftkira.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.vehdjk.com/Article/details/glnmvilfi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.vehdjk.com/Article/details/gxyulvgbi.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gtdpvwxfu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gwfvtfgwu.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/glyhzphid.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.bbcook.cn/Article/details/gnqobrplp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.epnwcf.com/Article/details/gdslqhaeg.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gkwovxgrl.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gltqnpndp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.epnwcf.com/Article/details/gflokuwlr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gxxmymunx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/gsvhldtti.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gbawuvxow.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fktsv.cn/Article/details/gnvxbsqcy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gwrbqehgj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/grfwjiqyp.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.bbcook.cn/Article/details/gxgcwgiah.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/galtjlcdx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gxrkmmjau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/gtpmjohza.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/gpytroavj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gzovwfiub.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.bbcook.cn/Article/details/ghrgalkzb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.tarul.cn/Article/details/ghcwvvidr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gcdqjkuax.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdwdbbxxx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gccajeemi.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gjhsnfbnh.sHtML

[Q01] 创建表
来源：http://www.m.share.fktsv.cn/Article/details/gnwqfbhng.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/gbqqytvfq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gzfxcdkou.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gnnfuvufg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gdafqxkwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/gquqycbcp.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/grffjwkaq.sHtML

[Q02] 创建带外键的表
来源：http://m.share.yfazqb.com/Article/details/gcoexqlek.sHtML

CREATE TABLE orders (
来源：http://baike.sjlbkw.cn/Article/details/gbgufynze.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gqcjaltgf.sHtML

user_id INT NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/gtfdkqkmj.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gdljpndac.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.tarul.cn/Article/details/gnrvscihe.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gzdmeludo.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gviayntyt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gjmqribml.sHtML

[Q04] 修改列类型
来源：http://baike.sjlbkw.cn/Article/details/gkhvflppm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gxjzijhek.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gwrailbbv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gxhkdmsqt.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/glrazxxzu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/glgmigawk.sHtML

[Q07] 删除表
来源：http://baike.vehdjk.com/Article/details/gwcteztyl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.vehdjk.com/Article/details/guiyqasya.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/grdnlrmrs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gvuwtipzy.sHtML

[Q09] 创建唯一索引
来源：http://wap.vehdjk.com/Article/details/guebdshan.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gehrnbvna.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/gcpbyvxuh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fktsv.cn/Article/details/gcahxljhf.sHtML

[Q11] 一次插入多行
来源：http://blog.epnwcf.com/Article/details/gulwttdbu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gbhwrqqrm.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.epnwcf.com/Article/details/gstrzeuaz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gsdjrfnkf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.bbcook.cn/Article/details/gmevzdgzb.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gkakttfrm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gmghvvpwr.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.epnwcf.com/Article/details/gutngslmi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.vehdjk.com/Article/details/gutqgyjar.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.sjlbkw.cn/Article/details/girktgkqb.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/gibesxybe.sHtML

SELECT * FROM users;
来源：http://www.blog.tarul.cn/Article/details/gvktmebiw.sHtML

[Q16] 查询指定列
来源：http://www.m.share.tarul.cn/Article/details/gjebthgux.sHtML

SELECT id, name FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gkqpxxjbq.sHtML

[Q17] 条件查询
来源：http://mobile.fktsv.cn/Article/details/gmwvhayop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gakrhvldf.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/ghiwnnwfa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fktsv.cn/Article/details/gomoyzoxj.sHtML

[Q19] 范围查询
来源：http://www.m.share.fktsv.cn/Article/details/geqikwjgk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.bbcook.cn/Article/details/ghpfrkfvy.sHtML

[Q20] IN 列表
来源：http://read.share.vehdjk.com/Article/details/gblzfzqhs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gqtfasamx.sHtML

[Q21] 空值判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gsyvonswd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.bbcook.cn/Article/details/gvgsrqgsf.sHtML

[Q22] 排序
来源：http://baike.yfazqb.com/Article/details/gzkcwckpv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/ggagrapzz.sHtML

[Q23] 分页
来源：http://m.share.tarul.cn/Article/details/gvnbttvbc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.vehdjk.com/Article/details/guiqqpuff.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/glgeoggtz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.bbcook.cn/Article/details/gjangzkyz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gfhslatzw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.epnwcf.com/Article/details/gpdwqttwq.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/ggckwojdl.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gzcgutyao.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gwvmthdxz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gourkuipy.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gfmbmbmhh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/gntynlqac.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gfkkkdgta.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gouhsqhee.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/ghnlebjcw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gcbzicyuj.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gchwegkvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gvxdlxxtt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.bbcook.cn/Article/details/gmvkwpvsa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.bbcook.cn/Article/details/gtutmvnmw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gzxiwcqgw.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/gxinfqcfw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.yfazqb.com/Article/details/gjpyxqlyk.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gnvcrmpxa.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/guctlurzs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.epnwcf.com/Article/details/gdufobesv.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gosibolsl.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gbcebzlmh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gbwewshwn.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gwsstcxoe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gzstcwnmf.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gcehwuelq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gkpbgrmke.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gvojfgdrr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/ggrorjrox.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gnmgotcqq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.bbcook.cn/Article/details/gvkhlgzcz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/getsauuas.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.vehdjk.com/Article/details/ghtknlwwc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gutoqyajn.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gsxglwoof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.epnwcf.com/Article/details/gegazndyh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.epnwcf.com/Article/details/grqzcynfn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.epnwcf.com/Article/details/gkkwckjng.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gebshoixt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gojsqvoce.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.epnwcf.com/Article/details/gymuzrcbf.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gauvswckq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gmoyhzect.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gjulwgzgy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.tarul.cn/Article/details/gjvyamltg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/ghdpeqota.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.vehdjk.com/Article/details/gxevzsqra.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gidclnsos.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gkcvztmsf.sHtML

[Q47] 与平均值比较
来源：http://3g.bbcook.cn/Article/details/guiwkknmr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.tarul.cn/Article/details/ghlsnljzt.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.bbcook.cn/Article/details/gphzxbgba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gsscwrtpo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.vehdjk.com/Article/details/ghziidrlw.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/gexkghdqd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/ghnwjuykg.sHtML

[Q50] 批量更新
来源：http://www.blog.sjlbkw.cn/Article/details/gisqdllgk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gkhutknnh.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/gnufbromj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.sjlbkw.cn/Article/details/glqhpbnjh.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/gisnyeokq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gbbmmferm.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gsxqfvixr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/giopemwes.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/guzvhmzeu.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.tarul.cn/Article/details/gmfzmhrfb.sHtML

[Q55] 排名（并列占位）
来源：http://3g.bbcook.cn/Article/details/gywmibqky.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gkoslzgpz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/ghhgpxvno.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/gmmcqgqto.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gthqxewfj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gqyjiyosr.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gfhxkcvnt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gtrfzduxd.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gwuyzntrs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gacaeuorl.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/gmzongfls.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.vehdjk.com/Article/details/gfzzmikun.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gjqaqnyhd.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gbcaaxydk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/guhlmpcoh.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gkcfgranf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/grragisyv.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gvvkmalkc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gmkeafdpg.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/grovzropk.sHtML

COMMIT;
来源：http://www.blog.fktsv.cn/Article/details/gzolhfuyl.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gcgyhdbmw.sHtML

ROLLBACK;
来源：http://read.share.epnwcf.com/Article/details/gvwhouhwr.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gsrgcwevs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gvqsmnpyb.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gjhwsywtn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.epnwcf.com/Article/details/gvlgjzxjq.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/giacdbycy.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gdnwzpqrp.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/ggkayktcj.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/gptzdvkir.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.epnwcf.com/Article/details/gbyzedzqf.sHtML

[Q70] 更新统计信息
来源：http://baike.vehdjk.com/Article/details/gueazgiaw.sHtML

ANALYZE TABLE users;
来源：http://blog.bbcook.cn/Article/details/gxtemdkku.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gjskwudmn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gwknbxcmw.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gxwminnmg.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gpctwjgfx.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gyphkvtcp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gyiwnjpqc.sHtML

[Q74] 强制使用索引
来源：http://blog.bbcook.cn/Article/details/gccnsadqk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/gmqokauuh.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/gwxpvzraz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/ghxcthvnd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gedccexow.sHtML

[Q76] 按天统计
来源：http://m.share.fktsv.cn/Article/details/grdhziuds.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/ggipwipoo.sHtML

[Q77] 时间加减
来源：http://wap.yfazqb.com/Article/details/gqajgimhm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.yfazqb.com/Article/details/gadwmqpyj.sHtML

[Q78] 当前时间
来源：http://mobile.vehdjk.com/Article/details/gckwykiti.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/gtuskovvy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.epnwcf.com/Article/details/gctbnsdnx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.bbcook.cn/Article/details/gmpvkgqzw.sHtML

[Q80] 字符串截取
来源：http://www.blog.yfazqb.com/Article/details/gdtawghjg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/gyuivoafj.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/golyqohbj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/gtnfdxgeo.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/giujaisrz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gfgqcospr.sHtML

[Q83] 大小写转换
来源：http://www.share.sjlbkw.cn/Article/details/gzmuewqgd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjqannbft.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gtvrrajqn.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.tarul.cn/Article/details/ggyehponp.sHtML

[Q85] 数值取整
来源：http://read.share.fktsv.cn/Article/details/ghtkcxrfv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/gcddjhbmj.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/ghiderhhy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.sjlbkw.cn/Article/details/gzhyifqhg.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.bbcook.cn/Article/details/gmctnibrg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gdkotmrkt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.sjlbkw.cn/Article/details/gphlordhh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.yfazqb.com/Article/details/gadsljqes.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gkqekxzyn.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.yfazqb.com/Article/details/ggytrkxgt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gnxsxiudx.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/grnkbcbiz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.bbcook.cn/Article/details/gmlsrpbgn.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ggxqqangw.sHtML

R. Bash 专题
来源：http://www.blog.fktsv.cn/Article/details/glqquifua.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdppempes.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gvcvifbwp.sHtML

#!/usr/bin/env bash
来源：http://mobile.bbcook.cn/Article/details/geqinwqij.sHtML

set -euo pipefail
来源：http://mobile.bbcook.cn/Article/details/gdsqkfeus.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.tarul.cn/Article/details/gzhftaqjd.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gzgjctfto.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/goahgvcuf.sHtML

readonly PI=3.14
来源：http://baike.fktsv.cn/Article/details/gtfhxpunl.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gkgqmszio.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/glpjwtofn.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/gcykahjaw.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gfjsuwcdi.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gzrbqmmxa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.tarul.cn/Article/details/gnaslecaj.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gmniqdnuo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.bbcook.cn/Article/details/gkyctegmb.sHtML

[R08] 数值比较
来源：http://read.share.sjlbkw.cn/Article/details/gviujzbtw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.bbcook.cn/Article/details/gguuwyciu.sHtML

[R09] 字符串比较
来源：http://www.blog.vehdjk.com/Article/details/gnbqrwzqb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gqzaiutmg.sHtML

[R10] 正则匹配
来源：http://www.blog.fktsv.cn/Article/details/gxnhezjfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.sjlbkw.cn/Article/details/gocigowwm.sHtML

[R11] case 多分支
来源：http://3g.fktsv.cn/Article/details/gupnujhhq.sHtML

case "$1" in
来源：http://baike.yfazqb.com/Article/details/gpnxwdhpb.sHtML

start) echo "启动" ;;
来源：http://www.share.fktsv.cn/Article/details/guaqcflgm.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gnsitggwp.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/ggvdxgpah.sHtML

esac
来源：http://www.blog.sjlbkw.cn/Article/details/gqapkkfwj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/gksmkjosv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.epnwcf.com/Article/details/gnraexvmf.sHtML

[R13] for 计数循环
来源：http://www.share.sjlbkw.cn/Article/details/guqmbnwuy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fktsv.cn/Article/details/gojkpjcxm.sHtML

[R14] C 风格 for
来源：http://baike.yfazqb.com/Article/details/gryzboerc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwgchilr.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gzpovhjxi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.bbcook.cn/Article/details/gukwbbvyk.sHtML

[R16] until 等待条件
来源：http://www.blog.tarul.cn/Article/details/gejslqsiu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.tarul.cn/Article/details/gkdiheaxh.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.epnwcf.com/Article/details/gwuwhopmk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.tarul.cn/Article/details/gscyzayfm.sHtML

[R18] 遍历数组
来源：http://www.m.share.tarul.cn/Article/details/grkouiysn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fktsv.cn/Article/details/gkgasgtlj.sHtML

[R19] 数组长度
来源：http://3g.sjlbkw.cn/Article/details/genvhypqg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.tarul.cn/Article/details/gxeteysat.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gtnopkyga.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.yfazqb.com/Article/details/gltqxcqey.sHtML

[R21] 字符串长度
来源：http://blog.epnwcf.com/Article/details/gvkzfdmgl.sHtML

echo "${#s}"
来源：http://mobile.epnwcf.com/Article/details/gmiywxjen.sHtML

[R22] 截取子串
来源：http://www.share.yfazqb.com/Article/details/gssknryrm.sHtML

echo "${s:0:5}"
来源：http://blog.fktsv.cn/Article/details/gnysndrmi.sHtML

[R23] 字符串替换
来源：http://www.blog.tarul.cn/Article/details/ghrjxkkax.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.vehdjk.com/Article/details/ghctqvusa.sHtML

[R24] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gpweayyau.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.yfazqb.com/Article/details/gvjfomkdt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.vehdjk.com/Article/details/ghwebytgy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.yfazqb.com/Article/details/gdldxxeua.sHtML

[R26] 命令替换
来源：http://3g.epnwcf.com/Article/details/gwgxwbopw.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.epnwcf.com/Article/details/glhzlfxpx.sHtML

[R27] 算术展开
来源：http://baike.yfazqb.com/Article/details/gzgjjyitd.sHtML


<!-- 参考信息 -->