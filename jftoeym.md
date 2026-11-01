代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/ggqliykcc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.vehdjk.com/Article/details/gdfzhuiyg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gcoywmwtv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gohoumglf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/gqeuulrur.sHtML

Go:   len(arr);  len(m)
来源：http://3g.epnwcf.com/Article/details/gfaflcwfs.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gxkswcznw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gsxdxxshi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.sjlbkw.cn/Article/details/gfcnftilx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gtfnjyoxz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gczrqauvw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gnwhcjuke.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gvuedbhli.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gzjlkuref.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gzgpspamj.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gmcrczncz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.tarul.cn/Article/details/gerytiwwk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.vehdjk.com/Article/details/gajbwfqfv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fktsv.cn/Article/details/gptljvzfp.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/ghoxfflnk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gtlexpoio.sHtML

TS:   if (x == null) {}
来源：http://blog.tarul.cn/Article/details/gbncnrijg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gqcngwrkt.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gxinhofug.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/guvxwepji.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gnrnhyfbs.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gwpdodula.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gacsgacoo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.bbcook.cn/Article/details/gpbqifopt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gaxjwqecu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/grsrsqezr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fktsv.cn/Article/details/gqhaxjvia.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/ghlpqjcbm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/gvtujzqld.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/gwpnapezw.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.tarul.cn/Article/details/grskllgst.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/glfygaobo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gmvgemhsl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.epnwcf.com/Article/details/gmjzrulca.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gycsoerso.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/gfsnxdvmg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gkvjhvoip.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gonvxtqog.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/gphllnihn.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grropehiq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gwtxqlheu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/grhybljjn.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/gqeohuxzn.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gmusjjhlb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gtcipuuwy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.epnwcf.com/Article/details/grqavincu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.sjlbkw.cn/Article/details/glrphorxq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gwnkrnjju.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gdinrilni.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/giqbpeenj.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/ghsbknava.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/guesixhsp.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gyxjqonfk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/geopfzutv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/guorzvnwb.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gkelpcyol.sHtML

[Q03] 增加列
来源：http://m.share.bbcook.cn/Article/details/gqcxexyyy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.sjlbkw.cn/Article/details/genvsozcn.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gzijmgmtv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/geneqirpo.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gacbrzonv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gravclmia.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gslwkkceh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gpxvhibrn.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gtuibtblv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gljkyxucc.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gxnosdwrz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gteawnyuk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gvvnizjwv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/gsehqdlug.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gddkcumef.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gwqcmjllv.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/ggdsdmqgl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.vehdjk.com/Article/details/gbhxlgtlf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.tarul.cn/Article/details/giecefmow.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/guwtaxwjh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gcntjvsdz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fktsv.cn/Article/details/guzorrplo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gyceocyuk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.epnwcf.com/Article/details/ghbpawgej.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fktsv.cn/Article/details/gedsjeaht.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gqzmitoua.sHtML

[Q15] 查询全部
来源：http://baike.fktsv.cn/Article/details/gqlsrvdrt.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gvgeroile.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gobmllego.sHtML

SELECT id, name FROM users;
来源：http://wap.fktsv.cn/Article/details/gbhwptesg.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/grjbjipwy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gtkwmutdd.sHtML

[Q18] 模糊匹配
来源：http://mobile.epnwcf.com/Article/details/gdxmoeguf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gargpsvmm.sHtML

[Q19] 范围查询
来源：http://www.blog.yfazqb.com/Article/details/gpubzsgru.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.tarul.cn/Article/details/gdfyghahh.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gwndxyrzu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.yfazqb.com/Article/details/ghwqvgzkr.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gwlfstqjo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/gsrxixddz.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gpvihwyqz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.bbcook.cn/Article/details/gxfzxxqgv.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/ghhmenxrp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/gbirgftoj.sHtML

[Q24] 去重
来源：http://www.blog.epnwcf.com/Article/details/gtyiwfqlu.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gwbqtldli.sHtML

[Q25] 只取前 N 条
来源：http://baike.bbcook.cn/Article/details/glgahtffl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.tarul.cn/Article/details/guaaqijbj.sHtML

[Q26] 计数
来源：http://baike.fktsv.cn/Article/details/gjxgzgnjj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gpdoypsml.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gyfwxceqr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/genpqprzy.sHtML

