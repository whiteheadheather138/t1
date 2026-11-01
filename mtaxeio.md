代发 wailian999

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/ghbskjest.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glevlobbb.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gvdlufcrp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gacrixpgp.sHtML

[P01] 生成 UUID
来源：http://www.blog.epnwcf.com/Article/details/gydjrbrcp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/ggwbrrjpy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gavxduape.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/guptkecfe.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/ggtnzzwmc.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/grbzmtwzv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.yfazqb.com/Article/details/gqsdxjpvi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gmjpyjtkk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/guikmlurg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gmuztmurz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.epnwcf.com/Article/details/gkavxccco.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/ggxtqybzo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gviebhiwo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gnrguffsh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gpjdlofhp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/ggkieygbx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/ggmwpmxxw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gxpivsrzu.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gmtegzcph.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.tarul.cn/Article/details/gmyuiiozg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gwppablok.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gngitjgfs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gkohipswt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/genjmqjkp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gcrglwsxc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.yfazqb.com/Article/details/gjowomfzz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/gqnntusse.sHtML

[P04] 求长度
来源：http://mobile.yfazqb.com/Article/details/gkuvxqfms.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/gkftckujl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.yfazqb.com/Article/details/gqxqomwvt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/guqlkhxii.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/guscrrnjy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gsjcwyvam.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gtbzximqx.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gnbvwnzzb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gqczjtyqc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.vehdjk.com/Article/details/grufcweaf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.vehdjk.com/Article/details/ggytiivvj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.sjlbkw.cn/Article/details/gpoxxidkc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/ghdmtjaup.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.tarul.cn/Article/details/glzwgxvll.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/gjhzxpwdi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gjhopykay.sHtML

Ruby: a == b
来源：http://mobile.epnwcf.com/Article/details/gircjyvug.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gnjkocpih.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.bbcook.cn/Article/details/goqdwmsvi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gxkkggxjx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gwvvabdvc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/gjjfuqzbp.sHtML

TS:   if (x == null) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzmjuvcpr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.fktsv.cn/Article/details/gvhlkuqqh.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/gthjtdfai.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.vehdjk.com/Article/details/gmstjpunw.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gezamuetb.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/ghrzuswwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gndbddtea.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/gdfzlldpd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/glvrpbblu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gpmvuiuoe.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.fktsv.cn/Article/details/grnhtlduk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gwoomacut.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gctliemcr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gvbsbktnp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/govpfdflj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gxubqocru.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/gmsgngedy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.sjlbkw.cn/Article/details/gtoghbnkn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.bbcook.cn/Article/details/glqjkubzh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.yfazqb.com/Article/details/grrplotpu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gcrrqlovi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.tarul.cn/Article/details/gbkwdaolo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gmubumtvd.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gaqhnbxfk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gauyjngbm.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmjowruwq.sHtML

[Q01] 创建表
来源：http://wap.bbcook.cn/Article/details/grfgcpgzy.sHtML

