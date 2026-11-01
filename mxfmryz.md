代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gcbvynaxg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gzctlccek.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gbgfwustb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gcrvwqjnh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/giwckupij.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fktsv.cn/Article/details/gnvvwyyti.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gwvmshdhs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gtusxlhtl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/goleerwpr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gdflmcjkc.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gjfawicli.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gzziixnfu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.epnwcf.com/Article/details/gfrwxtumm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/grlnwyysc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gcwovaigc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/guaxdmvae.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.vehdjk.com/Article/details/gjaliqrcj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/guavqflpt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gvmewaizh.sHtML

[P04] 求长度
来源：http://mobile.vehdjk.com/Article/details/gfmpzzjsu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.tarul.cn/Article/details/gftdbwkyi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gadlmaxaw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gldrhbpgo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gigssjmkk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gzevalttn.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/ghwhmutbs.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gqqwddwyt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.sjlbkw.cn/Article/details/gqlbflwjk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gcdsulujq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/gdxeccwfp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gumuqvhum.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gnznfenva.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.bbcook.cn/Article/details/gyyvxeana.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.tarul.cn/Article/details/gvtgpjsyq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/gnbykjeqa.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/grgkoybdr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/giliimitm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/gyzmutxtj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gvbebksci.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/ghgzelxdh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/ggyiqkqdz.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.tarul.cn/Article/details/gpynhwrqh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gbrtteybs.sHtML

Go:   if x == nil {}
来源：http://read.share.epnwcf.com/Article/details/gzzvvhrph.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.epnwcf.com/Article/details/gqyyyzzcv.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gvwbsvplz.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gbbxdbqzw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gurubdmid.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.fktsv.cn/Article/details/gdgkgswqs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gwounqxkt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gtreglawb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.yfazqb.com/Article/details/gqrgohhoh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.yfazqb.com/Article/details/giyuthsto.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.fktsv.cn/Article/details/gyymmfuti.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/gblkceoxu.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gqucjipup.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fktsv.cn/Article/details/gafhrudfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.yfazqb.com/Article/details/gqvhqpmtl.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.vehdjk.com/Article/details/gaowfnkkv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/ggzzsdhwe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fktsv.cn/Article/details/gvlomzgyp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.vehdjk.com/Article/details/gtarggfgw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.bbcook.cn/Article/details/gnovwlzgw.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gsatknvft.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gurmwqgup.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/grwunybww.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ghkmpurch.sHtML

[Q01] 创建表
来源：http://3g.bbcook.cn/Article/details/gtorektag.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gajxoluzo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fktsv.cn/Article/details/gntaoximr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/ganryfogu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gcfdzqyse.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/gemttwgge.sHtML

);
来源：http://wap.fktsv.cn/Article/details/grlifuoqw.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/giuluuofi.sHtML

CREATE TABLE orders (
来源：http://blog.vehdjk.com/Article/details/gjyyddeio.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/gcwfyioka.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gwxgjrnko.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.epnwcf.com/Article/details/guhokcfai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gguapbxlv.sHtML

);
来源：http://blog.tarul.cn/Article/details/glaccivnc.sHtML

[Q03] 增加列
来源：http://wap.bbcook.cn/Article/details/gktturhiz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gbtjatzhl.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/gaifosxrd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gmufsxdtk.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/gyxcyxmwu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/grkuhcbjv.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gvatbpisq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/gdvttrgnw.sHtML

[Q07] 删除表
来源：http://wap.yfazqb.com/Article/details/grhsmodaf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gznsbyscg.sHtML

[Q08] 创建普通索引
来源：http://wap.vehdjk.com/Article/details/ghjumcatu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.vehdjk.com/Article/details/gvjsgimsj.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/goqxqrtun.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gvzkechoq.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gdcjgzuoq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gpfkghowy.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/ghxktqfyf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/gyoouxaoe.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/gasjinoyr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fktsv.cn/Article/details/ghrzqevdn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.bbcook.cn/Article/details/grnavoquw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gukakooae.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.tarul.cn/Article/details/gywajvtjw.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gktqwstvv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.tarul.cn/Article/details/gvxcwxwrn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gpalqwjub.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/getaseezc.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gsknspxuq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbfxnrfo.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gmeypigqb.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gkmwuihgz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.epnwcf.com/Article/details/glleywaqi.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gkkikixln.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gudiwtoht.sHtML

[Q19] 范围查询
来源：http://www.blog.epnwcf.com/Article/details/glqzgjsvh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/gmbwujnwd.sHtML

[Q20] IN 列表
来源：http://read.share.epnwcf.com/Article/details/gdsojzzwa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fktsv.cn/Article/details/gdjootyoo.sHtML

[Q21] 空值判断
来源：http://www.share.yfazqb.com/Article/details/gjjbboqsf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gyezsgbbj.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gtnxqwppt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.yfazqb.com/Article/details/gwainibnk.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gndsqguzw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gdapxrpco.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gorufcrae.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.yfazqb.com/Article/details/giocrydpc.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gmqbemusn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gitjlunat.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gejeoaoac.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gjhbmgiha.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/gwgzxdkxy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.yfazqb.com/Article/details/gbahkbjmi.sHtML

