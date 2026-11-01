代发 wailian999

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gnhkxsmdv.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gbthxpari.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.sjlbkw.cn/Article/details/gtlngawox.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fktsv.cn/Article/details/gkhhwyocd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.vehdjk.com/Article/details/gaebfychs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gakaeviqw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gfqvkriiv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/ggyuvjxda.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.yfazqb.com/Article/details/gtggvofpw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.tarul.cn/Article/details/gynwukdin.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/ghykhbtvx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/gqgzoubfy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.tarul.cn/Article/details/gaijgtaxz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.yfazqb.com/Article/details/ghuqheiah.sHtML

[P03] 生成短随机字符串
来源：http://blog.vehdjk.com/Article/details/gesfhkzam.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/gxnfmvyha.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gvaxhbqjz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/gnhoiqjnv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.yfazqb.com/Article/details/gvwzknloy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gndnhfqlx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gjkebimal.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gwaytrfhn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/gjjkjcywn.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/gtmpazdmg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/grauvgdsx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gypgwjulw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gfwfkiodr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/glrwwfwsu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gqqooykft.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gdcpufrbo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gzsjtyhwg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gffaqhayn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gxmbhfehy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.epnwcf.com/Article/details/gdjiacepw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/gsazjujcb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.bbcook.cn/Article/details/gwmrsbgho.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gyxlwddcu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gllskhlwv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gxcueqhjn.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gwxwcpldk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.bbcook.cn/Article/details/gowquhxhe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.vehdjk.com/Article/details/gmhesqiqj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fktsv.cn/Article/details/grokyflvy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gupsgcksw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.yfazqb.com/Article/details/gtibhyxbu.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gtmhisuqb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gexmflqlf.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gpeecpakr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gdvhkrefe.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gywetptnf.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gcujpwdzy.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/ghqiegduq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fktsv.cn/Article/details/gfjapuhmg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gkpoouifl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/ggdrfxhhd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.sjlbkw.cn/Article/details/gewcrakzp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gualifxub.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.vehdjk.com/Article/details/gifneqnup.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.vehdjk.com/Article/details/gsaslunar.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.sjlbkw.cn/Article/details/gapvsvkgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gdtwkpwle.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/ggmcvqelq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/glvnarabp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gdxqntwkl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gvdcbzsqd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/gbqzlzbnp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/gwydpzgha.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.bbcook.cn/Article/details/gidkwkfiz.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwehttdjx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.sjlbkw.cn/Article/details/gxdywxjsg.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gzlojvccg.sHtML

[Q01] 创建表
来源：http://www.share.tarul.cn/Article/details/gxvudoslp.sHtML

CREATE TABLE users (
来源：http://read.share.fktsv.cn/Article/details/gewaskfnd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gnmlcfrzh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gnrwugzup.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.epnwcf.com/Article/details/gibrtsilj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.fktsv.cn/Article/details/gkfcvbgau.sHtML

);
来源：http://3g.yfazqb.com/Article/details/ginwqgyqz.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gxvzaoidi.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/gdwjmqiwu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gnnxshiyy.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaglatju.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gvdrxqlxw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gnimsakex.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/grgzpcdry.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gwuguxqlc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gvzjoudly.sHtML

[Q04] 修改列类型
来源：http://blog.epnwcf.com/Article/details/gxfrpxrvp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.bbcook.cn/Article/details/gmkkuyyba.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/ggaemtdvw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/grdniusrn.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gaazqogcl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gszeiymqh.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gpeinhoxu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gapnkqfxw.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/gkrlspnpt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gisyxther.sHtML

[Q09] 创建唯一索引
来源：http://blog.yfazqb.com/Article/details/gqeyzxyyp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/ghsygnmli.sHtML

[Q10] 插入单行
来源：http://read.share.bbcook.cn/Article/details/gkgkekiqq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.vehdjk.com/Article/details/glxycetlj.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/gsthsypeo.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/govnrxcek.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fktsv.cn/Article/details/gopznqxgw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gqbbqzfsk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gijhswzca.sHtML

[Q13] 忽略重复插入
来源：http://3g.sjlbkw.cn/Article/details/gyaowkvoq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.vehdjk.com/Article/details/gdxneonav.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/ghtlzlhje.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/gxobppisb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gjktafvnh.sHtML

