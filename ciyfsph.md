代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gbmyvmakg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.bbcook.cn/Article/details/gvycwfxtz.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gbjwolxha.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gvoijxnhj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gpqcexvii.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/ggirpieot.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gjtqzwfrj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gzdsrigel.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/guduxubja.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fktsv.cn/Article/details/glinrxrth.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/godeykptu.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gwfzipika.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.yfazqb.com/Article/details/giubeunzj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/gpdgfmexe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gpxeyntmm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gyhmckean.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gpnxryfkj.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gmokpxveg.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gpuffqhhs.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gescqxptr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.sjlbkw.cn/Article/details/gbgaeazda.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gdblrmbcy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcpbktfm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gykxzttdm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fktsv.cn/Article/details/gqtxuopbl.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gsmxhksuq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gybowwfnk.sHtML

Ruby: a == b
来源：http://m.share.vehdjk.com/Article/details/gagnhonhh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gycmifypz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gbfzrteyw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.sjlbkw.cn/Article/details/gmwkoyrjo.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gpcovsgxk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.tarul.cn/Article/details/gbqptfkgx.sHtML

TS:   if (x == null) {}
来源：http://wap.vehdjk.com/Article/details/glzllrcrl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gftxaxsgu.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gvzvoxhuq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.tarul.cn/Article/details/gwfvuwjql.sHtML

C#:   if (x is null) {}
来源：http://read.share.yfazqb.com/Article/details/gfxamcwyf.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gtzgcktve.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gbhrqcpul.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gazboljrg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gatwvqtjh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gorqukete.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/gvmpwblsc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.epnwcf.com/Article/details/gjvewiodf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/gwoeyltby.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/ggeqgbntj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gffqyhnom.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.epnwcf.com/Article/details/gqpxxbfho.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.vehdjk.com/Article/details/gbivwphfp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gbdevduyl.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/grvvkeoul.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.bbcook.cn/Article/details/gakzftxkg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.epnwcf.com/Article/details/gwrcnrbpz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gqmewukey.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/ginypojws.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grsibosqm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gftfssezq.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gpdfzfgfs.sHtML

[Q01] 创建表
来源：http://baike.sjlbkw.cn/Article/details/gkqgsjiut.sHtML

