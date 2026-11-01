代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gvtcomnaf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gtasctage.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gqtnrzyyc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gqjiqfmlx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gdnxfevih.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkkbqnhg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/glokipcnd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/gxilqsyzk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.sjlbkw.cn/Article/details/gkifttilp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/govevcqtr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.epnwcf.com/Article/details/gnndovxhc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gypjqgbqi.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/grnfelorz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gfswwosie.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gomrlyxoi.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gwlgttvrs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/gdvhlemmp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gmqqworkf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gduerxlhi.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gccenvlxs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gqbcqjbeq.sHtML

TS:   if (x == null) {}
来源：http://read.share.tarul.cn/Article/details/gazmnlrar.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/ggzhwigit.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gmmfjdugn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.fktsv.cn/Article/details/guxbxkixk.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gquxnapop.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gexubnkdz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/gvzcrgrbv.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fktsv.cn/Article/details/gedougdvy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gdbcrtkjy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gzplnfuzc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fktsv.cn/Article/details/gzfarkzva.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gpuzigsai.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.vehdjk.com/Article/details/gjasvoygq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/gxmvrvkjo.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gfuhewvie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gdefplfab.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.tarul.cn/Article/details/gxvvcgysd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/gzfyumfau.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.yfazqb.com/Article/details/gjlqemykb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/gufknqqce.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/ghbiangie.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gmtfrlxgk.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.yfazqb.com/Article/details/gnhkxzsxj.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gigagybvf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/guzzvwubt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkvbenzuw.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gcndlsvmp.sHtML

CREATE TABLE users (
来源：http://read.share.yfazqb.com/Article/details/gsmekcuty.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gnjrkwaob.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.fktsv.cn/Article/details/gcehdlrgu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.yfazqb.com/Article/details/gzlqxbhhg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gmcyvdxdb.sHtML

);
来源：http://blog.tarul.cn/Article/details/glotjrkdp.sHtML

[Q02] 创建带外键的表
来源：http://3g.tarul.cn/Article/details/guwyeowae.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gqxrxswzr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gcurobzza.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/grkzcmntk.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.tarul.cn/Article/details/gnxlksqqi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gnmefhdva.sHtML

);
来源：http://read.share.tarul.cn/Article/details/gxhkxppes.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/gnyiwslah.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/gbrtjycke.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/gsphmfdwq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gcwjjitxt.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/glcpzgmbi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gmxwdsnzm.sHtML

[Q06] 删除列
来源：http://www.m.share.bbcook.cn/Article/details/gtydknmmz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/goduufpam.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/grwiqakic.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/gjsrtxhqv.sHtML

[Q08] 创建普通索引
来源：http://mobile.tarul.cn/Article/details/gryjuajxa.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/goanqpbhu.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/geepbcaoo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/goszwsixx.sHtML

[Q10] 插入单行
来源：http://mobile.sjlbkw.cn/Article/details/gkdrznjxq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gulabzygk.sHtML

[Q11] 一次插入多行
来源：http://blog.yfazqb.com/Article/details/gqraobmtn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gpvstejdj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/ghikdciwh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.tarul.cn/Article/details/ghbidywzt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/gclyecjwl.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gvrparpso.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gxtlkprya.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gickrussc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/gnitslpow.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/genicqyvm.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gkorhxovx.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gcjrriciv.sHtML

[Q16] 查询指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gfajyabkl.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gcnyfsyav.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/grsutjbhr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gofjhwqeh.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gntfgtsww.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.vehdjk.com/Article/details/gdvjaykek.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gizmgigaf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gttuvcrzr.sHtML

[Q20] IN 列表
来源：http://m.share.epnwcf.com/Article/details/gitvvpirk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gxrjqtdhn.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gxcvsdsxb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.bbcook.cn/Article/details/ggfsomnlq.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/ghjtmredd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.sjlbkw.cn/Article/details/gqcmqbzyz.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/ggvbfgcqs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gjnqjkcox.sHtML

[Q24] 去重
来源：http://wap.yfazqb.com/Article/details/grapdzfhf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnfrmupfs.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gnyuetntm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.yfazqb.com/Article/details/gpirtdecg.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/giafcuobs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gghmgbdit.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/geoynuopw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gnivzupdd.sHtML

[Q28] 求和与平均
来源：http://blog.bbcook.cn/Article/details/guxcynqhu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gtdthjbgm.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/gqeleujdg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gqcnmpsaw.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gjsfmnfin.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gcqscemth.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/giylfrmjx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fktsv.cn/Article/details/geiszhltr.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gglbyrogo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gyneekptk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/grytkzghn.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/grxrfpted.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.bbcook.cn/Article/details/gkazrvqym.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/ggxhxlgef.sHtML

