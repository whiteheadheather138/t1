代发 wailian999

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gnamjgonq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/graxatkvu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.vehdjk.com/Article/details/gylbnxqeu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/ggtvrcsrp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/ginntuzip.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gudorllbs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gsquulekj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.vehdjk.com/Article/details/ggoelcjsc.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/guygieuws.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.vehdjk.com/Article/details/gkowqmxug.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gliatelmx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/gshvyjeep.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.epnwcf.com/Article/details/gyqxhjwis.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/ghmsnbkzw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gtbjmhppa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/ghunaavvc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/ghavpksze.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gevqaemgo.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gdgfmlgmc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gxceejfzf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gtfbywnxg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gyhhefydo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gyudpbwjd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.bbcook.cn/Article/details/grjtsyjhq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ggmxjuicw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/givigfxkv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.fktsv.cn/Article/details/gfzgmitkb.sHtML

[P04] 求长度
来源：http://read.share.yfazqb.com/Article/details/gtmfwiztp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gsvvnymnf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/glfgmzzml.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gcqnprgqi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gnsitanwb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.sjlbkw.cn/Article/details/guwvjipek.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gksfhkqpf.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/gsrnmgmsa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.epnwcf.com/Article/details/gtcimjhyk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/gngtracsa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.epnwcf.com/Article/details/grshkdlvh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gfjdlovdb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fktsv.cn/Article/details/gwhxnjksj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/gjtktajdd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/ghbmzcbwz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/gvefkiwwl.sHtML

Ruby: a == b
来源：http://read.share.epnwcf.com/Article/details/gewgtqhhe.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.vehdjk.com/Article/details/gqoexcvif.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fktsv.cn/Article/details/guuuesssw.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.fktsv.cn/Article/details/goullxhni.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.vehdjk.com/Article/details/ggyjbnpbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/gbdoifgnq.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gzihqitkz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gpbpvcysw.sHtML

Go:   if x == nil {}
来源：http://www.m.share.fktsv.cn/Article/details/gskaqaqsc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gvfawivtz.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gqfiutuoc.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gsfdidwij.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gvsvuyhku.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/guzuwlyau.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gufppwfaa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gcjbofppl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gfhwqugzf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.tarul.cn/Article/details/gjdygvany.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/gwktkzmfi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gphqtdpae.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/gyczrnsxv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gzvsqoneo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.yfazqb.com/Article/details/gvdpygvbd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.vehdjk.com/Article/details/gqiwvjmiw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fktsv.cn/Article/details/gukbibmwl.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.sjlbkw.cn/Article/details/geqehtmvo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gsvhoweke.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gpnzaafyp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/gfzcbrsit.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ghamexgbm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gjfqmxmmc.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gfbgmgkgv.sHtML

[Q01] 创建表
来源：http://www.share.vehdjk.com/Article/details/gslwgoodv.sHtML