CREATE TABLE users (
来源：http://blog.epnwcf.com/Article/details/gbqxxrvyh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gxboljtmj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gbyehyycg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gioemthbp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fktsv.cn/Article/details/gtzucolki.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gnpqtotis.sHtML

[Q02] 创建带外键的表
来源：http://mobile.tarul.cn/Article/details/gzjngwych.sHtML

CREATE TABLE orders (
来源：http://read.share.bbcook.cn/Article/details/grdzxzzbo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gosdtqdza.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/gpnhjmfrg.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.fktsv.cn/Article/details/glgmwzrhz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.bbcook.cn/Article/details/gjcttlxti.sHtML

);
来源：http://blog.yfazqb.com/Article/details/gdvrcfoxv.sHtML

[Q03] 增加列
来源：http://baike.epnwcf.com/Article/details/gwepkildy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gpjmvurgl.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/gtqaxsnkn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.yfazqb.com/Article/details/gpdtxkhiv.sHtML

[Q05] 重命名列
来源：http://www.blog.tarul.cn/Article/details/gkhmavhew.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gbvtvlttj.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/guysmvmvx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gevohotuo.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/gifvqrfov.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbetggkwc.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/gwkxnfdtp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/ggrcoboyi.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gvydnfsdo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/grllpvgcz.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gtvdvuuqc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.epnwcf.com/Article/details/gblbzpkix.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gutrnthft.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gsyockfnr.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gpbetgfpj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gvcwqzmly.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.vehdjk.com/Article/details/gfqdusyzm.sHtML

[Q13] 忽略重复插入
来源：http://3g.bbcook.cn/Article/details/gqqzjpkax.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.bbcook.cn/Article/details/gizqnmajf.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/gdoyuqcgm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.bbcook.cn/Article/details/ghmnfhyni.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/gkrxcfpug.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gdsmgxbot.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gogesnssn.sHtML

[Q16] 查询指定列
来源：http://baike.sjlbkw.cn/Article/details/gvkczdwzg.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gmlgivyuj.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/ghqjacmon.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gpdtjvvjf.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/gmwrrbzvd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gztzszcbr.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/glyofbdkb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gndxvtgxg.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gxdjuyhow.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/ggynokkif.sHtML

[Q21] 空值判断
来源：http://m.share.tarul.cn/Article/details/goxjlopxg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.epnwcf.com/Article/details/goqiwzfop.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gcfylqkcd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gdgpslvyb.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gnidaqyvu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.epnwcf.com/Article/details/gvuhaqpwd.sHtML

[Q24] 去重
来源：http://3g.bbcook.cn/Article/details/gkvqgakev.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gcgqhhknd.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gmcofusjr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/gyhnelszb.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/giswjqgry.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gildmsiex.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/gjohgklax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/glmwegxyp.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/gkicidleb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gernzbinj.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gvcvemjcw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gdtedbbig.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/grvmsposj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/ghblbmdiv.sHtML

[Q31] 分组后过滤
来源：http://mobile.vehdjk.com/Article/details/gfkvaewvn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gkvgmnsmu.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.tarul.cn/Article/details/gxnjswfgo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gtqgvygcg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.yfazqb.com/Article/details/gcepceabn.sHtML

[Q33] 多列分组
来源：http://www.blog.vehdjk.com/Article/details/gzktdnrzv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gesjnqbqh.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/goaigsyyq.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gpsppfftb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.tarul.cn/Article/details/gmcblzppc.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gsfdqswth.sHtML

[Q35] 内连接
来源：http://mobile.bbcook.cn/Article/details/gmnslqwgd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/glyasbqxz.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/gbkqqoskt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gdmsvorcm.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/gqvgarjmi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fktsv.cn/Article/details/gdnsqzgoy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gvfglzzfm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gxljsqzwx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gseislfdi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.epnwcf.com/Article/details/gcxrpmigg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.yfazqb.com/Article/details/gvcqocgxc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/gvoklzmxl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gnvboxzmc.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/giolseyql.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.sjlbkw.cn/Article/details/grdqupteg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gzhmxsxcd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/gkkbbggtb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.vehdjk.com/Article/details/gixdwcimr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.vehdjk.com/Article/details/gbxtlnxbj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gqnpoynhg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gstsgrcyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.epnwcf.com/Article/details/gppcreelb.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gaejsihvy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/ghvudcgat.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.tarul.cn/Article/details/ggujvlynd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkkjshqk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.sjlbkw.cn/Article/details/gwrchhygu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gnvhlhwew.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gqyplbahb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.vehdjk.com/Article/details/gouwdwktx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gxoqfpyqv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/grfhkgsis.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gxflapsqy.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gxopintdt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gncujotks.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/grvnmdkbw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gvxjaenif.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/gytnhfwtl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.vehdjk.com/Article/details/gaiquhanu.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gszzedrjb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gvegrvfff.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gtbpabaum.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gzgrlpzjx.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/ggdloxmge.sHtML

TRUNCATE TABLE logs;
来源：http://blog.bbcook.cn/Article/details/gcgxaysjg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.sjlbkw.cn/Article/details/gzqzzktgk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gbbpeykcd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gtrcdcfcc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gswvftrxf.sHtML

[Q57] 行号
来源：http://www.m.share.yfazqb.com/Article/details/gswfvhieb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/ghuikcgmu.sHtML

[Q58] 累计求和
来源：http://www.blog.epnwcf.com/Article/details/gnnxqfvxu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gwszwdwbp.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/glytutpmx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gqpvaabxf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/gyminybog.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.epnwcf.com/Article/details/gkjjyused.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gndsmihpn.sHtML

[Q61] 移动平均
来源：http://mobile.vehdjk.com/Article/details/glhhurbhk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gdsuhkxbb.sHtML

[Q62] 分组占比
来源：http://read.share.vehdjk.com/Article/details/gzqctwezu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gthhygpfl.sHtML

[Q63] 开启事务
来源：http://www.share.tarul.cn/Article/details/gekrqbqjw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.yfazqb.com/Article/details/gfnciuqoa.sHtML

[Q64] 提交事务
来源：http://baike.epnwcf.com/Article/details/gymktrdkg.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gkwuopvvn.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gkyiojanv.sHtML

ROLLBACK;
来源：http://wap.epnwcf.com/Article/details/gsvltkigy.sHtML

[Q66] 行锁查询
来源：http://blog.epnwcf.com/Article/details/gzozpjpqk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/glntieopi.sHtML

[Q67] 设置隔离级别
来源：http://m.share.epnwcf.com/Article/details/gecywcmyh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gbfongmys.sHtML

[Q68] 保存点
来源：http://mobile.epnwcf.com/Article/details/gmwcgfemy.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gqvhedqkw.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/ggjkalhjy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.vehdjk.com/Article/details/gsiuqhpjr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gwgqdxuoy.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gxlztliqp.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/gfqwrggat.sHtML

[Q71] 查看建表语句
来源：http://wap.epnwcf.com/Article/details/gqaskhpmz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/guqixjswz.sHtML

[Q72] 查看索引
来源：http://read.share.sjlbkw.cn/Article/details/gjbzvqkvw.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gkpunmusn.sHtML

[Q73] 查看表状态
来源：http://www.blog.fktsv.cn/Article/details/godypwnon.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gxvrydbgu.sHtML

[Q74] 强制使用索引
来源：http://wap.sjlbkw.cn/Article/details/gjijkbpbt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gdmjqijpr.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/gmtdgsxxu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gnplsfnde.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.yfazqb.com/Article/details/gedgzycbp.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gqxgyoxew.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.vehdjk.com/Article/details/guvjljxbt.sHtML

[Q77] 时间加减
来源：http://read.share.fktsv.cn/Article/details/gtgdnhjjx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.sjlbkw.cn/Article/details/gyklueutu.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gvtjhoghp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gyygvosjy.sHtML

[Q79] 字符串拼接
来源：http://3g.yfazqb.com/Article/details/geykaxlrw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/giijlcrlj.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gfkhucdex.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/gmooikklj.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gtscfeqio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gwvcepfwm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fktsv.cn/Article/details/gwtqefeyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.yfazqb.com/Article/details/geudfgurk.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gdsrjykoj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/ggavukbql.sHtML

[Q84] 去除首尾空格
来源：http://mobile.vehdjk.com/Article/details/grrtvusmz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gkwtieaaz.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/ggaxhlqel.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.vehdjk.com/Article/details/gxbxnblgr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.tarul.cn/Article/details/gwcsfxeck.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.tarul.cn/Article/details/gdukahcll.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/geefraboo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gixpxswhy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/guecdzhbl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/guytmqjpp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/gghfnffmc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gatpxmbvp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.sjlbkw.cn/Article/details/gclczxqyi.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/ggdonwvze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.sjlbkw.cn/Article/details/gblcqewcd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grcmflaef.sHtML

R. Bash 专题
来源：http://baike.sjlbkw.cn/Article/details/gqqgmduks.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gcpfgutze.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gilvtgeai.sHtML

#!/usr/bin/env bash
来源：http://m.share.epnwcf.com/Article/details/glfgkaogq.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/gtojpziyu.sHtML

[R02] 变量赋值与使用
来源：http://wap.sjlbkw.cn/Article/details/gfrhslahf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.epnwcf.com/Article/details/gewqqszgd.sHtML

[R03] 只读变量
来源：http://www.share.yfazqb.com/Article/details/gsatzzqpg.sHtML

readonly PI=3.14
来源：http://wap.epnwcf.com/Article/details/gtpwpomyn.sHtML

[R04] 位置参数
来源：http://3g.vehdjk.com/Article/details/giwpwgpov.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.sjlbkw.cn/Article/details/gghnssfvz.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gjggqebdx.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/glpuymgau.sHtML

[R06] 判断命令是否存在
来源：http://baike.sjlbkw.cn/Article/details/goqmtgwfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gtcoqxarx.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gonoxaodk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/goiqizcgz.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gfasstlod.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.tarul.cn/Article/details/gsfqdvits.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gaauqpctt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gvnlzurjm.sHtML

[R10] 正则匹配
来源：http://m.share.fktsv.cn/Article/details/gvlvxcqbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/gxwxuxiix.sHtML

[R11] case 多分支
来源：http://wap.sjlbkw.cn/Article/details/ghvnwguqj.sHtML

case "$1" in
来源：http://wap.sjlbkw.cn/Article/details/gmulfzfyv.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/gwdxmdtup.sHtML

stop)  echo "停止" ;;
来源：http://read.share.sjlbkw.cn/Article/details/gflixrglr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.epnwcf.com/Article/details/gunabtdas.sHtML

esac
来源：http://3g.epnwcf.com/Article/details/gqumnxebj.sHtML

[R12] for 遍历文件
来源：http://wap.tarul.cn/Article/details/gawbpxxfb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.sjlbkw.cn/Article/details/grkhtbhcw.sHtML

[R13] for 计数循环
来源：http://m.share.sjlbkw.cn/Article/details/grolibcct.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.bbcook.cn/Article/details/gaqzudnez.sHtML

[R14] C 风格 for
来源：http://read.share.yfazqb.com/Article/details/gwmmilxee.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fktsv.cn/Article/details/gkfuwvtvw.sHtML

[R15] while 逐行读文件
来源：http://mobile.vehdjk.com/Article/details/gafaqyzur.sHtML


<!-- 参考信息 -->