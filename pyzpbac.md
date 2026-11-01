代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gziuqkymh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gmnnrkkig.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gbhwblhbq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/gcjtalcbv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/ghgsyhhio.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/golyljtyp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/gjosyhkaz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gxhabexrl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fktsv.cn/Article/details/gpyyyuzmv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/gfmstdohc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/gsbfmupmx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/gmjypvaey.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.tarul.cn/Article/details/gpkhnnpaw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/grcnxbgwq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gtfedeods.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gytxehzfh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/goidfrawr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/gwxyrudux.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/gzbwkozcs.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gardphqmz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gleomuesb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gyjbkabaq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/geydciixj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gdjxnaqdx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gyliryhpj.sHtML

Go:   len(arr);  len(m)
来源：http://wap.tarul.cn/Article/details/gmhdpmtst.sHtML

Ruby: x.length;  x.size
来源：http://read.share.vehdjk.com/Article/details/gqcwdknnf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.yfazqb.com/Article/details/gqfivofrv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gmeypibmh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.tarul.cn/Article/details/gvottadqb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gubxhpbcu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gadmvhuly.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gwtlvdvmg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gelmytwru.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gsmjfrrpz.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/gpevnjvil.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gnlffxnqk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gcgeqpsjp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gzbcdjffk.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gowxrcvea.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.vehdjk.com/Article/details/gytozywem.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gyfxwhdbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.bbcook.cn/Article/details/gnchkelkg.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gmiscwhya.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/gtkkxsizb.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/gojpgsmmq.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gleijmfgu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gwwhcogrl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gfzlloqxo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/ggqsgbxgr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gcswyhqin.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.sjlbkw.cn/Article/details/gierfgsje.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.tarul.cn/Article/details/ghnuylrkh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/gvzdzkpzf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gbujonlix.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gxanampnp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.epnwcf.com/Article/details/gmlvlqzfq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.bbcook.cn/Article/details/ginhyvydd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gyemrnywz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gqwzecdyq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.tarul.cn/Article/details/gzkjvgreo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gwbnkebee.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gletabrtg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gkwsgpuap.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/glhzngola.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gnekxygur.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grlrzyeha.sHtML

[Q01] 创建表
来源：http://baike.epnwcf.com/Article/details/glcaxiaug.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gsqmkhlbg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gfwjmeqeg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gepnsnqso.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/gcemxteix.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/gyajbvqxv.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/gzchvboqj.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/gbtpyzasy.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gyfrhzvsq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gkhapcipe.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gitxhelva.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.vehdjk.com/Article/details/gkdomcygo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gddxjttwn.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gwudmpvbo.sHtML

[Q03] 增加列
来源：http://m.share.epnwcf.com/Article/details/gbsnvkoyk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fktsv.cn/Article/details/gfiddwmvt.sHtML

[Q04] 修改列类型
来源：http://wap.bbcook.cn/Article/details/gqsztcsax.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.yfazqb.com/Article/details/gdxwzcimm.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/ghlawipkw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/gewfisoyd.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gpxbsdfys.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwawfxla.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gopiidpbv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gplyhshcz.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gmqlgdhvn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gkjbxnrum.sHtML

[Q09] 创建唯一索引
来源：http://3g.vehdjk.com/Article/details/gjdcttwzp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gelorfwvf.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gmegdrgal.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gwvukxfxc.sHtML

[Q11] 一次插入多行
来源：http://baike.fktsv.cn/Article/details/gfshohrwi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/gvmbiuuhf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.yfazqb.com/Article/details/gsyqcybrf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.sjlbkw.cn/Article/details/gwfchlcnb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.tarul.cn/Article/details/gvplznher.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/glepekure.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gprzbyrbm.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/gywuxkvnx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbaoklcd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.tarul.cn/Article/details/gswgwnaiy.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/gskfovgpg.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/gvjfqgnff.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/gbugmadab.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/gtnxlvygw.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/gjcggtgdh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/ggztqjicj.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gvmxbmyoy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.yfazqb.com/Article/details/gtwlnoohu.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/grtsehlvk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gwhzdstns.sHtML

[Q20] IN 列表
来源：http://blog.epnwcf.com/Article/details/grvjzyawg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/givmuxsae.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/grnwwosaw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/guasiftau.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gmxsmiffp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gwuvsgseg.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/gpyxrellr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.tarul.cn/Article/details/gktwayfoi.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/gxpdtbsmq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/glyblyats.sHtML

