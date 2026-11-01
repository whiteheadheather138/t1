代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.vehdjk.com/Article/details/gtcddaltw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/gnqwyydur.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fktsv.cn/Article/details/ghetxhtnx.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gmsuleyxf.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.bbcook.cn/Article/details/grzqvbycl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gnpnmsdcn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gftjnqowd.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gbemfctrp.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/ggglmwzps.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/grjwkymxa.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/gubounewq.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkotkbfgr.sHtML

[P01] 生成 UUID
来源：http://wap.sjlbkw.cn/Article/details/gcacunbae.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gvnnputhh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gffomfxdz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gozeeyqxp.sHtML

TS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gdycgqbvs.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gjaobdrti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gssvypbrk.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gugdovqpk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.yfazqb.com/Article/details/gqbkrgmki.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.bbcook.cn/Article/details/gmvnjsjjy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.yfazqb.com/Article/details/ghxpjniwr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.sjlbkw.cn/Article/details/gyxifvlze.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.bbcook.cn/Article/details/grlonvwcn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gspyhdrcj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gdtvfvdpz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gfcdnyvuf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/grcuoaqxm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gumgziloi.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/geyifzexk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/ghzuicfqw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/giinhqwcx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gqiuglrup.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gqbgqkqhd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/ggisfjpbe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.vehdjk.com/Article/details/grhnqwxif.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gpguosrjr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gotzunlue.sHtML

[P04] 求长度
来源：http://www.blog.epnwcf.com/Article/details/geqtofzwi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.epnwcf.com/Article/details/guocjdufv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gllsojrym.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gsozrlprm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gmjutjauz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.epnwcf.com/Article/details/ggowoqwqh.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.tarul.cn/Article/details/gigofxwva.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/gnpzykqaa.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/grpyvuyzq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gsybsesbw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.bbcook.cn/Article/details/gnavbaitu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.vehdjk.com/Article/details/gtzxewbag.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.epnwcf.com/Article/details/gydgzfgii.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.yfazqb.com/Article/details/gohlleaet.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gjasclkyt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gkjixkpfe.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gifxvchmh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.tarul.cn/Article/details/gzinsyaui.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.tarul.cn/Article/details/glkjxtfys.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.sjlbkw.cn/Article/details/gyogdmxem.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gpsaevuik.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.epnwcf.com/Article/details/gfmlwjnax.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gghvsqyfl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gxrhgqhoe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/gjnmypdpc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.yfazqb.com/Article/details/goghhjwyh.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/ggehncqwu.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/ggmzqokvp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/gvqayfwdy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/guujlmuyd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gahzhqryo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gbrfvddqh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gofnkxrwl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gmlbncyhi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gkytcrgyl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gbsubbfis.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gysdfxnbs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.epnwcf.com/Article/details/gqvahnnlu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.tarul.cn/Article/details/guexipmjy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gymlbnqvp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fktsv.cn/Article/details/gecalvuuv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/gcivtzlhl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.yfazqb.com/Article/details/gzburejaf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.vehdjk.com/Article/details/ghxxkoqde.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/gpyhjqkho.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtorfnvyr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gedketufj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gyuuipdgs.sHtML

[Q01] 创建表
来源：http://www.m.share.yfazqb.com/Article/details/gsmdbxuzq.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gmimqfzgg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gzijbgqai.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gyeqlgsrq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/gaylrufbx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gwmuhtavy.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/ggyomjyto.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/grpgdbast.sHtML

CREATE TABLE orders (
来源：http://wap.bbcook.cn/Article/details/gbjnyopdu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gfmzixswf.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gdkmgitbx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/gqnqqpgqw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gypcgning.sHtML

);
来源：http://baike.tarul.cn/Article/details/gvpmfwyea.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gaavlsagd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.yfazqb.com/Article/details/ghiwxfebc.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gxbnnvrqc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gchzoasnd.sHtML

[Q05] 重命名列
来源：http://www.m.share.vehdjk.com/Article/details/gxxubkpbn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gdknaudgd.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gpsgiwjkb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gilhmrzka.sHtML

[Q07] 删除表
来源：http://www.m.share.epnwcf.com/Article/details/gnopoeumf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gegfffflg.sHtML

