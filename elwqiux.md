代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gvshhrrdd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/ghroyzqnt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/giblblrvj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gzduqmdrl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/grxddnxfu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/goxmsfors.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gvtygbvzd.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gfcdppvpf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/grythmqux.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/gwkuwlobx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/goyfiytgu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/grmweayth.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gvplxujpg.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/ghrqatikv.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gnqiwsyaq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gxpvjcopf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/ggzuidzrg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsazqsok.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/ghurezsrz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gjcqzyrlc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gfsbfomsh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.epnwcf.com/Article/details/gvvqrwasw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gqwmkwbvk.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/geqbcekkg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.epnwcf.com/Article/details/gvskvytbd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gwqnpnuvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gtoullqih.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/getpviebb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.vehdjk.com/Article/details/giohbppms.sHtML

TS:   if (x == null) {}
来源：http://m.share.tarul.cn/Article/details/gumjcvvit.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyzxamxao.sHtML

Go:   if x == nil {}
来源：http://www.m.share.tarul.cn/Article/details/gxashpaaj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gdgicgnwk.sHtML

C#:   if (x is null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gknulfjfu.sHtML

[P07] 防抖与节流
来源：http://m.share.yfazqb.com/Article/details/gxmrkpccj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gzjtbwhzs.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gkvizrhmp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gnulwxkoh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gzkkqyrdk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gkiptyism.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/gyunsgcba.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gxfleoxgx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gncszappv.sHtML

[P08] 处理浮点精度问题
来源：http://blog.sjlbkw.cn/Article/details/gacidozmp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/gwpgpbush.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.tarul.cn/Article/details/gebmdurfd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/gngeoygeq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/grjqrbnph.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gywsccnyv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.vehdjk.com/Article/details/gozsjqigz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fktsv.cn/Article/details/glmwseaic.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/grmyqdmcf.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gfzysreto.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.bbcook.cn/Article/details/ggnsfpasn.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/guryizqrz.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gafzvyugt.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gpoimlsjs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gnklnhbes.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/ghccjiptl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.vehdjk.com/Article/details/ghnkqjqhc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/givyxkgyq.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gmqnaunsp.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/gwxbqeadp.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/ggfvxrvvh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gjfiigatm.sHtML

user_id INT NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gdzsumtfn.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.bbcook.cn/Article/details/gqwxucxuo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gkbdojqvd.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gahdtwllr.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/ggrmooqtf.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gdbhyeqne.sHtML

[Q04] 修改列类型
来源：http://3g.tarul.cn/Article/details/gdzzjeodc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.yfazqb.com/Article/details/gpdpxwwmo.sHtML

[Q05] 重命名列
来源：http://www.m.share.sjlbkw.cn/Article/details/gyulcslkg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gxtolujqj.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gwxdwhqbf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/gxqjwlqqr.sHtML

[Q07] 删除表
来源：http://wap.epnwcf.com/Article/details/gjxgpwlrg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gvtpyqbhq.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gjbcvxnuf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.sjlbkw.cn/Article/details/gycrnezfa.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gdwxhkrcc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/gqrjvoddt.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gzontdxwj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gscflwhuz.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gvoccrioj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gpaiajqcg.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.yfazqb.com/Article/details/gtbsmujxn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fktsv.cn/Article/details/gxnwknbic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gaaqwuqmp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.tarul.cn/Article/details/gxjubexiv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/grcoxsmyc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/gzwhcofej.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.epnwcf.com/Article/details/gnebbuust.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/glifwefqq.sHtML

[Q15] 查询全部
来源：http://wap.sjlbkw.cn/Article/details/gcghbzyek.sHtML

SELECT * FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gctqlygkh.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gcgffqwaz.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gtoxunvsp.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gxnxxsenr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gugbhoojj.sHtML

[Q18] 模糊匹配
来源：http://blog.tarul.cn/Article/details/gybzfppxu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.vehdjk.com/Article/details/gsimiihhl.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gnwztqtgc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gusushunm.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gyhlskmfk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/ghwuhsuja.sHtML

[Q21] 空值判断
来源：http://mobile.sjlbkw.cn/Article/details/gcozwznfa.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gwlrzpsha.sHtML

[Q22] 排序
来源：http://read.share.yfazqb.com/Article/details/gggsyrdqu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/gbnuhltys.sHtML

