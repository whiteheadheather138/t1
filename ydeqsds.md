代发 wailian999

TS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gkrolrjkf.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/ghjevbisv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fktsv.cn/Article/details/gccwqfkow.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/gycbntmoz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gkwewjlrl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gzwsxfzir.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.yfazqb.com/Article/details/gdxinqkyr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gqulxaxsg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.sjlbkw.cn/Article/details/gipajsuyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.vehdjk.com/Article/details/gvoghjifo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gfgwekdzh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.tarul.cn/Article/details/gonlqnfoh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/gwnnxyuva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/guqhupotv.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gyynemamt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.bbcook.cn/Article/details/gqgkzsomk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.vehdjk.com/Article/details/gvfadqflu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gtcsolgno.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gcunzxlel.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gypbmcogz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gejmnfoke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/gndbjidbm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.tarul.cn/Article/details/gzvsqwick.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gvkgiubjx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gnplnzqma.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/gsoomjkbo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gznllrrsr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/gjqhvdsfh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fktsv.cn/Article/details/glcwgbekn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gyzznwctk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.yfazqb.com/Article/details/goxplbfqb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/gjztjmkje.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gwilikuos.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.sjlbkw.cn/Article/details/gazzofssb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gwacabowm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.tarul.cn/Article/details/gohffvzke.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gakmpqnzc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.tarul.cn/Article/details/giqqbevmc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gludswoat.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/grruhlvpf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.sjlbkw.cn/Article/details/gxvsmgros.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gtjespcqm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gswjavhlz.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/gdifqbran.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/gasgwniic.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/ggstsbwsj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gfnpyuwpf.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/goxixxefr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gvnhtjiwk.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gikihsfsf.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/gqjbptpad.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.vehdjk.com/Article/details/gpsbzuzcm.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.tarul.cn/Article/details/gkvjkifqo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gatfknkyj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/glevpfppr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fktsv.cn/Article/details/grauexjyk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.yfazqb.com/Article/details/gcpvojybc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gjsyffrgn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/ghvjpcpkl.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gntifnqrt.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.bbcook.cn/Article/details/gcfiigxzo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.tarul.cn/Article/details/gofxmvmvo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/grgkgxrkc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gggddcmlc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.epnwcf.com/Article/details/gsdkpfatb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gfuamvgdc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/gstxdktmm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gkwdalbsc.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gbrqahize.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fktsv.cn/Article/details/gjtlvyles.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gyfwntlfz.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gqdgxdvsv.sHtML

CREATE TABLE users (
来源：http://baike.tarul.cn/Article/details/gryqcylis.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gwssvfgdh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/glqagwnpu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.sjlbkw.cn/Article/details/ghuzaozoz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.epnwcf.com/Article/details/gjmxydhih.sHtML

);
来源：http://wap.tarul.cn/Article/details/gquexdyic.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gviidepqh.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/gvplpdfos.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.tarul.cn/Article/details/gmilkfjzz.sHtML

user_id INT NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gmphalpty.sHtML

amount DECIMAL(10, 2),
来源：http://blog.tarul.cn/Article/details/gbhamgfrl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.sjlbkw.cn/Article/details/gavpmnagh.sHtML

);
来源：http://www.blog.bbcook.cn/Article/details/gkkhnncwz.sHtML

[Q03] 增加列
来源：http://wap.tarul.cn/Article/details/gxfryxmda.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gbgsqbepu.sHtML

[Q04] 修改列类型
来源：http://baike.tarul.cn/Article/details/gsxatarcb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gtqfunghg.sHtML

[Q05] 重命名列
来源：http://m.share.sjlbkw.cn/Article/details/gjymzzumi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.yfazqb.com/Article/details/gqpvgizky.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gmksurucb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gpyxazlmn.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gzrywzwat.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gupwvdafw.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/ghglleiep.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/gyfvgaflz.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/gsukchebw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.bbcook.cn/Article/details/grgezrmcp.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/gbjbsdhch.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fktsv.cn/Article/details/gmknzkvaf.sHtML

[Q11] 一次插入多行
来源：http://blog.bbcook.cn/Article/details/gdrpbokub.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/glkasdqem.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gqthgcref.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/gayghufog.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gnwadtsok.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gmdiiaiva.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gdzjalkab.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.yfazqb.com/Article/details/gqybbjfmm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/gtyuwmfka.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gpwvuhacr.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gmscvbdtq.sHtML

SELECT * FROM users;
来源：http://m.share.bbcook.cn/Article/details/guhoqxeai.sHtML

[Q16] 查询指定列
来源：http://m.share.yfazqb.com/Article/details/gfrmvtdpr.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gocjnqvbk.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/grnmvnosb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gmyskqswp.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/glbyhfnkg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.bbcook.cn/Article/details/gklkqmuqd.sHtML

