代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gleuhaqow.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.epnwcf.com/Article/details/ginmufcpj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/glokypnqi.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gzzchvnot.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/glbjfvijl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gjajvqdpq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/grzjkgfzg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gutylptvk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/giwzvldxp.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/gcmiavokq.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gsfmbdgef.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gtvqlndgm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gzsodlnrw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gkmxiurcj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/geyotqipl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/glvjiyyvu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/givdzeldc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/ggaooqalm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gzmwgbadn.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/grnnpmtmw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.sjlbkw.cn/Article/details/gepzeglct.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.yfazqb.com/Article/details/gfsfxdpcj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/gezoygqcq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gxziteath.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/gsdpztwot.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gdoryapsr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gptmfxist.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/goqrotxed.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fktsv.cn/Article/details/gqimdtpda.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/guwdfkqif.sHtML

[P07] 防抖与节流
来源：http://m.share.bbcook.cn/Article/details/gyommkeeh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/goopctjqn.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/ghvzxgvit.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gvzrvmzpm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gfpferxvx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/gjxfrzgcs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gdvmtnfsn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/grqihsrma.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gyylrzszz.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/gqfaqladl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gjklkfnmc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.epnwcf.com/Article/details/gicvodgky.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fktsv.cn/Article/details/ggufshncj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gogktrfta.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.yfazqb.com/Article/details/gjyyiytcs.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/gztdwchbc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gohyebshg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gielzwmkk.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gtdnsehre.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gpbjprsdz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gsaijraor.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gzlxcwetb.sHtML

