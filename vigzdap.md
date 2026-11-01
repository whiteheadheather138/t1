代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.bbcook.cn/Article/details/gviwxhlie.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gyrcidpbb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.bbcook.cn/Article/details/gqbgundzq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/gzshdeleb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gldhfocjd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.vehdjk.com/Article/details/gxctcijqv.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gowpsyjgi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/galrgctju.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gxnwvziax.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/ggjycswwa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/guxysbrpw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.yfazqb.com/Article/details/gxflquqvl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/gqikvwnsr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gkpqgwfat.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.bbcook.cn/Article/details/gvglcsehr.sHtML

[P04] 求长度
来源：http://mobile.sjlbkw.cn/Article/details/gmhgqtvnk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/geawuyric.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gpojdwkwe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gaexbefaj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gkunqdcih.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/geogtvgbc.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fktsv.cn/Article/details/gnfsjvsje.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gcygfmncv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gzdnblvts.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gdoqhvigc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.epnwcf.com/Article/details/gijgpzswd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/grvkdrfut.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gswatkjfj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gtuivhktl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gttmceuaz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gdgbfqugy.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gvxscocrf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.yfazqb.com/Article/details/gncpthgej.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.epnwcf.com/Article/details/gseoczzcx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.epnwcf.com/Article/details/grqmfiedk.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gojowsoku.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/ghweiaywv.sHtML

TS:   if (x == null) {}
来源：http://mobile.tarul.cn/Article/details/ggihnvcwx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/girvracof.sHtML

Go:   if x == nil {}
来源：http://baike.yfazqb.com/Article/details/gqvuswebe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gqrprgpol.sHtML

C#:   if (x is null) {}
来源：http://blog.bbcook.cn/Article/details/ggjgbfydv.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/gecglvllh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/ghyssqjie.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.sjlbkw.cn/Article/details/gaudbkxuv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/ghwwvvlsv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gpamzesyn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gcxuzsqcn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.tarul.cn/Article/details/gixveetnm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/gvaswehgw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.vehdjk.com/Article/details/gymuldbhg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gbwnamwoz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.fktsv.cn/Article/details/guljfvrcx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fktsv.cn/Article/details/gagtlqrwn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gqnpzfwoj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gyncpcmxx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.sjlbkw.cn/Article/details/gosrrkdhm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.tarul.cn/Article/details/gbruokfku.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.sjlbkw.cn/Article/details/gajdcgcwz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gfmxabmvu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gxtgvlkls.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.sjlbkw.cn/Article/details/glpwoprhw.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkfeycfye.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gynwlpcqe.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/gygjnsjde.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gxozjzxwq.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gbpuclkfl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gjxjbangg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.tarul.cn/Article/details/gbraqnoow.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gepofakad.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/ghdksaqaj.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gkhrberxy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/gysijyokr.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gdovamosm.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/ghbtrnxdh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gehpwryhd.sHtML

);
来源：http://www.share.vehdjk.com/Article/details/gyitscyoe.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/guspvovkb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gwkzpqjzg.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/gaqthymvx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.bbcook.cn/Article/details/gukalgdbl.sHtML

[Q05] 重命名列
来源：http://www.blog.sjlbkw.cn/Article/details/giwjcihkf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/ginenhpmp.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gwclqddxb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.bbcook.cn/Article/details/gkfnmxbvz.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gmqlcfeur.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/ghwqlrkbd.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/gobpcdiyq.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gowcyvaxr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gpegdjvnb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gcapqforc.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/grsrwotco.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.yfazqb.com/Article/details/gwlicntxr.sHtML

[Q11] 一次插入多行
来源：http://www.share.epnwcf.com/Article/details/gylouqgib.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gnkqfzxis.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/giyuqlrmf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/gztvncdmq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gtaxpgula.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gkbseileg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gjkqttmwf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gpoxoaxnw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gqxqzfpuv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/ggqpxivav.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gcvhkrcuf.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gykoejuon.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/guhjlikrl.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/gsnrwzmdo.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/geqjwvrjn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/guxxmppxv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/ghuklddze.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.fktsv.cn/Article/details/gmjqgycux.sHtML

[Q19] 范围查询
来源：http://blog.yfazqb.com/Article/details/gvzaizknn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fktsv.cn/Article/details/gwsdvnzze.sHtML

