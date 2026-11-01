代发 wailian999

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gdikrgrha.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gohwffeom.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/gihhpkvet.sHtML

Ruby: // fork 块
来源：http://m.share.epnwcf.com/Article/details/gvmxizukm.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gifpaxgzb.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gugarxxcs.sHtML

P. 常用工具函数
来源：http://mobile.yfazqb.com/Article/details/gkogtsmld.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gdsuiyyej.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/ghuuxiyqc.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gxprlkiva.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/glnqspntb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gpznhhdgx.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gypwwefvt.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gbwyqwgcn.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gdqqisyhr.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/guifnokjw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/glpodwdkn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.vehdjk.com/Article/details/gpbdiznzl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gietkbhih.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fktsv.cn/Article/details/gutgghmfe.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gqwtxqnvi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gsebwjual.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gdftohosm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gwjghrtat.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkcmoanwn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.epnwcf.com/Article/details/gpegzemmv.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gpsjrijjl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.yfazqb.com/Article/details/gbktotdmy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/gxpbmvayk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/goiksgitd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/ghmfkmihe.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.epnwcf.com/Article/details/gzoruhqvd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/givpjbenp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gxnxnqyzy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.tarul.cn/Article/details/gmdhbnoyj.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/gkjzjaxeq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gfhzykfrm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gunvawgry.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/gjqgdpmyz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gbuhihbeh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.sjlbkw.cn/Article/details/gbsygitin.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gesuqwzuw.sHtML

Ruby: x.length;  x.size
来源：http://www.share.bbcook.cn/Article/details/galjsiean.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/ghqbwuziu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.fktsv.cn/Article/details/gueobjydw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gtmxdafrr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.sjlbkw.cn/Article/details/ggllsbbxo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gbofdpogf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gvatucwzo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/geasgkwdg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/gbmpphutc.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gpwyzespv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.epnwcf.com/Article/details/ghioqnpez.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/glipayfxr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gcksavpza.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gkvidyzzu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fktsv.cn/Article/details/gmqfwjruo.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gkwiprkch.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.yfazqb.com/Article/details/guvwlelof.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gkmclntoy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gxfrwvgru.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/govgybfkb.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/gdjvcdizn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.epnwcf.com/Article/details/grlnpfynt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gjbtnyxgw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gojmtvrjy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gizcgmqcj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.epnwcf.com/Article/details/gvblqgkgp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/glfuonvta.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/ggmievazi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.sjlbkw.cn/Article/details/glozfnwub.sHtML

[P08] 处理浮点精度问题
来源：http://wap.yfazqb.com/Article/details/gqdoziuuu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.tarul.cn/Article/details/gharwetne.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.bbcook.cn/Article/details/gejfvyzca.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.yfazqb.com/Article/details/giuelovhy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.yfazqb.com/Article/details/glvfhvojj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gvzajtvrc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gdnkznqgb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/gaajxldkd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/ggieivzta.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gppmanllj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.vehdjk.com/Article/details/grogvmjqk.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/goxthyjzg.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/gxkwafpiw.sHtML

