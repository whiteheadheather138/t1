代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gccuzufhj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/ghriyyqmu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.tarul.cn/Article/details/gihjicvqn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gitlhmicu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/gmpowqrku.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/ggmxkminn.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gepflyvxr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gyqthggfs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.bbcook.cn/Article/details/gviddxqtl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gcwerfmdf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gcwupctdc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.tarul.cn/Article/details/gngwcmhvk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.tarul.cn/Article/details/gkobvawew.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gksbautwu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gmniwhbjm.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/ghyadfzaa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.sjlbkw.cn/Article/details/gldtsqpma.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gfgdszewx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gkigxxpjw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gncijzejl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gffmswlij.sHtML

Go:   len(arr);  len(m)
来源：http://3g.vehdjk.com/Article/details/gnxmxhvvn.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gdejvtwnw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gzkqwkzhf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.sjlbkw.cn/Article/details/gzoekkcmy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/gptjvphcc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.tarul.cn/Article/details/gndlznmrr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/guovqpsco.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gpnhrnpjz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gwbxvwcpo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.vehdjk.com/Article/details/gzpmtebhv.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gkdssbmsf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.tarul.cn/Article/details/gwuharool.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gepybsrqt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gkzgyrjro.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/ghnzzvjbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/ghdflnnbg.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/glgeeeeny.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gafynyzci.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gezjmtmuf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/gwpazejtt.sHtML

C#:   if (x is null) {}
来源：http://www.share.tarul.cn/Article/details/gisjkgoun.sHtML

[P07] 防抖与节流
来源：http://read.share.yfazqb.com/Article/details/gohybajls.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gvkeqkzem.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fktsv.cn/Article/details/gvychhakh.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gvxxfossi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gwwsodqkk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gwuzjbvfg.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/glfcmmstp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gbibcyqgo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gonwlaspl.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fktsv.cn/Article/details/goyyrhdbd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.yfazqb.com/Article/details/gibaibwyh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.epnwcf.com/Article/details/gbmzbocbh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/ggscvlfzj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gpsgdlrjj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/gvtpfcxxp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/gsnaqrdbf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gipozcdpc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gohmsszhj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjbwsqqhg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fktsv.cn/Article/details/gjgavyquh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gmvtykrde.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/ggsajpxik.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gbeyhhfyt.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gebqpvmmm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gwpfdkbyq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gmmzflnkf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhwjkyly.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gktwyplro.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/gkqhrlnam.sHtML

CREATE TABLE orders (
来源：http://mobile.vehdjk.com/Article/details/gwjpjjhrx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.tarul.cn/Article/details/gujlyessy.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gaizcwfkm.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.tarul.cn/Article/details/gqebbfoxc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gepzwlkpj.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gclumgrta.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/gufciaaad.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gcbokfyfq.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/glwgfgivo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/gmtzjetuh.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gesrdpczl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/ghfsvuyjs.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gchmtxtix.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/gsbvkbmha.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gsotrdcch.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/ggzzkzyxk.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/guliqqhdp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gdyhzaxvz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/giaxmrykl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gsyipqujv.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/gamjuvhoo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gdiehbzxr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/ghbiyvrhl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gbhfdovci.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gnefbwqpk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.epnwcf.com/Article/details/gfnaflgij.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gcmnqkfuz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.sjlbkw.cn/Article/details/glklxsfpx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/grrlwvhoh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.sjlbkw.cn/Article/details/gnrpjzmwj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fktsv.cn/Article/details/gxvvfdlcs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.epnwcf.com/Article/details/gccahwmac.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gpymgxgxw.sHtML

SELECT * FROM users;
来源：http://www.share.yfazqb.com/Article/details/gciafvhhx.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/ggrdjhrop.sHtML

SELECT id, name FROM users;
来源：http://3g.yfazqb.com/Article/details/gdnexhatq.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gcrmlscnz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gbsfhocil.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gtifbbjhz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.vehdjk.com/Article/details/gqvydzkkt.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/guzsooose.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gdvopjmhg.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gcxfavebc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.vehdjk.com/Article/details/ggvompral.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/gwmixxzrm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.tarul.cn/Article/details/gqgnojfds.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gpmkydysu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gknfueuux.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gpwcgpgdq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhyvevtk.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/gtcgsfoqn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/guecsebco.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/ghxhouzdn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gehvqsyfp.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gdycqbbqq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/gqmqoajhq.sHtML

[Q27] 条件计数
来源：http://www.blog.vehdjk.com/Article/details/gcptslsjv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.yfazqb.com/Article/details/gibfrjzxn.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/geixgjijq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gedqqpsen.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gzdqqcmhk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gfykqgvzr.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/gflufqcae.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gsscamett.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gcmnhlfwx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/gwfvdzdyi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.vehdjk.com/Article/details/ghadnjcma.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gvfwnujfh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/gqvqeueae.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gwkfxhzpa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gdsxsxncp.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/guzfizmmg.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gdmzbvned.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.vehdjk.com/Article/details/glshftdve.sHtML

) t WHERE rn = 1;
来源：http://3g.vehdjk.com/Article/details/gwpdplupk.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gtwjpzivd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/grmcyxkyj.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/grufoazda.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/giquollnz.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gicempzvo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gvmyhtajm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/guetzuyjk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gcgsyxpbu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/gjxwrqgdw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.sjlbkw.cn/Article/details/gagokgdqo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/ggkpjfbmp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gbsajcqyt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.vehdjk.com/Article/details/gkludgsfk.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gazixjcaf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.yfazqb.com/Article/details/grdpacirk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gnwjwfcgy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gmjhukxfq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gydtgjhid.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fktsv.cn/Article/details/gqxplakkh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gspknukas.sHtML