SELECT * FROM (
来源：http://www.share.fktsv.cn/Article/details/gbepkkflw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gkvgdcodt.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/glogbiboj.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/ghwhhcrng.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gkaxidfwn.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gnrtnkjyv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/gqhkjptxw.sHtML

[Q37] 右连接
来源：http://www.share.epnwcf.com/Article/details/gcgugpkcx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.tarul.cn/Article/details/gdcrgytvy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gkokdrfum.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.vehdjk.com/Article/details/gavlcxozq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gzodnteib.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fktsv.cn/Article/details/gwmlnfcvy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.epnwcf.com/Article/details/glcnjapcj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gsijxoqtr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gizmkmrua.sHtML

[Q41] 多表连接
来源：http://baike.bbcook.cn/Article/details/gkrndayty.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/ggndiuixq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.vehdjk.com/Article/details/gfshlrknu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/ggjyxycgl.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.tarul.cn/Article/details/glfvjtlqc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gkipkxcqp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gnhfltyxw.sHtML

[Q43] 标量子查询
来源：http://read.share.fktsv.cn/Article/details/gzsgrphcd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gbsdhyukj.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gifjlkmho.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gdpoqlxrv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.bbcook.cn/Article/details/ghjejvvge.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gmrirwrai.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/gbmqbvbln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gmojojsyj.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gkkvvrfjx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fktsv.cn/Article/details/gklnukjix.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gyhgmhvlw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gbaatpdat.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gmytpicfo.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gvdyzmjbb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gdkuvscnh.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/giidwebbd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/ggjbzuytu.sHtML

[Q51] 用子查询更新
来源：http://www.blog.bbcook.cn/Article/details/gamtucplr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gwxczbast.sHtML

[Q52] 删除指定行
来源：http://blog.yfazqb.com/Article/details/gqnedanvj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/goaroochy.sHtML

[Q53] 按条件删除
来源：http://www.blog.epnwcf.com/Article/details/ggwdxarkd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gatdarwqc.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gfhqcyily.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/gqinmzptg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/gpdlrqowj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gupsvjdoi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gygaeiuzh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gmbgrnmcm.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gpxehjdjt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gqexhvxnn.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/goctufgxe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gyrokgnwk.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gdmxioiqo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gfajurboc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.epnwcf.com/Article/details/gvhnphbtb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.tarul.cn/Article/details/grtbsjuek.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gxgcdubgd.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gyefprnfy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/ggorlimtl.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/gbznydwxk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gwipexang.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gxkpvgarm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.tarul.cn/Article/details/gsueknpfl.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gvvbvabau.sHtML

COMMIT;
来源：http://m.share.tarul.cn/Article/details/gbchjdwqv.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/guctrfhhr.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gzmttzzac.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/ghqhtmpxq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/garnlhzwq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gcblcbxao.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gaecoptam.sHtML

[Q68] 保存点
来源：http://baike.vehdjk.com/Article/details/ggfgrxncg.sHtML

SAVEPOINT sp1;
来源：http://blog.bbcook.cn/Article/details/gszlxkmhe.sHtML

ROLLBACK TO sp1;
来源：http://baike.tarul.cn/Article/details/gfwqberyj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fktsv.cn/Article/details/gpxqwpvcy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gsxodidhk.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gzxklcnrt.sHtML

ANALYZE TABLE users;
来源：http://baike.yfazqb.com/Article/details/geiqfkdgi.sHtML

[Q71] 查看建表语句
来源：http://wap.vehdjk.com/Article/details/gpwxnhvvb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.vehdjk.com/Article/details/gusylhacg.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gogatlkme.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.tarul.cn/Article/details/gedredqxo.sHtML

[Q73] 查看表状态
来源：http://www.share.sjlbkw.cn/Article/details/gdkapgvnq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/ggrzhknwj.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/ghvwraoqt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.tarul.cn/Article/details/ghuvtaxvj.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/glustzmco.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gbhoczkbx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.epnwcf.com/Article/details/gugevayfn.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/ggavirkgk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/gjrxurhxp.sHtML

[Q77] 时间加减
来源：http://www.m.share.sjlbkw.cn/Article/details/ghsvqdyja.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.bbcook.cn/Article/details/gzhsvewwb.sHtML

[Q78] 当前时间
来源：http://baike.epnwcf.com/Article/details/gxqmdkqrv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/ggixngsuq.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrkvbgrb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbdkgabu.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gasqlwigf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gzerjgdlq.sHtML

[Q81] 字符串替换
来源：http://read.share.tarul.cn/Article/details/gsvxvyzks.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.vehdjk.com/Article/details/gkaathelc.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/gtptxkpay.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gqkvqaoej.sHtML

[Q83] 大小写转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgzezkvz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gwdexpgfp.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gdwrxvnlc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/glqyhhgjw.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/gvlwndded.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/gmzdkiqwg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gguqqrzxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.tarul.cn/Article/details/gmztxsble.sHtML

[Q87] JSON 字段做条件
来源：http://3g.yfazqb.com/Article/details/glojtngfr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.bbcook.cn/Article/details/gmolsfdbw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/geraeqwah.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.vehdjk.com/Article/details/gbbfvprbq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.tarul.cn/Article/details/gsaalcoxy.sHtML

[Q89] 判断表是否存在
来源：http://blog.yfazqb.com/Article/details/ggwthzplf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fktsv.cn/Article/details/globwawru.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gxtfckhco.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gjplvnfdn.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjboukxda.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/geddmddjw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyjblnvpr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fktsv.cn/Article/details/gwfmzzigt.sHtML

#!/usr/bin/env bash
来源：http://mobile.tarul.cn/Article/details/ginqdaekv.sHtML

set -euo pipefail
来源：http://baike.yfazqb.com/Article/details/gqnbzyygz.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtiozvzq.sHtML

name="Tom"; echo "$name"
来源：http://blog.bbcook.cn/Article/details/gsnyzbqzo.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/gcqxxeoee.sHtML

readonly PI=3.14
来源：http://read.share.bbcook.cn/Article/details/gdgfmzlxz.sHtML

[R04] 位置参数
来源：http://3g.yfazqb.com/Article/details/gqwvhujew.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gctrqdsrm.sHtML

[R05] 参数默认值
来源：http://blog.fktsv.cn/Article/details/gyevnnwsl.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gtegisjpj.sHtML

[R06] 判断命令是否存在
来源：http://mobile.epnwcf.com/Article/details/ghedbwgtu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/gbwygupqi.sHtML

[R07] if 判断文件
来源：http://baike.vehdjk.com/Article/details/glhevhdui.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gbzbzlwwx.sHtML

[R08] 数值比较
来源：http://www.blog.tarul.cn/Article/details/gjctcyzrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.epnwcf.com/Article/details/gqofznwcz.sHtML

[R09] 字符串比较
来源：http://www.m.share.tarul.cn/Article/details/ggwzsrvpa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.vehdjk.com/Article/details/ggepqgylf.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/glcdkmmkn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/guxnscemn.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gemxhaqzo.sHtML

case "$1" in
来源：http://mobile.vehdjk.com/Article/details/gaydhgbiu.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gkdmfpvzs.sHtML

stop)  echo "停止" ;;
来源：http://baike.fktsv.cn/Article/details/gugekkcsh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.sjlbkw.cn/Article/details/gsbczazqf.sHtML

