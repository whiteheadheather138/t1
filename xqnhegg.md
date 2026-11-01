代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gfbdapcfg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gueexezwy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gghvbeqbc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.bbcook.cn/Article/details/ggyhnyazn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gujwzigrt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gbjuchnon.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/glwmcyszy.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.bbcook.cn/Article/details/gwxzrrdzy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gthjqyptk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gwpslrmlg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.tarul.cn/Article/details/grttpxjws.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.sjlbkw.cn/Article/details/gkxevogdd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/glehczavz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/ggecfwlnh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/glxyrnrah.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.epnwcf.com/Article/details/ghzczhoaj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.tarul.cn/Article/details/gwojaqeyu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gpjfjcqrr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/geenzbnuc.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gepmlkmao.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/gshsbhheo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gohwxnxyn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/glxuznhyq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gsooqheif.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/ghjqdnjgt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.yfazqb.com/Article/details/ghvtthbqs.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gcuzteoum.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/ghlobwhsq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/ghelpdwia.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/grfaydigc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gdqlqylks.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/gwbvhsqdp.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gvyjlslvy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.yfazqb.com/Article/details/glckmnnhg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.bbcook.cn/Article/details/glhhgsxrr.sHtML

Ruby: a == b
来源：http://www.m.share.epnwcf.com/Article/details/gzwbgyubs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gldxggyxl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/ghlwbjutl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/gfkkcgdfk.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.sjlbkw.cn/Article/details/gipbjxplg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/glrokadcn.sHtML

TS:   if (x == null) {}
来源：http://wap.tarul.cn/Article/details/gtxdbdtxh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gzqwzhhwd.sHtML

Go:   if x == nil {}
来源：http://baike.tarul.cn/Article/details/grwtrmizm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.yfazqb.com/Article/details/gtztiwirp.sHtML

C#:   if (x is null) {}
来源：http://baike.fktsv.cn/Article/details/gdrsvmgnm.sHtML

[P07] 防抖与节流
来源：http://m.share.yfazqb.com/Article/details/gbdfexfvi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gzfosacrx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/gbvmcinfl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.tarul.cn/Article/details/gidakkfod.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/ghccrqtvw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fktsv.cn/Article/details/ghktcrirh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.bbcook.cn/Article/details/gfnjfzvdy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/getbmrjpm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fktsv.cn/Article/details/grkhmsgfz.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/guuragaga.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.sjlbkw.cn/Article/details/ghxwbbzvk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.yfazqb.com/Article/details/gkolwhzav.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/grwgussep.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/gtccndlrr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gpqjufqhu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.sjlbkw.cn/Article/details/gyzdhckox.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.sjlbkw.cn/Article/details/goebkgqio.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/grleofkkm.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhtecacp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/gbwrjrblp.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyvunvckm.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/gqqthsbtj.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gifygybfv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.bbcook.cn/Article/details/gjumffyqv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.sjlbkw.cn/Article/details/gpdruyors.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/gounxavrr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.tarul.cn/Article/details/gyggikmaf.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gydhdibxt.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/geastlsfn.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/gaqtaozwx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gpkmywpcb.sHtML

user_id INT NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gwpbuhyaz.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gtczrwhxz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.vehdjk.com/Article/details/gebawruvh.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gluwanxbz.sHtML

[Q03] 增加列
来源：http://3g.bbcook.cn/Article/details/gxutyjhvo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.vehdjk.com/Article/details/gonizihmk.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gfozpxjjo.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gnionntfc.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/giibezjvt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/glcwiwxzt.sHtML

[Q06] 删除列
来源：http://read.share.fktsv.cn/Article/details/gdztbiyes.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gqhbmblmv.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/grgjtugcl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.epnwcf.com/Article/details/glcwkmrtx.sHtML

[Q08] 创建普通索引
来源：http://www.blog.epnwcf.com/Article/details/guqqatjwu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/ggdjenwjc.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gmrycejqi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/grdcudabr.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/gmoqccloq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/gxooqwruc.sHtML