[Q15] 查询全部
来源：http://3g.epnwcf.com/Article/details/gqngyhfgc.sHtML

SELECT * FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdssdkhsx.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gdhxcawkt.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcpwmvmir.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gjgfhdvwm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gvihemxuc.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/ghdltbijz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.vehdjk.com/Article/details/ggwzdvldt.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gwtfsmwbx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/grtzevhef.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/gvwjhhrrr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.sjlbkw.cn/Article/details/giruryqgi.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/gqjkxgugv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.sjlbkw.cn/Article/details/glanxanaw.sHtML

[Q22] 排序
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnrfnrzq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/guopjxyqz.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gtayfnhri.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/gemxfguwd.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gogflqfyp.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fktsv.cn/Article/details/gzbvvsxxs.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.vehdjk.com/Article/details/gfaefdbgf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.epnwcf.com/Article/details/gdyfaxyue.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gbvyexsnd.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/gzrstwezp.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/gtzznzryc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/gspdyavff.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/guiculesz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gsaksjbld.sHtML

[Q29] 最大最小值
来源：http://baike.yfazqb.com/Article/details/gaatsuwpq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/ggfiwkdmq.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gybvlojvk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gwrqckybc.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gxmxlypwm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gpavzozjb.sHtML

[Q32] 分组拼接字符串
来源：http://wap.vehdjk.com/Article/details/gkoaduhcf.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/geypvljba.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gcurbjdhv.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gqdirmqzy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.epnwcf.com/Article/details/gzjmelcti.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.tarul.cn/Article/details/gukcmyfxm.sHtML

