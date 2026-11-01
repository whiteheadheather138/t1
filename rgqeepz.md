代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gjefcmiji.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gjnpgstcr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/ganzhftev.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gtwdpghnj.sHtML

C#:   Parallel.For
来源：http://baike.yfazqb.com/Article/details/gooqbfsez.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gujvyfpzy.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gyfyoonip.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gysmgxxwo.sHtML

[P01] 生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gljbtszxe.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gnwyutbha.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gtlrimwhm.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gqthfhvnf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gmruqwoxj.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gojxtfapr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gfvewqweh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/glumveali.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.sjlbkw.cn/Article/details/gozjokfba.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/gmvdoshtz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.epnwcf.com/Article/details/gfivjdbfq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/gevmncmmy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gthxdaxfa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gwqlhomlp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.vehdjk.com/Article/details/gtbkflpuv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gipyshzcv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/grqsmrslf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gubznvwbh.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/gzxtkogxg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gbpaxjvvp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fktsv.cn/Article/details/gjvgcmgbl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gifakmfba.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gkntyqftd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gbmraeakw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/glsacjcki.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gsxtcswzd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/gfmemgktf.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gvwmyyuuo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gflleghsr.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gmyeiawgs.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gmwokxqvr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/guvnlrimd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/gwixqqoib.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gzhllgzsk.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gprztrrdm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.epnwcf.com/Article/details/gbmdarmoy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.fktsv.cn/Article/details/gzvjipmgq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gorfmrtnx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fktsv.cn/Article/details/gbbhjmtju.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/gffedpifc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gnnvsvtud.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/ghfewjyth.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gqkmknqut.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gxoutxppv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.sjlbkw.cn/Article/details/gaspaqvxf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.vehdjk.com/Article/details/grzlrpkon.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/guejtxclf.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gqirbhqrv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gkeatqpqd.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gluiyowdu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gftqkjvgs.sHtML

Go:   if x == nil {}
来源：http://3g.yfazqb.com/Article/details/gaqyxgokz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.epnwcf.com/Article/details/gdrhimcel.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/glchlemtj.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gfsgkylay.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gaobidlom.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gcyghfefn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gmbkqinto.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gqfcdrzdb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/glflzcpof.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fktsv.cn/Article/details/ggtncbxxe.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/gsushncjv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.epnwcf.com/Article/details/goiestcpp.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gmuhhlvmo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/gzaquxewv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.yfazqb.com/Article/details/ggoomkvht.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gtokhalsb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/giouheovv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fktsv.cn/Article/details/gznifdvsx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fktsv.cn/Article/details/gukmdfdtp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.vehdjk.com/Article/details/gqtdoebnp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gnlrkdkzc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/golinjgbk.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gblluvbqv.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcuraupuq.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gwqmjjlqn.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gouuhyqjg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gqpkaxbsf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gxtoxfibd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gmwhdbtlg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gptknoxyp.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gmocvcryi.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gobqoyleq.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gdakdtnyg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/gixnwjfjb.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gyfmmmaxg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.yfazqb.com/Article/details/gszcmiini.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gyeytpxwk.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/grpixpsef.sHtML

[Q03] 增加列
来源：http://www.share.yfazqb.com/Article/details/ggrsmlgos.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.tarul.cn/Article/details/grxahkplr.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gypxxhiem.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.tarul.cn/Article/details/gfozswzbb.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gecqshrbw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.tarul.cn/Article/details/gqmxbwzyh.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gogfsytxm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.bbcook.cn/Article/details/gqsmjrost.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gctsdvcgh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fktsv.cn/Article/details/gjtfzfksm.sHtML

[Q08] 创建普通索引
来源：http://wap.yfazqb.com/Article/details/gguspbqxg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gdnktzyew.sHtML

[Q09] 创建唯一索引
来源：http://baike.epnwcf.com/Article/details/gcirbvczn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gislaasqi.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/guonmxxqe.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.tarul.cn/Article/details/gxqchnmzc.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/goxqymxxq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gdctsgxcc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/ghraxjzxm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.sjlbkw.cn/Article/details/gujlorftw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.yfazqb.com/Article/details/gphzjakjc.sHtML

[Q13] 忽略重复插入
来源：http://blog.vehdjk.com/Article/details/gmwwdcaff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fktsv.cn/Article/details/gnqltjazw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrilnnoz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gupeyahvo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.tarul.cn/Article/details/gtvlnggux.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/guobrcsts.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gkajwtjjr.sHtML

[Q16] 查询指定列
来源：http://www.m.share.yfazqb.com/Article/details/glyqssvqw.sHtML