[Q43] 标量子查询
来源：http://www.m.share.tarul.cn/Article/details/gnzthjfdi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gntijkfyb.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/gefkdpsxw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gorfaigiz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gohhafpcj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gvlnbhvpw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gvwarxwqg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gwxzrsemz.sHtML

[Q47] 与平均值比较
来源：http://www.share.yfazqb.com/Article/details/ggqqmkfdx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gtilpnxrw.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.bbcook.cn/Article/details/gzrqvmrip.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.epnwcf.com/Article/details/gzpjqaqmv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gvydamgki.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/ggkyhwisp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gutwrjghh.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/glwlcgrvg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/grclfbpyq.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gyvgkdbdy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/gziktcfpg.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/giwlmsmyg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gsrrmlpmu.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/gyepbgrnq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gnmusxjhl.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/guxwptsar.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/ghlogyyqj.sHtML

[Q55] 排名（并列占位）
来源：http://3g.epnwcf.com/Article/details/gqfthejpl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gkwugqllr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gwafbeflf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.bbcook.cn/Article/details/gauydskvj.sHtML

[Q57] 行号
来源：http://baike.yfazqb.com/Article/details/gywivaufy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfflhopzk.sHtML

[Q58] 累计求和
来源：http://3g.tarul.cn/Article/details/gpzpwolyc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gmxesjxpf.sHtML

[Q59] 分组内累计
来源：http://www.share.epnwcf.com/Article/details/gsqqlwcll.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/glmkwzfjo.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.vehdjk.com/Article/details/ggcfmupma.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gueynpbau.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gvoaodbvh.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gsdiahsgs.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gpznjxyjy.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/guugpwsoh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/ggvczshvq.sHtML

[Q63] 开启事务
来源：http://www.share.vehdjk.com/Article/details/gxouojofa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fktsv.cn/Article/details/ggagftcqu.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gkkiamdae.sHtML

COMMIT;
来源：http://www.share.bbcook.cn/Article/details/gqavhxlid.sHtML

[Q65] 回滚事务
来源：http://www.share.bbcook.cn/Article/details/gzbhdxxya.sHtML

ROLLBACK;
来源：http://baike.bbcook.cn/Article/details/gmvvllwds.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/gyafagbih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.vehdjk.com/Article/details/gktmwzbci.sHtML

[Q67] 设置隔离级别
来源：http://read.share.bbcook.cn/Article/details/ghyeozmtt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.tarul.cn/Article/details/gkzieksug.sHtML

[Q68] 保存点
来源：http://read.share.fktsv.cn/Article/details/grzqyhrdh.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gyurgsbku.sHtML

ROLLBACK TO sp1;
来源：http://blog.fktsv.cn/Article/details/gfghyxvns.sHtML

[Q69] 查看执行计划
来源：http://baike.vehdjk.com/Article/details/gnvalzolh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/gplkrzsuk.sHtML