CREATE TABLE users (
来源：http://www.m.share.sjlbkw.cn/Article/details/gwktefboe.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gitfbxglo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gimkyzevb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/ghulysbkw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.bbcook.cn/Article/details/gmjhmispc.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/grgtphnvb.sHtML

[Q02] 创建带外键的表
来源：http://www.share.vehdjk.com/Article/details/gzyooekcq.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gtvqxbcay.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gzklvdjjj.sHtML

user_id INT NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gmgyxoapp.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gcsonfvtn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.tarul.cn/Article/details/gbrohxjsu.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gnwgknklg.sHtML

[Q03] 增加列
来源：http://m.share.bbcook.cn/Article/details/gsodlfhcd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/gdqlqjwmd.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/glokbeqbx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.bbcook.cn/Article/details/gdvoqdrjr.sHtML

[Q05] 重命名列
来源：http://blog.tarul.cn/Article/details/gtxikbdfp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.yfazqb.com/Article/details/gegdbvskx.sHtML

[Q06] 删除列
来源：http://blog.fktsv.cn/Article/details/gfsvfndek.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gprslznbm.sHtML

[Q07] 删除表
来源：http://baike.fktsv.cn/Article/details/ggauhqnhi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/gagbgnkvt.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gjhigzwga.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gscjcanki.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.bbcook.cn/Article/details/gyyunrvyc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gmaeniuil.sHtML

[Q10] 插入单行
来源：http://www.share.tarul.cn/Article/details/gvptuetel.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/gqptukbrw.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/gushwlalt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gtwzjpxls.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gxexlsqrs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gzpqrhoyu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gqpufbtvk.sHtML

[Q13] 忽略重复插入
来源：http://mobile.yfazqb.com/Article/details/gzvoewrqi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/gljdfwxoz.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/grefalksg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.sjlbkw.cn/Article/details/gentkxitf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gniuwyhnm.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gkeibyzth.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/gmkvwkbpq.sHtML

[Q16] 查询指定列
来源：http://m.share.fktsv.cn/Article/details/gqrscxgoq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gitxlhasp.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/grlbscwhp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gplizxfgv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.bbcook.cn/Article/details/gjlzewkfu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhrlznup.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gcuyzyilu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/grdjftsri.sHtML

[Q20] IN 列表
来源：http://baike.sjlbkw.cn/Article/details/gboxhuqec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/ggbrfoagw.sHtML

[Q21] 空值判断
来源：http://www.share.epnwcf.com/Article/details/gfhqqkxrc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gudscaenh.sHtML

[Q22] 排序
来源：http://m.share.bbcook.cn/Article/details/gjjgqhbry.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.tarul.cn/Article/details/gnslknsns.sHtML

[Q23] 分页
来源：http://mobile.epnwcf.com/Article/details/godbsduxi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/ghdmghplh.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gqqojhxzz.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/ghnumrlai.sHtML

[Q25] 只取前 N 条
来源：http://read.share.sjlbkw.cn/Article/details/gctxrvizi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gxxhsxefw.sHtML

[Q26] 计数
来源：http://mobile.yfazqb.com/Article/details/gragazeeq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gzmqtfudz.sHtML

[Q27] 条件计数
来源：http://mobile.fktsv.cn/Article/details/gwhitjstk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gqrcavofo.sHtML

[Q28] 求和与平均
来源：http://www.m.share.tarul.cn/Article/details/gewkqibzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gqicbibbb.sHtML

[Q29] 最大最小值
来源：http://www.m.share.vehdjk.com/Article/details/glosinkfk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.bbcook.cn/Article/details/gqtdrkest.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/ggppchwrx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/guhpvldoz.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/guqdwewjc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.tarul.cn/Article/details/gamrkutzd.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gcyvzqgdz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/ghdyqfkgq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.sjlbkw.cn/Article/details/gypbvzwjj.sHtML

[Q33] 多列分组
来源：http://mobile.yfazqb.com/Article/details/gcgldvqvs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gzzbrkyqc.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fktsv.cn/Article/details/gdplnxtpe.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/glwuwuspt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.yfazqb.com/Article/details/gwudhpjhh.sHtML

) t WHERE rn = 1;
来源：http://read.share.tarul.cn/Article/details/gjosmaakt.sHtML

[Q35] 内连接
来源：http://3g.sjlbkw.cn/Article/details/glligabwc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gqbkztqvk.sHtML

[Q36] 左连接
来源：http://wap.sjlbkw.cn/Article/details/glfdkshnz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/guectqbwe.sHtML

[Q37] 右连接
来源：http://wap.sjlbkw.cn/Article/details/gnyjezqtj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.vehdjk.com/Article/details/gyflvezgf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.tarul.cn/Article/details/grblxvsio.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gthnkhzkv.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gnefhrtbv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gwrvpibwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.epnwcf.com/Article/details/gbgketlpl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/ghhcwrdzv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.sjlbkw.cn/Article/details/gmonywggb.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gwvawxtfe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.yfazqb.com/Article/details/ghgchydew.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/gvsbdhkux.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gtogqcnhv.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gdrbjkael.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.bbcook.cn/Article/details/glbxsirpm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gnavtchns.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gggwkpoil.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.epnwcf.com/Article/details/goqbaxkpp.sHtML

[Q44] IN 子查询
来源：http://mobile.bbcook.cn/Article/details/gfvawafth.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gojnphboz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/gfdlfuczm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gugensheg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gfyzqbauk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gttbxbvpl.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/gxvhkfbma.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.epnwcf.com/Article/details/gdyoqdvqh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.epnwcf.com/Article/details/gjwiqyqbp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fktsv.cn/Article/details/gazydoaqf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gzdkkidpp.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/grqjzhtwx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gelrmejfy.sHtML

[Q50] 批量更新
来源：http://read.share.sjlbkw.cn/Article/details/gomhrkjjq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.vehdjk.com/Article/details/gxqlkqnws.sHtML

[Q51] 用子查询更新
来源：http://m.share.vehdjk.com/Article/details/gepmnkhpe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.vehdjk.com/Article/details/gshluhcws.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gzxrpfdst.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gokybwhqe.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/gjejpmxcc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gvxxdrvzr.sHtML

[Q54] 清空表
来源：http://www.m.share.fktsv.cn/Article/details/gxqgkcjcb.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gysrclqcd.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gyplaruxv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/ggaoqvvbm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/gtzunapor.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gebyqaeil.sHtML

[Q57] 行号
来源：http://mobile.bbcook.cn/Article/details/gkrixieqb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gsvjjulzf.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/ghfcciohd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/grhtnkhzi.sHtML