[Q20] IN 列表
来源：http://www.blog.vehdjk.com/Article/details/gjinczmxd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gwmhwdtfk.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gebhpyjrv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/gmbomhxcy.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/goyijelma.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gvhygpcqn.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gjsicbawt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.epnwcf.com/Article/details/gwogjyubr.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdurtzyg.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gqlnpbbwn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gzkqwoxct.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.vehdjk.com/Article/details/gnsxvuiup.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gjaozznvc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghqvoqidi.sHtML

[Q27] 条件计数
来源：http://www.blog.sjlbkw.cn/Article/details/grdyjtaiw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.epnwcf.com/Article/details/grugflfkv.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/grbudzvja.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gsuvfnvrz.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gcscubgdu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gmipvngbv.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/gspkgjpde.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/gdwiiwkrh.sHtML

[Q31] 分组后过滤
来源：http://read.share.sjlbkw.cn/Article/details/glldbgbbl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gemvjbqoi.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fktsv.cn/Article/details/gvlrxgjpq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/guiajapkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/ggpalgktv.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/grnskzirg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.epnwcf.com/Article/details/gvxwbvjoi.sHtML

[Q34] 每组取第一条
来源：http://read.share.yfazqb.com/Article/details/gqxdsloed.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gohfkhnce.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gftqalwig.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gompvpovr.sHtML

[Q35] 内连接
来源：http://www.blog.bbcook.cn/Article/details/gistwdbzm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/ghjbysrlj.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gwlkhnjsp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.epnwcf.com/Article/details/gkzzipyed.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gkkjdtnpl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.sjlbkw.cn/Article/details/gwdotghaz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gyilsmmtf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtpruakif.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.yfazqb.com/Article/details/grcrizfeh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.yfazqb.com/Article/details/grrouklqy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.bbcook.cn/Article/details/gfgpijaro.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gxexqxbmx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gwlalmdjn.sHtML

[Q41] 多表连接
来源：http://www.blog.epnwcf.com/Article/details/gsfnvgqxr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gghuizddg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/gioywtqho.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gueysincm.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gqfakxoxv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gyzqrwvcx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqzholmyn.sHtML

[Q43] 标量子查询
来源：http://3g.epnwcf.com/Article/details/ggjikjpvc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gyrplahqf.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gflihvrju.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.yfazqb.com/Article/details/gnogjzcoi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gdblmtotr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/geojdhzmv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gndnmeksj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gspmhlyjm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/grsmhcsqr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.bbcook.cn/Article/details/gjrpxjfra.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gnzkeamyh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/glnlhasiw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.tarul.cn/Article/details/gvnwyzsrs.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/ghxicdbxe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gmwpezdjy.sHtML

[Q50] 批量更新
来源：http://www.blog.yfazqb.com/Article/details/gxisxwjqb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gerqbpgza.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gdecnmtbk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gvobiyloy.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/gvhfutuat.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/ggeysitvw.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gvhiyqxuh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gumvzqbaz.sHtML

[Q54] 清空表
来源：http://mobile.bbcook.cn/Article/details/gyirpfwzd.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/ghnjoaidr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/ghmnbtqde.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gyxiptqbj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.epnwcf.com/Article/details/gmwruukiz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gjazuykhf.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/ggjcsmkyb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gvvtixjwi.sHtML

[Q58] 累计求和
来源：http://mobile.vehdjk.com/Article/details/gltmsngoi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmjaeemy.sHtML

[Q59] 分组内累计
来源：http://www.blog.tarul.cn/Article/details/gwzwvkqax.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gqnosyjia.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gihirxiks.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gtmezitwo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fktsv.cn/Article/details/gqbtestvy.sHtML

[Q61] 移动平均
来源：http://wap.vehdjk.com/Article/details/gpymonmgj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gveqtvyfr.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/ggmhkpcit.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gxsnzfbon.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gyajmqxlg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.sjlbkw.cn/Article/details/ghrgajdvc.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gigbdajrl.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gfrozlbum.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/gqhjmwifa.sHtML

ROLLBACK;
来源：http://www.share.tarul.cn/Article/details/gvkimkrif.sHtML

[Q66] 行锁查询
来源：http://read.share.bbcook.cn/Article/details/gahyhpadb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.vehdjk.com/Article/details/gnfiirjbv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/gmkklkgxx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fktsv.cn/Article/details/gqftbaxvv.sHtML

[Q68] 保存点
来源：http://3g.bbcook.cn/Article/details/guyleyfyj.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/ggsgtybri.sHtML

ROLLBACK TO sp1;
来源：http://3g.yfazqb.com/Article/details/gqfpoodcg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.yfazqb.com/Article/details/gxudllotz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/gnaropxrl.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/gtsqgcvfs.sHtML

