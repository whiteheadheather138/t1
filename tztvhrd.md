代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.sjlbkw.cn/Article/details/ggirkfzbj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gemsbnldy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gcgkkhwtw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gsrmjuqah.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gekigkwzc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.vehdjk.com/Article/details/gthzpkddd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.tarul.cn/Article/details/gpkxzwwyv.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gjjskejfv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.tarul.cn/Article/details/gzvuhuhdk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.vehdjk.com/Article/details/ghfaimliv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/glqzogwsc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.sjlbkw.cn/Article/details/grfvhxblg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gvwwugksj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gkohyabyv.sHtML

Ruby: x.length;  x.size
来源：http://read.share.tarul.cn/Article/details/guervcqwg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/glhqaifol.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.bbcook.cn/Article/details/gqfdrwafe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.sjlbkw.cn/Article/details/ghnffrbmt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.vehdjk.com/Article/details/gkyrdjuqj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gtebvxrwu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gnikexdmj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gfenlyvej.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gbrammlis.sHtML

Ruby: a == b
来源：http://www.m.share.sjlbkw.cn/Article/details/gznbjcxag.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gstplqqeu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.sjlbkw.cn/Article/details/gyqrwhzfo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gtbnwedoq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.vehdjk.com/Article/details/gexpghzdv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gmbrkfuju.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/gaaspeehs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gditzfuqb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gqlgbooxx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/gifikbgqc.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/gmwuzzsjn.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gehtxowcs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/glgjqogrm.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/gttlgjrdf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gskwmmeov.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gfsqrthvp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.sjlbkw.cn/Article/details/gsekxoabh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.yfazqb.com/Article/details/gpupyvpou.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gnawltwvb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gffqpywbk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/gapozsyvv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gjxfrpteq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gcsjgohxs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/gdsnqfwtu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gcvtkbbmf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/guvqgxvrf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.tarul.cn/Article/details/ggznnxsdh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gytsrtloj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.bbcook.cn/Article/details/gksxywhbt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gltprebrn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.bbcook.cn/Article/details/gwdbxbwlt.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gpcfnfesv.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gbtfvptlu.sHtML