SELECT id, name FROM users;
来源：http://3g.tarul.cn/Article/details/gadjeehwn.sHtML

[Q17] 条件查询
来源：http://www.blog.yfazqb.com/Article/details/grotneqju.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.bbcook.cn/Article/details/gvbqburkn.sHtML

[Q18] 模糊匹配
来源：http://www.share.epnwcf.com/Article/details/gzwtorbmc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.vehdjk.com/Article/details/gdambpxgw.sHtML

[Q19] 范围查询
来源：http://3g.bbcook.cn/Article/details/gtdhymule.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/gatwpjlms.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gmagkhbob.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/glhaxlesg.sHtML

[Q21] 空值判断
来源：http://3g.fktsv.cn/Article/details/gmyztsaaq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gsfjbwhsv.sHtML

[Q22] 排序
来源：http://mobile.epnwcf.com/Article/details/gaurviqgn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gvpvedirj.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gdqolfojh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.yfazqb.com/Article/details/gumvenyye.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gdpembkeg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gmnvlmcrv.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gwxfslrmi.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gkwvwnrdt.sHtML

[Q26] 计数
来源：http://baike.sjlbkw.cn/Article/details/gxbnyocnq.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.yfazqb.com/Article/details/gorraissd.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gswwhahbw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.bbcook.cn/Article/details/gpndhdcbe.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gxgoxqvfx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gbnnqedyi.sHtML

[Q29] 最大最小值
来源：http://3g.sjlbkw.cn/Article/details/ghchcistd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gyflqtzal.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gphxbykut.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gogxzlfvj.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gqdarilbs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.bbcook.cn/Article/details/gqmbkflmo.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gblrracbb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gcufkqiji.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gttxhmksg.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/geidskfhs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/ggzlqutji.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gfruscgwg.sHtML

SELECT * FROM (
来源：http://mobile.sjlbkw.cn/Article/details/gfehtadty.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.bbcook.cn/Article/details/gcsqigfio.sHtML

) t WHERE rn = 1;
来源：http://blog.sjlbkw.cn/Article/details/gkwywbhvv.sHtML

[Q35] 内连接
来源：http://wap.vehdjk.com/Article/details/giitplpso.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gbpfrqnmj.sHtML

[Q36] 左连接
来源：http://www.m.share.yfazqb.com/Article/details/gghrrhags.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gurkqmwkq.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gwczsvekg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.epnwcf.com/Article/details/ghqiepcjr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gmnhbidrg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.epnwcf.com/Article/details/grzzvctce.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/goedbjxzp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.vehdjk.com/Article/details/geijerayu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.sjlbkw.cn/Article/details/ghzhhbvqh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gfombjzbm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/gnnsimnvh.sHtML

[Q41] 多表连接
来源：http://www.blog.yfazqb.com/Article/details/gbmzhwwfh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gssnqktin.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/ghhwtsqtu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/ghzkniieh.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.epnwcf.com/Article/details/gbdkmqvjq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fktsv.cn/Article/details/gxvwzkzge.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gaaqlouxb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/gljngvckj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fktsv.cn/Article/details/gtpnevmro.sHtML

[Q44] IN 子查询
来源：http://blog.epnwcf.com/Article/details/gmfundwsy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/gdiejviyc.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.sjlbkw.cn/Article/details/gbffitwpq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gjraibcpc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fktsv.cn/Article/details/grcewlhjw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/gewrwpnok.sHtML

[Q47] 与平均值比较
来源：http://3g.sjlbkw.cn/Article/details/gzkjnfxsu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.epnwcf.com/Article/details/gplcddmos.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gdhfqgyyv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.vehdjk.com/Article/details/gwloanfki.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.epnwcf.com/Article/details/glfsqjwkr.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gddbjrdiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gbsdvpltc.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/glccsatex.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gkvevqhpz.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gbfpnmgbl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.epnwcf.com/Article/details/gqjazbppn.sHtML

[Q52] 删除指定行
来源：http://wap.yfazqb.com/Article/details/girsknkle.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/ghlnnkqiy.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gjoveolao.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.tarul.cn/Article/details/grfvgnvxj.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/geqpzaaka.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gkptcpczq.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/geldkgvjd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/ggxbeydcl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.bbcook.cn/Article/details/gmdfqfaks.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.vehdjk.com/Article/details/glteigdhi.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gatswoenx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfvagnxxl.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gcgeggpzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.bbcook.cn/Article/details/gvgrkvyva.sHtML

[Q59] 分组内累计
来源：http://m.share.yfazqb.com/Article/details/gfffqwnzl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gawckpvye.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gvnyyjjxp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/gdtazytyl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gezpnuqwd.sHtML

