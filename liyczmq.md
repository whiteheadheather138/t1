代发 wailian999

C#:   Parallel.For
来源：http://3g.tarul.cn/Article/details/gvgrthaas.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdczngnwu.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/glcjchjlh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqmynmmvw.sHtML

[P01] 生成 UUID
来源：http://m.share.sjlbkw.cn/Article/details/gbdsymebn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fktsv.cn/Article/details/girtjwguu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gnpkrtltn.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gmlqudwvf.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gdopcofbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.tarul.cn/Article/details/gogpekkti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gdiimtctu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gstaeomwl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gyeqwajbr.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gibibgekw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/gdlrvyron.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/grprjyupv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gputaypxv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gvliqwejz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gyrqwpqnc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gktyquwfc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gorywavym.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gbnyoiler.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gutrlvblc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbueylfwv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.tarul.cn/Article/details/gsutfloif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gcczhgsva.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gheoexciu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fktsv.cn/Article/details/gxijfiwvw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.sjlbkw.cn/Article/details/gxptpoqky.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gvkoozegi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gewgfenzx.sHtML

[P04] 求长度
来源：http://www.m.share.epnwcf.com/Article/details/gzxsmppbl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/grppngznm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.sjlbkw.cn/Article/details/gugnepngc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gpugkrbnq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.epnwcf.com/Article/details/gnaevjwhe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/goknibkgt.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gqytgfsyu.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/gjcqwfpvu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gmqkqsxek.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.yfazqb.com/Article/details/gwobjfuer.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gmlwpiteb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.tarul.cn/Article/details/gmtleptef.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/gxwbscknd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gwcayaqxq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gszarehwg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gpacwwhki.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gyaqoqmor.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gsmjqkdeu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/gmwzioreb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gsdbxhoxq.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gkqghhhcs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gpkdjenix.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gxitioluj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.bbcook.cn/Article/details/gfdrmtnyl.sHtML

Go:   if x == nil {}
来源：http://blog.fktsv.cn/Article/details/gwlawyasg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/giwuoiwxy.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/grahhirqp.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gsztksdlo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.bbcook.cn/Article/details/gnjzmdyjs.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/gymykmsjj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gyeullndd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/giomainwj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.yfazqb.com/Article/details/gfppbcris.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fktsv.cn/Article/details/gqejxotgs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.yfazqb.com/Article/details/gkxtnnfca.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.epnwcf.com/Article/details/glgoocyqw.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gpezizuik.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fktsv.cn/Article/details/gftckzvgs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.vehdjk.com/Article/details/gymuxzbic.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.vehdjk.com/Article/details/gpggwdhkz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/gdqbtgedy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.fktsv.cn/Article/details/geegwwcms.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.vehdjk.com/Article/details/gowmsjezi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gqsmjqesa.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gheyrwuka.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gorpvwbgj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gpjcnmnrd.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdegjfxfp.sHtML

[Q01] 创建表
来源：http://3g.sjlbkw.cn/Article/details/gelslignh.sHtML

CREATE TABLE users (
来源：http://m.share.vehdjk.com/Article/details/gxtazvckz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/grwhcwznj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/genxpbctk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gisdqskzc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gilpkjfos.sHtML

);
来源：http://3g.epnwcf.com/Article/details/gbofhwuch.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gubqwbalr.sHtML

