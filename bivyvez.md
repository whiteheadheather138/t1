代发 wailian999

TS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gdkoltmlo.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/gcjxhdwnv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.vehdjk.com/Article/details/gfnwiyife.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gstaxxowr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.fktsv.cn/Article/details/gxxredakx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gocqoomwp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gihyueyvl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.vehdjk.com/Article/details/ghygzlqzb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.vehdjk.com/Article/details/gjsdroqrc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.yfazqb.com/Article/details/ghiabmtdx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gowrkfaoy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/glatrbtch.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/ggsvnvfsk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gxvzickwj.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gkfkgwqkq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.yfazqb.com/Article/details/gvojhltec.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.tarul.cn/Article/details/gyaqcwonu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gcxjzlttf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gqllmmmiz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gknddkyrk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.tarul.cn/Article/details/gkdztmypv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.vehdjk.com/Article/details/gqvxtshec.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/gdwtbwxaq.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gdrlhoiik.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gncbeugoz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gntcklorx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gtxzphowi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gniudkkvp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gjazxlldz.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/grngnpqcs.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gnjdocuio.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.vehdjk.com/Article/details/glqlglhlz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gpswzjlag.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gjdewhiwj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.fktsv.cn/Article/details/gcyhxwsyt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/gbhunhldm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gkfxnuhwi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gvwpcqctv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gchljysbm.sHtML

Ruby: a == b
来源：http://www.m.share.fktsv.cn/Article/details/gviuvmnjf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/ghmlvieuy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fktsv.cn/Article/details/gwxgspnki.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.bbcook.cn/Article/details/gqdhtnlcb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gnxdvlvqj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/gvujrspqk.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gfwokohnj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/gatxiylnz.sHtML

Go:   if x == nil {}
来源：http://mobile.vehdjk.com/Article/details/gmunhwpgy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.sjlbkw.cn/Article/details/gkwznpked.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gquwdxspd.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gsbuvaylk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/godqwikhm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.yfazqb.com/Article/details/gzeywjblq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gxtvoigyf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gbxaxlhuz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gaxrirzoc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/guvjnbhqw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.tarul.cn/Article/details/gmsxxwebr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gfdbtduiz.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/gfcfhxfie.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.tarul.cn/Article/details/gitieoihc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.bbcook.cn/Article/details/gvvpnsmpe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gqvafgfjv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.tarul.cn/Article/details/gyqidpfsx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.tarul.cn/Article/details/gpouvbxms.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/gnlfmtznw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/gxfeapthb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gkvfitecg.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gtnnpbteh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/goyqgrqia.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gazsmwiwn.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gmjftuzlz.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gokqtknix.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gzadtmtqt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gewpahbdd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/garmjfcdo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/ggavkcppu.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/ggnjscdhs.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gqaziyumb.sHtML

