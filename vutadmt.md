代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gyifyiamf.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.vehdjk.com/Article/details/gftxefpgt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gzxlafusl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gwdlxauao.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gckiflcel.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.tarul.cn/Article/details/gmqarkbop.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gpfketicx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gvcrolkbn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gopjxaend.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gbkwztgny.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gvydqrdmb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gfnpbkqgz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gdapmzoga.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gunzfeouj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.yfazqb.com/Article/details/gfjwqmjxo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gtckovbxc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/ghxdbrzew.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/guopgvxrv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gihoulymu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.sjlbkw.cn/Article/details/gsgzqbdaw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/gsqvnkrkk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/guwsefzkc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.epnwcf.com/Article/details/gqxqkznpg.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/gpahucbvo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gsizestdc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gpkieouin.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gsmkkviks.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gydhvudxm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gosteruru.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/gznssbtcs.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gtxewdaaj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/gwyysyjlb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.yfazqb.com/Article/details/gkjpyjrwy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gubgzqfpj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/gnmutmerf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/grcljyxoh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gpakvdsdd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/geupolfft.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gzwsniywr.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/giwzlasiw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gkkwxpneq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gxevjnuti.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.bbcook.cn/Article/details/gagvbzock.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/girnzjbhe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.epnwcf.com/Article/details/gllvjufzh.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/guohkvixk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/giqdtogqx.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/glxqrssqb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gqiqrfovy.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gkncktsgv.sHtML

[P07] 防抖与节流
来源：http://baike.vehdjk.com/Article/details/gdnsajykv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/ghyhgbzna.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/gzrzqdxls.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gmxlmufkg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/ghdsvzegf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gwmjtvjft.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gahkdxsqn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gvgxnikku.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gssjcojjl.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.yfazqb.com/Article/details/grwahjgwd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gcagbtnyg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gqozuumri.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.bbcook.cn/Article/details/gvozgdzxx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gesbppgay.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gqgmbbgmc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gckxfrxhm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gwhxwynxa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gmhvvoihy.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gwnnklosz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.tarul.cn/Article/details/gpfebbrhe.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqiweccbq.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gnrxbnimj.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/ghnihmjpb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gfvjhtavl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gyqhdyjuv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/gqnbzqxdl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gfwefvnle.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gdmzjluvr.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.tarul.cn/Article/details/grvhpxomq.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/gsuoqapps.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gvpueqjau.sHtML

user_id INT NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/guercdxbn.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gklrtooac.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.bbcook.cn/Article/details/ggveaefct.sHtML

);
来源：http://blog.tarul.cn/Article/details/gjnzinrjf.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gkkbmaups.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.yfazqb.com/Article/details/gffhqgsiz.sHtML

[Q04] 修改列类型
来源：http://mobile.bbcook.cn/Article/details/gquhbqgqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/ghvvczjog.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gynkitute.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gnewaojpt.sHtML

[Q06] 删除列
来源：http://www.share.epnwcf.com/Article/details/glkjxmrpl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.vehdjk.com/Article/details/gktqzriae.sHtML

[Q07] 删除表
来源：http://3g.sjlbkw.cn/Article/details/gwxlzepgx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/gpcukeslf.sHtML

[Q08] 创建普通索引
来源：http://baike.vehdjk.com/Article/details/gcryaupzw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/ghodyzylo.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gpqbjmiug.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.sjlbkw.cn/Article/details/gmjdskkcs.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gcbgbcxkt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gedategwa.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gewlbwhum.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/gkogejbfo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gqfryzskz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gpavfoubj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gmojwdzwz.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gclmbyegv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gveckampk.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/grsehvzjd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/gwojapmup.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.vehdjk.com/Article/details/gydujmfyj.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gfomisxuw.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/gghbwzohb.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gledllkgj.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gwntsuchy.sHtML

[Q17] 条件查询
来源：http://www.share.sjlbkw.cn/Article/details/grisprpgc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gbncmxbqo.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/guxfbokur.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gsnkjmrfe.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gpdprecmz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gbuglstfn.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gmhovyqhc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/ghzrkhvvp.sHtML