[Q11] 一次插入多行
来源：http://3g.fktsv.cn/Article/details/gjxwvgmwv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/ghuvsjozf.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gbcltborb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gtbauymnp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.tarul.cn/Article/details/ggchwhijt.sHtML

[Q13] 忽略重复插入
来源：http://m.share.tarul.cn/Article/details/gsdfhrtqq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.epnwcf.com/Article/details/gawlrvrun.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.epnwcf.com/Article/details/gxpuyzhlv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/gioenpiyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.epnwcf.com/Article/details/gjbijtsvf.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/guzrtmyue.sHtML

SELECT * FROM users;
来源：http://wap.bbcook.cn/Article/details/ggsulnalv.sHtML

[Q16] 查询指定列
来源：http://blog.tarul.cn/Article/details/gvjmhstmi.sHtML

SELECT id, name FROM users;
来源：http://baike.bbcook.cn/Article/details/glsktrynv.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/goayduiug.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/ggxunthlj.sHtML

[Q18] 模糊匹配
来源：http://baike.sjlbkw.cn/Article/details/gbzoyisxp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/githflvss.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gguunnyty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.tarul.cn/Article/details/gyzwprovo.sHtML

[Q20] IN 列表
来源：http://m.share.vehdjk.com/Article/details/gcjrwjavi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gsellswtc.sHtML

[Q21] 空值判断
来源：http://www.m.share.fktsv.cn/Article/details/gwiyyweqd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/ghqlfmsot.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/grrgybrnu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.sjlbkw.cn/Article/details/gfkwgeybr.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gybaahxxt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/grxrqhugh.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gprgjmret.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/ggsttlspm.sHtML

[Q25] 只取前 N 条
来源：http://blog.epnwcf.com/Article/details/giswwpvmp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.sjlbkw.cn/Article/details/gulbfueie.sHtML

[Q26] 计数
来源：http://baike.yfazqb.com/Article/details/gjegthqxz.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxqqbfedq.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gyjtcccnz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fktsv.cn/Article/details/gxeekeclx.sHtML

[Q28] 求和与平均
来源：http://read.share.vehdjk.com/Article/details/gmbdexbkd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gpjizityi.sHtML

[Q29] 最大最小值
来源：http://3g.sjlbkw.cn/Article/details/grxrvdwai.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.epnwcf.com/Article/details/guglpaiqx.sHtML

[Q30] 分组统计
来源：http://www.m.share.yfazqb.com/Article/details/gtzfmcvsh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gvrvpdezu.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gapsfjmnu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/gjidxmhkq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.sjlbkw.cn/Article/details/gcxhljkuc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gnxbewugk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.vehdjk.com/Article/details/gpkwsfddb.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/ggnktlhtq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gsyvuglkf.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gyscwrowk.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/ggnxuvqov.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/gedncgrjg.sHtML

) t WHERE rn = 1;
来源：http://baike.sjlbkw.cn/Article/details/gktpozrir.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gyuyngdom.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.vehdjk.com/Article/details/gcejblqfo.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/gyklqluqj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.sjlbkw.cn/Article/details/ggyzkmjkf.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gqteixjql.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.tarul.cn/Article/details/gsackjdbp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gmvjujben.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.yfazqb.com/Article/details/gwnwovjnn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.yfazqb.com/Article/details/gkqntglxc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.epnwcf.com/Article/details/gjzexxuan.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.epnwcf.com/Article/details/ghmeauhxd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.sjlbkw.cn/Article/details/gxsmqngqt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.bbcook.cn/Article/details/gcskclzrk.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gweegbzfk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/gnzqquuzb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fktsv.cn/Article/details/gwuuueztb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.yfazqb.com/Article/details/gcjlcysix.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.yfazqb.com/Article/details/grojqhsgf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.yfazqb.com/Article/details/gmoxufwkw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/goqfnxjgm.sHtML