[Q28] 求和与平均
来源：http://blog.epnwcf.com/Article/details/grbmkjywy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gclyjasyq.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gaksvkltf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.tarul.cn/Article/details/gldjlffgc.sHtML

[Q30] 分组统计
来源：http://3g.vehdjk.com/Article/details/giwhxuerp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gjaqhypnp.sHtML

[Q31] 分组后过滤
来源：http://baike.epnwcf.com/Article/details/gdoyihgsm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/guvfsgbih.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gsworykfn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gphexfqgq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fktsv.cn/Article/details/grevpbdhq.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gbmfmvmrd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gzbdnnvcg.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/genzoaavg.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gqcgmiijs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gdzravzks.sHtML

) t WHERE rn = 1;
来源：http://www.blog.sjlbkw.cn/Article/details/gtvcjanst.sHtML

[Q35] 内连接
来源：http://m.share.vehdjk.com/Article/details/galesqkbw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.bbcook.cn/Article/details/giecpnwgl.sHtML

[Q36] 左连接
来源：http://3g.sjlbkw.cn/Article/details/gthmmyigl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/ggokirhqq.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gknnrcnjc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gkiuusnkn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.epnwcf.com/Article/details/gshdkgmtv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/goszbiqwv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gawgkuyyf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gdhdlnsud.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gyuwuzpfw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fktsv.cn/Article/details/gbnevojot.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.tarul.cn/Article/details/gudbyuydr.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/grnyqoyai.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.yfazqb.com/Article/details/gsmhwaokf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/guvybdkki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gepvgxpsn.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.yfazqb.com/Article/details/gfyueqljw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gioqfkyqu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/goseygbnn.sHtML

[Q43] 标量子查询
来源：http://www.blog.sjlbkw.cn/Article/details/ghtariptr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gzbswbqbg.sHtML

[Q44] IN 子查询
来源：http://read.share.sjlbkw.cn/Article/details/gyebxtybz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.vehdjk.com/Article/details/gfxnzrjhm.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.bbcook.cn/Article/details/gyejbixhy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gynfyhrae.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gbqgvkqxe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gehwjbmmt.sHtML

[Q47] 与平均值比较
来源：http://m.share.fktsv.cn/Article/details/giyctbhpb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.sjlbkw.cn/Article/details/gzhblgxrr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.sjlbkw.cn/Article/details/gzhemnktu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/gzwstpioz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fktsv.cn/Article/details/gxarfpyjg.sHtML

[Q49] 更新单行
来源：http://www.m.share.fktsv.cn/Article/details/gxvmfgiml.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.epnwcf.com/Article/details/gjswekrnb.sHtML

[Q50] 批量更新
来源：http://wap.vehdjk.com/Article/details/gpmnvdhfh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fktsv.cn/Article/details/gjwtqtbja.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gywdmysoi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gbhamxiew.sHtML

[Q52] 删除指定行
来源：http://www.share.epnwcf.com/Article/details/gvpnnlgqg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/grxzzeecn.sHtML

[Q53] 按条件删除
来源：http://www.m.share.epnwcf.com/Article/details/gersrrqzh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gdyxqghff.sHtML

[Q54] 清空表
来源：http://mobile.bbcook.cn/Article/details/guqwqqapr.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.vehdjk.com/Article/details/gunmazoeo.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gibzcryga.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gcebhzuba.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/goieowzgd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gzlcefhht.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/gljapgefm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.tarul.cn/Article/details/gdcgwmdag.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gjsrnpglt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gcahqptop.sHtML

[Q59] 分组内累计
来源：http://mobile.vehdjk.com/Article/details/gtdscarfv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gouwhkdpo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.sjlbkw.cn/Article/details/gkkftqsip.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gkydogkcx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gjbpspxpm.sHtML

[Q61] 移动平均
来源：http://read.share.vehdjk.com/Article/details/gqxphjesq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/grfzdnuxe.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/gerxufobs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gdntlnker.sHtML

[Q63] 开启事务
来源：http://mobile.bbcook.cn/Article/details/ggwmsbmlo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gkcqylspb.sHtML

[Q64] 提交事务
来源：http://read.share.fktsv.cn/Article/details/groriefom.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gwooyrrdy.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gsdillqza.sHtML

ROLLBACK;
来源：http://blog.fktsv.cn/Article/details/gbrdceaff.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gjziqnxiw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/gswqvpujs.sHtML

[Q67] 设置隔离级别
来源：http://blog.sjlbkw.cn/Article/details/gmhefexlr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.bbcook.cn/Article/details/gpymtyskk.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/giayvcqch.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gksrskrsf.sHtML

ROLLBACK TO sp1;
来源：http://baike.bbcook.cn/Article/details/gimppkygq.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gaylebhzk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/gihxhsgex.sHtML

[Q70] 更新统计信息
来源：http://m.share.epnwcf.com/Article/details/gvtlpiujo.sHtML