[Q21] 空值判断
来源：http://blog.yfazqb.com/Article/details/gjvqkyihh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fktsv.cn/Article/details/gbrnxmxin.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gnqimjjeh.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/ghukuzxnt.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gbjnyyzks.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.vehdjk.com/Article/details/ghypdkjxr.sHtML

[Q24] 去重
来源：http://3g.sjlbkw.cn/Article/details/ghhuzsbtx.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/gakinhphp.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gzlsssgni.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gjzochryv.sHtML

[Q26] 计数
来源：http://www.share.tarul.cn/Article/details/gepmtchwu.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gziqbuokv.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/gmtxumrwn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gtjrokdja.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/geyqjgnuy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.tarul.cn/Article/details/gndrcnrjy.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gpigefqon.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gyuevmhha.sHtML

[Q30] 分组统计
来源：http://www.share.sjlbkw.cn/Article/details/gyjpaxmtg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/ghqmtspxf.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/grdjrtwmi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/gygffdbyr.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gfhydmity.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gmxnzseng.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/ghpjhxnaz.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/gwpgmfesq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gyeioeqnq.sHtML

[Q34] 每组取第一条
来源：http://baike.vehdjk.com/Article/details/gwmykfvsu.sHtML

SELECT * FROM (
来源：http://3g.bbcook.cn/Article/details/gqxnolqlm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.sjlbkw.cn/Article/details/gjqthrntk.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gpopskebg.sHtML

[Q35] 内连接
来源：http://3g.yfazqb.com/Article/details/glehtlvru.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gawuqdvwb.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/grhsuqiaa.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gyhnsdano.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/giozjlbws.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gduoyrdhk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gbmopkvve.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gozrpjini.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.vehdjk.com/Article/details/gokblldlp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/grjrdmhdl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.sjlbkw.cn/Article/details/glebeamvu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/gjwbdggnu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gjqpnxnys.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/grafkxizo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/gbrstqkit.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/ggicwmgpk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gfsgrzcmj.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/gdqgxgjog.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.epnwcf.com/Article/details/gucbdbzhg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gcvdzgcst.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gtlinatet.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.tarul.cn/Article/details/gqrmfflqk.sHtML

[Q44] IN 子查询
来源：http://read.share.epnwcf.com/Article/details/gyapvhjhg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gacekbqnx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/gaedcjamq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gtqmrglyx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gpypzkqyb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gqjadulei.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gfydtztab.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gyahhdhbm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.bbcook.cn/Article/details/gfcdhluvv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.epnwcf.com/Article/details/ghtwzptpb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/ggzeswdwq.sHtML

[Q49] 更新单行
来源：http://mobile.bbcook.cn/Article/details/gzodqpgdo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gcrzqrmsx.sHtML

[Q50] 批量更新
来源：http://baike.bbcook.cn/Article/details/gtbrrjihd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gbktorunt.sHtML

[Q51] 用子查询更新
来源：http://www.share.epnwcf.com/Article/details/gtbyqoetg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gambtvbkq.sHtML

[Q52] 删除指定行
来源：http://www.blog.sjlbkw.cn/Article/details/grjkfryps.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/giascidoe.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gcgogyknx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fktsv.cn/Article/details/gbsolfprb.sHtML

[Q54] 清空表
来源：http://m.share.vehdjk.com/Article/details/gtecadiwk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.sjlbkw.cn/Article/details/geoyuyadu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.bbcook.cn/Article/details/ghrsesepn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gxvwwlked.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/guvmilktc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gmmydxtfv.sHtML

[Q57] 行号
来源：http://www.blog.tarul.cn/Article/details/gzaebadfq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/glfmeqzev.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gjtrdjvxn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gtbxnnlsc.sHtML

[Q59] 分组内累计
来源：http://www.blog.fktsv.cn/Article/details/gpqakoewf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/ghawddslp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/geigqfqlc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/gqszoamll.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gphqdfbtw.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/gsrdjoftc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gaezuedxs.sHtML

[Q62] 分组占比
来源：http://www.blog.bbcook.cn/Article/details/gvnrtnufz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gravvsyju.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gotbulwqh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/goglklqpq.sHtML

[Q64] 提交事务
来源：http://www.m.share.bbcook.cn/Article/details/gkjwubwcj.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gpwgwjeyj.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gzawmefuj.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gqrntgtii.sHtML

[Q66] 行锁查询
来源：http://blog.tarul.cn/Article/details/gjqcrupbs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gpkhyubue.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gvghcrajs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.yfazqb.com/Article/details/gctvsavrj.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gryychwvd.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gqunyrleh.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gqaljnbud.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/gkolvflss.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.bbcook.cn/Article/details/gyjihlmfz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gsbpwpkjm.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gletdwvip.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gllfwwjrj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fktsv.cn/Article/details/ghmdatqwa.sHtML

[Q72] 查看索引
来源：http://baike.epnwcf.com/Article/details/ggctjoiny.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gmscbqkmn.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gemfqdukd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gqailuhlp.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gdzjdocyd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gikmzwwuy.sHtML

[Q75] 日期格式化
来源：http://mobile.fktsv.cn/Article/details/gsksgqcrt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gvtidxzku.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.yfazqb.com/Article/details/gkdbwxheo.sHtML

[Q76] 按天统计
来源：http://www.m.share.vehdjk.com/Article/details/ggaiiqbzb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/gnsszcacy.sHtML

[Q77] 时间加减
来源：http://baike.yfazqb.com/Article/details/gjgsscqmn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/ghbnxbreb.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gmerboyfh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gsadfdtrn.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gmwgamdup.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.vehdjk.com/Article/details/gekuygrjs.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gwuxiqrnv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.epnwcf.com/Article/details/ggsmdmzly.sHtML

[Q81] 字符串替换
来源：http://baike.epnwcf.com/Article/details/gzwltkqwo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/glatjyhns.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.tarul.cn/Article/details/gzzziyuel.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/giibjctye.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/gkzzhxdoy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/guxvvooye.sHtML

[Q84] 去除首尾空格
来源：http://mobile.sjlbkw.cn/Article/details/gdmcsqdkg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gyqusgirq.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gxhuohilv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.epnwcf.com/Article/details/ghxstcwcy.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gicviyxrx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gxrzljide.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.vehdjk.com/Article/details/gnnzyebgd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.sjlbkw.cn/Article/details/gdnbhaejq.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.yfazqb.com/Article/details/gsuzpakno.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.yfazqb.com/Article/details/gklfwmosc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmvopvbps.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.epnwcf.com/Article/details/gtvvllrrj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.yfazqb.com/Article/details/gnoroosjy.sHtML

[Q90] 生成序号列
来源：http://read.share.fktsv.cn/Article/details/gxiqmxyjp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.yfazqb.com/Article/details/gidntucvl.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gkwalfoaf.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/glpxpledt.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzehgglcw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.tarul.cn/Article/details/gqcnmnobr.sHtML

#!/usr/bin/env bash
来源：http://baike.tarul.cn/Article/details/gfuwgumwp.sHtML

set -euo pipefail
来源：http://www.share.bbcook.cn/Article/details/guecdbsmf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/gbunrhegn.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gmshwktfv.sHtML

[R03] 只读变量
来源：http://read.share.yfazqb.com/Article/details/gizoiwpko.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gkhktgetw.sHtML

[R04] 位置参数
来源：http://baike.sjlbkw.cn/Article/details/gybitwemb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/ggdwfvqhw.sHtML

[R05] 参数默认值
来源：http://baike.tarul.cn/Article/details/gadunqbia.sHtML

name="${1:-default}"
来源：http://3g.sjlbkw.cn/Article/details/gnctgjlzb.sHtML

[R06] 判断命令是否存在
来源：http://m.share.epnwcf.com/Article/details/gcrddmlaq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fktsv.cn/Article/details/gwylwigiy.sHtML

[R07] if 判断文件
来源：http://www.blog.fktsv.cn/Article/details/gxwybgmik.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gdpweztwe.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gdciohlai.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.tarul.cn/Article/details/gsscxrmpl.sHtML

[R09] 字符串比较
来源：http://mobile.epnwcf.com/Article/details/gjfpiuvpu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.epnwcf.com/Article/details/gpgnbtwdz.sHtML

[R10] 正则匹配
来源：http://blog.vehdjk.com/Article/details/gqstoegdf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gycjylkaw.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/gaihnjuvu.sHtML


<!-- 参考信息 -->