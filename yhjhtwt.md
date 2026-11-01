代发 wailian999

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gpuvbjcjo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gayjmxyte.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.vehdjk.com/Article/details/gcpqmfjxw.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gklgopzsh.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gygrvhkdq.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfhnsmvjb.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/ghorrzpcf.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/ghvdhbwju.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gffpctihj.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.vehdjk.com/Article/details/gggmzxvjk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.bbcook.cn/Article/details/gdxqvpafm.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gxktnldvl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gfdwfwgtl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gtxwlznmu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/glwhqtmft.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/glxanijiu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gwdnfffsb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/ggsoldsly.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/gopalvlup.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gybvycyxd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.epnwcf.com/Article/details/gkfjlxdzw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.tarul.cn/Article/details/gwkfvivfh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.sjlbkw.cn/Article/details/gysrfybcm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/geaoyjxml.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fktsv.cn/Article/details/ghvrnyoqd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/grwwkrkkv.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gmovfivnw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gdvlespzc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gwvgmjvgp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/giwodphlt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/geeitmyoh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gpupntsfe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.tarul.cn/Article/details/ggmtzeezb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gfrsbtiyp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.sjlbkw.cn/Article/details/gmrhuqmpq.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gyhskkrgd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gaxobxjef.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gpmcoltgw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gvpyryuvn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/glloplnzx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/ghbvqnnry.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gxjwkyeqi.sHtML

Ruby: x.length;  x.size
来源：http://blog.yfazqb.com/Article/details/gdixpfovl.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gqnwoajzt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/guofyjcyq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/grfsjofkg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.bbcook.cn/Article/details/gotpmicjz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/genajhzlh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.yfazqb.com/Article/details/gbpcdnyqc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gbjassobb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gqdqsjjdd.sHtML

Ruby: a == b
来源：http://blog.sjlbkw.cn/Article/details/gzzysryxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gixfgmwgu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gwmxcmomy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.bbcook.cn/Article/details/gqjozhkvx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gusufjvws.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/ggguuxcfw.sHtML

TS:   if (x == null) {}
来源：http://baike.fktsv.cn/Article/details/gdgkokaiq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.bbcook.cn/Article/details/gmhxhpycd.sHtML

Go:   if x == nil {}
来源：http://baike.fktsv.cn/Article/details/gqyfxpxxl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gkhoejdoz.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gxdmmcthn.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gmrcrjzoj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gzhbrlokq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gygnmhucz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gcnfhszrb.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gselimndi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/ghiezbrmp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.epnwcf.com/Article/details/glcyfpitw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gdnogmont.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.bbcook.cn/Article/details/gckzpilya.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gpsjcvvvy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/gspyadfqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.sjlbkw.cn/Article/details/gtqitagik.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/grtxrctme.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gkbkabful.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gwgiwcfyn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/glaubfwqf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/gxtiavhbu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.yfazqb.com/Article/details/gvlpsnelk.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghksoajkk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/gjgaapjot.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gpevmycjq.sHtML

[Q01] 创建表
来源：http://m.share.sjlbkw.cn/Article/details/gwhurximw.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gffdanlkn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.bbcook.cn/Article/details/gyjglakdh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/gdvspefhu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/ghxzdfvag.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.yfazqb.com/Article/details/gzrtxubgn.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gbfzfdieh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gnedhpkqf.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gugoczlnw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gqitjrndr.sHtML

user_id INT NOT NULL,
来源：http://wap.bbcook.cn/Article/details/gqlgqofnx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gjjfzkipi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.epnwcf.com/Article/details/gklouexef.sHtML

);
来源：http://baike.tarul.cn/Article/details/gzichqdho.sHtML

[Q03] 增加列
来源：http://www.m.share.epnwcf.com/Article/details/ghqdapenm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.vehdjk.com/Article/details/gpnljqpvj.sHtML

[Q04] 修改列类型
来源：http://read.share.sjlbkw.cn/Article/details/geypkedwz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fktsv.cn/Article/details/gsjuclmxz.sHtML

[Q05] 重命名列
来源：http://m.share.tarul.cn/Article/details/giwodjuao.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gsrrxvlkd.sHtML

[Q06] 删除列
来源：http://wap.tarul.cn/Article/details/gbpivoddx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gytqgcrpu.sHtML

[Q07] 删除表
来源：http://www.share.yfazqb.com/Article/details/gabulnavy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/gktyperwg.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/gugvwgtkf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gijtbyzyv.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/glnjximar.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.yfazqb.com/Article/details/gfyssbdml.sHtML

[Q10] 插入单行
来源：http://www.blog.sjlbkw.cn/Article/details/gfdfkbkya.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gfbsdzset.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/ggmxjtlnt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fktsv.cn/Article/details/gvipihdzs.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/genknvwta.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/ggcqhilvz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/gcemnpnno.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gqnlgsykq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gfzajvnqf.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/gopbuxxjv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.epnwcf.com/Article/details/gfpzprewu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.epnwcf.com/Article/details/gxznhmbnd.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gexxigpxw.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjijyxaec.sHtML

