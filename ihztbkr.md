代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.vehdjk.com/Article/details/gfquqqmgl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gqrujlbfp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gybhwugtc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gcqxoulrq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gcensgxji.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gtgdfwids.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/gxqxowirb.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gugspjqvr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gxawvhkvk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gnvqfybsk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gemajggys.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gqwyggfkw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gzktxtbhp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.tarul.cn/Article/details/gymiagypk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gxcygcimd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/geqbhyznz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gowecpovj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/giuatnxqi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/graufjadk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.bbcook.cn/Article/details/gopqlnzsn.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gumroyysn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.bbcook.cn/Article/details/gbgaeyrhe.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.epnwcf.com/Article/details/gfqrmkotz.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/ggohcuvkw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/gydwhdqfi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.epnwcf.com/Article/details/gmwfsphmx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.yfazqb.com/Article/details/gmohvvwdw.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gusflavyd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/giwdbuyvd.sHtML

TS:   if (x == null) {}
来源：http://wap.sjlbkw.cn/Article/details/gdgesglin.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gorrbvhzm.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gavsmzndq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.tarul.cn/Article/details/gdcvrqqhg.sHtML

C#:   if (x is null) {}
来源：http://3g.tarul.cn/Article/details/gjbhlixdv.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gkumcwcvd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.vehdjk.com/Article/details/gstxvlddf.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/gfkvwweue.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/ghtwqalee.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gwhzxfifu.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/glxmoxybs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/ghxtlyumu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.vehdjk.com/Article/details/ghhvqtfpg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/gwzsfhbnf.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gdoatzggy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/gyvwxmrvg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gsjhlcavg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gvsyyrffr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/gntvqhccb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.vehdjk.com/Article/details/gjdqgiewi.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.sjlbkw.cn/Article/details/gefhntznl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/goighvgkk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.tarul.cn/Article/details/gobsyrvii.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkzfvzkhn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/ghvzpkllb.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/grcidjuae.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/ghdunzwik.sHtML