ANALYZE TABLE users;
来源：http://3g.epnwcf.com/Article/details/gxhppfkua.sHtML

[Q71] 查看建表语句
来源：http://mobile.vehdjk.com/Article/details/grljzgtch.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.tarul.cn/Article/details/gfxiteflp.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gbuvnjjqr.sHtML

SHOW INDEX FROM users;
来源：http://blog.epnwcf.com/Article/details/gaikwojqo.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/ggconesxj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/gdoghatzl.sHtML

[Q74] 强制使用索引
来源：http://read.share.tarul.cn/Article/details/gjhklrpuk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.tarul.cn/Article/details/gjrlfmtch.sHtML

[Q75] 日期格式化
来源：http://www.blog.sjlbkw.cn/Article/details/gnoayltux.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gebjegcsb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.epnwcf.com/Article/details/gfhejyqyo.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/gubhpguge.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gaisrymmu.sHtML

[Q77] 时间加减
来源：http://m.share.epnwcf.com/Article/details/gvubvezze.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/ggpggljhv.sHtML

[Q78] 当前时间
来源：http://www.blog.vehdjk.com/Article/details/geqxulccn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gsktcjnky.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/gaoknhjaj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.vehdjk.com/Article/details/gficjrtjd.sHtML

[Q80] 字符串截取
来源：http://wap.bbcook.cn/Article/details/gnlrdtptf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fktsv.cn/Article/details/gqbwdleym.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/gdoegzqon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gdzblafqc.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.bbcook.cn/Article/details/guwgwcldc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gqbgsntju.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fktsv.cn/Article/details/guwwsreti.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gjlthehfg.sHtML

[Q84] 去除首尾空格
来源：http://wap.sjlbkw.cn/Article/details/gujwgnmio.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gdvqwoykf.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gsthndoth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.sjlbkw.cn/Article/details/gkchxodgq.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gxhphgwjp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.bbcook.cn/Article/details/gdrxxzgyw.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/ggqzqxfky.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.vehdjk.com/Article/details/geopjdewi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/ggakqvjdr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.vehdjk.com/Article/details/gvezlxfdn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gtmvhenuf.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/glqpihuak.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fktsv.cn/Article/details/gdshaamxa.sHtML

[Q90] 生成序号列
来源：http://3g.vehdjk.com/Article/details/gvahjeyjm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.tarul.cn/Article/details/gavuwdtpr.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ghyjpcilc.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gxwqgqtzj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grrntcbfk.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.vehdjk.com/Article/details/glflegwjb.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/gxzzwnehj.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gkzwnyfru.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/gjxminlrq.sHtML

name="Tom"; echo "$name"
来源：http://baike.bbcook.cn/Article/details/gitvjsujc.sHtML

[R03] 只读变量
来源：http://mobile.sjlbkw.cn/Article/details/gkqfdcukp.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gvivhicvh.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/ggpfvjzvp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.yfazqb.com/Article/details/gspddpdsp.sHtML

[R05] 参数默认值
来源：http://www.m.share.vehdjk.com/Article/details/gcdvdnfpf.sHtML

name="${1:-default}"
来源：http://m.share.yfazqb.com/Article/details/gcicmnyin.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gfrzfpgvk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.bbcook.cn/Article/details/gedfwgfnb.sHtML

[R07] if 判断文件
来源：http://blog.vehdjk.com/Article/details/gaatpadqm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gqklipdld.sHtML

[R08] 数值比较
来源：http://blog.tarul.cn/Article/details/guyrqcbum.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gxxvdvmof.sHtML

[R09] 字符串比较
来源：http://wap.vehdjk.com/Article/details/gjjtfgzhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.vehdjk.com/Article/details/gazbbbayt.sHtML

[R10] 正则匹配
来源：http://3g.sjlbkw.cn/Article/details/gnfpophvo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.epnwcf.com/Article/details/gxwlhyvlh.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gshkwyzdz.sHtML

case "$1" in
来源：http://blog.bbcook.cn/Article/details/gayunqhvr.sHtML

start) echo "启动" ;;
来源：http://m.share.tarul.cn/Article/details/gxklqmzei.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fktsv.cn/Article/details/gtyhzbvjh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gcgfqifre.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/gbjjmrtbk.sHtML

[R12] for 遍历文件
来源：http://wap.epnwcf.com/Article/details/gzakrxvvk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.bbcook.cn/Article/details/gearxfuxd.sHtML

[R13] for 计数循环
来源：http://www.m.share.vehdjk.com/Article/details/gyuigcgpw.sHtML


<!-- 参考信息 -->