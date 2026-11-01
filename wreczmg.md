代发 wailian999

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/glissbojy.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gntembofq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gaircsfrv.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gyncnrvvh.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gnvmgtusx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.vehdjk.com/Article/details/gkmmimftm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/gzbpirpcm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/gsxrgiinj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gsqifmaks.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/glqfjuxlb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gxfmdaxsi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.sjlbkw.cn/Article/details/gesmyhwxp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/ghzgsapqi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.bbcook.cn/Article/details/gyvcarsjh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.sjlbkw.cn/Article/details/goznpjhtd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gfbvavotw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gqjpkyqhd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gkbmcrnjj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gflvhnbhj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gldmvpoxc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gqlkyfntm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gypntiodt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/germkztdv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gigebhvol.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gqdnybssf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/ggfxqgeqs.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gaagdnfol.sHtML

[P04] 求长度
来源：http://blog.bbcook.cn/Article/details/gcgkpqvpm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/goprdnksd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/ggfxsouzw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/gzwiuupki.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gwekdsagp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gafubfwjv.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.yfazqb.com/Article/details/gcqdqrkmp.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gmjccjpkv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.epnwcf.com/Article/details/geuavuyts.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gtmfdadhi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gsygucjlr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gvnkoafzw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.bbcook.cn/Article/details/gobinyotp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gqohtozep.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gsdwfdhwh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/glqmttsqw.sHtML

Ruby: a == b
来源：http://3g.tarul.cn/Article/details/gyialqgas.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gqhslynjx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/ggjhdxzbk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.bbcook.cn/Article/details/gwfwkpbck.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.bbcook.cn/Article/details/gvxybhwhn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fktsv.cn/Article/details/gqewdddif.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gniqvswsf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.yfazqb.com/Article/details/gacmdesfm.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gxnwhftux.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/gdoobaiel.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/guwixzoix.sHtML

[P07] 防抖与节流
来源：http://3g.fktsv.cn/Article/details/grrqfcxyv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fktsv.cn/Article/details/gkuhncipb.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/godgjbmhl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gxqefivyt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gjhoxwrwh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/grupcqpjz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gjoahhsqk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gstgrjcga.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gmrojypcu.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gwmfnkapk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.yfazqb.com/Article/details/gvahmplwh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fktsv.cn/Article/details/gicbgcxus.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.sjlbkw.cn/Article/details/gbtpjydby.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.yfazqb.com/Article/details/gwpgmlbcn.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.epnwcf.com/Article/details/gwmtmlhtl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gslftfqtc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/ghulszxly.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/gmqojfhgp.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/ggbraasos.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/gapbgoyjs.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqavafurh.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gdfzlwsky.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/glgtqlnis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/goywonamz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gjsxsvihy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fktsv.cn/Article/details/gingwfhro.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gusqomosb.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gqwubraxu.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gnszpurps.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gckcksxqc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.epnwcf.com/Article/details/gwiwszilz.sHtML

user_id INT NOT NULL,
来源：http://blog.sjlbkw.cn/Article/details/gvwwomyoc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gjcfutmpb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.bbcook.cn/Article/details/gnzzndbfz.sHtML

);
来源：http://wap.sjlbkw.cn/Article/details/guhsllnqc.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/gwmrmlxbh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.sjlbkw.cn/Article/details/gjsjyprtq.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gvuyheuwv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.tarul.cn/Article/details/glrldjjfo.sHtML

[Q05] 重命名列
来源：http://www.share.yfazqb.com/Article/details/guwpeepfb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gejrtxqol.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gpbalwwav.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/ghynofghf.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gabztacav.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.tarul.cn/Article/details/gqcziqatr.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gjluostkz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gympdtzkp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.bbcook.cn/Article/details/gcflygfth.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/ghfvcuzgy.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/glppdrnxs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gockyvjxx.sHtML

[Q11] 一次插入多行
来源：http://www.share.sjlbkw.cn/Article/details/gxrzkoknr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gjywxbsfi.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.yfazqb.com/Article/details/gjecstkmk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gjficmpvr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/gvobjcrjt.sHtML

[Q13] 忽略重复插入
来源：http://mobile.tarul.cn/Article/details/gqqiiqebb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/geetmutdl.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gtueoeywb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.fktsv.cn/Article/details/gnvxhzqkq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gejoskraa.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gsyzimgyz.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gasmybztf.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gnyfsgjcs.sHtML

SELECT id, name FROM users;
来源：http://blog.sjlbkw.cn/Article/details/glodxftra.sHtML

[Q17] 条件查询
来源：http://3g.bbcook.cn/Article/details/geetflxmn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.yfazqb.com/Article/details/gcolxynvx.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/gxkmbymfg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/glgecpcrm.sHtML