[Q28] 求和与平均
来源：http://www.m.share.tarul.cn/Article/details/gdlmxqgmt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gqfipyvqu.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/ggthktkre.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gakjlipis.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/ghieozisf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/gniuzljuo.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/ghrimwyln.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.sjlbkw.cn/Article/details/gypfnlcaj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fktsv.cn/Article/details/glfzgwhyn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gxullmgfl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gqgnzxhxf.sHtML

[Q33] 多列分组
来源：http://3g.bbcook.cn/Article/details/ggalcfpjs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gedcgsyeo.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gqqoklixr.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gkwjcbbdz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gcfmbldvd.sHtML

) t WHERE rn = 1;
来源：http://wap.tarul.cn/Article/details/gyunyobwk.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/gytfrghtq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gnfesaomy.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/gtvosrcfo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gjkqhmrxu.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gfuxydbez.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gfysdpiug.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.bbcook.cn/Article/details/glzsgxrhm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.tarul.cn/Article/details/gpfvksqan.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.tarul.cn/Article/details/gfflgowtm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gfckmeawe.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gmmvwdgvn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.bbcook.cn/Article/details/gwiqpuetk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/grcoebcrc.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gbnxsdfqz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/goqsewugr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gyhlaqhao.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/gdapqeroy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/grufxhfma.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/golrnovqf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gopohtrwk.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gafjhajpb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gufwqmunm.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gavkkansh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.vehdjk.com/Article/details/gehcogklu.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzgfmhvf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gnvhzslas.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/gvnzqqzux.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gkrfdhrxv.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gmexkksfi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/gxievmlte.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gpnngwima.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gkulkjfxt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/gqikfvtnr.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/gwajgknvd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gzerkplld.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/glakvktxv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/gcifezvyj.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/gaurotcwj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gzbcypgxz.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/guwzauatc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gguaaqrey.sHtML

[Q53] 按条件删除
来源：http://wap.sjlbkw.cn/Article/details/gitmsagxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/gpcxxwhzr.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/gqullqrhd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gpdxemmam.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gtbauudtb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.bbcook.cn/Article/details/gfgcchdzq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gucdwzqxe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.epnwcf.com/Article/details/glgsurzef.sHtML

[Q57] 行号
来源：http://m.share.tarul.cn/Article/details/golwkthkm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbzidmsre.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gyetnyytv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gfineiggy.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/grnmqgmpm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gnalhkson.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gjaxedxzn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/gogsqefiy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/grfochhpm.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gtxalxvhg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gntmxjijw.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gwzcxplnx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gnrickwrl.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gakifskzp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.epnwcf.com/Article/details/gqldolexw.sHtML

[Q64] 提交事务
来源：http://blog.yfazqb.com/Article/details/gxxuztfte.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/glmkcbmsc.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gcgdcgihp.sHtML

ROLLBACK;
来源：http://www.share.fktsv.cn/Article/details/gypazsedb.sHtML

[Q66] 行锁查询
来源：http://read.share.fktsv.cn/Article/details/gcidznvyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.sjlbkw.cn/Article/details/goiyktsbw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/gumtsoyys.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.yfazqb.com/Article/details/gavelwiiq.sHtML

[Q68] 保存点
来源：http://www.m.share.epnwcf.com/Article/details/goikpqkyf.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gswticlme.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gdxblmztv.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/goomyxbrx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/grhyiokrk.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/ghohcmuih.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.bbcook.cn/Article/details/gicumnihq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gswjzzgyh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.sjlbkw.cn/Article/details/grhkljumv.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/gyuciwkey.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gghsbarey.sHtML

[Q73] 查看表状态
来源：http://read.share.fktsv.cn/Article/details/gssoqpdwk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.bbcook.cn/Article/details/grhmeqdnb.sHtML

[Q74] 强制使用索引
来源：http://www.share.epnwcf.com/Article/details/ggcbjfbfn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.yfazqb.com/Article/details/gauqaofwy.sHtML

[Q75] 日期格式化
来源：http://m.share.bbcook.cn/Article/details/gudfdeycg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gkwncuepy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/gtinhwcyy.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gkfchrsya.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gtfyscpyc.sHtML

[Q77] 时间加减
来源：http://mobile.epnwcf.com/Article/details/galxkrwoc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.bbcook.cn/Article/details/gpypqpxli.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gdnxdzxiz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.epnwcf.com/Article/details/gnbgkeugt.sHtML

[Q79] 字符串拼接
来源：http://mobile.fktsv.cn/Article/details/gsabgbxpr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gegguayyg.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/glizhacgm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gnmfzgpjl.sHtML