[Q70] 更新统计信息
来源：http://www.share.sjlbkw.cn/Article/details/gqtbercgt.sHtML

ANALYZE TABLE users;
来源：http://read.share.sjlbkw.cn/Article/details/gsbzsgyvv.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gorimgzzy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/ghowgbwbe.sHtML

[Q72] 查看索引
来源：http://3g.tarul.cn/Article/details/gjhunhorb.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gtgqhmxad.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gqtildoyh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gxovasvxx.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gpzcmntys.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.tarul.cn/Article/details/gstltvtuh.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gcpyuwpon.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gvmahaybi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.sjlbkw.cn/Article/details/gjqnzgltk.sHtML

[Q76] 按天统计
来源：http://wap.bbcook.cn/Article/details/gavimquwf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gilwryvsw.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/ghkcyhexf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.tarul.cn/Article/details/glmibtqww.sHtML

[Q78] 当前时间
来源：http://m.share.yfazqb.com/Article/details/gzplxmpkt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fktsv.cn/Article/details/gnlgjcfmt.sHtML

[Q79] 字符串拼接
来源：http://baike.yfazqb.com/Article/details/glpmzvxpm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.tarul.cn/Article/details/gmorvomod.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gyajywtht.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gsmdgcezf.sHtML

[Q81] 字符串替换
来源：http://www.m.share.tarul.cn/Article/details/gmduilzil.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/glajtsolr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gcicmbvxs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gwzmxfjoc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gwufigxsg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.tarul.cn/Article/details/gxjfjquel.sHtML

[Q84] 去除首尾空格
来源：http://www.share.sjlbkw.cn/Article/details/gvkpxraea.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gysdmjyjf.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gcffwdcnp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.tarul.cn/Article/details/gbojrnbpu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/grobznoij.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.bbcook.cn/Article/details/gqjkennko.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gwihhqoqw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.bbcook.cn/Article/details/gfrtsultf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.tarul.cn/Article/details/ghlpotrvp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gjytuzuak.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gxyhabiea.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gnohamrtr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/gqxfykqaj.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/goliduqzv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.yfazqb.com/Article/details/gezdyinui.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gzfjpvtua.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/grietfbvp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/glkuwugoe.sHtML

[R01] shebang 与严格模式
来源：http://www.share.vehdjk.com/Article/details/gumqsxpas.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gowjuyqma.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gsyfshysw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fktsv.cn/Article/details/gxxuswsyv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/gtxqkyyew.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gczzlyest.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/gcjcdkaxa.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gukryfssd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.epnwcf.com/Article/details/gyxjihrnp.sHtML

[R05] 参数默认值
来源：http://www.blog.yfazqb.com/Article/details/gwvlvvogz.sHtML

name="${1:-default}"
来源：http://mobile.epnwcf.com/Article/details/ggovzzelg.sHtML

[R06] 判断命令是否存在
来源：http://3g.sjlbkw.cn/Article/details/gbqscavlb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.bbcook.cn/Article/details/ghjbyfvhg.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/gwxjblyyy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.epnwcf.com/Article/details/ggcppmequ.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gvbpoyeod.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gzbisvxhi.sHtML

[R09] 字符串比较
来源：http://www.blog.yfazqb.com/Article/details/gbptytpga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.epnwcf.com/Article/details/gkqjyofzt.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/ggegsytah.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fktsv.cn/Article/details/gsygveeod.sHtML

[R11] case 多分支
来源：http://www.m.share.tarul.cn/Article/details/ggmvxhpmw.sHtML

case "$1" in
来源：http://3g.epnwcf.com/Article/details/gnjagtfft.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gctxcfxxa.sHtML

stop)  echo "停止" ;;
来源：http://baike.epnwcf.com/Article/details/gqfrlogtd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.yfazqb.com/Article/details/gwwqljmyr.sHtML

esac
来源：http://baike.yfazqb.com/Article/details/gplsycfzi.sHtML

[R12] for 遍历文件
来源：http://3g.fktsv.cn/Article/details/gfgmznbru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fktsv.cn/Article/details/gswcgkwvl.sHtML

[R13] for 计数循环
来源：http://wap.epnwcf.com/Article/details/gulzlmymc.sHtML


<!-- 参考信息 -->