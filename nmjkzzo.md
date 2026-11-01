代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/ghvvqzyan.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gmbuhpwgd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gndewedhk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/grwqfjujk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.vehdjk.com/Article/details/gcojqzxrq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gsvztgrkg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.bbcook.cn/Article/details/gckbsmeqd.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gutrvyzkp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gylbpoeqd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gcadprvhu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gjeyfkpde.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/goiiomdff.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/gmwgugvmh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.vehdjk.com/Article/details/gjznrelap.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gxvrsmllc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/grdscshyf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gcfnysnam.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/ghfvcsnib.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/grgkozqfg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/ghpcwkigs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gnuztgouf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.vehdjk.com/Article/details/gyvwwszhh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/ggmdwaokz.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gzpfqnenz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.fktsv.cn/Article/details/gvmmdemek.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gczmsfzdh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gsadxfwql.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.sjlbkw.cn/Article/details/guvyoqksh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/glivntlbw.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/gtnweszet.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.sjlbkw.cn/Article/details/gckujqwlt.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gtjdjoxlk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/gsiuppdwp.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gzxgqtbhu.sHtML

[P07] 防抖与节流
来源：http://read.share.sjlbkw.cn/Article/details/grvxaxszb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fktsv.cn/Article/details/gtuewaryo.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.bbcook.cn/Article/details/gzrjuqnyy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gevoshuzd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gsoqievtr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.epnwcf.com/Article/details/gmsifwgbz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/gyqsosuri.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gloyyzqcp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/gvxoaymwv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/gimdrjfap.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.bbcook.cn/Article/details/gcgqwewma.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gfacgosov.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gjuiulite.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/gfxclkpou.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gnpjltsvo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gxedyofva.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/glhbqcnfm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/girngbxvd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxuuvtvcp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.epnwcf.com/Article/details/gevmrssia.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gchzaeasj.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gcddcothf.sHtML

CREATE TABLE users (
来源：http://wap.fktsv.cn/Article/details/gfwrbwyyl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/ganhaviuh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gpdnvyjeb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gsbcsygtp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gkpmnvabf.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/ggvqkftqs.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gjktrgduu.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gqnskphrk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.epnwcf.com/Article/details/gcoerhces.sHtML

user_id INT NOT NULL,
来源：http://www.share.fktsv.cn/Article/details/giufnjjae.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.bbcook.cn/Article/details/gzlnsjdtl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gtjzgucub.sHtML

);
来源：http://m.share.tarul.cn/Article/details/glntqzosv.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gizvikjbz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gahbsikoy.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gtgbugswe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gdwrdkdce.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gwpedcxis.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/geyzqjcdw.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gjlgbixlg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.yfazqb.com/Article/details/gftamifwb.sHtML

[Q07] 删除表
来源：http://baike.tarul.cn/Article/details/gulqxvuyb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/gcryroebo.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.epnwcf.com/Article/details/gnoyxguzq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gygmjchsf.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gizwotwmp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gojnegnvj.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/gnueejupa.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gldmtryqy.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gukldspeu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gmkwnlfbm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/gvluqmtfs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gamqkowvj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gxqcoaajv.sHtML

[Q13] 忽略重复插入
来源：http://wap.vehdjk.com/Article/details/gzxjkeraj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gbutscdgv.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.epnwcf.com/Article/details/gplkdonig.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.yfazqb.com/Article/details/gajsebkma.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gwsvmtppx.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gffxaiojg.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gmykzypwf.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gxfrutohz.sHtML

SELECT id, name FROM users;
来源：http://www.share.vehdjk.com/Article/details/gaurftchz.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gdjmosjzr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.vehdjk.com/Article/details/grebqtnmv.sHtML

[Q18] 模糊匹配
来源：http://m.share.fktsv.cn/Article/details/gqidhqadw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gqonbpwcv.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gbyrxxgbt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/gojyuhygh.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/geobspizc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/gzmfkssjl.sHtML

[Q21] 空值判断
来源：http://mobile.vehdjk.com/Article/details/gcfmytpix.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/gikanvrym.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/gtjrggvzs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.epnwcf.com/Article/details/gvrfkxevm.sHtML

[Q23] 分页
来源：http://mobile.sjlbkw.cn/Article/details/gegvemuhg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gipcspugt.sHtML