esac
来源：http://blog.tarul.cn/Article/details/gojtlybro.sHtML

[R12] for 遍历文件
来源：http://baike.epnwcf.com/Article/details/gdfnolbpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.yfazqb.com/Article/details/giqjmsguc.sHtML

[R13] for 计数循环
来源：http://blog.yfazqb.com/Article/details/ggaaegmel.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.tarul.cn/Article/details/gxurrwsek.sHtML

[R14] C 风格 for
来源：http://www.blog.fktsv.cn/Article/details/gtfsikehd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.sjlbkw.cn/Article/details/gwbsmbjnp.sHtML

[R15] while 逐行读文件
来源：http://baike.vehdjk.com/Article/details/gdujxssrr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.vehdjk.com/Article/details/galmtzovu.sHtML

[R16] until 等待条件
来源：http://baike.tarul.cn/Article/details/gpxmwmbsu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.bbcook.cn/Article/details/gendopgyj.sHtML

[R17] 数组定义与取值
来源：http://wap.yfazqb.com/Article/details/gtzrozhof.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.yfazqb.com/Article/details/gqlomchaf.sHtML

[R18] 遍历数组
来源：http://mobile.vehdjk.com/Article/details/gjpfuwjma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fktsv.cn/Article/details/gndaosqmr.sHtML

[R19] 数组长度
来源：http://read.share.bbcook.cn/Article/details/gblplsykk.sHtML

echo "${#arr[@]}"
来源：http://read.share.epnwcf.com/Article/details/guhnmudvb.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fktsv.cn/Article/details/gqlabjhoa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.yfazqb.com/Article/details/gpyzyybvt.sHtML

[R21] 字符串长度
来源：http://www.m.share.bbcook.cn/Article/details/gquvtxmct.sHtML


<!-- 参考信息 -->