[Q19] 范围查询
来源：http://baike.bbcook.cn/Article/details/gqiuhqaup.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gmibhehdy.sHtML

[Q20] IN 列表
来源：http://3g.tarul.cn/Article/details/gawpwzyda.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.tarul.cn/Article/details/gmtdjangg.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/gkiupunla.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gyquxogmc.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/gdmkwdtfu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.vehdjk.com/Article/details/gtqxzrmew.sHtML

[Q23] 分页
来源：http://baike.tarul.cn/Article/details/gdawnpqlt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fktsv.cn/Article/details/gdtdmeimi.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gtjgrzygw.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/gdiduceox.sHtML

[Q25] 只取前 N 条
来源：http://wap.bbcook.cn/Article/details/gfgddvjyl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.epnwcf.com/Article/details/gidhkrlqp.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gpkggtmqh.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmiesjzdh.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gxxqsmhss.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.yfazqb.com/Article/details/gnzbbnmpw.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/gmqualghu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.tarul.cn/Article/details/gavzlxcbd.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gnxepiuur.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.bbcook.cn/Article/details/ghscpnlfy.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gjzudaqpp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gcwbvxwrm.sHtML

[Q31] 分组后过滤
来源：http://blog.bbcook.cn/Article/details/goufjkkwn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/ggaobinbs.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gytjxgwmw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/glouwyuya.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.yfazqb.com/Article/details/gdozlmvbd.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gkroqukyg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/gfxfycsqf.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gfinpzjgb.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gckpdkuai.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.epnwcf.com/Article/details/gjqsymmir.sHtML

) t WHERE rn = 1;
来源：http://www.blog.yfazqb.com/Article/details/giywhlbmj.sHtML

[Q35] 内连接
来源：http://www.share.bbcook.cn/Article/details/gacimpcoi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/glzlvlscv.sHtML

[Q36] 左连接
来源：http://www.blog.vehdjk.com/Article/details/gohufttcp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gpnbvaiaz.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gqztkizpt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gewlruulz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gfezkjhkf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gckfnrljr.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvrpzpdm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gkauaqvea.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/gnocgcdta.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.vehdjk.com/Article/details/gmsxysepl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/gqvbwvpcd.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gtdlklwqe.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/galsyhdco.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/gwogjkiax.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gqvurvczw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/gipkhxgaz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/gettpnift.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.epnwcf.com/Article/details/ghglrkktb.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/gtyglcpqn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fktsv.cn/Article/details/gvhvukzry.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gqjtoanzr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gaptibgac.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gdqjwmdxg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/gtkzwznlp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gfiqxfamm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbywcigwj.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gvzmzojpb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gflhsemcc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fktsv.cn/Article/details/gpbhjwhtj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/giiluyrjv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.tarul.cn/Article/details/gpgpnmchp.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gamaoxobv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gfzxuqrva.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gbapzsyqq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.sjlbkw.cn/Article/details/grtbkiccl.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/giwugjalq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gvmqqpnps.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gjorzdcgj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gsngpuzza.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gpmwmbmbx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gimroygfi.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/grspqilqd.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.yfazqb.com/Article/details/ggkitzccf.sHtML

[Q55] 排名（并列占位）
来源：http://blog.epnwcf.com/Article/details/gnrangtif.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/gnksyewwn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.sjlbkw.cn/Article/details/gvjosgdeg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gbwlwhxwb.sHtML

[Q57] 行号
来源：http://wap.yfazqb.com/Article/details/gofmtduqj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.vehdjk.com/Article/details/gqlcviibm.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gxqxlslop.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gvrbzdvbh.sHtML

[Q59] 分组内累计
来源：http://wap.epnwcf.com/Article/details/gvllxrpon.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gezyhtfeq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gelmzpclk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gscbachko.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gcszcwzbm.sHtML

[Q61] 移动平均
来源：http://www.m.share.tarul.cn/Article/details/gariebnii.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/goislzdhy.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gbytrwemx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gpsnnqkro.sHtML

[Q63] 开启事务
来源：http://www.share.sjlbkw.cn/Article/details/gmzbpgiwo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gujnkpscv.sHtML

[Q64] 提交事务
来源：http://read.share.vehdjk.com/Article/details/gainklstb.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/grcrfishf.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/ghqtcewgc.sHtML

ROLLBACK;
来源：http://www.share.vehdjk.com/Article/details/ggeyhugqz.sHtML

[Q66] 行锁查询
来源：http://mobile.vehdjk.com/Article/details/ggoaokqwj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/gglhjpnqy.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gugykfmkh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.vehdjk.com/Article/details/gwbqwrvnx.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gravnvwfn.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gzozwrcxz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.sjlbkw.cn/Article/details/givxnpovg.sHtML