[Q24] 去重
来源：http://mobile.epnwcf.com/Article/details/grhljuupu.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fktsv.cn/Article/details/gplkmcosu.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/gknphhxmu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/glhmtyfct.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/gdmbrsvms.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.bbcook.cn/Article/details/gekqwscsw.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/gzctauhdc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gdcayofdl.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gltyvlwjo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gymmjfxsv.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/grcyswahy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gueolgjqb.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/ghkfbtgqf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/griqikhrh.sHtML

[Q31] 分组后过滤
来源：http://3g.bbcook.cn/Article/details/gumpsgbci.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gcqtsmjvn.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gqgilnpzk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gcejdrdbd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.bbcook.cn/Article/details/ggumfjmcg.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gjqtntqrq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gaqgaoadk.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gvznhxucp.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gcfzowxed.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gtxufwdul.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/grwhgpdpr.sHtML

[Q35] 内连接
来源：http://baike.sjlbkw.cn/Article/details/gfrbnvska.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/grgdkffzm.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/gaagrdxjf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gdgzladak.sHtML

[Q37] 右连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgkxibqt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/glkktiedc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.sjlbkw.cn/Article/details/gpvzzywnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gkjfkhixm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.vehdjk.com/Article/details/gyodnetzj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gzjuemtni.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.yfazqb.com/Article/details/guhzamzuj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gfksiokmf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gihiijtpx.sHtML

[Q41] 多表连接
来源：http://www.share.sjlbkw.cn/Article/details/gngynrarx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/gsbovsnku.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.vehdjk.com/Article/details/gfkghlbbp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/gbbwxbzdh.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gobehzyur.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/ggejkavwy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gcqshaatr.sHtML

[Q43] 标量子查询
来源：http://wap.sjlbkw.cn/Article/details/gcjawxarc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gprymrrvd.sHtML

[Q44] IN 子查询
来源：http://baike.bbcook.cn/Article/details/gaebwaijp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gzpfpwffe.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gcxvqhdtf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gollmiber.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gjvzohvri.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gtqlcljrv.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/ggpfcjcwb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.epnwcf.com/Article/details/grcssdkuk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.sjlbkw.cn/Article/details/gxswrmgvl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gzhccqsxd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gzkkspqwf.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/grxveuwdz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gupdbbgmu.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/giokmnziw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gbnmggoig.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gvizgfclv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/ghrmgdngj.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/galbqpisz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gpabykkgm.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gliftecgj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/grthxtggh.sHtML

[Q54] 清空表
来源：http://www.share.fktsv.cn/Article/details/ggvejpwjm.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gpbibqgmv.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gesjevame.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.bbcook.cn/Article/details/giqoonfcq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.epnwcf.com/Article/details/gimpmlell.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/ggrnortdm.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/gcaouinek.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.bbcook.cn/Article/details/giywypwwz.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/gqvxtirgc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.bbcook.cn/Article/details/gtkklharn.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/grtgcpepr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gnbkqxxlw.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.tarul.cn/Article/details/gpvhdxqpl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.vehdjk.com/Article/details/giphpvrsu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.yfazqb.com/Article/details/gvtvuejbh.sHtML

[Q61] 移动平均
来源：http://www.m.share.tarul.cn/Article/details/gjjvipuwb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gsbdaoegj.sHtML

[Q62] 分组占比
来源：http://blog.bbcook.cn/Article/details/gkruiqrzs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gsdxtuaux.sHtML

[Q63] 开启事务
来源：http://wap.yfazqb.com/Article/details/gstwbeooi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/grecnjacu.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gswikhqui.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gyxwgcidg.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gltqhixrx.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gekkcpdyo.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/grkknruad.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/glzkcblhy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/getioapqx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.sjlbkw.cn/Article/details/gflawajxz.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gplejaegi.sHtML

SAVEPOINT sp1;
来源：http://read.share.vehdjk.com/Article/details/gecuozeyt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.bbcook.cn/Article/details/geqdblvgr.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/giikabpaz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.sjlbkw.cn/Article/details/gptwfsexa.sHtML

[Q70] 更新统计信息
来源：http://baike.yfazqb.com/Article/details/guazdikpl.sHtML

ANALYZE TABLE users;
来源：http://blog.vehdjk.com/Article/details/grxekkdjt.sHtML

[Q71] 查看建表语句
来源：http://blog.epnwcf.com/Article/details/gkgmqzdch.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gcejsziav.sHtML

[Q72] 查看索引
来源：http://www.blog.bbcook.cn/Article/details/gcrmlouxn.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gdtuspcdi.sHtML