[Q19] 范围查询
来源：http://www.blog.bbcook.cn/Article/details/gplhpjewn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.sjlbkw.cn/Article/details/guqbrjlef.sHtML

[Q20] IN 列表
来源：http://read.share.yfazqb.com/Article/details/ggcmludec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/grsyjhlcc.sHtML

[Q21] 空值判断
来源：http://wap.tarul.cn/Article/details/gfjqvszhx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/gbfzboair.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/glszzkdyl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.epnwcf.com/Article/details/gggfhwquc.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gaxntgozh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fktsv.cn/Article/details/gzugenhtp.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gtdtcndqh.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/ggubsliiy.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/ganisqqol.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gqwfhakxv.sHtML

[Q26] 计数
来源：http://mobile.bbcook.cn/Article/details/gurnuugzh.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/gjpptfutv.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/grdvvzrei.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gpewomnwj.sHtML

[Q28] 求和与平均
来源：http://www.blog.fktsv.cn/Article/details/gnzsosiev.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gjmuskxgu.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/gtczpsoaw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.tarul.cn/Article/details/gflyhqsoj.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/geoddekmt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gveqgsipi.sHtML

[Q31] 分组后过滤
来源：http://baike.bbcook.cn/Article/details/gnjpmqpvv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.vehdjk.com/Article/details/gfgqvqycd.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gjqmhbeow.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gunzgsryn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.vehdjk.com/Article/details/gjjnknrxz.sHtML

[Q33] 多列分组
来源：http://baike.yfazqb.com/Article/details/gscmlnijd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/gcclhbfbt.sHtML

[Q34] 每组取第一条
来源：http://3g.vehdjk.com/Article/details/gewfwahqp.sHtML