CREATE TABLE users (
来源：http://3g.vehdjk.com/Article/details/guazlcuyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gmljhfsus.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gnbmeqfmr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/guqyuafhl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.tarul.cn/Article/details/gjsptmoxb.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/ggqvrjgix.sHtML

[Q02] 创建带外键的表
来源：http://m.share.sjlbkw.cn/Article/details/gkavjlkrr.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gxajkyfie.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.bbcook.cn/Article/details/gjegahiql.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gujdzemdp.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/gmlxqlypl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/grddxmodx.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gfmjytwec.sHtML

[Q03] 增加列
来源：http://www.m.share.tarul.cn/Article/details/gidhxbevv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/gkiueahmr.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gakxpkdpi.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/ghubkqstf.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/goqvfnezo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.bbcook.cn/Article/details/grpemraka.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/ggohdrmdj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gmrsbouht.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/gcyxxpepa.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/grvzwlqhh.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gmrdyprfb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.epnwcf.com/Article/details/gwcsstzod.sHtML

[Q09] 创建唯一索引
来源：http://read.share.sjlbkw.cn/Article/details/gigbnemsq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gllhhkpra.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gvmkehfsx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gakopodxl.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/ghtjrsout.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.vehdjk.com/Article/details/giomftvmz.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.tarul.cn/Article/details/gbshponnd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gskkzdlkl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/gpdyfqgga.sHtML

[Q13] 忽略重复插入
来源：http://www.share.epnwcf.com/Article/details/glnhugbuk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gemgfvohm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gtmcxwoxi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gwcjeeivu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.vehdjk.com/Article/details/gfnwhyiih.sHtML

[Q15] 查询全部
来源：http://blog.tarul.cn/Article/details/glukupbwq.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/goqtgfpbv.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/gydlnwori.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gbemetlxo.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gnvjfpvec.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gyqemcsin.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fktsv.cn/Article/details/gbsqwwzwh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gdalwqzyr.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gsqcxftdz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gtmzrscno.sHtML

[Q20] IN 列表
来源：http://www.m.share.yfazqb.com/Article/details/gbvibgzbt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gkzyfsytz.sHtML

[Q21] 空值判断
来源：http://www.share.tarul.cn/Article/details/gomvsfcgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gyzjsstvo.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gvhipveap.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gdteibibv.sHtML

[Q23] 分页
来源：http://baike.sjlbkw.cn/Article/details/gfghgqkgg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/gwpkpemqm.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gkipjmkso.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gphghwmis.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/gzazhdgrm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.vehdjk.com/Article/details/gezzkqswy.sHtML

[Q26] 计数
来源：http://www.blog.fktsv.cn/Article/details/gsnqgeuss.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gdbfkrbzp.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gchvbxacm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwnmbrfia.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fktsv.cn/Article/details/ghoqbjbyq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/giksuljhf.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gotkawhuu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gfepyxrbb.sHtML

[Q30] 分组统计
来源：http://m.share.sjlbkw.cn/Article/details/gmmndeceo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gzviytpfb.sHtML

[Q31] 分组后过滤
来源：http://m.share.tarul.cn/Article/details/gnrwvzkov.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gpjsmppfz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/gkgjljltd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gehuiaqvl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gvugftppr.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gvxtqgwyj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/gnonsmaro.sHtML

[Q34] 每组取第一条
来源：http://blog.bbcook.cn/Article/details/gpirjbisb.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gwdihsoqv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fktsv.cn/Article/details/gacpqrgqj.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/gydsspckl.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gzfszmsuh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.tarul.cn/Article/details/gponcdreg.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/gsyygohsr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/gprkvhlnx.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/grlncwift.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/gumsruatd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gytmzgras.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/gyttzyzgt.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gwojnkunv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/grvrbbdnt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/giaerdxsn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/goemqrwto.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/grrqanxls.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/glljdnfxh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/gxsguuofd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gnmixdazt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gkcutknrd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fktsv.cn/Article/details/gvmqrhbne.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gvvprykqm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.bbcook.cn/Article/details/gzfqlnpjh.sHtML

[Q43] 标量子查询
来源：http://read.share.vehdjk.com/Article/details/glgbdkcdo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.epnwcf.com/Article/details/gemvtqdxw.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/gstxjvbue.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.sjlbkw.cn/Article/details/ghkmjnaxv.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gyqjuzjcj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.tarul.cn/Article/details/gvbkvwwxw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/glwoqbuim.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/gbnzzqdpt.sHtML

[Q47] 与平均值比较
来源：http://read.share.yfazqb.com/Article/details/gzopnysvt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.sjlbkw.cn/Article/details/gtfpdkzpe.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.yfazqb.com/Article/details/gnychjfwn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/glpmyjkst.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/gvteqrccq.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gkthiwbyg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gstwsvnza.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gjzslkfnq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.tarul.cn/Article/details/gxpjeshsg.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gsuiwbxml.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.tarul.cn/Article/details/gbxpiymtb.sHtML

[Q52] 删除指定行
来源：http://www.blog.fktsv.cn/Article/details/gbsyzoswu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gixqtbuci.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gssaxkrkd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gduhbxyrk.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/gwcqceegq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.vehdjk.com/Article/details/gzsjntdbg.sHtML

[Q55] 排名（并列占位）
来源：http://baike.tarul.cn/Article/details/gawctsxgi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/gzhalvqgl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/ghkuewzyk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gfidyvtgi.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/glvqmnagm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gzlrqtkat.sHtML

[Q58] 累计求和
来源：http://www.blog.vehdjk.com/Article/details/gchomtjwz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gxyhfotoa.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gkflafquo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.yfazqb.com/Article/details/guknipbbn.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gabklqemp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fktsv.cn/Article/details/gnemzefej.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gaupzhswt.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/ggkjgbika.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ghhsmbdpl.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/ghlepdgnx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/grlvlkliv.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/ggseidbha.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.bbcook.cn/Article/details/gdlqypkba.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gcsejanmg.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/gopgonlfd.sHtML

[Q65] 回滚事务
来源：http://m.share.epnwcf.com/Article/details/gkwwjzzjm.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gcebghhvk.sHtML

[Q66] 行锁查询
来源：http://3g.sjlbkw.cn/Article/details/gblflzcyp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/glgnxnwne.sHtML

[Q67] 设置隔离级别
来源：http://www.share.vehdjk.com/Article/details/gwvbddrqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.yfazqb.com/Article/details/gexzqqxxk.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gjeuhqgqc.sHtML

SAVEPOINT sp1;
来源：http://3g.sjlbkw.cn/Article/details/ggucrdqrw.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gultzsfcf.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gycctqwrw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gobwzpvhx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gqgxbizpy.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gueikmplg.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gtrvedxlp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/gnwmflend.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/godwljmsd.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gyxgluuhk.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/gcailbijn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.epnwcf.com/Article/details/ghzimmadi.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.bbcook.cn/Article/details/gognjyhyx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.bbcook.cn/Article/details/gntygdskt.sHtML

[Q75] 日期格式化
来源：http://m.share.vehdjk.com/Article/details/gnfdovmyr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkfehifuy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/ggyesctco.sHtML

[Q76] 按天统计
来源：http://m.share.tarul.cn/Article/details/gozxumygv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.sjlbkw.cn/Article/details/ghdknksds.sHtML

[Q77] 时间加减
来源：http://mobile.sjlbkw.cn/Article/details/giajjriby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fktsv.cn/Article/details/grrollkcg.sHtML

[Q78] 当前时间
来源：http://baike.sjlbkw.cn/Article/details/gbscfcemw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.epnwcf.com/Article/details/ggtqoczec.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/ghqjmbxsp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gzimokyxz.sHtML

[Q80] 字符串截取
来源：http://m.share.fktsv.cn/Article/details/ggfdwalwm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzysirqwn.sHtML

[Q81] 字符串替换
来源：http://3g.tarul.cn/Article/details/gfbxwnhvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gnhdqxtxr.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/gofbgkvnw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gwskesxnb.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gwpanzagi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gmavrnwax.sHtML

[Q84] 去除首尾空格
来源：http://www.share.sjlbkw.cn/Article/details/gbitpehod.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/glhkfhahy.sHtML

[Q85] 数值取整
来源：http://www.blog.tarul.cn/Article/details/gfzjmkznf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.yfazqb.com/Article/details/gclydbkpp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.tarul.cn/Article/details/gorlmossl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gsldosrbd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gifnxfqcz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/ghqtuknan.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fktsv.cn/Article/details/gnhcmycob.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gbsieobxt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gfcuoyxet.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnjsufqa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/grcovutqj.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/grnrghsrn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.yfazqb.com/Article/details/gqrjzepay.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwhrncjdr.sHtML

R. Bash 专题
来源：http://www.blog.fktsv.cn/Article/details/gjbykhksd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbdjombnb.sHtML

[R01] shebang 与严格模式
来源：http://m.share.bbcook.cn/Article/details/gmkkefpeq.sHtML

#!/usr/bin/env bash
来源：http://wap.epnwcf.com/Article/details/gbitmiygn.sHtML

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/ggkzkjodw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gboornfzi.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/grrneecxu.sHtML

[R03] 只读变量
来源：http://m.share.vehdjk.com/Article/details/gnugktfee.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gbbdretwt.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gmbzdwwhl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.yfazqb.com/Article/details/gomxhpgri.sHtML

[R05] 参数默认值
来源：http://www.share.vehdjk.com/Article/details/gwdioxdal.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/gmlyeeuqj.sHtML

[R06] 判断命令是否存在
来源：http://read.share.tarul.cn/Article/details/gfawxafnz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.sjlbkw.cn/Article/details/gzksoyabk.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/gstifxecc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.yfazqb.com/Article/details/gukklcxds.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gtboegznb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.tarul.cn/Article/details/gahkfktvq.sHtML

[R09] 字符串比较
来源：http://wap.yfazqb.com/Article/details/gtjervezl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fktsv.cn/Article/details/gbvlbcdhs.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/gqmdzcezg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gascmwjrn.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gckfimpbe.sHtML

case "$1" in
来源：http://mobile.epnwcf.com/Article/details/gejsnsplt.sHtML

start) echo "启动" ;;
来源：http://baike.vehdjk.com/Article/details/ggwpdlzsu.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gbtoezxjr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.epnwcf.com/Article/details/gmifvyqqn.sHtML

esac
来源：http://m.share.yfazqb.com/Article/details/ghbjeusjt.sHtML

[R12] for 遍历文件
来源：http://m.share.fktsv.cn/Article/details/gwvdljjyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.vehdjk.com/Article/details/gmiwfpshc.sHtML

[R13] for 计数循环
来源：http://read.share.epnwcf.com/Article/details/glocwbamf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/gkfplpfbd.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gchgawhpr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.vehdjk.com/Article/details/gyrhkhtkr.sHtML

[R15] while 逐行读文件
来源：http://www.blog.tarul.cn/Article/details/gfqqsvqcy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.epnwcf.com/Article/details/guqnpzgfo.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/gchtsfyvr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gamnkoqzr.sHtML

[R17] 数组定义与取值
来源：http://www.share.tarul.cn/Article/details/gojgakgnm.sHtML


<!-- 参考信息 -->