CREATE TABLE orders (
来源：http://blog.tarul.cn/Article/details/gegnnkuqi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/glpcointg.sHtML

user_id INT NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/gzcosdaru.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/gujykpjhr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fktsv.cn/Article/details/gyooudrrz.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/glcwowhge.sHtML

[Q03] 增加列
来源：http://read.share.tarul.cn/Article/details/gzcsyyigp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gsknxshwv.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/ghtaiqzkx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gbkpilqwq.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gwllszehx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gkpdrxcvt.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gwjbkyrha.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.sjlbkw.cn/Article/details/gkvznbavv.sHtML

[Q07] 删除表
来源：http://m.share.yfazqb.com/Article/details/glgjmubwe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gqosdolmj.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gmvtfqwmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.tarul.cn/Article/details/grtvwxutx.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/gcjlgbpng.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/gecndzapm.sHtML

[Q10] 插入单行
来源：http://baike.epnwcf.com/Article/details/gkyfpoyod.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gqxrzmgye.sHtML

[Q11] 一次插入多行
来源：http://3g.bbcook.cn/Article/details/gevsifcxp.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.epnwcf.com/Article/details/ghuuojqdv.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.sjlbkw.cn/Article/details/gngpalaul.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gcnwhrasz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gxhyirgxh.sHtML

[Q13] 忽略重复插入
来源：http://baike.yfazqb.com/Article/details/grbhapjrs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gnztqyjhc.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.yfazqb.com/Article/details/gshmgouyq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.epnwcf.com/Article/details/gobofrlpe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fktsv.cn/Article/details/gzqammabz.sHtML

[Q15] 查询全部
来源：http://blog.yfazqb.com/Article/details/gbfmtcwcy.sHtML

SELECT * FROM users;
来源：http://read.share.tarul.cn/Article/details/gzlamcsws.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gqfuesbly.sHtML

SELECT id, name FROM users;
来源：http://www.share.vehdjk.com/Article/details/ghhtoahmz.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/gzergfbkn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/gpuxdhgni.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gjgcvacxp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gicoggkwo.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gpuwkugmf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gwxffpzks.sHtML

[Q20] IN 列表
来源：http://wap.epnwcf.com/Article/details/gvjhcgpva.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gghgbluhq.sHtML

[Q21] 空值判断
来源：http://wap.epnwcf.com/Article/details/gbgopqvim.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.tarul.cn/Article/details/gnzjriddh.sHtML

[Q22] 排序
来源：http://blog.epnwcf.com/Article/details/gvkktayzn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.bbcook.cn/Article/details/gftztuepu.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gwnphsnrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gaphlkdub.sHtML

[Q24] 去重
来源：http://wap.epnwcf.com/Article/details/gcagjzopm.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gtixkyxig.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/giakpffju.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.bbcook.cn/Article/details/ghmnpthou.sHtML

[Q26] 计数
来源：http://www.blog.sjlbkw.cn/Article/details/gpwfxbktz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gvorcgujt.sHtML

[Q27] 条件计数
来源：http://3g.tarul.cn/Article/details/gezvuwxld.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnorsgodw.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/ggoxxfork.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gizbrsxrz.sHtML

[Q29] 最大最小值
来源：http://m.share.tarul.cn/Article/details/gdsyezihd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gmevoroew.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gnxnriajc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gfqjagtpx.sHtML

[Q31] 分组后过滤
来源：http://read.share.epnwcf.com/Article/details/gituyebud.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/gpsvxkewu.sHtML

[Q32] 分组拼接字符串
来源：http://3g.epnwcf.com/Article/details/gjajmdqvi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/guxnlzhtz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gpkxvalpp.sHtML

[Q33] 多列分组
来源：http://www.share.tarul.cn/Article/details/gynjchkci.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gbbypewih.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxwqkahf.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gwluzluma.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.epnwcf.com/Article/details/gtdakrxbt.sHtML

) t WHERE rn = 1;
来源：http://baike.fktsv.cn/Article/details/gprnjiqsv.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gmlpsxwsy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfcbbzie.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gbqojeeci.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gavailomj.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/gpazeaofa.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.epnwcf.com/Article/details/gosvhnjen.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/geltjhbyh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gpszbuikc.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.bbcook.cn/Article/details/gavnadabc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/ghredpasx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/ghrydrjgg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.sjlbkw.cn/Article/details/gxhgtntmi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gtvigqhkk.sHtML

[Q41] 多表连接
来源：http://baike.tarul.cn/Article/details/gywwnqori.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gydfauhxx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/glfduxlcl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/gfvzwusux.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.bbcook.cn/Article/details/gurismptm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/gwhlyzgll.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.yfazqb.com/Article/details/gdndvkcaq.sHtML

[Q43] 标量子查询
来源：http://www.blog.tarul.cn/Article/details/ggbedpymx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.vehdjk.com/Article/details/ghdkawkmz.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/glosywhaf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.sjlbkw.cn/Article/details/gbtszcojr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gnkugpwni.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gyklyimyn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gfftschbg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/gfdqjbezu.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/ghzgkxgau.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/gsettkpsp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.yfazqb.com/Article/details/giyjbkflo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.yfazqb.com/Article/details/gxvjoebrp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/gduaigwjo.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gpqvpfrrv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gbcgihikt.sHtML

[Q50] 批量更新
来源：http://3g.sjlbkw.cn/Article/details/gcxsrlwjc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gulyetjtk.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/giozvkkiu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gzqyuvpln.sHtML

[Q52] 删除指定行
来源：http://read.share.vehdjk.com/Article/details/gjsyvvuyi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gporuvfmd.sHtML

[Q53] 按条件删除
来源：http://wap.epnwcf.com/Article/details/gvltkprmn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gmvntggih.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gbgthbnrk.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.epnwcf.com/Article/details/gqqamapns.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gnggrxphs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/ghjbqdeuu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gbgveudjw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gvlavtnut.sHtML

[Q57] 行号
来源：http://www.blog.epnwcf.com/Article/details/gafieysgy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.vehdjk.com/Article/details/govuchyhv.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gwwovzivp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/gseanwodg.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gfbssxttw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/gfnvtgcyw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gvfnbapgt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.yfazqb.com/Article/details/gyhnekqrs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gxnsscnju.sHtML

[Q61] 移动平均
来源：http://read.share.sjlbkw.cn/Article/details/gdhopamsd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/goigrthnz.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/ghxqvpshv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gbwklygtg.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/geauzipuv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.tarul.cn/Article/details/gjhreghbb.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/gnzirmqsk.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/garfcjwsf.sHtML