CREATE TABLE users (
来源：http://www.m.share.bbcook.cn/Article/details/gwnaeictp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/grprdxgne.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/gkdwfkbzw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.sjlbkw.cn/Article/details/gavhjdoxg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/gduutjmfk.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gcxvijczq.sHtML

[Q02] 创建带外键的表
来源：http://baike.yfazqb.com/Article/details/gzuqngunx.sHtML

CREATE TABLE orders (
来源：http://baike.bbcook.cn/Article/details/gvkpsuvae.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/gvzrmuqav.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/ggnboirlp.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gcgrilrsy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gxpsihsru.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gtlsevpxv.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/gqhaeqjtb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.epnwcf.com/Article/details/gzmbgeojw.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/guvbhgdjx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.tarul.cn/Article/details/gzogpbqxc.sHtML

[Q05] 重命名列
来源：http://blog.epnwcf.com/Article/details/gugawfjte.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/gpkagkmdj.sHtML

[Q06] 删除列
来源：http://www.blog.sjlbkw.cn/Article/details/gtunhawuu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.epnwcf.com/Article/details/giulkytui.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gnvysshaf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gqqfftxtg.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gqqisfaks.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gqaknfzdp.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gcfskvzbd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gqimnkfdy.sHtML

[Q10] 插入单行
来源：http://baike.bbcook.cn/Article/details/gamttccxe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gvwnweszk.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/gxeldsfes.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gcpxzpzql.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.bbcook.cn/Article/details/givijrxfd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.tarul.cn/Article/details/gvbvvsymr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/ggeispyiu.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gklwlvojw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/glafxitlu.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gqevbsaeb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gtrgxnpmp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/ghxlfdebz.sHtML

[Q15] 查询全部
来源：http://3g.epnwcf.com/Article/details/gnwjjpket.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gnazqhvge.sHtML

[Q16] 查询指定列
来源：http://mobile.yfazqb.com/Article/details/gwglzdyyr.sHtML

SELECT id, name FROM users;
来源：http://3g.fktsv.cn/Article/details/gamfiwwno.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gvxijiwvu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fktsv.cn/Article/details/gpfpnxfll.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gmirvsihr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gqmfuzefd.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/gxgunlbmj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/ggqtdiydk.sHtML

[Q20] IN 列表
来源：http://www.blog.bbcook.cn/Article/details/gjpkovpfz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gmzzjtpnu.sHtML

[Q21] 空值判断
来源：http://m.share.bbcook.cn/Article/details/gzatrazlx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gsrzohmev.sHtML

[Q22] 排序
来源：http://3g.tarul.cn/Article/details/gfcmtfkzb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/ghaaphmua.sHtML

[Q23] 分页
来源：http://mobile.fktsv.cn/Article/details/gavbxzrvm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.epnwcf.com/Article/details/glvxdxmje.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/gynktplvi.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/gnqxkuete.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gyhjekare.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/ggpegnbwd.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gtxljlpgz.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/goyoplfez.sHtML

[Q27] 条件计数
来源：http://www.blog.fktsv.cn/Article/details/gsubgcxaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gznkynyiv.sHtML

[Q28] 求和与平均
来源：http://m.share.fktsv.cn/Article/details/gwkgpgvlw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gqsznzclv.sHtML

[Q29] 最大最小值
来源：http://www.share.fktsv.cn/Article/details/gkoabqdog.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gmyqxryzo.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/geuftysmp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gkkoejinz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fktsv.cn/Article/details/gnxdrrybo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/giazprrcl.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gqyqxlxfc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gzveyiccd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/gvsgoejqc.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/gojhywhco.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/ganlnxnik.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gkjniljti.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gwreejlqo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gunvbrwgt.sHtML

) t WHERE rn = 1;
来源：http://mobile.bbcook.cn/Article/details/grlggvkue.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gcvfyutdq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gymtlhaaw.sHtML

[Q36] 左连接
来源：http://www.blog.yfazqb.com/Article/details/gojgnnshu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gncsglqsu.sHtML

[Q37] 右连接
来源：http://www.share.yfazqb.com/Article/details/gdjknwhni.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gbmxqbqas.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.yfazqb.com/Article/details/gydjydrft.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fktsv.cn/Article/details/girzoroff.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/gsqfdtiae.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/gmeeziafo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrsaweoc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.sjlbkw.cn/Article/details/gmkxpzgdl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gfmhhzudp.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/glgqcbscq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gddtqricr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/gybjmqedv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gsiisbfix.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.tarul.cn/Article/details/gkamcmgod.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gcjqqsszd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.yfazqb.com/Article/details/gwlcllbpi.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/grmsajynm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.tarul.cn/Article/details/gzlvkosqk.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/ggwupejge.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.sjlbkw.cn/Article/details/gouenpkha.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.sjlbkw.cn/Article/details/ghnjsfamz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/grivtodqw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.bbcook.cn/Article/details/goatybxbz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/grmybbqab.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/gtbdogjus.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/gyerauvhw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gyecwbwfa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/gpkflurtu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/gqvjucqqy.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/gvcyapiaf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gggtfjdza.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/gksbohqwq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.tarul.cn/Article/details/gsziklyvl.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gvsilcvsa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.vehdjk.com/Article/details/gyeedoecc.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gqmqovriv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fktsv.cn/Article/details/gxqunrjhg.sHtML

[Q53] 按条件删除
来源：http://blog.sjlbkw.cn/Article/details/glxghudhc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.tarul.cn/Article/details/guvbvbpnd.sHtML

[Q54] 清空表
来源：http://wap.epnwcf.com/Article/details/gkcswfauf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmwvezmi.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gjaubyqxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.epnwcf.com/Article/details/gvcytimby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.bbcook.cn/Article/details/gboupcgoi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gdtwsekyq.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/grpswnopp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/ghxseaxey.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gslqnntrr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmbcondgp.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/geikokuwa.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gizfasdpo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fktsv.cn/Article/details/gfcmsspzi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/guezozbnx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gbfznhcfw.sHtML

[Q61] 移动平均
来源：http://m.share.sjlbkw.cn/Article/details/gjgwdacyl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gfxhhujry.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gciecqlao.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gwrecejsk.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gwynyjbuy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/gpnyytyyc.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/grkqmjzls.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/gzymslvnn.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gmlgzqwev.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gnsufykqk.sHtML

[Q66] 行锁查询
来源：http://m.share.tarul.cn/Article/details/gznzllilt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/ghmpxzxli.sHtML

[Q67] 设置隔离级别
来源：http://3g.tarul.cn/Article/details/gxrhupbkm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.bbcook.cn/Article/details/goxnlaamk.sHtML

[Q68] 保存点
来源：http://read.share.bbcook.cn/Article/details/guswmxjdl.sHtML

SAVEPOINT sp1;
来源：http://m.share.tarul.cn/Article/details/gkqfqyegt.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gptbplpth.sHtML

[Q69] 查看执行计划
来源：http://read.share.vehdjk.com/Article/details/gregdhmlk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/gxlnccrif.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gccvtxalk.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/ghgbptkaq.sHtML

[Q71] 查看建表语句
来源：http://www.blog.epnwcf.com/Article/details/gzlrfnxyn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.sjlbkw.cn/Article/details/gwmipcxbd.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gszaeytho.sHtML

SHOW INDEX FROM users;
来源：http://baike.fktsv.cn/Article/details/gqcigyuzk.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/ghpevxwjf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/glzgqflyc.sHtML

[Q74] 强制使用索引
来源：http://www.share.bbcook.cn/Article/details/gqgtwlmtc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/getpkwdzs.sHtML

[Q75] 日期格式化
来源：http://www.share.tarul.cn/Article/details/gdkimsloa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gopkzolbt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/giudqghvn.sHtML

[Q76] 按天统计
来源：http://www.blog.vehdjk.com/Article/details/gujiunwml.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.epnwcf.com/Article/details/gelqbresb.sHtML

[Q77] 时间加减
来源：http://m.share.yfazqb.com/Article/details/ghbovzhwo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gfhszsasn.sHtML

[Q78] 当前时间
来源：http://wap.tarul.cn/Article/details/gucfcdybr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gyvatkwib.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/ganhkxdry.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gqcvtavcw.sHtML

[Q80] 字符串截取
来源：http://m.share.epnwcf.com/Article/details/gkfbpesnk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gcsdpnuef.sHtML

[Q81] 字符串替换
来源：http://wap.yfazqb.com/Article/details/grckpukkm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/gahutykdd.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gibyrmrbb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gezlkcnnc.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gambdpofe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gtbeyiqld.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gqkgzpkfx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gwkclxhyr.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/giktxzncu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/giiamhkki.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gfaywhqex.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.epnwcf.com/Article/details/grrcdmcau.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gjkidpxta.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gbnamwxmt.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.bbcook.cn/Article/details/gojkudwxy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/gakpnxqmj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/guirrqjed.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gvurrpywi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/gsgjojhqy.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gwcybyoyk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.sjlbkw.cn/Article/details/gjmcyeege.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gggkrhret.sHtML

R. Bash 专题
来源：http://www.share.yfazqb.com/Article/details/gtyuiuaog.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/ghknglrlh.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/gjhmkxrxa.sHtML

#!/usr/bin/env bash
来源：http://www.share.bbcook.cn/Article/details/gonkgqczg.sHtML

set -euo pipefail
来源：http://blog.fktsv.cn/Article/details/gkhflqzpo.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gfvvipzhv.sHtML

name="Tom"; echo "$name"
来源：http://www.share.yfazqb.com/Article/details/ggjitnjiv.sHtML

[R03] 只读变量
来源：http://3g.vehdjk.com/Article/details/gibbjicug.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gjoqgtajn.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/gkysbtpsf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gddadmaao.sHtML

[R05] 参数默认值
来源：http://wap.sjlbkw.cn/Article/details/giqmdwusx.sHtML

name="${1:-default}"
来源：http://www.m.share.fktsv.cn/Article/details/gkogrlwof.sHtML

[R06] 判断命令是否存在
来源：http://read.share.bbcook.cn/Article/details/gfcwdovou.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.tarul.cn/Article/details/geemukohw.sHtML

[R07] if 判断文件
来源：http://baike.sjlbkw.cn/Article/details/ghusojxza.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gmgrryjso.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/ghzkmzbmy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/guierarit.sHtML

[R09] 字符串比较
来源：http://baike.vehdjk.com/Article/details/gbnwleqbs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjqlkcec.sHtML

[R10] 正则匹配
来源：http://m.share.tarul.cn/Article/details/ghcosizco.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.tarul.cn/Article/details/gigyivknw.sHtML

[R11] case 多分支
来源：http://www.share.tarul.cn/Article/details/gaudyncry.sHtML

case "$1" in
来源：http://blog.yfazqb.com/Article/details/gpkvwdkhx.sHtML

start) echo "启动" ;;
来源：http://read.share.yfazqb.com/Article/details/grgxtoqsq.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gzcxguvuc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.tarul.cn/Article/details/ghpfsifsv.sHtML

esac
来源：http://www.share.yfazqb.com/Article/details/gpwizcbjk.sHtML

[R12] for 遍历文件
来源：http://wap.sjlbkw.cn/Article/details/guvwgtums.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.bbcook.cn/Article/details/gwevcpihs.sHtML

[R13] for 计数循环
来源：http://mobile.sjlbkw.cn/Article/details/gepnnxmaz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.sjlbkw.cn/Article/details/gcnokuitv.sHtML

[R14] C 风格 for
来源：http://m.share.sjlbkw.cn/Article/details/gzrunkwao.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.tarul.cn/Article/details/gvfnqvquf.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.vehdjk.com/Article/details/gsyohkqov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.yfazqb.com/Article/details/gtsnfmwpp.sHtML

[R16] until 等待条件
来源：http://www.blog.vehdjk.com/Article/details/ggowprmrt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fktsv.cn/Article/details/gbvlvohin.sHtML

[R17] 数组定义与取值
来源：http://m.share.yfazqb.com/Article/details/gzrjoblqi.sHtML


<!-- 参考信息 -->