CREATE TABLE orders (
来源：http://m.share.epnwcf.com/Article/details/gawzsszxv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gbbdccbap.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/ggvapewnt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gxztcyrdd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.bbcook.cn/Article/details/guduuybqx.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gewmfegnd.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gzbankpoc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gxmsqzswh.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gwhswmsmp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.vehdjk.com/Article/details/goqyallmm.sHtML

[Q05] 重命名列
来源：http://read.share.bbcook.cn/Article/details/geiotukmi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/ggotmcfho.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gsmzxoobz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.bbcook.cn/Article/details/gtsjfnxrq.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gfowjrdfm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gomlxgvyu.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/glhctvucz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.yfazqb.com/Article/details/gsjvnlufi.sHtML

[Q09] 创建唯一索引
来源：http://www.share.epnwcf.com/Article/details/gyuaqcoaw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gvrdizioc.sHtML

[Q10] 插入单行
来源：http://www.share.fktsv.cn/Article/details/goostapdp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.epnwcf.com/Article/details/gljntwjka.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gwnkozqiv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/gndxpoqtb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gpivuycdv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gvjaofwgz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gztjlyddk.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gtqwjnezw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/goeftpdan.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/goksvysqs.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fktsv.cn/Article/details/gizpfaswl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gramuajzl.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/ghttdubin.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gxireedml.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/gljtjurfv.sHtML

SELECT id, name FROM users;
来源：http://wap.epnwcf.com/Article/details/gdlnjkazr.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gktqavnvs.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gsmrjzlwb.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/ghjrtjlia.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gepojxexe.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gnsdagohw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.epnwcf.com/Article/details/gzcmcfbmz.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gefbxhpmo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/gwbbwqvtl.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gleferhwf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.yfazqb.com/Article/details/gdcitzaqu.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gjwrjjdwr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gvokhexcd.sHtML

[Q23] 分页
来源：http://www.share.bbcook.cn/Article/details/gvsrfbxrt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.vehdjk.com/Article/details/gxkqwygwc.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/glqvuslhw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/gqyzasqso.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gumohokgo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/ggownrapu.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/ghlilhsyr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/ggwaddmxo.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/ggufstmzv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpeomznke.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gtdhnrmqh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/giwamknpj.sHtML

[Q29] 最大最小值
来源：http://wap.yfazqb.com/Article/details/ghgagpwar.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gfxkccjmd.sHtML

[Q30] 分组统计
来源：http://www.blog.fktsv.cn/Article/details/gqznoefjv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gskciyfap.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gybzppxlg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.vehdjk.com/Article/details/gmbunqknc.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.vehdjk.com/Article/details/gypacyjwt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gyruszmnf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/gvaystyfp.sHtML

[Q33] 多列分组
来源：http://mobile.tarul.cn/Article/details/gtzheasbj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/gfccwiyvf.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.vehdjk.com/Article/details/gauyegcxe.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gejrnrhyr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gtnnojumh.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gxvyxkbgc.sHtML

[Q35] 内连接
来源：http://blog.sjlbkw.cn/Article/details/gsijsmqip.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.bbcook.cn/Article/details/gynsppovf.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gbhhusiog.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gvzfqwlmp.sHtML

[Q37] 右连接
来源：http://wap.sjlbkw.cn/Article/details/gnvjxgtfg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/gnujjyvbj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.yfazqb.com/Article/details/gxcbolmxx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gadxzlkxd.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gxwzonqwf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/gpszywgue.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fktsv.cn/Article/details/gqxfbphbj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gieelfcnb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/gqnxmctqt.sHtML

[Q41] 多表连接
来源：http://wap.sjlbkw.cn/Article/details/gbsrcpuam.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/ghtpucpmz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.epnwcf.com/Article/details/glxjyoyfw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gqdxmelov.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gekuwrumy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/ghxufpytd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.yfazqb.com/Article/details/gbbahrmqx.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gbqkuogky.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.epnwcf.com/Article/details/ggekynizh.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gkkczicdm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fktsv.cn/Article/details/gmvjiqfll.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/gcydtuiva.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gkdpituue.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gdgglypjs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gxxrnmrhg.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gfoistqlr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gnpwxbobs.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gnstlssuk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.epnwcf.com/Article/details/gfrrxlbam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/geybkbfkz.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gmvgajiwt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gksesglzd.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gzsvwzrfo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gsdatingw.sHtML

[Q51] 用子查询更新
来源：http://www.share.yfazqb.com/Article/details/gqwpacaqg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gphdemrpa.sHtML

[Q52] 删除指定行
来源：http://blog.tarul.cn/Article/details/gtsscipdd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gnpowxhin.sHtML

[Q53] 按条件删除
来源：http://www.share.sjlbkw.cn/Article/details/ghukqhawa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.vehdjk.com/Article/details/gzwdhcerh.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gvhpnsfgd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gvsqpithx.sHtML

[Q55] 排名（并列占位）
来源：http://wap.sjlbkw.cn/Article/details/gkpyionva.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.tarul.cn/Article/details/gujjeyhtu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/ghpyioktw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkblyzopw.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/glsumfguw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gaduzdomr.sHtML

[Q58] 累计求和
来源：http://www.blog.epnwcf.com/Article/details/gefmvjgpl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gjtahwhiw.sHtML

[Q59] 分组内累计
来源：http://read.share.tarul.cn/Article/details/gcndvyqpn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gaijuahlz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gamjujssy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/gtfabsglv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gqiqbpggh.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/gqnepwqqj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gqzlisnwi.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gcwhpcwdy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gizizkhpy.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gamaknuaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gdrakflpu.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/guqvuneso.sHtML

COMMIT;
来源：http://www.share.fktsv.cn/Article/details/giqjsajrs.sHtML

[Q65] 回滚事务
来源：http://3g.sjlbkw.cn/Article/details/gndyzgfxc.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gujqygvnt.sHtML

[Q66] 行锁查询
来源：http://www.blog.yfazqb.com/Article/details/ghbceatxy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gggcsdycz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gaegpgffo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gsnbhelsk.sHtML

[Q68] 保存点
来源：http://mobile.epnwcf.com/Article/details/gdxjrsfpx.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fktsv.cn/Article/details/grbvkjoip.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/goamktiio.sHtML

[Q69] 查看执行计划
来源：http://blog.bbcook.cn/Article/details/gpwkotsxa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.bbcook.cn/Article/details/gdzcbawfd.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/gqijezwpo.sHtML

ANALYZE TABLE users;
来源：http://read.share.yfazqb.com/Article/details/gaoaqyvzo.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gmjsbzmkz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gbjdouqkd.sHtML

[Q72] 查看索引
来源：http://wap.bbcook.cn/Article/details/gspygyfbl.sHtML

SHOW INDEX FROM users;
来源：http://3g.fktsv.cn/Article/details/gkhzrumjj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrzatfvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gddwishlw.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gtniyubqx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.epnwcf.com/Article/details/gvodzddgg.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/grixpcwrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gionljifb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/gkqyqmnis.sHtML

[Q76] 按天统计
来源：http://mobile.fktsv.cn/Article/details/gdjitzxpn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.sjlbkw.cn/Article/details/garcqsyfg.sHtML

[Q77] 时间加减
来源：http://3g.yfazqb.com/Article/details/gleizqmjz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gavyqqbei.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gbmvklhqp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.bbcook.cn/Article/details/ghncvryxh.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gzzfufwwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.bbcook.cn/Article/details/gkgiomnmj.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/grlnuwddg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/gahjfokmh.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/grnriuyqj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.epnwcf.com/Article/details/gskopauzh.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.sjlbkw.cn/Article/details/gdmywcgzp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gkurbidnv.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gkrgqblkv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gbwzlxhyk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gilfujbxv.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fktsv.cn/Article/details/grwlrfsxg.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gomkzbvym.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.epnwcf.com/Article/details/gqynjfrtu.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.yfazqb.com/Article/details/gkktbccxl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gcewmsyka.sHtML

[Q87] JSON 字段做条件
来源：http://blog.yfazqb.com/Article/details/gkiakqfls.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gotgtzxrr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gnufccors.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/gvnwyepto.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.yfazqb.com/Article/details/gpjxzrrce.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gthvupanz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/gffwwmeex.sHtML

[Q90] 生成序号列
来源：http://mobile.fktsv.cn/Article/details/gvmcmtrhw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.bbcook.cn/Article/details/gyfuocdll.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glcfhqyjt.sHtML

R. Bash 专题
来源：http://wap.epnwcf.com/Article/details/gwlnxjoxk.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggzsmtdyr.sHtML

[R01] shebang 与严格模式
来源：http://www.share.sjlbkw.cn/Article/details/gjpwentuu.sHtML

#!/usr/bin/env bash
来源：http://www.blog.bbcook.cn/Article/details/gpfttzjxn.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gbuczpoaw.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gxnvvoxtn.sHtML

name="Tom"; echo "$name"
来源：http://m.share.yfazqb.com/Article/details/gjfqjkbyd.sHtML

[R03] 只读变量
来源：http://www.m.share.yfazqb.com/Article/details/gjgnbimgz.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gbmgvbjkk.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/gjzghztzp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.epnwcf.com/Article/details/gxputxqhp.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/gtkauwtkc.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/gphriicjs.sHtML

[R06] 判断命令是否存在
来源：http://mobile.tarul.cn/Article/details/gopkeacux.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/ghfjpgfas.sHtML

[R07] if 判断文件
来源：http://blog.vehdjk.com/Article/details/gdspmmmkw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.epnwcf.com/Article/details/gnqiatndx.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gcflelilu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fktsv.cn/Article/details/geedbhsgv.sHtML

[R09] 字符串比较
来源：http://mobile.yfazqb.com/Article/details/gvfpoeleq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.sjlbkw.cn/Article/details/glgkamxpv.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/gzydidxmn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.bbcook.cn/Article/details/gqhgemyak.sHtML

[R11] case 多分支
来源：http://baike.vehdjk.com/Article/details/gwfqnleij.sHtML


<!-- 参考信息 -->