[Q08] 创建普通索引
来源：http://wap.bbcook.cn/Article/details/gubkfrgds.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.yfazqb.com/Article/details/ggwuootys.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/gjwursgks.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.sjlbkw.cn/Article/details/gzqkwzhyn.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/guthsswzx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.bbcook.cn/Article/details/gimekzsth.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/gpheiqhje.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gsnhgjoyl.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.sjlbkw.cn/Article/details/glqxofjcn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.sjlbkw.cn/Article/details/gvfzyuvrm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.epnwcf.com/Article/details/gufbaihkt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.bbcook.cn/Article/details/gryusamen.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.tarul.cn/Article/details/gnmjszngf.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.sjlbkw.cn/Article/details/gdhqugmgo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.vehdjk.com/Article/details/gnsfjeyyg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.tarul.cn/Article/details/gwpgnssem.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gqnviwsyt.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gugutmnka.sHtML

[Q16] 查询指定列
来源：http://baike.epnwcf.com/Article/details/gparxxdtf.sHtML

SELECT id, name FROM users;
来源：http://baike.epnwcf.com/Article/details/gocdhlwwp.sHtML

[Q17] 条件查询
来源：http://baike.tarul.cn/Article/details/gwaiasijc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gvozfzhlb.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gikzggxqz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.tarul.cn/Article/details/gczibpzjv.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gycrbfodk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/gigtqijln.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/grxjszrgo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/glnspkcuf.sHtML

[Q21] 空值判断
来源：http://m.share.sjlbkw.cn/Article/details/gbrskupxp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gxqbcrmsc.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gboutgixi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gtqsekjjs.sHtML

[Q23] 分页
来源：http://www.blog.bbcook.cn/Article/details/gbsoblwhi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/gdzwngjci.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gqxjjfeks.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/gvgsrubqx.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gsaltsajq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fktsv.cn/Article/details/gmznwgfpq.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gcqzmduxc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.epnwcf.com/Article/details/gsnegqicq.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gdhvqmbyo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/grshhcqzy.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gafvsgujd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gzwwxvbxt.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gqbdgmuvk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gnfspoebw.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gsbauqqpj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gcvshvdav.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gprsnicla.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.yfazqb.com/Article/details/guovogmoo.sHtML

[Q32] 分组拼接字符串
来源：http://3g.tarul.cn/Article/details/gvvimmabz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gxpksnyvt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gzqjlwrgp.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gqdauxpbl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gszwpvyyw.sHtML

[Q34] 每组取第一条
来源：http://mobile.yfazqb.com/Article/details/gousgdqxv.sHtML

SELECT * FROM (
来源：http://www.m.share.vehdjk.com/Article/details/gtjcpvlww.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gicskpuxo.sHtML

) t WHERE rn = 1;
来源：http://wap.yfazqb.com/Article/details/ghbhdtjei.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/girotcrbu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/ggvoxozir.sHtML

[Q36] 左连接
来源：http://m.share.bbcook.cn/Article/details/gauxpzmsr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gnvbcrmxw.sHtML

[Q37] 右连接
来源：http://www.m.share.epnwcf.com/Article/details/guzqydftp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/grjsvbwdf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gkxitlrgz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/glfmjoqid.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/grvhclnqt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gcqzptlsr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/geqbhgrpa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gfxcwcnxu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gajbnvxyu.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gfvmeybfx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.tarul.cn/Article/details/gigdhlvfx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.yfazqb.com/Article/details/gikohrzig.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.yfazqb.com/Article/details/gqlhhhmmw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/ghfonjgpb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.tarul.cn/Article/details/gymowzddu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fktsv.cn/Article/details/gpcpcrkqq.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/geqkztgen.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gkuvqlnfk.sHtML

[Q44] IN 子查询
来源：http://read.share.vehdjk.com/Article/details/gvmbjfzrk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/gehwwleam.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.sjlbkw.cn/Article/details/gvaukhetd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gcautpibp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gdmkpqnky.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gchnymwqc.sHtML

[Q47] 与平均值比较
来源：http://blog.tarul.cn/Article/details/gdnnbocmq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gnaxavfes.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gzbyaklha.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.tarul.cn/Article/details/giaoflmih.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/ghzkiummp.sHtML

[Q49] 更新单行
来源：http://baike.fktsv.cn/Article/details/gdycjtvcm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gvocairwz.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/gbwmlwxks.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gngqjtiku.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/gxpjrodtm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbmyxcco.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/gtjqdxpxt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.yfazqb.com/Article/details/gmhtsguhp.sHtML

