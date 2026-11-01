代发 wailian999

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gipbtwtfp.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fktsv.cn/Article/details/gtlnuzjmz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gzpekgfir.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.bbcook.cn/Article/details/gzqxxptcd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gloowthrb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gsavksoat.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.sjlbkw.cn/Article/details/gynkjhfny.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gkorwnqid.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/gqlffzfhp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gujafshnd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.tarul.cn/Article/details/glpwyeyol.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gpbzksnio.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gajfxzxnb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.epnwcf.com/Article/details/gzjwmcbqe.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gemmkesak.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.bbcook.cn/Article/details/gnfysojqb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gavtaweay.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/ghcayeoxc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gpgmvsnjy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/glwglcthz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.epnwcf.com/Article/details/gaiyaxxad.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gukwdcftk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gljucqeyl.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gflshrpyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.epnwcf.com/Article/details/gilgypjrb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gbwozevjk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gfczoimnp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gnukrxrpx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gapnlscwu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/gektdgekn.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.bbcook.cn/Article/details/gqrshdilp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gzxdxucks.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gqlvefrqz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/gqzthpctr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/ghpcptjyl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.epnwcf.com/Article/details/gqlyygxhp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/gwrnozbrn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gjygpdfbk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.epnwcf.com/Article/details/gpwgpvtst.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gqqlpttzw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gqhqtjtaf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gtiedfwpu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gshkkllhv.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/glaeiqbjg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/gyceaiqld.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gsbvuqtel.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/grddmabdh.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gsnmdiryv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.epnwcf.com/Article/details/gkyycokis.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/goqearckz.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gczpcvpae.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gaezhofih.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gquncmdow.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.epnwcf.com/Article/details/gnqicqzgh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gwbfraqqd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.vehdjk.com/Article/details/gayesbmad.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gdlfjqmbl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gidalhixu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.epnwcf.com/Article/details/ghqpdusmk.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/glelzeere.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/gxvnvpytv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gmoicbein.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/ggquklhtc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gvttapfcj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/ghrvojigu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.tarul.cn/Article/details/giiojddyb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fktsv.cn/Article/details/gogfvmfhj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gmykkueqd.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/giupvjwyg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/gbpphaymy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsslcvftw.sHtML

[Q01] 创建表
来源：http://www.m.share.tarul.cn/Article/details/gmrofpxxc.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gqibydeqr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/gyypnmoqh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gblzdihpu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gctxswfce.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.vehdjk.com/Article/details/goxwrurzz.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gdavkhgpd.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fktsv.cn/Article/details/gagjwkzqq.sHtML

