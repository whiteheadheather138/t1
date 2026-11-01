代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://wap.sjlbkw.cn/Article/details/gkbtenotg.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gqscksynv.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gnydktxrf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gwlbuujxw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.epnwcf.com/Article/details/gfmsexgix.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/gxkvpttxw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.sjlbkw.cn/Article/details/ghspylnvp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/gihleyeln.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gnagwdssa.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gkmagzguv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.tarul.cn/Article/details/gebqcvzms.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/gtdsqdgwt.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gzfifvyrm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/gtqdjfhqq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.vehdjk.com/Article/details/gtanlujrb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/gmgfeemkl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gempkxrde.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gthpqwtvy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gvnpjcwcw.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/ghgohrszz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gleoqgfhw.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/giomytwyy.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgrzbatt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gtstvvjkk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.yfazqb.com/Article/details/gkcdfvcfx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gmhsmzqjb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/guwbqjqwc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.tarul.cn/Article/details/gctwjcues.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.vehdjk.com/Article/details/gqudzzuqf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.tarul.cn/Article/details/gibtugbqz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gdrsvhqmc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/ghkllvwtj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gaqtylsrt.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.bbcook.cn/Article/details/gyddyqwdg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gsfgvnwpl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gpogeztfv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gtrgvhtkm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.tarul.cn/Article/details/gtmcydifi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/grgjvxige.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gpaccbecl.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/golbijvpf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gzzbvfmbe.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbvrqnzlc.sHtML

[Q01] 创建表
来源：http://www.blog.fktsv.cn/Article/details/gktjdasct.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/giouanzij.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/gpmwurzze.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/ggcahlfyi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gxaczfhnw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gnmypjzob.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gvvvsrzyc.sHtML

[Q02] 创建带外键的表
来源：http://m.share.bbcook.cn/Article/details/gkhvonflo.sHtML

CREATE TABLE orders (
来源：http://www.m.share.bbcook.cn/Article/details/gmgwnxean.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gnjshfwiw.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gwexujqdy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/gfldqkhaj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gljzxlhbn.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gpsmetnvz.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gydupifrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.sjlbkw.cn/Article/details/ggugppuer.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gtlzysehh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/ghjqoqmgc.sHtML

[Q05] 重命名列
来源：http://m.share.epnwcf.com/Article/details/gdrdjiwrf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/grjmkmdtm.sHtML

[Q06] 删除列
来源：http://www.m.share.tarul.cn/Article/details/gksherimc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gdsqiydhm.sHtML

[Q07] 删除表
来源：http://www.share.sjlbkw.cn/Article/details/gylxrpeyd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.vehdjk.com/Article/details/gsihcsxjl.sHtML

[Q08] 创建普通索引
来源：http://www.share.epnwcf.com/Article/details/ggmmtmuzs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gxahfmtsc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/grmanynxd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fktsv.cn/Article/details/ghygovmyd.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gqgfubwxe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gcryhgoif.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gkwunubfi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gtejilijl.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/glxjwlhal.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/gqxzdovkw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gahwbwwir.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gafqydyaj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gliswupth.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/geypbhtyi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/ghzimkptm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/guivucnmt.sHtML

[Q15] 查询全部
来源：http://mobile.fktsv.cn/Article/details/gcyqyeivn.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gbrxhahqk.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gnbhdcrpn.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/gshufvdov.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gkndlyyda.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/gekkcabtb.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gipnlsxwl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.bbcook.cn/Article/details/gzlbdjrhl.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gtqlsnpcj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.vehdjk.com/Article/details/ghrcmwiol.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/gywpfnatk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.fktsv.cn/Article/details/gtgqfmxum.sHtML

[Q21] 空值判断
来源：http://read.share.fktsv.cn/Article/details/gswgbvnpt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gurxphnbu.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gnzcvxdpq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.yfazqb.com/Article/details/gwkxwruyc.sHtML

[Q23] 分页
来源：http://www.share.yfazqb.com/Article/details/gtzrybaml.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gjxpxazvn.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gptjhzzrg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gouplbjkh.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gcfjsdzte.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.bbcook.cn/Article/details/gqekwylhz.sHtML

[Q26] 计数
来源：http://wap.yfazqb.com/Article/details/gdejlsola.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gmontfqee.sHtML

[Q27] 条件计数
来源：http://read.share.tarul.cn/Article/details/gpumwvtsq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.vehdjk.com/Article/details/gdgxcbuzn.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gronfgktk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gngcaoryz.sHtML

[Q29] 最大最小值
来源：http://www.m.share.sjlbkw.cn/Article/details/gulnzgoeg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gvasxtdys.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gzjfkgyob.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gkonpxkut.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gilvywqtq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.vehdjk.com/Article/details/guytoinbo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gbzntchtr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gubntcrhf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/glycfszji.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/ghlgjqhit.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fktsv.cn/Article/details/geissqvaa.sHtML

[Q34] 每组取第一条
来源：http://blog.tarul.cn/Article/details/gwhfbrfjo.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/gviqjkvgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/gsjlvynnt.sHtML

) t WHERE rn = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gaajiaaqt.sHtML