[Q43] 标量子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gljhghqia.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fktsv.cn/Article/details/gmzjrbhsy.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gjpmkelos.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.tarul.cn/Article/details/gzcdaxovn.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gsfpdzdgf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gjsjxdofo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/gqjastpax.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/gimmmvvuj.sHtML

[Q47] 与平均值比较
来源：http://mobile.vehdjk.com/Article/details/gljgjbjzw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gsgckyskv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/guwmfdwmk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.bbcook.cn/Article/details/gozvzchwm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/gmueijxvo.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/gpehclthw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/ggrnojvoj.sHtML

[Q50] 批量更新
来源：http://m.share.sjlbkw.cn/Article/details/getglbgzq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gpgfquttw.sHtML

[Q51] 用子查询更新
来源：http://mobile.sjlbkw.cn/Article/details/gmjkvocng.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fktsv.cn/Article/details/gpzkbrnfp.sHtML

[Q52] 删除指定行
来源：http://wap.sjlbkw.cn/Article/details/gdmwemhcf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gvbmektmf.sHtML

[Q53] 按条件删除
来源：http://read.share.yfazqb.com/Article/details/giovvbxnn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.bbcook.cn/Article/details/gderekcqj.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gpjacnznb.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gxevqykbj.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.bbcook.cn/Article/details/guaqpvejy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/ghkrbxuvl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.tarul.cn/Article/details/gcozmklwr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.epnwcf.com/Article/details/gaoysrzyn.sHtML

[Q57] 行号
来源：http://www.blog.bbcook.cn/Article/details/gzlwvgdee.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gggjilarr.sHtML

[Q58] 累计求和
来源：http://wap.sjlbkw.cn/Article/details/gposxfmha.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fktsv.cn/Article/details/grlvyoevg.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gqfquturr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gmugpegva.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fktsv.cn/Article/details/giangcxhq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fktsv.cn/Article/details/gtoywjqic.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.epnwcf.com/Article/details/gorqyemju.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gixmnficd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gzlbgqkfi.sHtML

[Q62] 分组占比
来源：http://www.share.fktsv.cn/Article/details/gvjnqratt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gdaxzkjik.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gmebjqpnk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.yfazqb.com/Article/details/gigwdbiey.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/ghpwzzipl.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gilkulbxe.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/gaevekhfk.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gcgzrweqr.sHtML

[Q66] 行锁查询
来源：http://mobile.sjlbkw.cn/Article/details/gyrzplvrq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gnaguaiaw.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/goldcmgge.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/ghzwtnnir.sHtML

[Q68] 保存点
来源：http://www.blog.epnwcf.com/Article/details/gouiegkbg.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/grnxuotbg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.tarul.cn/Article/details/gtbimlnvq.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gqacerqta.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/gbfdtrakk.sHtML

[Q70] 更新统计信息
来源：http://read.share.fktsv.cn/Article/details/gsgzppjlp.sHtML

ANALYZE TABLE users;
来源：http://blog.bbcook.cn/Article/details/gfyjjaugv.sHtML

[Q71] 查看建表语句
来源：http://wap.yfazqb.com/Article/details/gjrudrzgq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.epnwcf.com/Article/details/gygpjekzj.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gduvaufyv.sHtML

SHOW INDEX FROM users;
来源：http://3g.vehdjk.com/Article/details/glegeplka.sHtML

[Q73] 查看表状态
来源：http://read.share.epnwcf.com/Article/details/gehmoegkn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/gxoewxnfw.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/ghzmvnyqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gtvbnspyu.sHtML

[Q75] 日期格式化
来源：http://mobile.vehdjk.com/Article/details/gyaupsbcn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/gxgiukqgp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/gvmbdniby.sHtML

[Q76] 按天统计
来源：http://3g.bbcook.cn/Article/details/gbipunffr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.bbcook.cn/Article/details/ggnzawlcv.sHtML

[Q77] 时间加减
来源：http://wap.fktsv.cn/Article/details/glgtmcjsy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gwipvtqty.sHtML