[Q25] 只取前 N 条
来源：http://3g.vehdjk.com/Article/details/gfgrsfypp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gttldjblv.sHtML

[Q26] 计数
来源：http://baike.epnwcf.com/Article/details/grodauqne.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gzdluuyii.sHtML

[Q27] 条件计数
来源：http://blog.yfazqb.com/Article/details/gypeknyjv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gsdugoqwm.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/giiqqsjgi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gzvqnavmz.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gzcuotggu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gyiutfirl.sHtML

[Q30] 分组统计
来源：http://m.share.tarul.cn/Article/details/gqgsvvsqs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/gtmtyixyb.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/guopvrsjy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fktsv.cn/Article/details/gejsxpbcm.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.yfazqb.com/Article/details/gaszrupyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/ggwefgrby.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.bbcook.cn/Article/details/gxihajcmr.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/gnvjtxctm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.tarul.cn/Article/details/gtbxbrnwr.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/guruyvavb.sHtML

SELECT * FROM (
来源：http://blog.bbcook.cn/Article/details/gtqloekxb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.epnwcf.com/Article/details/gpbzlrqtl.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/galfctrrv.sHtML

[Q35] 内连接
来源：http://m.share.tarul.cn/Article/details/gwsckxphf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/ganvogbxn.sHtML

[Q36] 左连接
来源：http://read.share.bbcook.cn/Article/details/gddeoysfh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/gyrsihqae.sHtML

[Q37] 右连接
来源：http://3g.vehdjk.com/Article/details/gfyeidboy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/gyddnfcxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gxvnoewec.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.tarul.cn/Article/details/gdgyredok.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gzzlnugfy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/gribyfxhx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.yfazqb.com/Article/details/giyaujclk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/grfxhzhop.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gqsxnwmug.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/ggibfqfbq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.sjlbkw.cn/Article/details/gmnbfbzid.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gapxhvzzl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gfjmzujvv.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gzbevfrnd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.bbcook.cn/Article/details/ghaprvrkx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fktsv.cn/Article/details/gsomqilpv.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gakksqdch.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gqbxsoula.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/gyduvvyqv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.tarul.cn/Article/details/gokdzytwf.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gliqpbwux.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gubudlwsw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/ghmajzdnx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gtbyowwxo.sHtML

[Q47] 与平均值比较
来源：http://wap.vehdjk.com/Article/details/gwzjqipvf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gnpgwdasi.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gxrzwwnsu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gnjfqbaia.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gjqevavon.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/gdeqqnetv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/guamknmyi.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gkovqlggt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fktsv.cn/Article/details/gtjlgllpv.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/goikyvcoj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/ghxcxeway.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gpuvuiybe.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gycqjejnm.sHtML

[Q53] 按条件删除
来源：http://www.share.tarul.cn/Article/details/gltwtbbwj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.bbcook.cn/Article/details/godtwzsgs.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gpoejlcns.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/gatpcoidf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gsoatnrkv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.tarul.cn/Article/details/gofzvujll.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcjtclems.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fktsv.cn/Article/details/guaqoxuyk.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gcbnxupul.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gsgmlifol.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/gawjnhqtn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gzfrhmrut.sHtML

[Q59] 分组内累计
来源：http://m.share.fktsv.cn/Article/details/gdzatluxn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/glmnimqth.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.sjlbkw.cn/Article/details/gorwyxogt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/gpzvevtxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gyghhqaif.sHtML

[Q61] 移动平均
来源：http://3g.sjlbkw.cn/Article/details/gsbirdyvu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gyefvgsje.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gteolyquw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gjgxnbgwl.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gbmlathfw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gbumddeyg.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/gynljutxk.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/gjaoexmlw.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/gkhxcbfkz.sHtML

ROLLBACK;
来源：http://m.share.yfazqb.com/Article/details/gqnuynvud.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/ghhfwbwxi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gvysbrpei.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fktsv.cn/Article/details/gyewtohfr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.vehdjk.com/Article/details/gzgbgxpnf.sHtML

[Q68] 保存点
来源：http://www.share.yfazqb.com/Article/details/gpbubilwd.sHtML

SAVEPOINT sp1;
来源：http://wap.sjlbkw.cn/Article/details/gtzbriaey.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/gvdopknsm.sHtML

[Q69] 查看执行计划
来源：http://baike.vehdjk.com/Article/details/gpfiuvlpq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.epnwcf.com/Article/details/gculmypkh.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/gwbodiaqw.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/glwldmuls.sHtML

[Q71] 查看建表语句
来源：http://read.share.bbcook.cn/Article/details/gplnwnhco.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fktsv.cn/Article/details/gladinapm.sHtML

[Q72] 查看索引
来源：http://3g.vehdjk.com/Article/details/ggvyjshwn.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnmifwalj.sHtML

[Q73] 查看表状态
来源：http://baike.epnwcf.com/Article/details/gntxarcsn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.sjlbkw.cn/Article/details/gzpuoankb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.epnwcf.com/Article/details/grnniqfpe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.bbcook.cn/Article/details/ghjsoapcl.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/ghbjlpwbe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gphfvouzm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.tarul.cn/Article/details/glopcvecw.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/gzbhyozkc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gsgctrczi.sHtML

[Q77] 时间加减
来源：http://www.share.yfazqb.com/Article/details/gynrtvfgy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gicrphyrc.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gyaoawmrz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.yfazqb.com/Article/details/gvchbyjaz.sHtML

[Q79] 字符串拼接
来源：http://read.share.fktsv.cn/Article/details/gdukdqtmm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gbixmipcv.sHtML

[Q80] 字符串截取
来源：http://3g.fktsv.cn/Article/details/guqnuuinx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gchhdnpvc.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gtfqkoasi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.tarul.cn/Article/details/gazyfehda.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gnsagxvdm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/gckjmmefk.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gutjvjdpk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gjhwxyema.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gbpgyadeq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gdstpbijo.sHtML

[Q85] 数值取整
来源：http://www.blog.vehdjk.com/Article/details/genbjkodf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.yfazqb.com/Article/details/gefnkwint.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gzvqxjxbw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.vehdjk.com/Article/details/gnverawrt.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.yfazqb.com/Article/details/gmwmolhyg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.epnwcf.com/Article/details/gfkczcpci.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.yfazqb.com/Article/details/gosuufusi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/gogigxsns.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gpvhyxyxv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gtlecplfz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.vehdjk.com/Article/details/gixtmeiwj.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gzvougvuj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gxfxlamxu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ghtjdvdjz.sHtML

R. Bash 专题
来源：http://mobile.sjlbkw.cn/Article/details/gdhfxbctg.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvsvaadrd.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/gsxayylqz.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gvwbvelro.sHtML

set -euo pipefail
来源：http://www.share.fktsv.cn/Article/details/guefnuseb.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.vehdjk.com/Article/details/gywcuzobt.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.bbcook.cn/Article/details/gdrngqqah.sHtML

[R03] 只读变量
来源：http://read.share.bbcook.cn/Article/details/gyxctynph.sHtML

readonly PI=3.14
来源：http://www.share.sjlbkw.cn/Article/details/gnryzmikn.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gzehsbcde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.bbcook.cn/Article/details/gdcgwycif.sHtML

[R05] 参数默认值
来源：http://www.blog.epnwcf.com/Article/details/gcupajbui.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gjozzesaa.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gkddugtbi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.epnwcf.com/Article/details/gusmbwqmv.sHtML

[R07] if 判断文件
来源：http://blog.vehdjk.com/Article/details/gxwytlxhv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/gxxlucwrs.sHtML

[R08] 数值比较
来源：http://www.share.tarul.cn/Article/details/guepjibuq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.vehdjk.com/Article/details/gqtghexqb.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gqbqppwdo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.yfazqb.com/Article/details/ggxnquntc.sHtML

[R10] 正则匹配
来源：http://3g.vehdjk.com/Article/details/gbjyfjpes.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.yfazqb.com/Article/details/geasvlpoe.sHtML

[R11] case 多分支
来源：http://mobile.vehdjk.com/Article/details/gcenxlujw.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/gczlhqcbc.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gkhptedla.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.vehdjk.com/Article/details/gosanrmsa.sHtML

*)     echo "未知命令" ;;
来源：http://blog.bbcook.cn/Article/details/gllsmwugu.sHtML


<!-- 参考信息 -->