[Q16] 查询指定列
来源：http://read.share.epnwcf.com/Article/details/gwifkeqoi.sHtML

SELECT id, name FROM users;
来源：http://wap.epnwcf.com/Article/details/gffswukap.sHtML

[Q17] 条件查询
来源：http://m.share.sjlbkw.cn/Article/details/gyfmrtjwr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/garxyiqjv.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/gdgtjkqii.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjjimkti.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/gmwbtujdr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gogckeyxe.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gfudlboga.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gfirbpjka.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/glquagosp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.tarul.cn/Article/details/gpbqivhvf.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/gsgomuroe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.bbcook.cn/Article/details/gbgxwdqbw.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/ggxkmymbx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.sjlbkw.cn/Article/details/ggljaqvbt.sHtML

[Q24] 去重
来源：http://www.share.fktsv.cn/Article/details/ggwggcktn.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gbbyzsjtq.sHtML

[Q25] 只取前 N 条
来源：http://blog.sjlbkw.cn/Article/details/gtyqsfvqi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gnqrgmcvs.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gybhymeax.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gwzhwvzbv.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gyuoxqvyu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gstwgiurl.sHtML

[Q28] 求和与平均
来源：http://www.share.bbcook.cn/Article/details/gzpuoehwp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmcewpfao.sHtML

[Q29] 最大最小值
来源：http://3g.bbcook.cn/Article/details/glnhmuixt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gwpvctqoh.sHtML

[Q30] 分组统计
来源：http://wap.bbcook.cn/Article/details/grydieuoi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gjnxgnpes.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/glpmvjxgn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fktsv.cn/Article/details/gpkgwhcaz.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gfurjyhth.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gyjksnnjw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fktsv.cn/Article/details/gmqvkxbhl.sHtML

[Q33] 多列分组
来源：http://blog.epnwcf.com/Article/details/grmexfpku.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.yfazqb.com/Article/details/gtdvhtqnu.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gyrhqjmzb.sHtML

