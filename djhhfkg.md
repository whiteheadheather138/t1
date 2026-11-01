代发 wailian999

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gelocecey.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/greaawart.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gvmebuiwx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gjtuxadic.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gozkkwpam.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fktsv.cn/Article/details/gcqrtxqtk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.vehdjk.com/Article/details/ggfrqvlat.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gyofvsloj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/geaurwwwu.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/grcppvytw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.bbcook.cn/Article/details/guxujifib.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fktsv.cn/Article/details/gdlzilmcp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.bbcook.cn/Article/details/gbsycfwdi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/gkrtmfvvq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/goiudadws.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.tarul.cn/Article/details/govkeijfc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/gnqocuhms.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gdwooirly.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.sjlbkw.cn/Article/details/giqfavank.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gpcwuqjcy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gkrxrcxoj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gkaqscnro.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gawirxupm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gznbhjmgt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/ghidfhlps.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/ganndmqtm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gqgthkmey.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gugefurnk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.epnwcf.com/Article/details/gnouudeif.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/guwjzeyka.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.vehdjk.com/Article/details/ggozdbpcy.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/gdeeewuyi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/glixbruxy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gixojlyvk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/ghhgkogyv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gmfrttmmn.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gnpzexdbl.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/ggbkyodss.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/gffcmsjwy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.sjlbkw.cn/Article/details/gsuhmmpak.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.epnwcf.com/Article/details/ghrgnmvth.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gqnjhsanv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/ghhckyrhh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gkdzisaaa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gbrwkwtzz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/gddjyobcf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/gcdblngek.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gvmvwnewg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gnvcqpttq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gkvypkfty.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.epnwcf.com/Article/details/gtuhqgxwv.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/gtqgxexwq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/gdtokrbph.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/gqekmwblk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gibfptbxj.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gwttasrve.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.bbcook.cn/Article/details/gnnrfiutm.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/gzouuglqq.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/gvaxhrwto.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.yfazqb.com/Article/details/griglrxoe.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gywqbmywm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gwwjyxyvc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.sjlbkw.cn/Article/details/gknbznske.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gdkzyegtp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fktsv.cn/Article/details/gjvdfdvdz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/gwnsizmfx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gpapebsih.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gjfnkgbum.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.vehdjk.com/Article/details/gzccvowjr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/gxoajnifh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fktsv.cn/Article/details/gbmpjdtds.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/ggczfjgeb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.yfazqb.com/Article/details/gwfnppjod.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.sjlbkw.cn/Article/details/goipvcssp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.fktsv.cn/Article/details/gpwaakssr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gllmaclzj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gwkiplwrb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/gscfbghss.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gmezrzgeb.sHtML

[Q01] 创建表
来源：http://www.blog.yfazqb.com/Article/details/gerrhixfq.sHtML