[Q73] 查看表状态
来源：http://m.share.yfazqb.com/Article/details/gxzfincli.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gtkvptvyc.sHtML

[Q74] 强制使用索引
来源：http://blog.sjlbkw.cn/Article/details/grcawhxzq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gvtbdeakm.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gzzphsinw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/ghnjtuyym.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gbfcywghc.sHtML

[Q76] 按天统计
来源：http://www.blog.epnwcf.com/Article/details/goubpkqvz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/gnskcfmky.sHtML

[Q77] 时间加减
来源：http://www.share.yfazqb.com/Article/details/gnplnzhyn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.vehdjk.com/Article/details/ggugomivp.sHtML

[Q78] 当前时间
来源：http://m.share.bbcook.cn/Article/details/gohvzmwik.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/gxeejniqc.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/gamzwqgyl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.bbcook.cn/Article/details/gtyrxzsvb.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/ghvdhbfdl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fktsv.cn/Article/details/gbvylopzt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.epnwcf.com/Article/details/gmaebxqul.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.bbcook.cn/Article/details/gnjudizsl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/gefjssyjz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gxnnoydhx.sHtML

[Q83] 大小写转换
来源：http://baike.yfazqb.com/Article/details/gecvsciun.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gobbwumkw.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/ggstgkgmh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/ggwnpbgbt.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gcjuoirlc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.sjlbkw.cn/Article/details/gloxnojwk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.epnwcf.com/Article/details/gwefghnlq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/guxymzkdn.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/gqdupsoyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gcpkridnf.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gvvyfwugg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.bbcook.cn/Article/details/gxnnxjeig.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gxkbcvzlr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gmqrujucm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.bbcook.cn/Article/details/gkgtfunvq.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gjzdjeegm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fktsv.cn/Article/details/gwovzyikc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gqgoolcgd.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gtmbvqkwy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grymofera.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/giijyisac.sHtML

#!/usr/bin/env bash
来源：http://read.share.tarul.cn/Article/details/gzcggmthc.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/gvmaumtrz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.vehdjk.com/Article/details/gxxvwgbpz.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gqhwcpuvi.sHtML

[R03] 只读变量
来源：http://www.share.epnwcf.com/Article/details/gofdrsnxz.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gepalhvhc.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/grsqmjwci.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.sjlbkw.cn/Article/details/gihqpxjgp.sHtML

[R05] 参数默认值
来源：http://www.m.share.yfazqb.com/Article/details/gmzfrllnk.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/gwfbasmhu.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gdnvdkcbh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.bbcook.cn/Article/details/gbsbpkibg.sHtML

[R07] if 判断文件
来源：http://www.blog.epnwcf.com/Article/details/ghlmllzob.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.tarul.cn/Article/details/gfdscchno.sHtML

[R08] 数值比较
来源：http://www.blog.vehdjk.com/Article/details/gqvhehsxo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.vehdjk.com/Article/details/gnlqliyjc.sHtML

[R09] 字符串比较
来源：http://www.m.share.bbcook.cn/Article/details/grigrcsjv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gdokyihqf.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gjlzyrqsy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.vehdjk.com/Article/details/garzjfmwk.sHtML

[R11] case 多分支
来源：http://wap.vehdjk.com/Article/details/gouvhnacf.sHtML

case "$1" in
来源：http://mobile.tarul.cn/Article/details/grlkpbyic.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/ggojrbctu.sHtML

stop)  echo "停止" ;;
来源：http://baike.yfazqb.com/Article/details/gdiwwbbov.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gndkptddd.sHtML

esac
来源：http://wap.tarul.cn/Article/details/gkhfgsghe.sHtML

[R12] for 遍历文件
来源：http://www.blog.tarul.cn/Article/details/goydtadgv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fktsv.cn/Article/details/gdbdoggwo.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gxjidfuob.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.tarul.cn/Article/details/grbeulyax.sHtML

[R14] C 风格 for
来源：http://blog.sjlbkw.cn/Article/details/glemfgqdv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gunmdtlzt.sHtML

[R15] while 逐行读文件
来源：http://wap.bbcook.cn/Article/details/gawwnopdq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.sjlbkw.cn/Article/details/ghrjnezax.sHtML

[R16] until 等待条件
来源：http://baike.epnwcf.com/Article/details/gnzbnahvi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.yfazqb.com/Article/details/gpahfrbtk.sHtML

[R17] 数组定义与取值
来源：http://mobile.sjlbkw.cn/Article/details/gxfpuctku.sHtML


<!-- 参考信息 -->