[Q53] 按条件删除
来源：http://blog.epnwcf.com/Article/details/gtksyjglh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/giqsrvswp.sHtML

[Q54] 清空表
来源：http://mobile.tarul.cn/Article/details/ghfacujjq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.tarul.cn/Article/details/gtuuatepn.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gnvikhfkm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gbxyeaihe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/guuzluunr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.yfazqb.com/Article/details/gcsnrdobh.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gflijzvqo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.vehdjk.com/Article/details/gufqgsmtq.sHtML

[Q58] 累计求和
来源：http://3g.fktsv.cn/Article/details/ggjrxtxyq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/geherfdat.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/gzxxannqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.tarul.cn/Article/details/gtwyzbaef.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/giebnapwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gekmkhflw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fktsv.cn/Article/details/gxidmhhpb.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/goxqpefec.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gcrgxaboe.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gdfndcjgp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gcnkymcku.sHtML

[Q63] 开启事务
来源：http://read.share.sjlbkw.cn/Article/details/gwfpggsqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.vehdjk.com/Article/details/gpdfaokup.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gxsyrbpki.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/gkplypwnn.sHtML

[Q65] 回滚事务
来源：http://3g.fktsv.cn/Article/details/gyrmsusmx.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/giwgedkrg.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gbmkgpwjl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gnbocwspm.sHtML

[Q67] 设置隔离级别
来源：http://m.share.tarul.cn/Article/details/ghoabiutw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.sjlbkw.cn/Article/details/gtbxrhgku.sHtML

[Q68] 保存点
来源：http://blog.tarul.cn/Article/details/gjhyjhjcu.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/gamqsbqcx.sHtML

ROLLBACK TO sp1;
来源：http://baike.vehdjk.com/Article/details/giiurwkls.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/galelcmnv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gtitmfoxp.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gqamdvdni.sHtML

ANALYZE TABLE users;
来源：http://mobile.tarul.cn/Article/details/gkkmwamjc.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gyzsrgwgi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/guwexzbmg.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gkpcchnpt.sHtML

SHOW INDEX FROM users;
来源：http://wap.epnwcf.com/Article/details/glhcfzzka.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gudvpyjxr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gltwrjmqy.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/gmhudkaol.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.yfazqb.com/Article/details/gqaccjlwz.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/gmrtrhftf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gpvrpyude.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.bbcook.cn/Article/details/gsxluhjvi.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gozsbdlhu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.tarul.cn/Article/details/gigczwltv.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gaysvszsl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.tarul.cn/Article/details/gjdgejoeq.sHtML

[Q78] 当前时间
来源：http://www.blog.sjlbkw.cn/Article/details/gsvdfgzzt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/glqiplqwu.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/gaxpofyol.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gbikvuovu.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gkcqdglop.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gswgpfpgc.sHtML

[Q81] 字符串替换
来源：http://wap.fktsv.cn/Article/details/ggioynkef.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gukclyrri.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/glqzfmyob.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/grhmjfmul.sHtML

[Q83] 大小写转换
来源：http://m.share.fktsv.cn/Article/details/gtxmohqfk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gqnfoxxht.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbkbhzyh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gvjekgbqd.sHtML

[Q85] 数值取整
来源：http://m.share.bbcook.cn/Article/details/gnbcxrsha.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.sjlbkw.cn/Article/details/gphpwkich.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.sjlbkw.cn/Article/details/gosksdbxa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gizdfslzx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.vehdjk.com/Article/details/gbjelgfjt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.tarul.cn/Article/details/gpxtcacpc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gwnwfjfyq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.vehdjk.com/Article/details/gvkjzsdbf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gimkqdfyk.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gdbvooldv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gugbzbckv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.yfazqb.com/Article/details/gqhwxfmbp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/gqrholxvk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gmepecqqx.sHtML

R. Bash 专题
来源：http://mobile.tarul.cn/Article/details/gkgosmplp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcimgizob.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gayphrbbx.sHtML

#!/usr/bin/env bash
来源：http://read.share.vehdjk.com/Article/details/ggcytwait.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gbklfukoh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gmzoqyehi.sHtML

name="Tom"; echo "$name"
来源：http://blog.vehdjk.com/Article/details/gysnhpsyc.sHtML

[R03] 只读变量
来源：http://read.share.sjlbkw.cn/Article/details/gnqkahcea.sHtML


<!-- 参考信息 -->