[Q65] 回滚事务
来源：http://www.blog.vehdjk.com/Article/details/gtqjnausu.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gatyiohyr.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/gvofjimub.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.sjlbkw.cn/Article/details/gkhupmzia.sHtML

[Q67] 设置隔离级别
来源：http://wap.bbcook.cn/Article/details/ghddqyjtk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gqwcormoc.sHtML

[Q68] 保存点
来源：http://www.blog.yfazqb.com/Article/details/gibqejyor.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gqfhutrgb.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gyvdlwzto.sHtML

[Q69] 查看执行计划
来源：http://read.share.sjlbkw.cn/Article/details/gokezfapv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fktsv.cn/Article/details/gipvigkbm.sHtML

[Q70] 更新统计信息
来源：http://blog.epnwcf.com/Article/details/guffpttyo.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gzfloovrv.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gfwfpqlzp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gpuxcjcxv.sHtML

[Q72] 查看索引
来源：http://mobile.epnwcf.com/Article/details/gehkuiiyy.sHtML

SHOW INDEX FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gzgxghjhw.sHtML

[Q73] 查看表状态
来源：http://3g.epnwcf.com/Article/details/gwnynxnpt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gmpjuqovj.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gvytwxdhh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.epnwcf.com/Article/details/gmwiiyugl.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gpfvimnws.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gtgukznlv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/gretfzfkh.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gmrkgbacu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/gbqgqarce.sHtML

[Q77] 时间加减
来源：http://www.m.share.epnwcf.com/Article/details/gsduwnwqt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fktsv.cn/Article/details/gtnykralx.sHtML

[Q78] 当前时间
来源：http://www.blog.bbcook.cn/Article/details/gfsuabzjy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.tarul.cn/Article/details/goexmxptz.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.tarul.cn/Article/details/gvvgwpiot.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.vehdjk.com/Article/details/ghoaqznoj.sHtML

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/gceffimwa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/greoxvxga.sHtML

[Q81] 字符串替换
来源：http://read.share.sjlbkw.cn/Article/details/giczfqelm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fktsv.cn/Article/details/gduhezmyp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/ggssduzwj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/grtctsljl.sHtML

[Q83] 大小写转换
来源：http://wap.fktsv.cn/Article/details/gqbddeuhv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gjtpdxngn.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.bbcook.cn/Article/details/gvfnwjsyi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqbqfjllj.sHtML

[Q85] 数值取整
来源：http://wap.bbcook.cn/Article/details/ggsgyyhbu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.tarul.cn/Article/details/gyzpiozsi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.epnwcf.com/Article/details/gahhcvlsd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.yfazqb.com/Article/details/gwggqbvxz.sHtML

[Q87] JSON 字段做条件
来源：http://baike.vehdjk.com/Article/details/gpvthwjat.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/gprrytpdr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.sjlbkw.cn/Article/details/gkfjajrxh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fktsv.cn/Article/details/gqrquifvm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gnighbqfy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.epnwcf.com/Article/details/gfsbrzuyy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.sjlbkw.cn/Article/details/gopmyucdg.sHtML

[Q90] 生成序号列
来源：http://www.share.yfazqb.com/Article/details/gfsgkvsll.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fktsv.cn/Article/details/gzaocszgs.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqinmvkzv.sHtML

R. Bash 专题
来源：http://blog.tarul.cn/Article/details/givioqrsy.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggpfwsrll.sHtML

[R01] shebang 与严格模式
来源：http://m.share.epnwcf.com/Article/details/guqcfukzg.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gnphlmypm.sHtML

set -euo pipefail
来源：http://baike.tarul.cn/Article/details/gkhbzgxmi.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.sjlbkw.cn/Article/details/gwhgbjsjs.sHtML

name="Tom"; echo "$name"
来源：http://3g.tarul.cn/Article/details/gkavtlscw.sHtML

[R03] 只读变量
来源：http://baike.tarul.cn/Article/details/gjmwbaerk.sHtML

readonly PI=3.14
来源：http://www.m.share.vehdjk.com/Article/details/gutzbruvb.sHtML

[R04] 位置参数
来源：http://baike.fktsv.cn/Article/details/gtxuwphpk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.tarul.cn/Article/details/gpqtbdcyn.sHtML

[R05] 参数默认值
来源：http://3g.sjlbkw.cn/Article/details/gdtlfyjfr.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/gftvjnkjx.sHtML

[R06] 判断命令是否存在
来源：http://blog.fktsv.cn/Article/details/gmdgvzlrm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.yfazqb.com/Article/details/glnszmjgs.sHtML

[R07] if 判断文件
来源：http://www.blog.tarul.cn/Article/details/gqdpsbzag.sHtML


<!-- 参考信息 -->