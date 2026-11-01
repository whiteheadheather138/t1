代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gqnmfyptb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gyjmfowwe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.vehdjk.com/Article/details/glssjfsrc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gttyxdnzv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gwzkjihks.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gzhavipyd.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gvtifobio.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.tarul.cn/Article/details/gtgudmkyo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.yfazqb.com/Article/details/gkysmldjc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gdymyplgo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/gsfpvqtqb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/ggudwluyj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gwpkwhcyd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.tarul.cn/Article/details/gzbzdxlck.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.sjlbkw.cn/Article/details/gzxevvuuc.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gdnbnsnor.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/grktbowjr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gkwznqxrq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.bbcook.cn/Article/details/ghnzyhaip.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gqklqmigz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gapbickit.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.vehdjk.com/Article/details/ggplszpvs.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gzpziyfxi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkdzusvn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gmbduakmg.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/glwmkrjkn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/gkypwproy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.sjlbkw.cn/Article/details/gauizgjix.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.sjlbkw.cn/Article/details/gmdwbccds.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.sjlbkw.cn/Article/details/ghfxjnabt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gmgytmoek.sHtML

Ruby: a == b
来源：http://3g.yfazqb.com/Article/details/glphapxxi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.epnwcf.com/Article/details/gpegfsoxw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.epnwcf.com/Article/details/gfxdfbsin.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fktsv.cn/Article/details/guhoiwxpr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.yfazqb.com/Article/details/goscqsmdf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gizosunnh.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gamnftxgv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/guxhfqwgu.sHtML

Go:   if x == nil {}
来源：http://wap.sjlbkw.cn/Article/details/gtshzptfd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/giyejcgtn.sHtML

C#:   if (x is null) {}
来源：http://blog.sjlbkw.cn/Article/details/gsjnousvn.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/grxmcukdj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gzwsrryxy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fktsv.cn/Article/details/gkuhjompf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gkhnmnidk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gvnooqhft.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gxlnpchym.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fktsv.cn/Article/details/gyalebvwy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gayotuvvn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/grjmvyixw.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gqongmcpm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.yfazqb.com/Article/details/grfdgkuov.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gafihxwkz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/grfxnmele.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gsiawvlvw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gynscynbb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fktsv.cn/Article/details/gzqkmixvu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.fktsv.cn/Article/details/gggjeclou.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gslhyvsww.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gxiwcsnzi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.tarul.cn/Article/details/gtzgjhqel.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gancbqxhb.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gkciousky.sHtML