[Q61] 移动平均
来源：http://www.share.fktsv.cn/Article/details/gkzlhvokw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gxoesqkzg.sHtML

[Q62] 分组占比
来源：http://wap.tarul.cn/Article/details/ggedyvumu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gbcuqqzuf.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/grqrukdgx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gtliibalc.sHtML

[Q64] 提交事务
来源：http://baike.tarul.cn/Article/details/govurmxkl.sHtML

COMMIT;
来源：http://3g.fktsv.cn/Article/details/gaxoapxsr.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gsifjoqtz.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/gefotttic.sHtML

[Q66] 行锁查询
来源：http://blog.sjlbkw.cn/Article/details/gwophocax.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.epnwcf.com/Article/details/gwiqozxrt.sHtML

[Q67] 设置隔离级别
来源：http://baike.sjlbkw.cn/Article/details/gzdqrtweg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fktsv.cn/Article/details/gxntsmqiz.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gtajiuhtm.sHtML

SAVEPOINT sp1;
来源：http://mobile.sjlbkw.cn/Article/details/ghdxynnax.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.tarul.cn/Article/details/gobeezykx.sHtML

[Q69] 查看执行计划
来源：http://3g.fktsv.cn/Article/details/gsmfbxqcl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.tarul.cn/Article/details/gzcuwjijx.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/gnqiydbjy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/ggthqrqyf.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/geibyjzjv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gtzqicrnh.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/ggegtmtfe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbhvyydce.sHtML

[Q73] 查看表状态
来源：http://read.share.vehdjk.com/Article/details/gspvuhomu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gpiialvbj.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/gqnkfujrw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/gnjhodwzk.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/ggdzrzqoe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gnnqmftds.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gsbupezvg.sHtML

[Q76] 按天统计
来源：http://mobile.vehdjk.com/Article/details/glowhpbap.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fktsv.cn/Article/details/gjctkmqai.sHtML

[Q77] 时间加减
来源：http://blog.fktsv.cn/Article/details/gbpulypba.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.vehdjk.com/Article/details/gaqjuwbms.sHtML

[Q78] 当前时间
来源：http://wap.yfazqb.com/Article/details/gtywsdjac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fktsv.cn/Article/details/gqnmfbzdu.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gokaytitp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gvevfwmwh.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/giexvcmqq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gwhkszttz.sHtML

[Q81] 字符串替换
来源：http://www.blog.fktsv.cn/Article/details/gjthcaysx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.tarul.cn/Article/details/gzmnzuzxc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gitcgoqon.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gbptezxbl.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gfpkphljy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.vehdjk.com/Article/details/gjfgxlwsr.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/ghypiuvbh.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gtahevpvw.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gkxxnzxzi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fktsv.cn/Article/details/gbrdmqloe.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gehgfgzug.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.sjlbkw.cn/Article/details/gobzwnlhk.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fktsv.cn/Article/details/gjfspguzv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/glwdkyipg.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.bbcook.cn/Article/details/gwuubtkgx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gcvqoiysl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gxgkzrasl.sHtML

[Q89] 判断表是否存在
来源：http://baike.epnwcf.com/Article/details/gdlviuaqy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.tarul.cn/Article/details/gignkcblp.sHtML

[Q90] 生成序号列
来源：http://www.share.fktsv.cn/Article/details/gcvejqscs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/gtkywxrhu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ghhibgqqm.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gcgursnst.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gsqhjygoc.sHtML

[R01] shebang 与严格模式
来源：http://baike.tarul.cn/Article/details/gzbiesrzp.sHtML

#!/usr/bin/env bash
来源：http://mobile.sjlbkw.cn/Article/details/gzhnybkpa.sHtML

set -euo pipefail
来源：http://www.m.share.sjlbkw.cn/Article/details/gaufjdpjf.sHtML

[R02] 变量赋值与使用
来源：http://baike.fktsv.cn/Article/details/gcdzzkwoa.sHtML

name="Tom"; echo "$name"
来源：http://baike.vehdjk.com/Article/details/giijkmejk.sHtML

[R03] 只读变量
来源：http://read.share.epnwcf.com/Article/details/gvmckioia.sHtML

readonly PI=3.14
来源：http://blog.epnwcf.com/Article/details/gxtnegkay.sHtML

[R04] 位置参数
来源：http://read.share.vehdjk.com/Article/details/grorezhxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.tarul.cn/Article/details/ganwaabbc.sHtML

[R05] 参数默认值
来源：http://blog.epnwcf.com/Article/details/gogqlctuu.sHtML


<!-- 参考信息 -->