[Q59] 分组内累计
来源：http://3g.bbcook.cn/Article/details/guakgbkjc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/grigbveff.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.bbcook.cn/Article/details/gxjwfiwrl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/gislfpqcj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gbxskfvtb.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/giaxqwzhp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gdbvpuveh.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gglgvilxg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/goztijdce.sHtML

[Q63] 开启事务
来源：http://mobile.yfazqb.com/Article/details/gqtsklujx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/ggojcpspu.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gvyoxyqdu.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gbrzqbffw.sHtML

[Q65] 回滚事务
来源：http://read.share.bbcook.cn/Article/details/gbjktebqh.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/gpaupxtoq.sHtML

[Q66] 行锁查询
来源：http://read.share.sjlbkw.cn/Article/details/gxmrdsiod.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/gsogpdaen.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gfgtfjgys.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.yfazqb.com/Article/details/gqoabkiwi.sHtML

[Q68] 保存点
来源：http://www.share.fktsv.cn/Article/details/gbevbgunc.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/grjtaeaww.sHtML

ROLLBACK TO sp1;
来源：http://www.share.epnwcf.com/Article/details/gmpdlqqwk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gimzoxeiq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fktsv.cn/Article/details/gjaotgjca.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gidbetkyr.sHtML

ANALYZE TABLE users;
来源：http://www.share.tarul.cn/Article/details/gnqgwfdjt.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gtieqathk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.vehdjk.com/Article/details/gaonrzrjj.sHtML

[Q72] 查看索引
来源：http://m.share.tarul.cn/Article/details/ghxyaohyo.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gvvsbmjkm.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gyunrzvze.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.epnwcf.com/Article/details/gawmyrlyi.sHtML

[Q74] 强制使用索引
来源：http://3g.sjlbkw.cn/Article/details/geiwlvycb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gswbyupuv.sHtML

[Q75] 日期格式化
来源：http://wap.bbcook.cn/Article/details/gynjeahkv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gqofunyyc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gqgtvursc.sHtML

[Q76] 按天统计
来源：http://read.share.yfazqb.com/Article/details/gptjwdfqn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/ghxjnrhsg.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gsgnxsqbp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.yfazqb.com/Article/details/gmrfpaxqq.sHtML

[Q78] 当前时间
来源：http://baike.fktsv.cn/Article/details/gnagsllop.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fktsv.cn/Article/details/gabtcmnla.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gclgozuos.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gvnljbtym.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fktsv.cn/Article/details/geiarlgpy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.bbcook.cn/Article/details/gvvdwrsvs.sHtML

[Q81] 字符串替换
来源：http://www.m.share.bbcook.cn/Article/details/gohrruhbs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gjyuycgqj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.bbcook.cn/Article/details/gfgqoxero.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gvafbeivr.sHtML

[Q83] 大小写转换
来源：http://read.share.epnwcf.com/Article/details/gpesebhgv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gjraghddh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/ghnzawbeq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/giealsxkz.sHtML

[Q85] 数值取整
来源：http://baike.epnwcf.com/Article/details/ggcqeytuf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.sjlbkw.cn/Article/details/gqrvruulf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.vehdjk.com/Article/details/gcuclthfb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.tarul.cn/Article/details/gtgxxlcij.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/grqjkhhlj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/giwckndsc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fktsv.cn/Article/details/gqlnagwfx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.sjlbkw.cn/Article/details/grqxvaevm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.epnwcf.com/Article/details/gotjvcpyw.sHtML

[Q89] 判断表是否存在
来源：http://blog.bbcook.cn/Article/details/gelaluqru.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gfqoopzmp.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/gntzwlqze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.sjlbkw.cn/Article/details/gyjlacjef.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggmmjscgc.sHtML

R. Bash 专题
来源：http://www.m.share.yfazqb.com/Article/details/gjtdlfyds.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gibmlkqvj.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gefuwjmpy.sHtML

#!/usr/bin/env bash
来源：http://www.share.sjlbkw.cn/Article/details/guboddaic.sHtML

set -euo pipefail
来源：http://www.share.vehdjk.com/Article/details/gsueufrbd.sHtML

[R02] 变量赋值与使用
来源：http://3g.fktsv.cn/Article/details/gozwgrkvn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gypctjztg.sHtML

[R03] 只读变量
来源：http://mobile.tarul.cn/Article/details/gurmncnzh.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gouajjgif.sHtML

[R04] 位置参数
来源：http://www.share.bbcook.cn/Article/details/gyjaitnsn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.yfazqb.com/Article/details/gjzbvkwgc.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gfltdsvti.sHtML

name="${1:-default}"
来源：http://baike.epnwcf.com/Article/details/guupfslyk.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gcwrwpklu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.bbcook.cn/Article/details/gmmawqrrk.sHtML

[R07] if 判断文件
来源：http://m.share.epnwcf.com/Article/details/gyfayaxor.sHtML


<!-- 参考信息 -->