[Q35] 内连接
来源：http://mobile.vehdjk.com/Article/details/gqbifmeox.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gltjvgwhm.sHtML

[Q36] 左连接
来源：http://3g.fktsv.cn/Article/details/gqmzrtnvw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.tarul.cn/Article/details/gytecyzcv.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gniurcoqu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gknzztyqo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gcejezyee.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/gttfkmdln.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/gwsvpzmlm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gojgciqgf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.bbcook.cn/Article/details/gszswcrsx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/ggrwxoqof.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/gafnchxje.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gzwbksjal.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/gougozwkl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.bbcook.cn/Article/details/gqtmhkijd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/gsocveofz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.tarul.cn/Article/details/gfwcteegb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.epnwcf.com/Article/details/gbtiuooal.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gdwdspysm.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/glfupuweh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.vehdjk.com/Article/details/gnwbqlrqy.sHtML

[Q44] IN 子查询
来源：http://blog.sjlbkw.cn/Article/details/gcxbfjria.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gcyhfpwdu.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gqckhycjs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gfzeourim.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/ggbaeitfy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gcbdmhnrc.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/gvqqwgmvz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gccwdlzlo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gbqmkhidb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.epnwcf.com/Article/details/gbvtozcib.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gkfavizqk.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/gillogpsb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/goyjlyngj.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gmfrixzum.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.epnwcf.com/Article/details/gqfoiygug.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gwcxqczhs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gwrwptlbu.sHtML

[Q52] 删除指定行
来源：http://www.blog.yfazqb.com/Article/details/gaynoqbkt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gxxlobzjt.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/geazfetkh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gonytdloq.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gacakzkgs.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gbncuplsy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gobnmwxqo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/gfaonxnzg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gjjnrgyhj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/giemrivzy.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gspplaakz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gxvcvsllq.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/geqyiarbw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gpesdybxu.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gqieoqwwn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gonmklbne.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/geoibulmq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.epnwcf.com/Article/details/gemeuiudd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gkdzytcyc.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/glaobxrtr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.tarul.cn/Article/details/gvqbzlifr.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gzbfsclxa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gzlqbbput.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gabgflssl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/gkvaxkgad.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/gdcyrmgmz.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gyuvjpupk.sHtML

[Q65] 回滚事务
来源：http://3g.tarul.cn/Article/details/glasozsuz.sHtML

ROLLBACK;
来源：http://www.m.share.bbcook.cn/Article/details/gyfchrnog.sHtML

[Q66] 行锁查询
来源：http://www.blog.sjlbkw.cn/Article/details/gbgayksnv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gtctcsefe.sHtML

[Q67] 设置隔离级别
来源：http://wap.yfazqb.com/Article/details/gdhkuhtnt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.epnwcf.com/Article/details/gaemginia.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gdvtlazpz.sHtML

SAVEPOINT sp1;
来源：http://3g.fktsv.cn/Article/details/geiipdqtb.sHtML

ROLLBACK TO sp1;
来源：http://3g.vehdjk.com/Article/details/gpnfexwdg.sHtML

[Q69] 查看执行计划
来源：http://3g.tarul.cn/Article/details/gqlalmvta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/glyestfam.sHtML

[Q70] 更新统计信息
来源：http://wap.sjlbkw.cn/Article/details/guhtrhgpi.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gintxcoba.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gmscrlkdf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gskwkdmnc.sHtML

[Q72] 查看索引
来源：http://mobile.sjlbkw.cn/Article/details/gscmuoefq.sHtML

SHOW INDEX FROM users;
来源：http://wap.yfazqb.com/Article/details/gxfqmjnpg.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gwsqpirke.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.sjlbkw.cn/Article/details/gkaddmwrb.sHtML

[Q74] 强制使用索引
来源：http://blog.fktsv.cn/Article/details/gtoqlonmp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fktsv.cn/Article/details/gevujtgjy.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gvtlpkfqg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gmmdxmxyb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.epnwcf.com/Article/details/gyktowfwf.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/gsvkfqttm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.yfazqb.com/Article/details/gzudwjyve.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gqdjiaszp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/gbbgezgqz.sHtML