[Q23] 分页
来源：http://www.m.share.epnwcf.com/Article/details/gujhwrtpu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.sjlbkw.cn/Article/details/ggtdpascw.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/gseaocsce.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gayehtnmo.sHtML

[Q25] 只取前 N 条
来源：http://read.share.bbcook.cn/Article/details/ggbdapwly.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gohgzspdn.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gnjudcnwq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gjrbnhkpq.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gzazefqny.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gkwbhoolf.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gcgeprdel.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/geacigyma.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gqgdmiddz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gcqfqjmoh.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/gqvrgxfqx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gnbxbibrp.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gciudalqb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.yfazqb.com/Article/details/gvgmphymi.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gywkjjisw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gigexkplu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gccpijagq.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gjwqibwzu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gbhwceedf.sHtML

[Q34] 每组取第一条
来源：http://m.share.tarul.cn/Article/details/gzdzjqgqa.sHtML

SELECT * FROM (
来源：http://blog.tarul.cn/Article/details/gddczdhrk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gqroklmca.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/gvegwlnvy.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/guhmrjahw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fktsv.cn/Article/details/gnrrdxtug.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gvpppdkum.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gyrhvojxl.sHtML

[Q37] 右连接
来源：http://m.share.tarul.cn/Article/details/gbpkwtjzj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/gsfjjagcz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gfrwvrldm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/gcyjrwjom.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gxyvwnxox.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gflpmbxxi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gyqlkodlg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.epnwcf.com/Article/details/gbldnhwmb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/gopofajjy.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/garaxtbqo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.vehdjk.com/Article/details/gwholfsyl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gducicuaq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.tarul.cn/Article/details/gcsgjvyom.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/guwenoymb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.tarul.cn/Article/details/gcxiyybre.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.epnwcf.com/Article/details/grydbmole.sHtML

[Q43] 标量子查询
来源：http://www.blog.epnwcf.com/Article/details/gcytfzogm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gtbhmakew.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/ggjhfreuf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/ggtbznmxd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.epnwcf.com/Article/details/gszbfmrop.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gcifetjnx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/giwdpnocq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/ghziimosf.sHtML

[Q47] 与平均值比较
来源：http://baike.bbcook.cn/Article/details/ggvqkvgpm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gaqsjiipf.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.epnwcf.com/Article/details/gbskoadtv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.epnwcf.com/Article/details/gmndknjpp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.vehdjk.com/Article/details/goeqfiixw.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gjanrorto.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.tarul.cn/Article/details/gixpfnckf.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gloajpeup.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gnfsevyvg.sHtML

[Q51] 用子查询更新
来源：http://m.share.epnwcf.com/Article/details/geckmlzei.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gghvtrmyz.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gxmwfzkhp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/gpxpdoqwi.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/ggpxmjpvj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gejljlrwc.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gtrexcixg.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.yfazqb.com/Article/details/ganwpchzq.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gnzrlggog.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gqotjmkyd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.epnwcf.com/Article/details/gnjfcccxx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gmwipnhat.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/gmjknywwt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/golkmgtkd.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gfiylhmur.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/ginwlgahr.sHtML

[Q59] 分组内累计
来源：http://www.share.bbcook.cn/Article/details/gfevwacxv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/glcmuyqkm.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gryqzdizm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.sjlbkw.cn/Article/details/ghhnxcqau.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/gmrjlbwgy.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gyvyszqyp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gzcokwrsv.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/guqxhldue.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gbjnabcqw.sHtML

[Q63] 开启事务
来源：http://3g.bbcook.cn/Article/details/gbfadcmpu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fktsv.cn/Article/details/grrkbnqzf.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/ghzukxddd.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gvqfmknsl.sHtML

[Q65] 回滚事务
来源：http://baike.fktsv.cn/Article/details/gbqhkuhyf.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gccznbive.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/gvythiuxb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gwtwcqoms.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gpifawxbx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/gjmvtmtri.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gfxifiyvc.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gwftcqobe.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gzkbjweqi.sHtML

[Q69] 查看执行计划
来源：http://wap.epnwcf.com/Article/details/grfbzskxd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/girnlhznn.sHtML

[Q70] 更新统计信息
来源：http://mobile.tarul.cn/Article/details/gdqedliwx.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gfyeyobts.sHtML

[Q71] 查看建表语句
来源：http://m.share.bbcook.cn/Article/details/gcslqltfx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.sjlbkw.cn/Article/details/gzvvtfare.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gnuvwpumc.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gpvsttarr.sHtML

[Q73] 查看表状态
来源：http://baike.fktsv.cn/Article/details/ghraqjwar.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.sjlbkw.cn/Article/details/gnifujnbo.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gjjjwnagt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.sjlbkw.cn/Article/details/geqqesdrh.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/gyefzljlw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gwucpiytm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gfgjnuvvr.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/ghlbykhil.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.bbcook.cn/Article/details/gayshwyay.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/gkdnqogvh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.vehdjk.com/Article/details/gfsauttul.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/ggygmksmm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gocqxpqyu.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gghjpjndd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fktsv.cn/Article/details/gsutqxtcs.sHtML

[Q80] 字符串截取
来源：http://baike.epnwcf.com/Article/details/gpissghtx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/guoqfuizr.sHtML

[Q81] 字符串替换
来源：http://read.share.vehdjk.com/Article/details/gladnjhql.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/goepcfvvr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.vehdjk.com/Article/details/gmhiegpbo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/giqizbwgz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.bbcook.cn/Article/details/gthfabwnh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/glizpizeh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/ggmwjlrgm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gvsmlppqb.sHtML

[Q85] 数值取整
来源：http://www.share.bbcook.cn/Article/details/gyiuatzky.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.bbcook.cn/Article/details/guotpsgar.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gustdlofl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gogxdawaw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gjjhayeto.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.tarul.cn/Article/details/gwmazygjr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.yfazqb.com/Article/details/gafesweya.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gbebgxqmq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gykfadasr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gccwxkjuy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/gffsfrteg.sHtML

[Q90] 生成序号列
来源：http://m.share.epnwcf.com/Article/details/gvlqsifbt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.tarul.cn/Article/details/gqrxfiylm.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbfyrxeuj.sHtML

R. Bash 专题
来源：http://baike.epnwcf.com/Article/details/gvbyplcfd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmfhohqxn.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/ghmjjwkwi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fktsv.cn/Article/details/gqkglhdjc.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gtmkacbgv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gxrzhwngi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.tarul.cn/Article/details/gbxsjtmgl.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gmqchldnl.sHtML

readonly PI=3.14
来源：http://baike.tarul.cn/Article/details/gurlccblj.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gppgdctot.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fktsv.cn/Article/details/gdmvsbfny.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/gdyrvfdyw.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/grbhjdhff.sHtML

[R06] 判断命令是否存在
来源：http://mobile.bbcook.cn/Article/details/ggwwnlujf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.sjlbkw.cn/Article/details/gpraiahwg.sHtML

[R07] if 判断文件
来源：http://mobile.epnwcf.com/Article/details/gkygintxh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.tarul.cn/Article/details/gdpxbkdoi.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gvimbgifa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.sjlbkw.cn/Article/details/gohswmchi.sHtML

[R09] 字符串比较
来源：http://read.share.epnwcf.com/Article/details/gwpncxjma.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.vehdjk.com/Article/details/godbxjllj.sHtML

[R10] 正则匹配
来源：http://m.share.epnwcf.com/Article/details/gnjolwalr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.tarul.cn/Article/details/gfcxaqcnr.sHtML

[R11] case 多分支
来源：http://www.share.yfazqb.com/Article/details/gxjjentjy.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gszrrnoqe.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/groadnznt.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.tarul.cn/Article/details/gdxxhwycx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/ggcqbgpmm.sHtML

esac
来源：http://m.share.bbcook.cn/Article/details/gurmwissg.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/gvrcqtspi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.epnwcf.com/Article/details/gvhcawnlk.sHtML

[R13] for 计数循环
来源：http://www.share.yfazqb.com/Article/details/gnrswazbu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.yfazqb.com/Article/details/gkdyhodmo.sHtML

[R14] C 风格 for
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqcdwsp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/gcvhyoxqe.sHtML

[R15] while 逐行读文件
来源：http://mobile.sjlbkw.cn/Article/details/gxizpsbww.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.tarul.cn/Article/details/gjxoqleom.sHtML

[R16] until 等待条件
来源：http://baike.sjlbkw.cn/Article/details/gloybhxmr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.sjlbkw.cn/Article/details/grqqlsfws.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fktsv.cn/Article/details/gbsfubcjj.sHtML


<!-- 参考信息 -->