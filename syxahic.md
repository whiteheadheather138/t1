代发 wailian999

[O06] 使用进程池
来源：http://m.share.vehdjk.com/Article/details/gqrqnpycr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gyaemwvnu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.yfazqb.com/Article/details/gwatyprje.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gcmyusbtb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gjazjyvvx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/geeahgago.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.yfazqb.com/Article/details/gqvvgjcli.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/gnfkwqdvq.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/ghrwigkyz.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjzwvavrz.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gzehfypnc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gvsqoxlgq.sHtML

[P01] 生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gkgvcfire.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gjfbdbueu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gczbqzbmh.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/grnuyjpmc.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/ggsepwefx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.sjlbkw.cn/Article/details/giuzcqall.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gbljclvjd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gnniqoefh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.tarul.cn/Article/details/gugyvbcsd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.sjlbkw.cn/Article/details/gxumtlxme.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.epnwcf.com/Article/details/gqnqsvduz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/gdjoiatag.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gbveeuhdr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/ghusvpnjb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/gytprwpxz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/gbfowmcar.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.vehdjk.com/Article/details/gdvwbzcnm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/gvidrtxnd.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gedxeafhf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gxgpaetqw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gfqxfepks.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gwumwtqyo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.sjlbkw.cn/Article/details/gfacjjzvg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.epnwcf.com/Article/details/gkuhiuuac.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.tarul.cn/Article/details/gbhhykzav.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gszgzaiuu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.tarul.cn/Article/details/gaaklzmsp.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gcdoicxeg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gvrxpgljc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.sjlbkw.cn/Article/details/gykkgzknj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gvgdnjexh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gslwfgpnz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/godeshwjo.sHtML

Go:   len(arr);  len(m)
来源：http://3g.sjlbkw.cn/Article/details/gpfnlxqse.sHtML

Ruby: x.length;  x.size
来源：http://3g.tarul.cn/Article/details/gxbzzzobc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gvmgshjzb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gblmymwhv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gzpnzbucj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxyyjxrp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/geoyhksod.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gqyfqnbej.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gyqesugoh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gvynbffhy.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gmxeiebkv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.epnwcf.com/Article/details/gejjhnjqt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.vehdjk.com/Article/details/geoebuqiq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.epnwcf.com/Article/details/ggdgpxptu.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.epnwcf.com/Article/details/getrykteh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gqmdnumov.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gpmpaszwh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/ggvdomyrn.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/gbropgvmo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.yfazqb.com/Article/details/gsdkldzmg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gcirzvnwt.sHtML

[P07] 防抖与节流
来源：http://www.m.share.yfazqb.com/Article/details/gbasflinb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.epnwcf.com/Article/details/gjfyhyeuz.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gmoyktauc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhwxdjzf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gpnoyhuoi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gtiivuxtz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.bbcook.cn/Article/details/gwhmytovq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.epnwcf.com/Article/details/gpquckygb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/gyyvstcnp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gntbqrowr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.bbcook.cn/Article/details/grklfvlyo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fktsv.cn/Article/details/gpjynwaki.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gpgxkoqqw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gxykwfkhc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gltuqklpn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gpfcxrjel.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.sjlbkw.cn/Article/details/gdgcyhkoy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gvssuxgci.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxglrliyi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.epnwcf.com/Article/details/gcymhycfs.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gqxgmeowb.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/gkdafqnyl.sHtML