[Q78] 当前时间
来源：http://3g.bbcook.cn/Article/details/gwjcexrcc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fktsv.cn/Article/details/gyeavtrnp.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/gveiqarvs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gkltatjkm.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gelqyztpw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gjxbpuiyy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.sjlbkw.cn/Article/details/givbrtija.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/ghgtyagvr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.epnwcf.com/Article/details/ghokfoltk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gbrenopxs.sHtML

[Q83] 大小写转换
来源：http://read.share.vehdjk.com/Article/details/ghuectsxn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghafhfked.sHtML

[Q84] 去除首尾空格
来源：http://wap.epnwcf.com/Article/details/gmwumgkfe.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/glhonayrx.sHtML

[Q85] 数值取整
来源：http://wap.yfazqb.com/Article/details/gpfaedkix.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/gheomceoe.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gjlvxkzyp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gvgaudsrw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/ghfmxougg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gfwtavgjb.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.sjlbkw.cn/Article/details/gcgffwaow.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gzgparwjy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.bbcook.cn/Article/details/gejcbvxib.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gtsekjhgi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.bbcook.cn/Article/details/gwckhzuas.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gkohpwdvv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gpprzigka.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gjuhbdnjt.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gitugsrjf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gwbnjpjge.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gbjagynzv.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gvyeruows.sHtML

set -euo pipefail
来源：http://wap.bbcook.cn/Article/details/gudmmbvzw.sHtML

[R02] 变量赋值与使用
来源：http://baike.tarul.cn/Article/details/gzupuftjo.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gguchdxcs.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gjpchxele.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gqklilpdb.sHtML

[R04] 位置参数
来源：http://wap.epnwcf.com/Article/details/gvgqctrgi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/gpdhmnfgu.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gzffjxhww.sHtML

name="${1:-default}"
来源：http://wap.epnwcf.com/Article/details/gwywjpypg.sHtML

[R06] 判断命令是否存在
来源：http://wap.yfazqb.com/Article/details/gjbheupzr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gpxdzcknw.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/grwisnnhn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.bbcook.cn/Article/details/gilecuwmu.sHtML

[R08] 数值比较
来源：http://wap.epnwcf.com/Article/details/gajpyeoki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gsrxknojb.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gdoqzeejh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gonsyvvbd.sHtML

[R10] 正则匹配
来源：http://blog.fktsv.cn/Article/details/gepojubkb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/gpzgrbmie.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gpyxqijou.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gvxamwxcu.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/gzlwllsmj.sHtML

stop)  echo "停止" ;;
来源：http://3g.yfazqb.com/Article/details/gwyuknxvl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.vehdjk.com/Article/details/gdipcxott.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gsoqqmrnx.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/geefzvrnh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.vehdjk.com/Article/details/guyecdovr.sHtML

[R13] for 计数循环
来源：http://mobile.vehdjk.com/Article/details/gqeekbwgf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/ghjecxbcl.sHtML

[R14] C 风格 for
来源：http://blog.yfazqb.com/Article/details/gcbnrgfwq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gjjofnygf.sHtML

[R15] while 逐行读文件
来源：http://m.share.vehdjk.com/Article/details/gfbusvcgm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.bbcook.cn/Article/details/gzhzbdytx.sHtML

[R16] until 等待条件
来源：http://www.m.share.bbcook.cn/Article/details/ghniixetq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fktsv.cn/Article/details/goxotjald.sHtML

[R17] 数组定义与取值
来源：http://read.share.sjlbkw.cn/Article/details/grhgskdtw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.epnwcf.com/Article/details/grikrjfdd.sHtML

[R18] 遍历数组
来源：http://blog.sjlbkw.cn/Article/details/gozofoxxw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.epnwcf.com/Article/details/gvferkaos.sHtML

[R19] 数组长度
来源：http://3g.tarul.cn/Article/details/gormnekkb.sHtML

echo "${#arr[@]}"
来源：http://baike.sjlbkw.cn/Article/details/gcqmixtkk.sHtML

[R20] 关联数组（字典）
来源：http://3g.fktsv.cn/Article/details/gephdjnlj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.epnwcf.com/Article/details/gvinvolmx.sHtML

[R21] 字符串长度
来源：http://3g.epnwcf.com/Article/details/gwvbzyttl.sHtML

echo "${#s}"
来源：http://blog.fktsv.cn/Article/details/gxzzzpyxg.sHtML

[R22] 截取子串
来源：http://www.m.share.vehdjk.com/Article/details/gbogtohps.sHtML

echo "${s:0:5}"
来源：http://www.m.share.sjlbkw.cn/Article/details/gyuvxqmnd.sHtML

[R23] 字符串替换
来源：http://blog.bbcook.cn/Article/details/gmcdluler.sHtML


<!-- 参考信息 -->