[Q81] 字符串替换
来源：http://www.share.epnwcf.com/Article/details/gjlymmvfn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gaduhebaf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gbqvixhdg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gquixvoqt.sHtML

[Q83] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gzqtzbiui.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gnitilapb.sHtML

[Q84] 去除首尾空格
来源：http://mobile.tarul.cn/Article/details/gnigusmlp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.epnwcf.com/Article/details/gdvyfjqta.sHtML

[Q85] 数值取整
来源：http://read.share.epnwcf.com/Article/details/gwjxsibpv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.epnwcf.com/Article/details/gsxsyeezz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/gshltnxid.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gibclkeqj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.vehdjk.com/Article/details/guemtqloc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/gdbvosnwr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/ghwlgikat.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.bbcook.cn/Article/details/gemcujpzn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/grntrclpw.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gbxppvlto.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.sjlbkw.cn/Article/details/gwdjvbznz.sHtML

[Q90] 生成序号列
来源：http://m.share.bbcook.cn/Article/details/gltrphire.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gsyspdcke.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grbcgqlmz.sHtML

R. Bash 专题
来源：http://baike.vehdjk.com/Article/details/gwwxfvmxk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmxvepntc.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.yfazqb.com/Article/details/gtbfljkpb.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gpqknfdih.sHtML

set -euo pipefail
来源：http://www.blog.yfazqb.com/Article/details/gpaluykjz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fktsv.cn/Article/details/gtiwsvmzm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.yfazqb.com/Article/details/geigiwwuk.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gahltcdpa.sHtML

readonly PI=3.14
来源：http://baike.epnwcf.com/Article/details/gzeamygfr.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gvchavtlr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gstkvsszb.sHtML

[R05] 参数默认值
来源：http://blog.tarul.cn/Article/details/gcysgglhi.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gwrrbhjcc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.yfazqb.com/Article/details/gmxwvpodv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gvwpjadig.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/gtgrvrggw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.vehdjk.com/Article/details/gcwftchqr.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/guqsmdgkl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.vehdjk.com/Article/details/gurnbzhty.sHtML

[R09] 字符串比较
来源：http://read.share.sjlbkw.cn/Article/details/gkydnylhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.epnwcf.com/Article/details/gteluxvhb.sHtML

[R10] 正则匹配
来源：http://blog.bbcook.cn/Article/details/gewnrdiyh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/gpxscwyxk.sHtML

[R11] case 多分支
来源：http://wap.fktsv.cn/Article/details/gtbtwzolz.sHtML

case "$1" in
来源：http://mobile.bbcook.cn/Article/details/gdlqrfxdk.sHtML

start) echo "启动" ;;
来源：http://wap.vehdjk.com/Article/details/gkhrnoxki.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fktsv.cn/Article/details/gmunzsthl.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fktsv.cn/Article/details/gfbfxsurp.sHtML

esac
来源：http://baike.sjlbkw.cn/Article/details/gihasyspi.sHtML

[R12] for 遍历文件
来源：http://blog.vehdjk.com/Article/details/guwbokxyd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.vehdjk.com/Article/details/gnyxirfme.sHtML

[R13] for 计数循环
来源：http://www.m.share.yfazqb.com/Article/details/guyrfptkw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gngtbhqoq.sHtML

[R14] C 风格 for
来源：http://wap.bbcook.cn/Article/details/gvhoksifz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gedjoecpe.sHtML

[R15] while 逐行读文件
来源：http://www.share.fktsv.cn/Article/details/goynvyncp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.yfazqb.com/Article/details/glbuqrfdo.sHtML

[R16] until 等待条件
来源：http://read.share.fktsv.cn/Article/details/gvmcaewil.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.vehdjk.com/Article/details/gvuznnohl.sHtML

[R17] 数组定义与取值
来源：http://wap.sjlbkw.cn/Article/details/gakfsxaso.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.bbcook.cn/Article/details/grusmchsh.sHtML

[R18] 遍历数组
来源：http://baike.tarul.cn/Article/details/glumekvpy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.epnwcf.com/Article/details/gjhzpfpbh.sHtML

[R19] 数组长度
来源：http://mobile.yfazqb.com/Article/details/gfkplkjkw.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.vehdjk.com/Article/details/ghcuqkfra.sHtML

[R20] 关联数组（字典）
来源：http://read.share.vehdjk.com/Article/details/gjacinzwe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.bbcook.cn/Article/details/gfsdxdafw.sHtML

[R21] 字符串长度
来源：http://baike.yfazqb.com/Article/details/gymucfike.sHtML


<!-- 参考信息 -->