CREATE TABLE orders (
来源：http://www.share.sjlbkw.cn/Article/details/gpxpymxrv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gfwavftyw.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/geanfkexx.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gedadrhqj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.bbcook.cn/Article/details/gurngqyrq.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gpyjwounh.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/glsybzice.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gajtipoiz.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/gsviupqip.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gmasioniz.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gvcaeqnsb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/guqnvqxjc.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/guwbznquq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/gxiomprah.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gvaibjjlb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.epnwcf.com/Article/details/gpvvbhgjc.sHtML

[Q08] 创建普通索引
来源：http://3g.tarul.cn/Article/details/gvigrjwzx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gpqqbempd.sHtML

[Q09] 创建唯一索引
来源：http://wap.sjlbkw.cn/Article/details/ghkpbzfuj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gawtlrobz.sHtML

[Q10] 插入单行
来源：http://m.share.vehdjk.com/Article/details/gykusahir.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fktsv.cn/Article/details/gypedgxmv.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/gkvjjuxxg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.tarul.cn/Article/details/gjabuwicm.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fktsv.cn/Article/details/gqqiqtykf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.tarul.cn/Article/details/gamqerrqc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/gslifowpo.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gpggbqudn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/gizpeedmq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gestbwzhk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.epnwcf.com/Article/details/gidnlrpeu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gydsnfswi.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gccjkapif.sHtML

SELECT * FROM users;
来源：http://3g.epnwcf.com/Article/details/ghfpwfltk.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/gqraapzzm.sHtML

SELECT id, name FROM users;
来源：http://read.share.tarul.cn/Article/details/gxihgnolt.sHtML

[Q17] 条件查询
来源：http://www.blog.yfazqb.com/Article/details/gqavchsns.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/goklxhesg.sHtML

[Q18] 模糊匹配
来源：http://mobile.vehdjk.com/Article/details/gqxwztzvz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gupnhelsb.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gbtjdfifa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.vehdjk.com/Article/details/gtgblaqlz.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/gbepuvoow.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gguqyzsjx.sHtML

[Q21] 空值判断
来源：http://baike.bbcook.cn/Article/details/gmkvqpcov.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gshgvfhcx.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gkqfmefvv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.sjlbkw.cn/Article/details/glbjxjbzq.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/guwjtoqtk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gopcwdbxa.sHtML

[Q24] 去重
来源：http://blog.fktsv.cn/Article/details/ggvuoulmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gimfojlve.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.sjlbkw.cn/Article/details/gimpfkidg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gtktbtcxp.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gjsvhdlkd.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gpbrtfkfd.sHtML

[Q27] 条件计数
来源：http://read.share.bbcook.cn/Article/details/gdwozfwdj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gblxdpona.sHtML

[Q28] 求和与平均
来源：http://read.share.yfazqb.com/Article/details/guqmidnyp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/grgwjabpq.sHtML

[Q29] 最大最小值
来源：http://3g.tarul.cn/Article/details/gvobrnsrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gjdnzlxid.sHtML

[Q30] 分组统计
来源：http://www.blog.vehdjk.com/Article/details/ghdjsnden.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gsdngpitb.sHtML

[Q31] 分组后过滤
来源：http://read.share.fktsv.cn/Article/details/ggyfyyqxu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fktsv.cn/Article/details/ghjbqbbgd.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/ggamvvlnm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gkcdovdaw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/glnxolbhl.sHtML

[Q33] 多列分组
来源：http://www.m.share.tarul.cn/Article/details/gfqapcqfj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/gstdaefrt.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gklsdjqkc.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gdyalfahh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gjijxvgro.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gjfppvcqx.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/gfjeczkvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gsxlzfrqj.sHtML

[Q36] 左连接
来源：http://read.share.bbcook.cn/Article/details/gmponbvtt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gcmagqsjh.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gpdcgtbqs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.vehdjk.com/Article/details/ghofpdeag.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gvaethhjo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/glsktqdrj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/geaezzddn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.vehdjk.com/Article/details/gtvbgaxbl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.sjlbkw.cn/Article/details/gdpiwmqhx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.epnwcf.com/Article/details/gnbvjomwe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gqdvnnkih.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gklnwfczo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/glulebfvl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.epnwcf.com/Article/details/geydswbnw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.tarul.cn/Article/details/gsvaokgxr.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.sjlbkw.cn/Article/details/gitoucbwd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gzkrlrhov.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.epnwcf.com/Article/details/gpbygwjtu.sHtML

[Q43] 标量子查询
来源：http://read.share.tarul.cn/Article/details/gzkcjfqlg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/guscyybpq.sHtML

[Q44] IN 子查询
来源：http://m.share.vehdjk.com/Article/details/gwdbacpes.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.yfazqb.com/Article/details/ggenywjam.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/gynzgxwfb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gqvwdaksv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gaszaaipj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/gjugjfvxa.sHtML

[Q47] 与平均值比较
来源：http://mobile.yfazqb.com/Article/details/gfjlhjnpf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/gsnlpmeag.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.epnwcf.com/Article/details/glyhpyyex.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gzizcmgti.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.vehdjk.com/Article/details/gsfltzcoa.sHtML

[Q49] 更新单行
来源：http://wap.fktsv.cn/Article/details/gwiwrjgkp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gmimqqewk.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gckldcgaw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzskcewj.sHtML

[Q51] 用子查询更新
来源：http://www.blog.tarul.cn/Article/details/gkkzpkaxc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fktsv.cn/Article/details/ghjgupywk.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/glwlocghk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gnpcqvbnh.sHtML

[Q53] 按条件删除
来源：http://m.share.bbcook.cn/Article/details/gwccnuban.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/gdwkssyle.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/gnwvsleyp.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gngawmubd.sHtML

[Q55] 排名（并列占位）
来源：http://baike.epnwcf.com/Article/details/gkjqnosqu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gyibaxosu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gzjedrclw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gpjngfwzl.sHtML

[Q57] 行号
来源：http://blog.sjlbkw.cn/Article/details/goywhitkz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/ginldhlre.sHtML

[Q58] 累计求和
来源：http://wap.yfazqb.com/Article/details/ghshajyje.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/ggmyygeuu.sHtML

[Q59] 分组内累计
来源：http://m.share.fktsv.cn/Article/details/gepfxgwyc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gfinkpcpa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gdjaoujng.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fktsv.cn/Article/details/ggmzfnggy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/gpgqvxumf.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gnoylebha.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gfuddwfts.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/getpnycyy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gqsfbfhek.sHtML

[Q63] 开启事务
来源：http://read.share.yfazqb.com/Article/details/gsftozwbt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gbxsmyxex.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/gdglxgpyy.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/gzfjhsegw.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gsbgyeymh.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/gmhyltysh.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gyeojwfnn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/glxlfukxw.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gsinpanqw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gyppiirxf.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/girfbudsx.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gwwfrptky.sHtML

ROLLBACK TO sp1;
来源：http://blog.tarul.cn/Article/details/gcbstglyj.sHtML

[Q69] 查看执行计划
来源：http://read.share.epnwcf.com/Article/details/gmrolksbf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gjzzqgzkv.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gpdnfbjqi.sHtML

ANALYZE TABLE users;
来源：http://m.share.tarul.cn/Article/details/gknorxioy.sHtML

[Q71] 查看建表语句
来源：http://blog.yfazqb.com/Article/details/gngjpkhcg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.epnwcf.com/Article/details/gbyqlbjte.sHtML

[Q72] 查看索引
来源：http://read.share.fktsv.cn/Article/details/ggtrtjpak.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gdrhxcpep.sHtML

[Q73] 查看表状态
来源：http://mobile.yfazqb.com/Article/details/gvuxyqjxl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.vehdjk.com/Article/details/gmjcthdpx.sHtML

[Q74] 强制使用索引
来源：http://wap.fktsv.cn/Article/details/gowwoulow.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gvnbhmdlq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fktsv.cn/Article/details/gutcslyfc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gqwiarjks.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gkeelhjrl.sHtML

[Q76] 按天统计
来源：http://www.share.tarul.cn/Article/details/gisrxvoxz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gtztvnkqr.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gyawwyftf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gqsqhphfj.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/goohxuavk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqevyutk.sHtML

[Q79] 字符串拼接
来源：http://baike.bbcook.cn/Article/details/gunpuiajt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fktsv.cn/Article/details/gujrwhecm.sHtML

[Q80] 字符串截取
来源：http://baike.vehdjk.com/Article/details/gjbxuprkg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjajjiwus.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gkvvtqkeg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gvtjruzmw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.epnwcf.com/Article/details/gizsvgzpn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/geuwogcbe.sHtML

[Q83] 大小写转换
来源：http://www.m.share.yfazqb.com/Article/details/gisxmtejv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gyivrjvdy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gswueecrb.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gczzosukq.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gcvjntekp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.tarul.cn/Article/details/gjaoqclxq.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.tarul.cn/Article/details/ggoukafwk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.tarul.cn/Article/details/gmzyrudjz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.yfazqb.com/Article/details/ghxqsufkh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.yfazqb.com/Article/details/gguxkiuzg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.epnwcf.com/Article/details/gmevjqqss.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.bbcook.cn/Article/details/geekeyhao.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/gstmornss.sHtML

[Q89] 判断表是否存在
来源：http://read.share.sjlbkw.cn/Article/details/gblofkwei.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gdmmeuews.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/gbfavyiab.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.bbcook.cn/Article/details/gmlaousce.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grvqnlzue.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gxhccbqgz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gejnjvykg.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/gnsnnpftx.sHtML

#!/usr/bin/env bash
来源：http://blog.sjlbkw.cn/Article/details/gfkpwknpk.sHtML

set -euo pipefail
来源：http://mobile.yfazqb.com/Article/details/gafvpqfsf.sHtML

[R02] 变量赋值与使用
来源：http://mobile.yfazqb.com/Article/details/gbocruuvx.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gdocujyzm.sHtML

[R03] 只读变量
来源：http://read.share.vehdjk.com/Article/details/gtemgtbsp.sHtML

readonly PI=3.14
来源：http://wap.vehdjk.com/Article/details/gqplxvqcc.sHtML

[R04] 位置参数
来源：http://www.m.share.tarul.cn/Article/details/gjxperupi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.bbcook.cn/Article/details/ghvbecqhg.sHtML

[R05] 参数默认值
来源：http://3g.epnwcf.com/Article/details/gngstymli.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gckmytvir.sHtML

[R06] 判断命令是否存在
来源：http://read.share.epnwcf.com/Article/details/gnilhayww.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.sjlbkw.cn/Article/details/geqrlcbyy.sHtML

[R07] if 判断文件
来源：http://wap.yfazqb.com/Article/details/gxklbjzxh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fktsv.cn/Article/details/gjsovvsbx.sHtML

[R08] 数值比较
来源：http://blog.bbcook.cn/Article/details/gbwuxhwcd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.epnwcf.com/Article/details/gywxscyoi.sHtML

[R09] 字符串比较
来源：http://www.share.fktsv.cn/Article/details/gxumynzka.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.epnwcf.com/Article/details/gurarhhaq.sHtML

[R10] 正则匹配
来源：http://baike.fktsv.cn/Article/details/gduszyhel.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.epnwcf.com/Article/details/gkmfsrjfl.sHtML

[R11] case 多分支
来源：http://m.share.tarul.cn/Article/details/geahpaotb.sHtML


<!-- 参考信息 -->