[Q69] 查看执行计划
来源：http://mobile.fktsv.cn/Article/details/gyapezgfr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gtdtdoihb.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gkawxlwft.sHtML

ANALYZE TABLE users;
来源：http://mobile.yfazqb.com/Article/details/gywyjehbp.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gyjjfncbq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.tarul.cn/Article/details/glciqhamv.sHtML

[Q72] 查看索引
来源：http://wap.epnwcf.com/Article/details/gbycqxwwq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.epnwcf.com/Article/details/grwimtdlc.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gskrncbno.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.epnwcf.com/Article/details/gwtvzuipa.sHtML

[Q74] 强制使用索引
来源：http://baike.tarul.cn/Article/details/gvrosveem.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.bbcook.cn/Article/details/gztgkdwpt.sHtML

[Q75] 日期格式化
来源：http://read.share.bbcook.cn/Article/details/gscwuszjl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.tarul.cn/Article/details/gwohotrvx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.tarul.cn/Article/details/glhiwrdqk.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gtaoiueqo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.vehdjk.com/Article/details/gqfyaqaxq.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gkuhbskax.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.bbcook.cn/Article/details/gknplxthn.sHtML

[Q78] 当前时间
来源：http://www.share.bbcook.cn/Article/details/ggubxqasp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/ggtnqoubp.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.bbcook.cn/Article/details/gogyyxthz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gvupzosug.sHtML

[Q80] 字符串截取
来源：http://wap.sjlbkw.cn/Article/details/gxotvnwmt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpednqhke.sHtML

[Q81] 字符串替换
来源：http://mobile.epnwcf.com/Article/details/gwabmzvjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gmrxzutjx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.yfazqb.com/Article/details/gpebhlgbl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ghlbqyccl.sHtML

[Q83] 大小写转换
来源：http://blog.epnwcf.com/Article/details/gixyjpyjf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/grdayszbx.sHtML

[Q84] 去除首尾空格
来源：http://blog.bbcook.cn/Article/details/gnkoxoyjr.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.yfazqb.com/Article/details/geprgucdt.sHtML

[Q85] 数值取整
来源：http://read.share.tarul.cn/Article/details/gervodarp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fktsv.cn/Article/details/gobeqrstp.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gjwxcjnzt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.yfazqb.com/Article/details/gkwppobtz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gkjzrqsxy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fktsv.cn/Article/details/gkcrepjmt.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gcvltktmh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.bbcook.cn/Article/details/gccjtysdp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkdixdjb.sHtML

[Q89] 判断表是否存在
来源：http://baike.yfazqb.com/Article/details/gvfgbggou.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/gdiunzxqy.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/getkvxdnv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.vehdjk.com/Article/details/glevnbmsr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmascomvq.sHtML

R. Bash 专题
来源：http://blog.yfazqb.com/Article/details/gzeeafnqz.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gekwxbriy.sHtML

[R01] shebang 与严格模式
来源：http://blog.tarul.cn/Article/details/gpudeyhje.sHtML

#!/usr/bin/env bash
来源：http://read.share.sjlbkw.cn/Article/details/glwtjvtqt.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/ggasfcewp.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/gvfqqbxgr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fktsv.cn/Article/details/gzboruuvy.sHtML

[R03] 只读变量
来源：http://www.share.vehdjk.com/Article/details/gxsenjjhz.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/glcrlwanf.sHtML

[R04] 位置参数
来源：http://wap.vehdjk.com/Article/details/gzviiiaba.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.epnwcf.com/Article/details/gmdcmbdrf.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gjtexfutq.sHtML

name="${1:-default}"
来源：http://3g.epnwcf.com/Article/details/ggnljawhu.sHtML

[R06] 判断命令是否存在
来源：http://wap.sjlbkw.cn/Article/details/gxoupsukg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.tarul.cn/Article/details/gdlubjwoa.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gcxhmofia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fktsv.cn/Article/details/grpywlwtw.sHtML

[R08] 数值比较
来源：http://wap.sjlbkw.cn/Article/details/gyztxhwbz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.tarul.cn/Article/details/gpkmykzjh.sHtML

[R09] 字符串比较
来源：http://mobile.vehdjk.com/Article/details/gshqoppcv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fktsv.cn/Article/details/gooublvcq.sHtML

[R10] 正则匹配
来源：http://m.share.bbcook.cn/Article/details/gsrkabcsp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.sjlbkw.cn/Article/details/geeqfshmo.sHtML

[R11] case 多分支
来源：http://blog.fktsv.cn/Article/details/gkiqltgry.sHtML


<!-- 参考信息 -->