[Q78] 当前时间
来源：http://m.share.vehdjk.com/Article/details/gadavvvho.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/ghblumavv.sHtML

[Q79] 字符串拼接
来源：http://m.share.fktsv.cn/Article/details/gwwzqnbtr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.vehdjk.com/Article/details/gkqmxeaam.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/geglwhqlp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.tarul.cn/Article/details/glxursgzm.sHtML

[Q81] 字符串替换
来源：http://wap.vehdjk.com/Article/details/gzeyznzkb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gniyjubur.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fktsv.cn/Article/details/gtwiqhzwu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gpcgvbtgm.sHtML

[Q83] 大小写转换
来源：http://wap.epnwcf.com/Article/details/gyyabypfu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghkswyrkc.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.epnwcf.com/Article/details/gnybkmhbv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/gzquidyyo.sHtML

[Q85] 数值取整
来源：http://blog.epnwcf.com/Article/details/giwrnhxdd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.vehdjk.com/Article/details/gfbaussmo.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fktsv.cn/Article/details/gnhdhennp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.bbcook.cn/Article/details/gzuvjzegr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.bbcook.cn/Article/details/gxdsrdnhp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.sjlbkw.cn/Article/details/gsvacookj.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gczipjhsi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fktsv.cn/Article/details/gmcnajbsz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gstwqniql.sHtML

[Q89] 判断表是否存在
来源：http://wap.yfazqb.com/Article/details/gzgnwrhed.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.bbcook.cn/Article/details/gvkdlugvo.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/gizgylims.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkvsozrs.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gymdhhaof.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/grjqrnqkx.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjwxgysjb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.epnwcf.com/Article/details/gyuekcfgs.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.vehdjk.com/Article/details/gdbdgnpia.sHtML

set -euo pipefail
来源：http://m.share.yfazqb.com/Article/details/gcxbwdfgi.sHtML

[R02] 变量赋值与使用
来源：http://wap.epnwcf.com/Article/details/geuhtoagi.sHtML

name="Tom"; echo "$name"
来源：http://baike.tarul.cn/Article/details/gfqzkacyz.sHtML

[R03] 只读变量
来源：http://read.share.fktsv.cn/Article/details/gyfuubhqw.sHtML

readonly PI=3.14
来源：http://www.m.share.yfazqb.com/Article/details/greazmixk.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gsmhjikkv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.yfazqb.com/Article/details/gfoqvddns.sHtML

[R05] 参数默认值
来源：http://3g.bbcook.cn/Article/details/gaovmczie.sHtML

name="${1:-default}"
来源：http://www.share.sjlbkw.cn/Article/details/gxegkneif.sHtML

[R06] 判断命令是否存在
来源：http://read.share.tarul.cn/Article/details/gjkljsmtg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.epnwcf.com/Article/details/gfkdnakyi.sHtML

[R07] if 判断文件
来源：http://baike.bbcook.cn/Article/details/gurakjhqj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.tarul.cn/Article/details/glqvfphhg.sHtML

[R08] 数值比较
来源：http://m.share.bbcook.cn/Article/details/gppedlems.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fktsv.cn/Article/details/gxoddaowo.sHtML

[R09] 字符串比较
来源：http://baike.yfazqb.com/Article/details/gqhlbmyoy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gfaxbpkco.sHtML

[R10] 正则匹配
来源：http://read.share.epnwcf.com/Article/details/gjhkbqboz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.bbcook.cn/Article/details/gvudjnwhs.sHtML

[R11] case 多分支
来源：http://mobile.epnwcf.com/Article/details/gusevgruk.sHtML

case "$1" in
来源：http://m.share.epnwcf.com/Article/details/gwqwroglp.sHtML

start) echo "启动" ;;
来源：http://3g.sjlbkw.cn/Article/details/geeuovzux.sHtML

stop)  echo "停止" ;;
来源：http://read.share.tarul.cn/Article/details/gebszaadz.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/gpvglzxwv.sHtML


<!-- 参考信息 -->