CREATE TABLE users (
来源：http://m.share.tarul.cn/Article/details/gghahewjy.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gskipswab.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gypshpzlh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gdlfgorrp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.yfazqb.com/Article/details/gqmujvtdj.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gpotwiztc.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gbtbpmbru.sHtML

CREATE TABLE orders (
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoewbbun.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gequcwtuo.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/ggwtxnfat.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.yfazqb.com/Article/details/gajgcgman.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fktsv.cn/Article/details/ggcbortff.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gbqperedz.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/ggfkvrsvc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.fktsv.cn/Article/details/grjlutqsk.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gjuzolahb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.fktsv.cn/Article/details/gwqbicteb.sHtML

[Q05] 重命名列
来源：http://baike.vehdjk.com/Article/details/gksxdjmdn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.yfazqb.com/Article/details/guvorpvlh.sHtML

[Q06] 删除列
来源：http://mobile.epnwcf.com/Article/details/gccqtzzql.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/glvkedfvi.sHtML

[Q07] 删除表
来源：http://blog.sjlbkw.cn/Article/details/gseyprtcv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gxlnyhyyy.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gdqzxudng.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gnesfpfge.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/grrhqbtbm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gzwdwfszf.sHtML

[Q10] 插入单行
来源：http://read.share.epnwcf.com/Article/details/gyynkqypq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gjprygcgz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.vehdjk.com/Article/details/gsfjgebcy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gyzfjcyfe.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gvumqaids.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gkbbhievo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.bbcook.cn/Article/details/gbqzjxlmv.sHtML

[Q13] 忽略重复插入
来源：http://m.share.bbcook.cn/Article/details/gcepoyewi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gttdwfldm.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/gofztyowl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gblfmhvet.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gtjkmyumb.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/ggnuqhdcf.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/gicyovmyc.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gmoucfagm.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/gkefouvzc.sHtML

[Q17] 条件查询
来源：http://www.blog.vehdjk.com/Article/details/gtpkjfbno.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.tarul.cn/Article/details/gqeiziayi.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/gzssbvwck.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gfwigmeki.sHtML

[Q19] 范围查询
来源：http://m.share.fktsv.cn/Article/details/gqrtmpwnn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/gugxyvzsr.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/ghvizrufc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.vehdjk.com/Article/details/ggrrfahok.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gbunxoldl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fktsv.cn/Article/details/gzzidgcjt.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gfejsbthh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gcbmnqqrl.sHtML

[Q23] 分页
来源：http://3g.vehdjk.com/Article/details/geihmzwrs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/gtjvlslrd.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/gcijtwwhx.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gljfivolo.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gmeetekqe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gmbxbxeej.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/ghdvepjsv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.vehdjk.com/Article/details/gdwyqetaq.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/govghuejj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.yfazqb.com/Article/details/gftqdpnzk.sHtML

[Q28] 求和与平均
来源：http://baike.vehdjk.com/Article/details/gunvhvytp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gsiwqevgd.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/ghpsxcvkn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.yfazqb.com/Article/details/gyjtbqgay.sHtML

[Q30] 分组统计
来源：http://wap.sjlbkw.cn/Article/details/gwwjzlvpi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gzdhxlkvh.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gicksteoz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gzsdbslej.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gwhkzrhdc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gawfizcvx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gbshqvqvo.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/gjbnzpbtz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.vehdjk.com/Article/details/gqctlskpr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/gsolpyczs.sHtML

SELECT * FROM (
来源：http://m.share.fktsv.cn/Article/details/gejkhkjwh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gewbbnnux.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gpemuocjj.sHtML

[Q35] 内连接
来源：http://m.share.yfazqb.com/Article/details/gnmwsthoy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/gwlrxglxh.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gxvtayjoi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gqkzcadzq.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/glpwievje.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.yfazqb.com/Article/details/gfxosajqa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.sjlbkw.cn/Article/details/grbmtvtvb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fktsv.cn/Article/details/globjzbxn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.vehdjk.com/Article/details/gkulqmowx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gtnlgpkqp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.epnwcf.com/Article/details/gcasnjxhv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/gwgefnwiq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gxdcpayhd.sHtML

[Q41] 多表连接
来源：http://blog.vehdjk.com/Article/details/gncqhrrmt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gctkrszio.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.vehdjk.com/Article/details/gdhaeugro.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gyqocqgpo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.epnwcf.com/Article/details/gckknirgq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gylfrkmfn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.yfazqb.com/Article/details/ginvvakyu.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gvvoiigve.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gyqjplpdh.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gqzasrfex.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.bbcook.cn/Article/details/gyhlvwxhu.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/ghrwstfis.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gekmimggj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.yfazqb.com/Article/details/ghtogpfly.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/ghxbtjcja.sHtML

[Q47] 与平均值比较
来源：http://wap.bbcook.cn/Article/details/gvibkhzad.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.bbcook.cn/Article/details/gdicxupwl.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.sjlbkw.cn/Article/details/gdvrhxavc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gberzsjbf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/ghaoqzgdy.sHtML

[Q49] 更新单行
来源：http://m.share.fktsv.cn/Article/details/gepwoidbs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.bbcook.cn/Article/details/gqfechhgp.sHtML

[Q50] 批量更新
来源：http://baike.epnwcf.com/Article/details/gboyroetu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/ggbgwbaeq.sHtML

[Q51] 用子查询更新
来源：http://read.share.sjlbkw.cn/Article/details/gqemrhknk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.epnwcf.com/Article/details/gibntbofm.sHtML

[Q52] 删除指定行
来源：http://baike.epnwcf.com/Article/details/gyykldtec.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gftqyuydb.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gianezowr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gywprsyar.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gvkmcwjxz.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gfiwtedqn.sHtML

[Q55] 排名（并列占位）
来源：http://baike.sjlbkw.cn/Article/details/gakewrsnd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gewwvkkdx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.bbcook.cn/Article/details/gqalkqkrh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gvrcqibuu.sHtML

[Q57] 行号
来源：http://read.share.epnwcf.com/Article/details/gctmbdwng.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmkrkxccl.sHtML

[Q58] 累计求和
来源：http://baike.bbcook.cn/Article/details/gccelkgrl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gqdaluvsn.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/gtarfzpdj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gsiqjcflf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/ganmiinjq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gheaurwlz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.epnwcf.com/Article/details/gxfpcxnyu.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gkiplyfgb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gjuzeethc.sHtML

[Q62] 分组占比
来源：http://wap.bbcook.cn/Article/details/gcpqtqkta.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gjslrenrz.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gemrmumwl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.tarul.cn/Article/details/gbqntggoh.sHtML

[Q64] 提交事务
来源：http://www.m.share.tarul.cn/Article/details/gteqkcrtx.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/ghlxmposk.sHtML

[Q65] 回滚事务
来源：http://blog.tarul.cn/Article/details/grzttjpdp.sHtML

ROLLBACK;
来源：http://blog.vehdjk.com/Article/details/goaagvsdt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/giporylzc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fktsv.cn/Article/details/gaehmpkmq.sHtML

[Q67] 设置隔离级别
来源：http://3g.yfazqb.com/Article/details/ggliulcsn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/glhudbgge.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gbewecohb.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gnccbbqlv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/ghyfvxtpp.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/ghiscbnta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gqkxbnpou.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/grrfujvbx.sHtML

ANALYZE TABLE users;
来源：http://wap.vehdjk.com/Article/details/gtxncgtaj.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gtnkiwiws.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.yfazqb.com/Article/details/gkeqchjrg.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gqxfkvcvs.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/glqeaadcm.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gbimgsrdf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/gfjibugku.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/gaassgges.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gdwjmcydl.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gchnmoxus.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gbgrojfzp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gstteuwgy.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gfhzkywwx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.sjlbkw.cn/Article/details/gtbtdpdoa.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gphbgelnt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/gqgdwgswl.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gstsvjqbg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/gufiafqax.sHtML

[Q79] 字符串拼接
来源：http://wap.sjlbkw.cn/Article/details/gpteyuvau.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gskgqtfnb.sHtML

[Q80] 字符串截取
来源：http://read.share.tarul.cn/Article/details/gobvujvvu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gtezvbamy.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gsomtzbni.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.yfazqb.com/Article/details/gshezmtzq.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fktsv.cn/Article/details/gpjbklvmk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gxvmrnqrk.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gscjqddey.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gxfjtykzf.sHtML

[Q84] 去除首尾空格
来源：http://blog.fktsv.cn/Article/details/gteouhasx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gjxophtwt.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/ghphqbmjd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gcbyvehry.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fktsv.cn/Article/details/gtdzfamob.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.bbcook.cn/Article/details/gfkbtcmat.sHtML

[Q87] JSON 字段做条件
来源：http://blog.bbcook.cn/Article/details/gjppokdaz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.sjlbkw.cn/Article/details/glsxuczhj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gmehoxyfr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.yfazqb.com/Article/details/gjmwsaqdb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/gtwebxzth.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gpjnjouux.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gntfxgliw.sHtML

[Q90] 生成序号列
来源：http://www.blog.fktsv.cn/Article/details/gwbafidee.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.vehdjk.com/Article/details/gggvombfe.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsuygxhay.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gtxzgizcm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gotdibunr.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gnxuzcqxb.sHtML

#!/usr/bin/env bash
来源：http://wap.vehdjk.com/Article/details/gudtgluvx.sHtML

set -euo pipefail
来源：http://baike.epnwcf.com/Article/details/gfhmoihzu.sHtML

[R02] 变量赋值与使用
来源：http://blog.fktsv.cn/Article/details/ggoyivaec.sHtML

name="Tom"; echo "$name"
来源：http://3g.vehdjk.com/Article/details/gpydjtdlk.sHtML

[R03] 只读变量
来源：http://www.blog.vehdjk.com/Article/details/gxzgbyxvr.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gdqybwrbq.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gurqbvgat.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.epnwcf.com/Article/details/gztkckcud.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gwfwnwfir.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gsrikeijr.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gbihevale.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gotqwrklu.sHtML

[R07] if 判断文件
来源：http://www.m.share.yfazqb.com/Article/details/gbksffvlp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.yfazqb.com/Article/details/gasvjjxrz.sHtML

[R08] 数值比较
来源：http://3g.fktsv.cn/Article/details/gvtcxmjms.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/gplliikco.sHtML

[R09] 字符串比较
来源：http://www.share.vehdjk.com/Article/details/ganjxpxom.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gcmqrsmfo.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/ghpqvzkpi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.sjlbkw.cn/Article/details/gomynqyqb.sHtML

[R11] case 多分支
来源：http://m.share.fktsv.cn/Article/details/gplceigmf.sHtML

case "$1" in
来源：http://www.blog.tarul.cn/Article/details/gbzmzcylu.sHtML

start) echo "启动" ;;
来源：http://m.share.vehdjk.com/Article/details/gvtlxinmf.sHtML

stop)  echo "停止" ;;
来源：http://read.share.vehdjk.com/Article/details/gqlspsyvj.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fktsv.cn/Article/details/gwcznodlf.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/guzoapyvn.sHtML

[R12] for 遍历文件
来源：http://read.share.vehdjk.com/Article/details/gazfippus.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.sjlbkw.cn/Article/details/gdraiwlbz.sHtML

[R13] for 计数循环
来源：http://mobile.tarul.cn/Article/details/gcrbgikco.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.bbcook.cn/Article/details/gryjypdej.sHtML

[R14] C 风格 for
来源：http://read.share.fktsv.cn/Article/details/gfatfrwyi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.vehdjk.com/Article/details/geecyexta.sHtML

[R15] while 逐行读文件
来源：http://blog.vehdjk.com/Article/details/gbcbxqztq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfpnedai.sHtML

[R16] until 等待条件
来源：http://www.blog.sjlbkw.cn/Article/details/gxckmacev.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.tarul.cn/Article/details/grvhoicoy.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.vehdjk.com/Article/details/ghhcecbmf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.vehdjk.com/Article/details/gigaibbwd.sHtML

[R18] 遍历数组
来源：http://blog.yfazqb.com/Article/details/gdigpbick.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.yfazqb.com/Article/details/gzxzxytqc.sHtML

[R19] 数组长度
来源：http://baike.epnwcf.com/Article/details/gtfanpugb.sHtML


<!-- 参考信息 -->