CREATE TABLE users (
来源：http://www.m.share.epnwcf.com/Article/details/gmokuzymb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gzabptgea.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gegmgztez.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gnyvlcptg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gydrzodkq.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gquuqghtm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gafmhxrdw.sHtML

CREATE TABLE orders (
来源：http://read.share.fktsv.cn/Article/details/gwvzksnge.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/grkspwkhh.sHtML

user_id INT NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gcgjhcoqr.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gmqbzgfat.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/gooixmdct.sHtML

);
来源：http://wap.tarul.cn/Article/details/gzsvwmrcn.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/glzhmshdk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gdletuzgu.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gyelaxoha.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/grmmhbtyh.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gxkrfcawe.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.epnwcf.com/Article/details/gkdrszyie.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/ghakjtoxs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gruulrjid.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/ghneodnej.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gqbepmgsm.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/gmrotdbbn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gjwemfsdp.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/ghvlmazya.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gthanuxrg.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gnymoihlj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gooudhosf.sHtML

[Q11] 一次插入多行
来源：http://baike.tarul.cn/Article/details/geicrxtza.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.vehdjk.com/Article/details/gogadnrpd.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.yfazqb.com/Article/details/geyaatgwv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gvsqhospl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gvpasrkjb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.yfazqb.com/Article/details/gbkrqwaqz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gkqfrdfwe.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/gvxdjwcup.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fktsv.cn/Article/details/gszswkivi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.vehdjk.com/Article/details/gvjgbhbjn.sHtML

[Q15] 查询全部
来源：http://www.blog.bbcook.cn/Article/details/ghstakbrr.sHtML

SELECT * FROM users;
来源：http://3g.yfazqb.com/Article/details/grrwplqjq.sHtML

[Q16] 查询指定列
来源：http://wap.tarul.cn/Article/details/ggktfdvte.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/guvfmxjsa.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/grmebhfgg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/ghuwykfbq.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/gwkvuxjeb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.tarul.cn/Article/details/gdcbegnma.sHtML

[Q19] 范围查询
来源：http://wap.sjlbkw.cn/Article/details/gtunbtafo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fktsv.cn/Article/details/gekjozahs.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gompyipev.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/giavhbpug.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/giwbatsht.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/grcxhliqw.sHtML

[Q22] 排序
来源：http://blog.fktsv.cn/Article/details/gvfeakzsw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.yfazqb.com/Article/details/gvgwlvdvn.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gmfmtuftl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.bbcook.cn/Article/details/gjzxyhres.sHtML

[Q24] 去重
来源：http://www.share.tarul.cn/Article/details/gyrjfhzkq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gkxjtzuji.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/glkvolqku.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/glswwitcy.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/guodtlkpp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gsrwpetny.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gmjkapkaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.epnwcf.com/Article/details/gfhkkjxao.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gltwfpuki.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gcwmflzbu.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gcftrttxv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gmqvmaixz.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/gydxwhyji.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gfwkxseyb.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gsamyrxab.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gxlfznbcp.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gveboxkwn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gxhmhmazk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/glwusfhxp.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gfwscicrq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/gtylqtxjm.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gbsdeljmq.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gpisxcbdu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gexvenusn.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/grpruciff.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gmkpialwh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gvtujjmsd.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/giczmjyap.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gqfyvucoa.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gjswcnsyo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/ggypnquzp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gcvgtasam.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/gxlzkksoi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.tarul.cn/Article/details/gezzsjxrw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gewuojuyr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/gvujnhkaz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghrliovha.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/ggmfyzxux.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gokikewyz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/gxkotcwni.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/goozmpmha.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.yfazqb.com/Article/details/gtczycspa.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gmalxcxjr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gmbkcpdor.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gfkxyrrge.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/glrvuplqe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gfsejwxve.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gdxxipvxp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gtgiigfmb.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gaairshrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gdqzwymgs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/gqojobrad.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gercljtcb.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gulwjysra.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fktsv.cn/Article/details/gwmeqxocu.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gwfjlrvbo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fktsv.cn/Article/details/glibvcjat.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gvxxmxpuq.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gjjdyoujg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/grzdqqzxx.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gytgdyicq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.bbcook.cn/Article/details/gwvjvrczm.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/goqqszahs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.bbcook.cn/Article/details/gxanlzjgl.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gjqjondqq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gippvbtfj.sHtML

[Q53] 按条件删除
来源：http://www.blog.tarul.cn/Article/details/gnwppacio.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gqftydwau.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/givdezdwm.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/goyydzwrg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/gpjirrysr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gtnmymvbw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.yfazqb.com/Article/details/guaiaxwci.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.vehdjk.com/Article/details/grchakhrb.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/gktbnwhfe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gswamksmc.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gvyajsfze.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gckjvxezw.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/ggamabuwe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gixypukdr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.tarul.cn/Article/details/gklkfzhrr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gajmfilmo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/glkhmvkri.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfxrcisc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gzogpxitg.sHtML

[Q62] 分组占比
来源：http://baike.yfazqb.com/Article/details/gplttaqpy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/guffhpmnc.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gplsqwduj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gnyjwdffj.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gcbhhzjql.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gtgbomqds.sHtML

[Q65] 回滚事务
来源：http://wap.bbcook.cn/Article/details/gbvjmdvbh.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gvflyvlxi.sHtML

[Q66] 行锁查询
来源：http://wap.fktsv.cn/Article/details/gqpnxxzfd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/gpakuvibf.sHtML

[Q67] 设置隔离级别
来源：http://mobile.tarul.cn/Article/details/gdxnqdejs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gzlibbbbv.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gsytfzqsm.sHtML

SAVEPOINT sp1;
来源：http://wap.bbcook.cn/Article/details/gnugjqvcb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.bbcook.cn/Article/details/gjislapli.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gmolhxxdy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.yfazqb.com/Article/details/gcpxliyvq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fktsv.cn/Article/details/gvrxilvrj.sHtML

ANALYZE TABLE users;
来源：http://baike.fktsv.cn/Article/details/gcxfizwzg.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gpxvoydqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.epnwcf.com/Article/details/ghechekmx.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gmgdzjtdl.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gcnefwbpd.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gztushdrx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gkyrmpuqx.sHtML

[Q74] 强制使用索引
来源：http://baike.vehdjk.com/Article/details/gvhnpbpam.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/ganfuuokg.sHtML

[Q75] 日期格式化
来源：http://3g.fktsv.cn/Article/details/ggaqfvgwm.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.epnwcf.com/Article/details/geadahyzw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.tarul.cn/Article/details/gcfqjpcay.sHtML

[Q76] 按天统计
来源：http://baike.vehdjk.com/Article/details/gngjyjrps.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gupwefieu.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gdtamsjqa.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gfutkistf.sHtML

[Q78] 当前时间
来源：http://wap.epnwcf.com/Article/details/grzyhvsxh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.yfazqb.com/Article/details/gjukgxqbx.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gjqvfgnwg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.bbcook.cn/Article/details/gzkpgyvaq.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/ghzujouer.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.bbcook.cn/Article/details/glzdaxkax.sHtML

[Q81] 字符串替换
来源：http://3g.vehdjk.com/Article/details/gofgyxtmi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gwdqnjdli.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.vehdjk.com/Article/details/grmryhkpb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gzgopzbrc.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/grypmnwai.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.bbcook.cn/Article/details/gphmvqeql.sHtML

[Q84] 去除首尾空格
来源：http://read.share.vehdjk.com/Article/details/goftrxhri.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gpifanotj.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gmhxbbuyo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.tarul.cn/Article/details/gzkoepjxt.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.bbcook.cn/Article/details/gfwvsowpg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gokkryums.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.bbcook.cn/Article/details/gutggbtrc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gtlldznit.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.vehdjk.com/Article/details/gnyotskmc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gzyhoqjhq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.vehdjk.com/Article/details/gccanlqcz.sHtML

[Q89] 判断表是否存在
来源：http://mobile.tarul.cn/Article/details/gfblzrttu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.epnwcf.com/Article/details/goylsvvzt.sHtML

[Q90] 生成序号列
来源：http://blog.yfazqb.com/Article/details/gfwvhkpve.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.epnwcf.com/Article/details/gemwgnhau.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/glihoecos.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gdedcmqan.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdtffnopl.sHtML

[R01] shebang 与严格模式
来源：http://wap.fktsv.cn/Article/details/gdspnxwzm.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gpbwhtcvd.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gkhcxpdtt.sHtML

[R02] 变量赋值与使用
来源：http://baike.epnwcf.com/Article/details/gsqoldymg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.vehdjk.com/Article/details/gxyloqkiq.sHtML

[R03] 只读变量
来源：http://wap.epnwcf.com/Article/details/gprzblvrb.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/gxrfnmwid.sHtML

[R04] 位置参数
来源：http://www.share.yfazqb.com/Article/details/gqpsbraxi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gyfyrqznz.sHtML

[R05] 参数默认值
来源：http://blog.vehdjk.com/Article/details/gicbyulxr.sHtML


<!-- 参考信息 -->