CREATE TABLE users (
来源：http://mobile.tarul.cn/Article/details/gifotzcxs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gixkppapl.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gddzvcghq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.bbcook.cn/Article/details/gefitgbmt.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/glgacndzn.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gqofbkgzv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gabstvcmc.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/giizifcje.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzklhxcg.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gdicoymat.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/gezpsjfmx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gfjwnojqe.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gusjjsqgc.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gassuuluc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gqxkdchks.sHtML

[Q04] 修改列类型
来源：http://blog.yfazqb.com/Article/details/gjwwnfqvf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.epnwcf.com/Article/details/gzcqbblsc.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/gdrzfufja.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fktsv.cn/Article/details/ghrqiflry.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/gqouokiyq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.sjlbkw.cn/Article/details/gzqcvgthk.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/gitdcetkl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/glbtjmauf.sHtML

[Q08] 创建普通索引
来源：http://blog.sjlbkw.cn/Article/details/gdktujlep.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/grcydnret.sHtML

[Q09] 创建唯一索引
来源：http://baike.bbcook.cn/Article/details/gwuaqxjue.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/grjwdfyjy.sHtML

[Q10] 插入单行
来源：http://blog.tarul.cn/Article/details/glqknpwwh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gtomybvvv.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gyuceyfkq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gtecxiron.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gqoxqzrkg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/gmzcbghtx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/giorhmpqc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/giyijqnmf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gyvlusxck.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gpgdecknk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gkxpwpeqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fktsv.cn/Article/details/gsqisrwgt.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gdzigyilv.sHtML

SELECT * FROM users;
来源：http://mobile.bbcook.cn/Article/details/gbhijjirr.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gtvputxyy.sHtML

SELECT id, name FROM users;
来源：http://mobile.yfazqb.com/Article/details/gzvnvtwja.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gponmbkce.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.yfazqb.com/Article/details/gqchcvptu.sHtML

[Q18] 模糊匹配
来源：http://baike.bbcook.cn/Article/details/gjxoiofzs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gnejkmjbz.sHtML

[Q19] 范围查询
来源：http://wap.epnwcf.com/Article/details/grtvugdvk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.epnwcf.com/Article/details/gsquhzpsj.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gsdmihkit.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.bbcook.cn/Article/details/gwlhzdsyi.sHtML

[Q21] 空值判断
来源：http://mobile.tarul.cn/Article/details/gsiccxduo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gjyjriiyr.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gcoywfzhf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.bbcook.cn/Article/details/gugnzikku.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gdwnxddyq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gdoobhhri.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gvsgktjnr.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gvkluzwrp.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gjqmezsfr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gkiaghawy.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gyqwncrhv.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/grlbopakw.sHtML

[Q27] 条件计数
来源：http://mobile.vehdjk.com/Article/details/gzooprjxl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbbyrquuq.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/geafzdthc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gskcchnho.sHtML

[Q29] 最大最小值
来源：http://wap.sjlbkw.cn/Article/details/gbxhadmgq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.vehdjk.com/Article/details/geknokdqm.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gwvyomols.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gdmgkeyml.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/gpvnsqbee.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/grtqwucjv.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gkjxtgvaq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gdhevyhrj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gsujqlzqu.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gtetpzflv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gjixpybye.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gdhnxjzey.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/ggkbrcjkw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/grsaqkkme.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gknplsucz.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/gqsypgnez.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/gdqtauuqj.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gvpksngjh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gnpttoqti.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/ghejcctuz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gkgjbovcb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.vehdjk.com/Article/details/gdyftqryr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/gvctwuzwe.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.bbcook.cn/Article/details/gpseoyfkh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.sjlbkw.cn/Article/details/gpaaqzhie.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/gotldjcxr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/gufxoehuh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/gcpaqamfw.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/ghhfbdwge.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gubpvmdov.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gcjogacwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fktsv.cn/Article/details/gjjfbudte.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.yfazqb.com/Article/details/gruorlcdg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gkffvbzwb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/gahdxbxbp.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/gfhqltblw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gbpcxpyke.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gcvgheofs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/golnpsemj.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gqeaipxqf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gnvdasjgm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/glldupaoj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.epnwcf.com/Article/details/gsfbmgudp.sHtML

[Q47] 与平均值比较
来源：http://baike.yfazqb.com/Article/details/grlklpewp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gqwplfpkg.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gdzahhdpp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gfwtitjxt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.tarul.cn/Article/details/ggmdfswhb.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gpmjsgcul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gaqidubut.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gtfpugkuh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gmzxuxcpg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/gdordcuzx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gcxylylce.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gxeffapgq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/giyyzzmas.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gmhgzyvun.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.sjlbkw.cn/Article/details/gtztihpcd.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gpwfknhxc.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/ggfdxjhzp.sHtML

[Q55] 排名（并列占位）
来源：http://wap.yfazqb.com/Article/details/glgarajng.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/glipnykbb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvdfwuqg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.vehdjk.com/Article/details/gnihegtfw.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gpoceyzuq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/guqubgaqs.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gdoyuyvkn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gseqsdvsw.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gwbsmuaml.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gfxbvszjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fktsv.cn/Article/details/gpvlofthn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gtktgqsqs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.epnwcf.com/Article/details/gvyqwokvo.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gjtudxvna.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.tarul.cn/Article/details/guanhbeow.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gsfzwtbxw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gmmcbqofp.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/ghwqvqzom.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/guugwpyqm.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gfbmfqbdg.sHtML

COMMIT;
来源：http://mobile.tarul.cn/Article/details/gtnicygau.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/guwqcsbmb.sHtML

ROLLBACK;
来源：http://www.blog.epnwcf.com/Article/details/gqlcltelp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.vehdjk.com/Article/details/gndhcxsnq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.vehdjk.com/Article/details/gqycnqqou.sHtML

[Q67] 设置隔离级别
来源：http://3g.sjlbkw.cn/Article/details/gyuleuerh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gvcdscpzv.sHtML

[Q68] 保存点
来源：http://baike.fktsv.cn/Article/details/gvhqtgdoq.sHtML

SAVEPOINT sp1;
来源：http://m.share.yfazqb.com/Article/details/gxuceujat.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gqbtceoma.sHtML

[Q69] 查看执行计划
来源：http://read.share.fktsv.cn/Article/details/gvgapujjh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/gcvjkklrs.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gywfsimoa.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gnutrnpqy.sHtML

[Q71] 查看建表语句
来源：http://baike.tarul.cn/Article/details/gpysfflqq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.bbcook.cn/Article/details/gfxmimnca.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/ggfbgsnrh.sHtML

SHOW INDEX FROM users;
来源：http://www.share.yfazqb.com/Article/details/gstqjulbf.sHtML

[Q73] 查看表状态
来源：http://mobile.vehdjk.com/Article/details/gpzpkuoqw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gbotkxnbi.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/geimdulia.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.bbcook.cn/Article/details/geawogikd.sHtML

[Q75] 日期格式化
来源：http://wap.tarul.cn/Article/details/grzkdkwqh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/giyzsuieb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.tarul.cn/Article/details/gyztwrnag.sHtML

[Q76] 按天统计
来源：http://mobile.tarul.cn/Article/details/geqrzosdq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/gwkityvug.sHtML

[Q77] 时间加减
来源：http://3g.fktsv.cn/Article/details/ggwnenzuv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gojblgbwv.sHtML

[Q78] 当前时间
来源：http://read.share.vehdjk.com/Article/details/gpwvppzwx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gswljueyw.sHtML

[Q79] 字符串拼接
来源：http://www.share.tarul.cn/Article/details/gyrusypuv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gzaqcdwfm.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfuoymwp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghuwqhlgi.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gxhpfgkmc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.vehdjk.com/Article/details/gimkvhnee.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gsqklodim.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gwgtgyixg.sHtML

[Q83] 大小写转换
来源：http://baike.bbcook.cn/Article/details/gwlfjrrss.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.bbcook.cn/Article/details/gnkzcmfnw.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.epnwcf.com/Article/details/gfojfljun.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gglqdfdkm.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gtxijfqkn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fktsv.cn/Article/details/glkzwwnup.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fktsv.cn/Article/details/ggbssubyt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.epnwcf.com/Article/details/ggrpstzbf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gctweeexb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.epnwcf.com/Article/details/gvitzdeus.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fktsv.cn/Article/details/gqwdgauts.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.bbcook.cn/Article/details/gkouldnvl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gubfqmyzu.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/gmktrdxuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/grogacjea.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/gswpbflbu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.vehdjk.com/Article/details/gegzwissv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gocedgzuy.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gpmnianpp.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gumawmfsx.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.yfazqb.com/Article/details/gdqboazeu.sHtML

#!/usr/bin/env bash
来源：http://3g.sjlbkw.cn/Article/details/gyixnpewd.sHtML

set -euo pipefail
来源：http://www.m.share.fktsv.cn/Article/details/gwgpeusaa.sHtML

[R02] 变量赋值与使用
来源：http://wap.yfazqb.com/Article/details/gtajkbhwp.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/grqymlumk.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gcgwrosml.sHtML


<!-- 参考信息 -->