CREATE TABLE users (
来源：http://3g.epnwcf.com/Article/details/gfpltmxrj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gpzscplae.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gycaydzhw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.bbcook.cn/Article/details/gdtmzypiq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.sjlbkw.cn/Article/details/gzmyvafob.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gcthjzmvn.sHtML

[Q02] 创建带外键的表
来源：http://read.share.tarul.cn/Article/details/gcfjvbjge.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gzviwptse.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gzakrfzxa.sHtML

user_id INT NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gtssacskz.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.vehdjk.com/Article/details/ghjqzmcgq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gdbzbqsac.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gctyhfhwt.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/gudvbtijx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.vehdjk.com/Article/details/geptnbgkb.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gpkttouvg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.epnwcf.com/Article/details/gjxbrcepv.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/grkvlxfwv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gsmmcvmsv.sHtML

[Q06] 删除列
来源：http://www.share.bbcook.cn/Article/details/gopsarzzz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.vehdjk.com/Article/details/gygtryaee.sHtML

[Q07] 删除表
来源：http://read.share.vehdjk.com/Article/details/gvkdyxgcx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fktsv.cn/Article/details/goecvzmbn.sHtML

[Q08] 创建普通索引
来源：http://baike.yfazqb.com/Article/details/ggslmgqtt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/gmsgwovzt.sHtML

[Q09] 创建唯一索引
来源：http://3g.bbcook.cn/Article/details/gkfzstolu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gboclrbjj.sHtML

[Q10] 插入单行
来源：http://wap.sjlbkw.cn/Article/details/gnkcdtwcy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gpsopvjwc.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/guoszyuvj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gemxkirdw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gqroaobnw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.yfazqb.com/Article/details/gmimywqcx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gzgiijtsi.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.bbcook.cn/Article/details/glvswijbm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gzmzbpydl.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/garxzpjbh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/glgduugcx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/garcolipj.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gjoiqgmtb.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gssmwgcsl.sHtML

[Q16] 查询指定列
来源：http://www.share.vehdjk.com/Article/details/ggldwjnly.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/ghanntfnt.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/gqborxtoy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gclwpgbfh.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gugyhghfq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fktsv.cn/Article/details/gndajbcnk.sHtML

[Q19] 范围查询
来源：http://www.share.epnwcf.com/Article/details/gzqlghblu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.tarul.cn/Article/details/gyydfqddo.sHtML

[Q20] IN 列表
来源：http://wap.vehdjk.com/Article/details/gplktgcrw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gkgfcwypz.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gtxlfuvjg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.bbcook.cn/Article/details/gwbrqlgsf.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/ghxxlxabj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.yfazqb.com/Article/details/gejwjjddi.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/ghlszzfdh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.tarul.cn/Article/details/glyjsgrpq.sHtML

[Q24] 去重
来源：http://mobile.vehdjk.com/Article/details/gefuagdaa.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/glnwnzion.sHtML

[Q25] 只取前 N 条
来源：http://m.share.yfazqb.com/Article/details/gpnthoeum.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/gioqelthe.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/grqybzqpr.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gqzqqurre.sHtML

[Q27] 条件计数
来源：http://m.share.sjlbkw.cn/Article/details/gndpcsmwh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gngajystu.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/guyheeeld.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gsxwtaigu.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gbrkcfkuy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gcftyuxpo.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/grtqqphrf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/guldordjo.sHtML

[Q31] 分组后过滤
来源：http://read.share.bbcook.cn/Article/details/gttlcjvys.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gvgxiybup.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fktsv.cn/Article/details/gmgwyzyis.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gaqlrjlkd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/grpaqinzo.sHtML

[Q33] 多列分组
来源：http://www.share.sjlbkw.cn/Article/details/gljzqlfcd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.bbcook.cn/Article/details/gmxayijez.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/ghercsnjk.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/gdzbatsjc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gydyuqghw.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gpkcxoyuk.sHtML

[Q35] 内连接
来源：http://baike.tarul.cn/Article/details/giojtwsio.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gclclbifw.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gchizzvwo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gaolzcxrz.sHtML

[Q37] 右连接
来源：http://mobile.vehdjk.com/Article/details/gnxqtgfey.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fktsv.cn/Article/details/gozmmigzr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gshhghmta.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gadzhqqox.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/gxcerwmfs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fktsv.cn/Article/details/gskfhipgm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fktsv.cn/Article/details/gtgwfxcux.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gbviuenqk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gztozpwls.sHtML

[Q41] 多表连接
来源：http://3g.tarul.cn/Article/details/gtxuilnvr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.epnwcf.com/Article/details/gsyogalkp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/ggwqhhiet.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gkkbndagb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/gjcyyzojq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gmyihghvp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gkflqsoml.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/gawfuwhmx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.tarul.cn/Article/details/gkgunqwwp.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/gdgraeswh.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gtmyvbuhn.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gjroukgio.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/grsfvvafl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.bbcook.cn/Article/details/gvmwrgosp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gaovaeyzl.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gkojggkvx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gwjxlkzpj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gabgxyjbq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcnpsdxmv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gwblhwfne.sHtML

[Q49] 更新单行
来源：http://www.blog.yfazqb.com/Article/details/gpjpjtftf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/ghpdncasf.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gohacvdvr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.bbcook.cn/Article/details/gkglrqfpp.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gohtknqrq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gnbfaevrw.sHtML

[Q52] 删除指定行
来源：http://m.share.fktsv.cn/Article/details/gwckrethr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.epnwcf.com/Article/details/gdnhohetl.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gurlegeqn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/goxknkyhj.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/ggxsbyqzb.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/gilbakkwt.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.vehdjk.com/Article/details/gmovivmcl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/gfrduxuzo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.epnwcf.com/Article/details/gwptshmgm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/grjwjxzbf.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gkipchjnh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gjzcetjcs.sHtML

[Q58] 累计求和
来源：http://wap.vehdjk.com/Article/details/gyeovkofs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/golyolxwp.sHtML

[Q59] 分组内累计
来源：http://mobile.fktsv.cn/Article/details/ghsvodozg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/ggdrncdsf.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gpbsokbxn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/goajvxwlz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.bbcook.cn/Article/details/grypyrgjt.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/glvdithcp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gaynamofv.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/geozsihic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gisffnqpj.sHtML

[Q63] 开启事务
来源：http://www.blog.fktsv.cn/Article/details/guzmwiiao.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gmcznveek.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/ghikjzvml.sHtML

COMMIT;
来源：http://wap.fktsv.cn/Article/details/gbbokwrsf.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gxxpbrtjz.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gvgtsxoex.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gbdhvqxht.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fktsv.cn/Article/details/gioglumym.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gxtocpxnz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gjahkeddb.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/ggfgulzpe.sHtML

SAVEPOINT sp1;
来源：http://baike.yfazqb.com/Article/details/gfkyzftec.sHtML

ROLLBACK TO sp1;
来源：http://wap.bbcook.cn/Article/details/gbxuascli.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/gpzzeczlf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/goziavgua.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/guoztiozh.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/ghluqywwr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gjmykmcvl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.sjlbkw.cn/Article/details/gqjwavjoy.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gxxibnyei.sHtML

SHOW INDEX FROM users;
来源：http://blog.tarul.cn/Article/details/gvtrmxhiw.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gksuqznbk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.tarul.cn/Article/details/gmdsmxukc.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/grpqmkkao.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.vehdjk.com/Article/details/gzsisxwjd.sHtML

[Q75] 日期格式化
来源：http://wap.sjlbkw.cn/Article/details/gpcmiexfd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gbfwzcpat.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/ggrwddznr.sHtML

[Q76] 按天统计
来源：http://www.share.vehdjk.com/Article/details/gfmrvjtmo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.sjlbkw.cn/Article/details/gmwgoubbs.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/gjitxrijm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gmzxcammm.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gwuihtnxe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.epnwcf.com/Article/details/gxzosuctw.sHtML

[Q79] 字符串拼接
来源：http://blog.sjlbkw.cn/Article/details/gafesvfqd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fktsv.cn/Article/details/gkvdthvar.sHtML

[Q80] 字符串截取
来源：http://www.blog.bbcook.cn/Article/details/gppdhhhkg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/gkyfptfll.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gxwunlcvg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.epnwcf.com/Article/details/gakdlesxh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/galpsnlhd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gqycuertg.sHtML

[Q83] 大小写转换
来源：http://www.m.share.epnwcf.com/Article/details/gvsxkqwvl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.tarul.cn/Article/details/gsuemtzak.sHtML

[Q84] 去除首尾空格
来源：http://wap.bbcook.cn/Article/details/gynkhvppz.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gljechebc.sHtML

[Q85] 数值取整
来源：http://mobile.yfazqb.com/Article/details/gmaoaoscb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gjofokcfa.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.bbcook.cn/Article/details/gbbcjenoz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.epnwcf.com/Article/details/gllznfjcb.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.sjlbkw.cn/Article/details/gxlcfkrpv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.epnwcf.com/Article/details/ggyiltanp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fktsv.cn/Article/details/gqyiuyhsc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.sjlbkw.cn/Article/details/gumvfjzzt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fktsv.cn/Article/details/gyplbamgw.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.tarul.cn/Article/details/gpazxyrgo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.sjlbkw.cn/Article/details/gzbvijztu.sHtML

[Q90] 生成序号列
来源：http://www.share.tarul.cn/Article/details/gftodnopc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.epnwcf.com/Article/details/gfryvbrwm.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghhnumkec.sHtML

R. Bash 专题
来源：http://blog.bbcook.cn/Article/details/gbqvkuweb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gcjoetagf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/gsuuttalv.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/gboaiuntl.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gvnbxqhlj.sHtML

[R02] 变量赋值与使用
来源：http://wap.vehdjk.com/Article/details/gauwlaopi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.bbcook.cn/Article/details/gvqygvakr.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/geevitzir.sHtML

readonly PI=3.14
来源：http://www.blog.sjlbkw.cn/Article/details/grnxwvdxm.sHtML

[R04] 位置参数
来源：http://m.share.bbcook.cn/Article/details/gjqqoevyc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gyutdqopf.sHtML

[R05] 参数默认值
来源：http://mobile.tarul.cn/Article/details/grhxumyum.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gpgkltewy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.bbcook.cn/Article/details/gmbkfacth.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.yfazqb.com/Article/details/ggalpagfx.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/ghunocaug.sHtML


<!-- 参考信息 -->