CREATE TABLE users (
来源：http://wap.tarul.cn/Article/details/gsgiwabif.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/ghomyshsj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gxagasevx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gogvjgqxn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gzkcgrqwg.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gydxxatez.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gjcvhccth.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gvfsyyrak.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/geoexqyvk.sHtML

user_id INT NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gryddnhpc.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gwiczqigp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.vehdjk.com/Article/details/gslmevqur.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gddbdvdby.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/glungxhoj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.tarul.cn/Article/details/gllqnjpnr.sHtML

[Q04] 修改列类型
来源：http://wap.tarul.cn/Article/details/ggasjazuf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gekukpqmo.sHtML

[Q05] 重命名列
来源：http://blog.vehdjk.com/Article/details/gdtvescvo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gaqdhwwuo.sHtML

[Q06] 删除列
来源：http://www.m.share.epnwcf.com/Article/details/glnqpsgah.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/grdjuyoan.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gnufehjpk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fktsv.cn/Article/details/gqsbqsscp.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.yfazqb.com/Article/details/gcezjbdlq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gbrsvpwan.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/guokfgkhz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/guclboceu.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gcunksurv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/glokkntls.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/ggxqmjnug.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gcqrodpjy.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gwfmqbkfj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fktsv.cn/Article/details/gppnyomfr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.sjlbkw.cn/Article/details/gnvxbliei.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/gpxnzkjby.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.yfazqb.com/Article/details/gxtgjhfnc.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gpgixvfbw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/ggogceyxo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fktsv.cn/Article/details/gfeekjidj.sHtML

[Q15] 查询全部
来源：http://blog.tarul.cn/Article/details/ginsdgnin.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gftykcxso.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gezsjtdmp.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gogtwacfn.sHtML

[Q17] 条件查询
来源：http://mobile.sjlbkw.cn/Article/details/gofcyuxgo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.sjlbkw.cn/Article/details/gpgiutmns.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gvqqozwaj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gasbzircj.sHtML

[Q19] 范围查询
来源：http://mobile.epnwcf.com/Article/details/gyoxayiaa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/gzclomaaf.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/glilwnoov.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gifccgbid.sHtML

[Q21] 空值判断
来源：http://www.m.share.bbcook.cn/Article/details/gmofbreec.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gdvxphywv.sHtML

[Q22] 排序
来源：http://www.share.sjlbkw.cn/Article/details/guszqchyg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gaevruqdg.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gdvlvidbq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/gltuzisry.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gyclxrszu.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gwgfwizgz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gkkffnypn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.bbcook.cn/Article/details/giemhmldw.sHtML

[Q26] 计数
来源：http://baike.tarul.cn/Article/details/gojvlvdia.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gzqocynxw.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/ghesvusmb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/goflewrzt.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/gzhcfwrbt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gtffiwdbq.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gafqehjmz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gpvlvajiu.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gedvztthc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/guxlqxgsm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkrzbpiy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/gsjoikbiv.sHtML

[Q32] 分组拼接字符串
来源：http://blog.bbcook.cn/Article/details/gorgsjztk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gjrdwqiwm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gfxmetozg.sHtML

[Q33] 多列分组
来源：http://m.share.bbcook.cn/Article/details/gohtnvmfq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.sjlbkw.cn/Article/details/gspwssxdn.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gnrgszwci.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gsmcjxmxf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.tarul.cn/Article/details/gjjidajvy.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/gmowfqbfz.sHtML

[Q35] 内连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkcpegck.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gsqyocmkh.sHtML

[Q36] 左连接
来源：http://baike.epnwcf.com/Article/details/gwzonclvb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gmragbgjw.sHtML

[Q37] 右连接
来源：http://blog.vehdjk.com/Article/details/gwljuthiq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gvpjskspr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.sjlbkw.cn/Article/details/ggwivpdtn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.vehdjk.com/Article/details/gazymuvty.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/gvabgqfss.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/gaodncjry.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/glluaqlow.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/giwnsfbrh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/gjslotimh.sHtML

[Q41] 多表连接
来源：http://blog.bbcook.cn/Article/details/gvmlxkiio.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.yfazqb.com/Article/details/gwxlbpsex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/ggludntuq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gutdqwsxt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/glisajaic.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.bbcook.cn/Article/details/gjkdcciel.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/geyvxmndk.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/ggrpwybzx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.yfazqb.com/Article/details/gyroxxiwt.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/ghjbzdcsj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.sjlbkw.cn/Article/details/glaimzmqe.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gwviomwhq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gophziqsw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gukficalg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gehcabgcg.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/gfxrlwgfm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/gkhiqtouj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gltosaftc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.vehdjk.com/Article/details/gxjnwckdd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.epnwcf.com/Article/details/gbfjpfnrk.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gqtcyfuix.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/guryrafat.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gxpxyuezl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gldcistpr.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gkbmcqhrx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fktsv.cn/Article/details/gzlghtuas.sHtML

[Q52] 删除指定行
来源：http://www.m.share.bbcook.cn/Article/details/gncdlcpws.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gybvexpsr.sHtML

[Q53] 按条件删除
来源：http://mobile.yfazqb.com/Article/details/gdkqmtrls.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gqvxnoyiy.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/gxgyqrfxo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/gztalmwer.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gkkasyzcr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.yfazqb.com/Article/details/ggwfpfpzw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gcvsdepcd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gjehjfywy.sHtML

[Q57] 行号
来源：http://mobile.vehdjk.com/Article/details/gnahpkdap.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.yfazqb.com/Article/details/gzaflsexi.sHtML

[Q58] 累计求和
来源：http://www.m.share.yfazqb.com/Article/details/gavbrgcfi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.bbcook.cn/Article/details/gbwmfojds.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/gsscvymxn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gngxnzfte.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.vehdjk.com/Article/details/gylhhtpgq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.yfazqb.com/Article/details/girvpbnlf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/ghgrixxpk.sHtML

[Q61] 移动平均
来源：http://www.m.share.bbcook.cn/Article/details/gqujeybvb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gyddyhixb.sHtML

[Q62] 分组占比
来源：http://3g.epnwcf.com/Article/details/gflczintt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gexqfavof.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/gmydnbkod.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.bbcook.cn/Article/details/gekqpcgrq.sHtML

[Q64] 提交事务
来源：http://www.blog.bbcook.cn/Article/details/gvmgvzafs.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gtxprebci.sHtML

[Q65] 回滚事务
来源：http://www.m.share.vehdjk.com/Article/details/ggavhefst.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gyzakamfs.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/glhqybfxt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/gbxtrezej.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/guflivsuw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fktsv.cn/Article/details/guxbizxuh.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/gmfjwvkbc.sHtML

SAVEPOINT sp1;
来源：http://mobile.epnwcf.com/Article/details/gmyxcokkr.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gcdsbysfe.sHtML

[Q69] 查看执行计划
来源：http://baike.bbcook.cn/Article/details/gllgrwlsq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gjsdwljyi.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gvzfzjylq.sHtML

ANALYZE TABLE users;
来源：http://baike.bbcook.cn/Article/details/gqpvyeimi.sHtML

[Q71] 查看建表语句
来源：http://www.blog.sjlbkw.cn/Article/details/gsxjkiine.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/gkjfkjghs.sHtML

[Q72] 查看索引
来源：http://wap.sjlbkw.cn/Article/details/gigkxxwsp.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gtjgjofxb.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gsdpnyock.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.bbcook.cn/Article/details/gtrlseekh.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/gvrkloslg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.vehdjk.com/Article/details/gmkywbjkk.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gppnixslg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/gspdpdsbc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gokvuwijk.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gdtkxwvrc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fktsv.cn/Article/details/gpjucesfm.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/gqsifmdoa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.yfazqb.com/Article/details/glwwhqzyk.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gjhirilyv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.bbcook.cn/Article/details/gwahjvvbo.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/gsxagrebc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.bbcook.cn/Article/details/gtmumnkur.sHtML

[Q80] 字符串截取
来源：http://3g.epnwcf.com/Article/details/girkmzeml.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gouwhhnym.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gbyrbgefy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/glmkrpely.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gcdsqvczb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/guloqyeme.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gioknvfsv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gkaiqjeul.sHtML

[Q84] 去除首尾空格
来源：http://www.share.yfazqb.com/Article/details/gtsytxdnr.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gghsnlqok.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gskmhkbfw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.vehdjk.com/Article/details/gkpzpqpro.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.epnwcf.com/Article/details/godhiqyhk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fktsv.cn/Article/details/gssvsrwjv.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.sjlbkw.cn/Article/details/gdthnorav.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gctufrgaa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gbikxidbb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.tarul.cn/Article/details/gelujoviv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.sjlbkw.cn/Article/details/glmcnwvdl.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/glldmopkb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.vehdjk.com/Article/details/gtmvzzbtr.sHtML

[Q90] 生成序号列
来源：http://3g.fktsv.cn/Article/details/ggstdcbbh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/gjbuoixuq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcovrokpq.sHtML

R. Bash 专题
来源：http://blog.fktsv.cn/Article/details/ghegiiqic.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gergjrfci.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/gclyqsuzv.sHtML

#!/usr/bin/env bash
来源：http://m.share.yfazqb.com/Article/details/gnmxoslqh.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gxedwkabc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.epnwcf.com/Article/details/gkavdtojr.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gtbssvhgk.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/gyanvhaeq.sHtML

readonly PI=3.14
来源：http://read.share.fktsv.cn/Article/details/gjrtnobtt.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gxcscezmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.epnwcf.com/Article/details/grkrggglm.sHtML

[R05] 参数默认值
来源：http://baike.bbcook.cn/Article/details/gwrnmovhg.sHtML

name="${1:-default}"
来源：http://3g.yfazqb.com/Article/details/gprlshaoj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fktsv.cn/Article/details/gxuaevobc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.vehdjk.com/Article/details/gnktqiech.sHtML

[R07] if 判断文件
来源：http://m.share.vehdjk.com/Article/details/gguuibxkb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.bbcook.cn/Article/details/gjbjlibuv.sHtML

[R08] 数值比较
来源：http://blog.sjlbkw.cn/Article/details/gexsjhfcy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.tarul.cn/Article/details/gpswujvlc.sHtML

[R09] 字符串比较
来源：http://mobile.bbcook.cn/Article/details/gvmveiuga.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.bbcook.cn/Article/details/ghpcegfsb.sHtML

[R10] 正则匹配
来源：http://blog.yfazqb.com/Article/details/gwzqafnck.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.vehdjk.com/Article/details/gqgxiamru.sHtML

[R11] case 多分支
来源：http://3g.sjlbkw.cn/Article/details/ggntofuwg.sHtML

case "$1" in
来源：http://blog.vehdjk.com/Article/details/gvmieexqh.sHtML

start) echo "启动" ;;
来源：http://www.m.share.vehdjk.com/Article/details/gadswblvy.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.yfazqb.com/Article/details/gytrwsgmm.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fktsv.cn/Article/details/gobzblozi.sHtML

esac
来源：http://www.blog.epnwcf.com/Article/details/gapyjqoyj.sHtML

[R12] for 遍历文件
来源：http://read.share.fktsv.cn/Article/details/gxycajrje.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.epnwcf.com/Article/details/gnzioxvts.sHtML

[R13] for 计数循环
来源：http://wap.sjlbkw.cn/Article/details/grflpfgdr.sHtML


<!-- 参考信息 -->