SELECT * FROM (
来源：http://3g.epnwcf.com/Article/details/glzzjtogw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.yfazqb.com/Article/details/ghtzzfdbz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gbzjlmxik.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/gdbdnyrgs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gpdbtdcgx.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gdwmjodnm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/gekvysgwv.sHtML

[Q37] 右连接
来源：http://mobile.tarul.cn/Article/details/gmosrvelc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.sjlbkw.cn/Article/details/giqarwpws.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fktsv.cn/Article/details/gzicbuhzd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/ggjglkclq.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.tarul.cn/Article/details/ggqvlhcrc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.yfazqb.com/Article/details/geqrpizkw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gymvalmsq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.bbcook.cn/Article/details/gsrlbfoug.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/glsofjxtz.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gwwtmkaot.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.epnwcf.com/Article/details/guutjrzlx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gnmgtjaym.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gsuczalxe.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gqrdlnnga.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.sjlbkw.cn/Article/details/gfyznpcyx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.yfazqb.com/Article/details/gtbtvdkbe.sHtML

[Q43] 标量子查询
来源：http://mobile.yfazqb.com/Article/details/gswuafpgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gmuilimmt.sHtML

[Q44] IN 子查询
来源：http://baike.sjlbkw.cn/Article/details/gnasjzdtk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gggmdswnh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.sjlbkw.cn/Article/details/grlatveyd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gmybcpfyy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gmzhdvkoh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gqjsdutxq.sHtML

[Q47] 与平均值比较
来源：http://www.share.epnwcf.com/Article/details/galtbxjtf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gyosmlgpb.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.tarul.cn/Article/details/gpcyywaqu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.sjlbkw.cn/Article/details/gxsxxfczk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gltahqbxx.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/ggqcvonhe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/godelzzev.sHtML

[Q50] 批量更新
来源：http://blog.vehdjk.com/Article/details/gnufpcndl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/gwrgflovb.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gpgvfiimt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gtsfceken.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/guftuaqjt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gdycxgqog.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/getniadst.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gnahckain.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gbulyhduh.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/gbxeuuado.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/garoilokf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fktsv.cn/Article/details/gvadflhvf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.bbcook.cn/Article/details/grlavtpqf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/gujgrahdk.sHtML

[Q57] 行号
来源：http://wap.epnwcf.com/Article/details/gayakskqe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gcxxhhfzl.sHtML

[Q58] 累计求和
来源：http://www.blog.tarul.cn/Article/details/giajdawgs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fktsv.cn/Article/details/gihfgniyq.sHtML

[Q59] 分组内累计
来源：http://m.share.bbcook.cn/Article/details/gtfjovemy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gaczvdmcx.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fktsv.cn/Article/details/gmlhxxiet.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gyibwrnmw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gwnaeihim.sHtML

[Q61] 移动平均
来源：http://wap.yfazqb.com/Article/details/gnljwopft.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gkfpgfryn.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/givusfjpv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/gcamabqoe.sHtML

[Q63] 开启事务
来源：http://3g.vehdjk.com/Article/details/gdmcmvdhs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gbdqzmwpa.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gqjbplfmv.sHtML

COMMIT;
来源：http://mobile.bbcook.cn/Article/details/gwfyvueyq.sHtML

[Q65] 回滚事务
来源：http://read.share.sjlbkw.cn/Article/details/gomlmchok.sHtML

ROLLBACK;
来源：http://read.share.yfazqb.com/Article/details/gkoshcjok.sHtML

[Q66] 行锁查询
来源：http://read.share.sjlbkw.cn/Article/details/gziphkwti.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fktsv.cn/Article/details/gqhgumtmv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/gffpxhvwb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/ggrgoexac.sHtML

[Q68] 保存点
来源：http://mobile.fktsv.cn/Article/details/gfjkyqape.sHtML

SAVEPOINT sp1;
来源：http://read.share.epnwcf.com/Article/details/gtdwkaruo.sHtML

ROLLBACK TO sp1;
来源：http://3g.sjlbkw.cn/Article/details/gaybcmypu.sHtML

[Q69] 查看执行计划
来源：http://m.share.fktsv.cn/Article/details/gsslvddhh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/gwwhpbioi.sHtML

[Q70] 更新统计信息
来源：http://wap.vehdjk.com/Article/details/gqjjtkzrt.sHtML

ANALYZE TABLE users;
来源：http://mobile.epnwcf.com/Article/details/gcpjqjmpe.sHtML

[Q71] 查看建表语句
来源：http://www.share.tarul.cn/Article/details/gxipdyors.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gngyhsyzi.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/gtiwwowsr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gnjrqfrjl.sHtML

[Q73] 查看表状态
来源：http://blog.sjlbkw.cn/Article/details/gqenmfhni.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.epnwcf.com/Article/details/gykcepyyf.sHtML

[Q74] 强制使用索引
来源：http://3g.vehdjk.com/Article/details/gumprvugq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gihgpyfwj.sHtML

[Q75] 日期格式化
来源：http://m.share.tarul.cn/Article/details/gzpxsbycc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gcawwshxq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.bbcook.cn/Article/details/ggjjbledp.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gywhxyllo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.vehdjk.com/Article/details/gglahqgxp.sHtML

[Q77] 时间加减
来源：http://m.share.tarul.cn/Article/details/gzencbtby.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.bbcook.cn/Article/details/gsbgithez.sHtML

[Q78] 当前时间
来源：http://read.share.sjlbkw.cn/Article/details/gysenjjmi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.yfazqb.com/Article/details/gcdnpjfye.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.sjlbkw.cn/Article/details/gitktbcps.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgkkmiue.sHtML

[Q80] 字符串截取
来源：http://3g.vehdjk.com/Article/details/gbhizeulb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gjkzeeyjm.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/ggwmdifsh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gfczxxumn.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.tarul.cn/Article/details/gveztfxfo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gjiklzdhk.sHtML

[Q83] 大小写转换
来源：http://read.share.bbcook.cn/Article/details/gojptkdnj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gauuwxkzm.sHtML

[Q84] 去除首尾空格
来源：http://mobile.epnwcf.com/Article/details/gtjkembky.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gnokqdmns.sHtML

[Q85] 数值取整
来源：http://www.m.share.fktsv.cn/Article/details/gqkbmzqzq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.bbcook.cn/Article/details/gfbgofcht.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.sjlbkw.cn/Article/details/gzjhwqhty.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.vehdjk.com/Article/details/gbpmazzea.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fktsv.cn/Article/details/gtxssxtew.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gyohxbsdz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.sjlbkw.cn/Article/details/gcjwscfub.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.tarul.cn/Article/details/gozzokity.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/gylwjqhso.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/goatdndru.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.tarul.cn/Article/details/gxxxsgxie.sHtML

[Q90] 生成序号列
来源：http://m.share.tarul.cn/Article/details/gberkbfhe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.vehdjk.com/Article/details/gwogelaed.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvqmtyhka.sHtML

R. Bash 专题
来源：http://baike.yfazqb.com/Article/details/gtnpntodj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwkbqnstp.sHtML

[R01] shebang 与严格模式
来源：http://read.share.tarul.cn/Article/details/gftvguuky.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gclxbsgqf.sHtML

set -euo pipefail
来源：http://www.m.share.bbcook.cn/Article/details/galvwcnyt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/gujvxjflr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/gazpqfuok.sHtML

[R03] 只读变量
来源：http://m.share.epnwcf.com/Article/details/gjuhiehvq.sHtML

readonly PI=3.14
来源：http://read.share.yfazqb.com/Article/details/gxntehywo.sHtML

[R04] 位置参数
来源：http://www.blog.vehdjk.com/Article/details/gamoehjny.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.bbcook.cn/Article/details/gwvrxsofh.sHtML

[R05] 参数默认值
来源：http://m.share.epnwcf.com/Article/details/gbqnzjpqo.sHtML


<!-- 参考信息 -->