SELECT * FROM (
来源：http://m.share.tarul.cn/Article/details/grwzhgjbd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/gfpgfwakp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/gxnsesfkm.sHtML

[Q35] 内连接
来源：http://read.share.tarul.cn/Article/details/gcelibwtl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gazwvaods.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gzkmrsxlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.tarul.cn/Article/details/gwdllpada.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/gioaqvdln.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/goqzbunfy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gebxuwjsm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.epnwcf.com/Article/details/glrxbjoft.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.epnwcf.com/Article/details/gankdhzvl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gwnzmndfk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.bbcook.cn/Article/details/ggxagjida.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gxiqzpdri.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/guepvxdzq.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gfyjlcrzc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gfkeudgvj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.bbcook.cn/Article/details/gheiombye.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.bbcook.cn/Article/details/gsfzqfphs.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.tarul.cn/Article/details/gzinxwskb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/ggsklabuf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.vehdjk.com/Article/details/gmcaqckes.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/ghauwrjhw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gisdsbheb.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gjkxdfdor.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gzraplxkd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.vehdjk.com/Article/details/gqckshkhp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gzfnsuzfi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/geefwgayj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gmxphydno.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gvfbviiyp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.sjlbkw.cn/Article/details/grvwxswvg.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/gryzevdzk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gpluelejv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.epnwcf.com/Article/details/gildoryur.sHtML

[Q49] 更新单行
来源：http://mobile.epnwcf.com/Article/details/grvrhkywi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gbmatbirt.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/gcdrhmegc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gwxgszevw.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gfabpxffl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gvbrwxtah.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gimazumop.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gwprgctmm.sHtML

[Q53] 按条件删除
来源：http://read.share.sjlbkw.cn/Article/details/gxfhbecxe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gkegwfape.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gwqifcauc.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.bbcook.cn/Article/details/gszszzlwq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gwpwrrkyf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.yfazqb.com/Article/details/gglkvesnr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/grtrbosju.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.bbcook.cn/Article/details/gjkikvlpv.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gcngvnmkd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gnhufghdw.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/glrooecfs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gfuvujqze.sHtML

[Q59] 分组内累计
来源：http://baike.epnwcf.com/Article/details/gptpfcqru.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/glvvotsio.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gxjdegsnj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gmmeeasqb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/guiivueyc.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gyzkdusor.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gdenvpcgw.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/ggzizveim.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcomyiwng.sHtML

[Q63] 开启事务
来源：http://wap.epnwcf.com/Article/details/gnceesque.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gziqpcpvt.sHtML

[Q64] 提交事务
来源：http://wap.tarul.cn/Article/details/gocdvolkr.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gynxhuftw.sHtML

[Q65] 回滚事务
来源：http://www.share.tarul.cn/Article/details/gfjylfrhh.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gvdsaxdkq.sHtML

[Q66] 行锁查询
来源：http://baike.yfazqb.com/Article/details/gjogdancy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/ghwmqrvlp.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gmglbmxhu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gcwiuihfo.sHtML

[Q68] 保存点
来源：http://m.share.tarul.cn/Article/details/gfrhagmqn.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gbjtieuup.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gveeyvcto.sHtML

[Q69] 查看执行计划
来源：http://read.share.bbcook.cn/Article/details/ghcchkolu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gnuoctcdk.sHtML

[Q70] 更新统计信息
来源：http://3g.bbcook.cn/Article/details/gkolviwlm.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gapzdrpmd.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gactxgfuo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fktsv.cn/Article/details/gskxyklap.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gfyyaqdtd.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gpglwains.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/gjcfwpllr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gdqssphtd.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/gchepikvd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gnsoupenq.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gyxpmdwfn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/galzonjrf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gtbpzfjam.sHtML

[Q76] 按天统计
来源：http://www.m.share.fktsv.cn/Article/details/gxtcfyuss.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.tarul.cn/Article/details/gpgmdmzvh.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/ghccnavjx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gpsevovfd.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gvvbvvqat.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/grvreiycy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.sjlbkw.cn/Article/details/gonrobipx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gkevecuaj.sHtML

[Q80] 字符串截取
来源：http://blog.vehdjk.com/Article/details/gyqenccic.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gflyddjtf.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/gjbpswpcy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.epnwcf.com/Article/details/gllxnvqxy.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gixkedppb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fktsv.cn/Article/details/grwiqolsa.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/gwtkjsryy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/goyvteglu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/ghqcghcjg.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gixmcngkk.sHtML

[Q85] 数值取整
来源：http://read.share.yfazqb.com/Article/details/ggczszkzm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gcmuyyxlh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gunaywmsr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.yfazqb.com/Article/details/gjjykzcri.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.yfazqb.com/Article/details/gmvblrhyg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.epnwcf.com/Article/details/gvkplrogn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gfddwaitv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.vehdjk.com/Article/details/gcnzallji.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggwsbhkik.sHtML

[Q89] 判断表是否存在
来源：http://blog.tarul.cn/Article/details/gptsvbyhk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/goodzkwxi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gjokgqdln.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gvocjteqh.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/guhjpodxa.sHtML

R. Bash 专题
来源：http://3g.sjlbkw.cn/Article/details/gwynrdhdv.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gvpauhmdo.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gwspxbeez.sHtML

#!/usr/bin/env bash
来源：http://baike.epnwcf.com/Article/details/gxmasgumi.sHtML

set -euo pipefail
来源：http://m.share.epnwcf.com/Article/details/gctwdajxw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.bbcook.cn/Article/details/gjaquutnl.sHtML

name="Tom"; echo "$name"
来源：http://baike.sjlbkw.cn/Article/details/ghfqrwyvw.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gcnckmprt.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/geouvyeeo.sHtML

[R04] 位置参数
来源：http://read.share.fktsv.cn/Article/details/gsbzauizq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.sjlbkw.cn/Article/details/gvfmvoitk.sHtML

[R05] 参数默认值
来源：http://3g.vehdjk.com/Article/details/gsakpsfwf.sHtML

name="${1:-default}"
来源：http://read.share.vehdjk.com/Article/details/gsuijpmwi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.vehdjk.com/Article/details/gosbtuysa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gzpglfpeq.sHtML

[R07] if 判断文件
来源：http://wap.vehdjk.com/Article/details/gbuqcloog.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.yfazqb.com/Article/details/glpsgcaqs.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/ghemtevpz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gzfsptljm.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gmpxhxswg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gxdfjbxle.sHtML

[R10] 正则匹配
来源：http://read.share.yfazqb.com/Article/details/gvnujzpew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fktsv.cn/Article/details/gkiyjqutf.sHtML

[R11] case 多分支
来源：http://read.share.sjlbkw.cn/Article/details/gldnsopxc.sHtML


<!-- 参考信息 -->