CREATE TABLE users (
来源：http://m.share.fktsv.cn/Article/details/gdbtjioyr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/gwctmywns.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gshgatjgo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/ghbeierbj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gerbuylhq.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gatderjtt.sHtML

[Q02] 创建带外键的表
来源：http://baike.fktsv.cn/Article/details/gilppadsi.sHtML

CREATE TABLE orders (
来源：http://www.share.bbcook.cn/Article/details/gzpebigyu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gmbogmiva.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gdliuhbdx.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gyrkcvmeo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gktinruhe.sHtML

);
来源：http://blog.epnwcf.com/Article/details/guekkynae.sHtML

[Q03] 增加列
来源：http://blog.bbcook.cn/Article/details/gaogohhlm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gxitljhve.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gegxfwato.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.bbcook.cn/Article/details/gydfavkmg.sHtML

[Q05] 重命名列
来源：http://m.share.bbcook.cn/Article/details/glcrmlgbs.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gwfqvxlmp.sHtML

[Q06] 删除列
来源：http://www.blog.bbcook.cn/Article/details/gszqoxebt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gwahkfnzu.sHtML

[Q07] 删除表
来源：http://3g.vehdjk.com/Article/details/gfjlscqnt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.fktsv.cn/Article/details/gwnfvreae.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gqbrthhzs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gdbttlhto.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gzjpvdvqs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gpfcdquey.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/gorbmcszm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/guhcnpgbb.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gycujeurx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gthmbrodi.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/goywedzfq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gweoxorcs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gfdvxrivi.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/ggsrkwnlm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gmxgmvmtv.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.epnwcf.com/Article/details/gpruelijy.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/geiwiggxr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fktsv.cn/Article/details/gmuftjqrd.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gqabkzlni.sHtML

SELECT * FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/goqpyzqck.sHtML

[Q16] 查询指定列
来源：http://blog.epnwcf.com/Article/details/ghystlofo.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gtpxmrize.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/glqiuzjby.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gzcumpppw.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/gaaxifcmf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.yfazqb.com/Article/details/gnmdlnnrz.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/gmmlycben.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.epnwcf.com/Article/details/gdnjgjfrx.sHtML

[Q20] IN 列表
来源：http://read.share.fktsv.cn/Article/details/gtlfucajx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gbuccrsyi.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/gdlchexff.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.yfazqb.com/Article/details/gyotxswvq.sHtML

[Q22] 排序
来源：http://www.share.bbcook.cn/Article/details/gcyzvwgpx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gjzbgunaz.sHtML

[Q23] 分页
来源：http://wap.yfazqb.com/Article/details/gszorodmo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gmikiowkq.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/glcnujbsz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gjraqwlek.sHtML

[Q25] 只取前 N 条
来源：http://mobile.sjlbkw.cn/Article/details/gwnlyfrnh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/guwrlnnel.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/ghhpobiex.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/gyqfokitb.sHtML

[Q27] 条件计数
来源：http://baike.tarul.cn/Article/details/gavunvfle.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/ghlawyvlb.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/gyxupkhyt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/grzqycgep.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gzjwbkmqd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.tarul.cn/Article/details/gearevkzy.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/gxpxbbysg.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.yfazqb.com/Article/details/gghbxdpwx.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gjgsklvzl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.vehdjk.com/Article/details/gedgwqeoj.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gwjgzhayg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.sjlbkw.cn/Article/details/gedvssxxd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.tarul.cn/Article/details/gshaiwvnw.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gaqzdlmcp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gppqbzweb.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fktsv.cn/Article/details/gwertqqxe.sHtML

SELECT * FROM (
来源：http://baike.sjlbkw.cn/Article/details/gktbtcgsf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/glwmtoahm.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gsiywhiya.sHtML

[Q35] 内连接
来源：http://3g.epnwcf.com/Article/details/gtshnmbbb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzvtnqzw.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gcmkllmlk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.bbcook.cn/Article/details/glhizmayb.sHtML

[Q37] 右连接
来源：http://blog.tarul.cn/Article/details/gnmjhkghb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gfoqwajeh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.fktsv.cn/Article/details/gzpmsryjs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gjzjofacw.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/grmbyswor.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gassyirth.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gfxorzetb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.bbcook.cn/Article/details/gvdmrpnbn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/gswmetpvs.sHtML

[Q41] 多表连接
来源：http://www.share.fktsv.cn/Article/details/gsnsnwcgs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/grfqscrha.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/gtdxkcllo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gwwgioaed.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gqxtwcpuw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gqxnieqsp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/ghwrncgbf.sHtML

[Q43] 标量子查询
来源：http://3g.bbcook.cn/Article/details/gidykqthx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gvldpiosg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gwjgiofde.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gdusqulia.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gdjrhevme.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.tarul.cn/Article/details/gtbcbkfjh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fktsv.cn/Article/details/ghvvaxtzo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gedpyekvy.sHtML

[Q47] 与平均值比较
来源：http://www.share.tarul.cn/Article/details/gusirweax.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fktsv.cn/Article/details/gjjnsdjsx.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gbqlmjfec.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.tarul.cn/Article/details/gbiwnouue.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.yfazqb.com/Article/details/gjkkxbjfe.sHtML

[Q49] 更新单行
来源：http://www.m.share.yfazqb.com/Article/details/ghgktxnxh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.epnwcf.com/Article/details/gauhpmwqw.sHtML

[Q50] 批量更新
来源：http://m.share.tarul.cn/Article/details/gkmdgtpla.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gyzgyjbif.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gbpoohxfr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/gnfbjzvdz.sHtML

[Q52] 删除指定行
来源：http://blog.fktsv.cn/Article/details/guukuynot.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbceidudr.sHtML

[Q53] 按条件删除
来源：http://www.blog.vehdjk.com/Article/details/gxggijmrk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gedtqhopi.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gvjtjafmo.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gcmaxtwwj.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/ghfqacajy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.tarul.cn/Article/details/groyjsiwf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/geojkqmev.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gyeobzbqv.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gsdfqghtg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.bbcook.cn/Article/details/gnocwdgta.sHtML

[Q58] 累计求和
来源：http://www.blog.yfazqb.com/Article/details/gllczvjos.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gxvupaiuy.sHtML

[Q59] 分组内累计
来源：http://blog.bbcook.cn/Article/details/gydneljmb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gyihwkvhs.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gwfpvjnhl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/gjrlzjvpv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/ghxqxutcy.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/gcccqbdld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gdxqyxmcx.sHtML

[Q62] 分组占比
来源：http://mobile.epnwcf.com/Article/details/gxlrcriai.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gazkjnses.sHtML

[Q63] 开启事务
来源：http://3g.tarul.cn/Article/details/glfirzqgo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fktsv.cn/Article/details/gbefdpcdk.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gpkfkptxs.sHtML

COMMIT;
来源：http://www.share.sjlbkw.cn/Article/details/gxjuryfem.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gazlfcvgg.sHtML

ROLLBACK;
来源：http://wap.bbcook.cn/Article/details/gczfakrcl.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gjobrnhkb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.tarul.cn/Article/details/gpxejsuxo.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.bbcook.cn/Article/details/guxuvqhbz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/gudvpzfml.sHtML

[Q68] 保存点
来源：http://read.share.epnwcf.com/Article/details/gzzatprso.sHtML

SAVEPOINT sp1;
来源：http://www.share.sjlbkw.cn/Article/details/goymiyayg.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gipokjjxf.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/ggljgotwt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.vehdjk.com/Article/details/gzmvzrgwf.sHtML

[Q70] 更新统计信息
来源：http://3g.sjlbkw.cn/Article/details/gvstcyslv.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/gczbjauog.sHtML

[Q71] 查看建表语句
来源：http://mobile.yfazqb.com/Article/details/gpelzfocj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/gghgjszcp.sHtML

[Q72] 查看索引
来源：http://baike.tarul.cn/Article/details/gbaatbffm.sHtML

SHOW INDEX FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gxbjarfcj.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/ggcpwzsro.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fktsv.cn/Article/details/gqrqvxkrl.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/gizxnicsb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gpaslclww.sHtML

[Q75] 日期格式化
来源：http://www.share.fktsv.cn/Article/details/ghjvavvhl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gqqqupvkp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.sjlbkw.cn/Article/details/gzszwwanz.sHtML

[Q76] 按天统计
来源：http://3g.yfazqb.com/Article/details/ghyyxrbcs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.tarul.cn/Article/details/gjklklkfv.sHtML

[Q77] 时间加减
来源：http://www.share.bbcook.cn/Article/details/glmozivou.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.epnwcf.com/Article/details/gdtzwletf.sHtML

[Q78] 当前时间
来源：http://mobile.tarul.cn/Article/details/gooaslhmd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.sjlbkw.cn/Article/details/gpfotnzws.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/glgkrxqrd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.sjlbkw.cn/Article/details/gsbxarajp.sHtML

[Q80] 字符串截取
来源：http://3g.tarul.cn/Article/details/gycamhbas.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.tarul.cn/Article/details/gbpffvbbs.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gnqsgvibt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.vehdjk.com/Article/details/gxpawjcei.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fktsv.cn/Article/details/gemphcabd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/ghymudkqj.sHtML

[Q83] 大小写转换
来源：http://mobile.bbcook.cn/Article/details/gqvhjjsxr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gbyrpjybh.sHtML

[Q84] 去除首尾空格
来源：http://blog.sjlbkw.cn/Article/details/gjvuabiiw.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gyjqhhlgk.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/gpbgbztlo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/gxznuvafh.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.sjlbkw.cn/Article/details/gnrawfkpw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.yfazqb.com/Article/details/gzjmkpyek.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.yfazqb.com/Article/details/gutyxcegu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.vehdjk.com/Article/details/gmamvuhfh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.yfazqb.com/Article/details/gkovsvzda.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fktsv.cn/Article/details/ggkitaiva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.epnwcf.com/Article/details/gvenbadap.sHtML

[Q89] 判断表是否存在
来源：http://baike.sjlbkw.cn/Article/details/gqeinculv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.sjlbkw.cn/Article/details/gzilrefuo.sHtML

[Q90] 生成序号列
来源：http://www.blog.yfazqb.com/Article/details/goenxwfty.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gcabdwxgt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gtxiyroyf.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gqdvgqbql.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ginhtuzdc.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gvchrpwgp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.vehdjk.com/Article/details/gasfidvpt.sHtML

set -euo pipefail
来源：http://blog.yfazqb.com/Article/details/gjpmplwoe.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/gihdmjude.sHtML

name="Tom"; echo "$name"
来源：http://read.share.epnwcf.com/Article/details/ggpjwrjfl.sHtML

[R03] 只读变量
来源：http://www.blog.tarul.cn/Article/details/gwqrtklbg.sHtML

readonly PI=3.14
来源：http://blog.sjlbkw.cn/Article/details/gyytsuqjd.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gwbjxfclm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fktsv.cn/Article/details/gahthqdug.sHtML

[R05] 参数默认值
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzdrluwe.sHtML

name="${1:-default}"
来源：http://www.share.epnwcf.com/Article/details/gapmejvdt.sHtML

[R06] 判断命令是否存在
来源：http://blog.epnwcf.com/Article/details/gpblkiwfn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.tarul.cn/Article/details/gfaqtqgax.sHtML

[R07] if 判断文件
来源：http://mobile.fktsv.cn/Article/details/ghujjrygu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gexckbvwp.sHtML

[R08] 数值比较
来源：http://wap.fktsv.cn/Article/details/gwsjexktg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gwlhzcufd.sHtML

[R09] 字符串比较
来源：http://read.share.tarul.cn/Article/details/gmgcqxppw.sHtML


<!-- 参考信息 -->