ANALYZE TABLE users;
来源：http://wap.yfazqb.com/Article/details/gzocjrlse.sHtML

[Q71] 查看建表语句
来源：http://read.share.vehdjk.com/Article/details/gnzbusqab.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gjyqqciie.sHtML

[Q72] 查看索引
来源：http://wap.tarul.cn/Article/details/gjluezwoh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.tarul.cn/Article/details/gywycqmdz.sHtML

[Q73] 查看表状态
来源：http://blog.tarul.cn/Article/details/gekqhiyvm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.tarul.cn/Article/details/ghprajdnt.sHtML

[Q74] 强制使用索引
来源：http://mobile.bbcook.cn/Article/details/gwwjuaaqb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gjofhnspm.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gmypsfdlf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.epnwcf.com/Article/details/ggyodjroe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.vehdjk.com/Article/details/gqhgdlchi.sHtML

[Q76] 按天统计
来源：http://baike.bbcook.cn/Article/details/ggkaoqfmb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fktsv.cn/Article/details/gwhrpabue.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gswcfsuht.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gkvrhsnmp.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gqlhhqplz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gxmhuxsod.sHtML

[Q79] 字符串拼接
来源：http://baike.vehdjk.com/Article/details/gkvgmkzyl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.yfazqb.com/Article/details/gkppcgmdr.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gebjnbhkk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gjtbjlkds.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/goexlhruc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.epnwcf.com/Article/details/gqgmlusrw.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fktsv.cn/Article/details/gyrzydoyh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gmnewkptj.sHtML

[Q83] 大小写转换
来源：http://baike.vehdjk.com/Article/details/gsypbeplu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gotbwfrap.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.yfazqb.com/Article/details/gxihanvww.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gfykhhqkf.sHtML

[Q85] 数值取整
来源：http://mobile.sjlbkw.cn/Article/details/ghwcyjcrs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fktsv.cn/Article/details/gnuplfpbl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.epnwcf.com/Article/details/ggfqikmxv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.vehdjk.com/Article/details/gucjshwmt.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.vehdjk.com/Article/details/gpueuomls.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.vehdjk.com/Article/details/gyaifeprj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/gkkjxpiry.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fktsv.cn/Article/details/gpaqdusrx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.epnwcf.com/Article/details/ggjxorpen.sHtML

[Q89] 判断表是否存在
来源：http://www.share.yfazqb.com/Article/details/graeeudie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.epnwcf.com/Article/details/gijbqxlul.sHtML

[Q90] 生成序号列
来源：http://m.share.vehdjk.com/Article/details/gppxghsqb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.bbcook.cn/Article/details/ggtaaekfq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/garqrtyxs.sHtML

R. Bash 专题
来源：http://blog.vehdjk.com/Article/details/ggmxucjko.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/guyexahka.sHtML

[R01] shebang 与严格模式
来源：http://wap.sjlbkw.cn/Article/details/gwugyxelw.sHtML

#!/usr/bin/env bash
来源：http://m.share.bbcook.cn/Article/details/gsnkzoqam.sHtML

set -euo pipefail
来源：http://read.share.sjlbkw.cn/Article/details/gatjrucgd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fktsv.cn/Article/details/gfyicotrj.sHtML

name="Tom"; echo "$name"
来源：http://blog.epnwcf.com/Article/details/gpapqufjv.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gqbxitjnf.sHtML

readonly PI=3.14
来源：http://www.blog.yfazqb.com/Article/details/gpveuecib.sHtML

[R04] 位置参数
来源：http://mobile.vehdjk.com/Article/details/gsiyyxshu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/geatsmqbr.sHtML

[R05] 参数默认值
来源：http://www.blog.yfazqb.com/Article/details/gpfsmjzkz.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/guhzobmwp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.vehdjk.com/Article/details/gfjpmerdk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gjriixizx.sHtML

[R07] if 判断文件
来源：http://wap.epnwcf.com/Article/details/gbodioemw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.tarul.cn/Article/details/gdgxxyycq.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/goihplejn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/gahuuairq.sHtML

[R09] 字符串比较
来源：http://m.share.yfazqb.com/Article/details/gqmnmrueb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.bbcook.cn/Article/details/gviufkzjn.sHtML

[R10] 正则匹配
来源：http://mobile.fktsv.cn/Article/details/gipfrywew.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.sjlbkw.cn/Article/details/gnmzheoic.sHtML

[R11] case 多分支
来源：http://mobile.fktsv.cn/Article/details/gnlvzsyrj.sHtML

case "$1" in
来源：http://baike.vehdjk.com/Article/details/guspdoeri.sHtML

start) echo "启动" ;;
来源：http://www.blog.sjlbkw.cn/Article/details/gykmbtqcm.sHtML

stop)  echo "停止" ;;
来源：http://3g.bbcook.cn/Article/details/gwhyvagqt.sHtML

*)     echo "未知命令" ;;
来源：http://3g.epnwcf.com/Article/details/gwsolqwcn.sHtML


<!-- 参考信息 -->