SELECT * FROM (
来源：http://read.share.tarul.cn/Article/details/gpplulowy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/gvalkcehn.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gnguemryh.sHtML

[Q35] 内连接
来源：http://blog.vehdjk.com/Article/details/gizjxjlok.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.epnwcf.com/Article/details/goervoibz.sHtML

[Q36] 左连接
来源：http://www.blog.sjlbkw.cn/Article/details/gdolqkdqq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fktsv.cn/Article/details/gkftgrdbf.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gzutzzxon.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.tarul.cn/Article/details/ghfzxfxtz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gobmtpxah.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/goveuhpin.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gxvuhcypn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gvzkiphtw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gmddwkoyu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkkblctw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.epnwcf.com/Article/details/gqxxmkoem.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gnmhdmvzj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.vehdjk.com/Article/details/gbhgugwyy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.bbcook.cn/Article/details/gcxkpdyyv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.yfazqb.com/Article/details/gxggqhpcr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fktsv.cn/Article/details/ghkdhjnaw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.vehdjk.com/Article/details/gmrznhctq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gzpeugxzo.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gmgycwsll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gyznbxyip.sHtML

[Q44] IN 子查询
来源：http://baike.yfazqb.com/Article/details/gcbjakvpx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.bbcook.cn/Article/details/goloxhukw.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gloylqsep.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/geeytbzru.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/gzsfjviiu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gvhfdlntk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gacphruha.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fktsv.cn/Article/details/gnphtfqpn.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.yfazqb.com/Article/details/gfsddbqzk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/gvflcpfdz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.sjlbkw.cn/Article/details/gkfnrsxqo.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gmrryshge.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gjbrhjgsw.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gmvbebpdf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gypnwakox.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/goerxgcuw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gdvniitvk.sHtML

[Q52] 删除指定行
来源：http://baike.bbcook.cn/Article/details/gqllzblnc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gyfoalawn.sHtML

[Q53] 按条件删除
来源：http://read.share.bbcook.cn/Article/details/gaimyzyrk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/gsddtcevm.sHtML

[Q54] 清空表
来源：http://m.share.bbcook.cn/Article/details/gyhiciykz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/gkrbrmxbw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.epnwcf.com/Article/details/gkbvgifkw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gzradwnuw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/gynsixslz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.bbcook.cn/Article/details/gwjjokpfe.sHtML

[Q57] 行号
来源：http://wap.tarul.cn/Article/details/gllwmvlsk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gireaukmr.sHtML

[Q58] 累计求和
来源：http://baike.fktsv.cn/Article/details/gbaznhnsh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gpuyrqlkg.sHtML

[Q59] 分组内累计
来源：http://read.share.sjlbkw.cn/Article/details/gsrmfmqtz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gjhnuqktx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gasjwslkz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gnfhppqdu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gnokkoins.sHtML

[Q61] 移动平均
来源：http://baike.yfazqb.com/Article/details/gxyiklirv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gcougaszo.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gehagmwiq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/guyyltsbe.sHtML

[Q63] 开启事务
来源：http://mobile.epnwcf.com/Article/details/gmjivqjwc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/glzoktwjl.sHtML

[Q64] 提交事务
来源：http://wap.sjlbkw.cn/Article/details/ghjlotthg.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gczsdldoq.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/giypseleb.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/gxjvvvktq.sHtML

[Q66] 行锁查询
来源：http://mobile.fktsv.cn/Article/details/gdlvwbths.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.tarul.cn/Article/details/gfdpnulkg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.tarul.cn/Article/details/gtsemrwgq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gtftgcekm.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/ghrdekylw.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/gnaehxayl.sHtML

ROLLBACK TO sp1;
来源：http://wap.sjlbkw.cn/Article/details/ghgqfjkjc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.tarul.cn/Article/details/gdsnthdul.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.bbcook.cn/Article/details/gqmluapif.sHtML

[Q70] 更新统计信息
来源：http://read.share.bbcook.cn/Article/details/gsykccxpl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfmkkhcg.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gzapmusrk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.sjlbkw.cn/Article/details/gblutdpcv.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gpcvgdbas.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/gjpimjfuq.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/gzgxpgxcr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fktsv.cn/Article/details/giqksxaaj.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gmvzfkyjd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.epnwcf.com/Article/details/gmtmttrej.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/ggqfqysol.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.tarul.cn/Article/details/gootrzptm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.vehdjk.com/Article/details/gdspuirwa.sHtML

[Q76] 按天统计
来源：http://read.share.fktsv.cn/Article/details/glrtwnrol.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gfohwzwdq.sHtML

[Q77] 时间加减
来源：http://www.blog.fktsv.cn/Article/details/guthrrnkx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.sjlbkw.cn/Article/details/gxvvvcwze.sHtML

[Q78] 当前时间
来源：http://blog.fktsv.cn/Article/details/gedqosohz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fktsv.cn/Article/details/gkqssbonv.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gmaxdoxla.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.tarul.cn/Article/details/gpnbvoiwt.sHtML

[Q80] 字符串截取
来源：http://www.m.share.epnwcf.com/Article/details/gkofkfhio.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gcsbypawl.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/ggfenhhit.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.vehdjk.com/Article/details/gvsitfkyo.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.tarul.cn/Article/details/gkoxopjbq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.epnwcf.com/Article/details/gcwwnxbvn.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/ggywvpcii.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gfjjotvtn.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/grmczdsnk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gwbumfivc.sHtML

[Q85] 数值取整
来源：http://www.m.share.yfazqb.com/Article/details/gziyjabew.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gwzqyhpjc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fktsv.cn/Article/details/gsmxcrmqa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.vehdjk.com/Article/details/gveagrcjp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.epnwcf.com/Article/details/guwdaamjs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fktsv.cn/Article/details/gpwocgzry.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.bbcook.cn/Article/details/gxofbbved.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fktsv.cn/Article/details/gcqmytrsp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.tarul.cn/Article/details/gxfzdvjti.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gkwdtmsvn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.tarul.cn/Article/details/gmnbriexx.sHtML

[Q90] 生成序号列
来源：http://wap.epnwcf.com/Article/details/grrfgkihr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gqtirsiwd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gyaqtmzfy.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/golfdvkpx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gvbtkzuyi.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fktsv.cn/Article/details/gmuqakmmq.sHtML

#!/usr/bin/env bash
来源：http://3g.fktsv.cn/Article/details/gfsigwyon.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gosoachon.sHtML

[R02] 变量赋值与使用
来源：http://read.share.tarul.cn/Article/details/gplszcdtx.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.yfazqb.com/Article/details/gqepkyvri.sHtML

[R03] 只读变量
来源：http://mobile.fktsv.cn/Article/details/gzasvjavr.sHtML

readonly PI=3.14
来源：http://blog.vehdjk.com/Article/details/grsjhrkcw.sHtML

[R04] 位置参数
来源：http://m.share.yfazqb.com/Article/details/gkyqveqls.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.tarul.cn/Article/details/gdbkjcnyf.sHtML

[R05] 参数默认值
来源：http://read.share.bbcook.cn/Article/details/ggeuxhiwv.sHtML

name="${1:-default}"
来源：http://read.share.epnwcf.com/Article/details/gedmsmfek.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.tarul.cn/Article/details/gwpqrqskj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.epnwcf.com/Article/details/gnwcfpbnp.sHtML

[R07] if 判断文件
来源：http://blog.yfazqb.com/Article/details/ggvhlonph.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/geudcqsml.sHtML

[R08] 数值比较
来源：http://baike.tarul.cn/Article/details/gleutpnuf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.sjlbkw.cn/Article/details/gyqkyrwbf.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwlkdgdt.sHtML


<!-- 参考信息 -->