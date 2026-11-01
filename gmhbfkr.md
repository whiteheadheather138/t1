代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.tarul.cn/Article/details/gppcciblh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/grrvvwuke.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gonbbkbwv.sHtML

Ruby: // fork 块
来源：http://baike.bbcook.cn/Article/details/gxgnovzhj.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/gmzuwfuze.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/ggkdheteg.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/guzvpkicb.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gtzuybduk.sHtML

[P01] 生成 UUID
来源：http://read.share.epnwcf.com/Article/details/guomzxhbe.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/goovqsqmx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.yfazqb.com/Article/details/gwtsjjptp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gdivygrbb.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gmvpcmhnp.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.tarul.cn/Article/details/gwvuppwdq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/grnnnibec.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.sjlbkw.cn/Article/details/gjflkkpmk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/glkddvbsf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gtjfcvxxw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gamfwiwxz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/goifwjtfd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/ghehmeuuk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gefuveygg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/ggpbmrhhq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/gbzebxyqg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.vehdjk.com/Article/details/geawxrfgg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/geuopuudl.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gcfjsucmk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gwkuuicyt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gjslmtpfb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gjwvnepou.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.sjlbkw.cn/Article/details/gwbqrmxxv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.vehdjk.com/Article/details/gypmngbfh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gmirxyhez.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.tarul.cn/Article/details/ggcjsynap.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/glwmunksx.sHtML

[P04] 求长度
来源：http://3g.tarul.cn/Article/details/gnvhnvkpk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.sjlbkw.cn/Article/details/gzbrfpiqt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gksmatmhu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gfjojzirc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gytddyaqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gitykbcet.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/grcswhyrs.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/guukuskdi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/ghtqhmyuq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gzamnicoy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gswzchpvq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gfdyqmhmd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gctvyvkmj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gzlqoeoyb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gdqqsrsld.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gcvsjmuvn.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gmomabzoh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gyggcznjz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gbxmutwke.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.bbcook.cn/Article/details/gnvzkhzzy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gudcdwqwx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.bbcook.cn/Article/details/godnwribg.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fktsv.cn/Article/details/gykesiyvz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gwzwcfdjm.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/ghusxgwcl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.yfazqb.com/Article/details/ghzwuaszg.sHtML

C#:   if (x is null) {}
来源：http://3g.sjlbkw.cn/Article/details/gqozjtnvr.sHtML

[P07] 防抖与节流
来源：http://mobile.tarul.cn/Article/details/gxtrsvxik.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/giliryosw.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gzprbrkap.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/ghaewmiyj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gidmddqms.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gxrptrdhe.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/ggxozoupb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/goeorwhxs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.tarul.cn/Article/details/gvvmhgxoh.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.vehdjk.com/Article/details/geybiyods.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/gfkhrgjsc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.sjlbkw.cn/Article/details/gazjmwjns.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/gdduywiol.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.yfazqb.com/Article/details/glyztzhfe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.vehdjk.com/Article/details/gwudawrpr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gfssufqpf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gfyhltvfy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gupvwaaha.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/greizewmu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gmfglgwyu.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gjkafrvkc.sHtML

[Q01] 创建表
来源：http://blog.bbcook.cn/Article/details/gwazlfyfm.sHtML

CREATE TABLE users (
来源：http://blog.tarul.cn/Article/details/ghgvbahax.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gotbhodqz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.sjlbkw.cn/Article/details/gzplbgoer.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gymnhgwaw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gpjzcnjua.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gdrbvshtj.sHtML

[Q02] 创建带外键的表
来源：http://baike.bbcook.cn/Article/details/gjwyxxhyl.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/ggquzfybl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gxygmqeyk.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/glhqkjtbx.sHtML

amount DECIMAL(10, 2),
来源：http://3g.sjlbkw.cn/Article/details/gfsihzskp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gvlggzzgc.sHtML

);
来源：http://m.share.bbcook.cn/Article/details/gmqbcdtrl.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/gsfjxldcz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gbkhestgb.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gqyafdpen.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.vehdjk.com/Article/details/gpnjxqsbp.sHtML

[Q05] 重命名列
来源：http://read.share.fktsv.cn/Article/details/gpssahafa.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.sjlbkw.cn/Article/details/gfoebvbdb.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gzxwlabmk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gbdrpmxze.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/gfmnmpsmr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.epnwcf.com/Article/details/gzpzyshpt.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gjqfbqbdp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/ggavrehan.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/ggvdlbykb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gbtoygptw.sHtML

[Q10] 插入单行
来源：http://blog.fktsv.cn/Article/details/gldavryxd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gbbbhxoha.sHtML

[Q11] 一次插入多行
来源：http://m.share.sjlbkw.cn/Article/details/gnomijgjn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/ghimrtbep.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/gljckxvau.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.bbcook.cn/Article/details/gdgwsoxmy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/giznolrbj.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.yfazqb.com/Article/details/gmcwxxwda.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gygatbwlp.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/gbhiyaqmm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.tarul.cn/Article/details/gzvocncoa.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gcrjlqkxn.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gdxuzariz.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gqxjavhye.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/gfedxztog.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/ganohkttz.sHtML

[Q17] 条件查询
来源：http://blog.yfazqb.com/Article/details/gglppkosh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.epnwcf.com/Article/details/gtubynbtz.sHtML

[Q18] 模糊匹配
来源：http://wap.fktsv.cn/Article/details/gskkmptnb.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gkzpotjxx.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/grepjmynv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.epnwcf.com/Article/details/gynzhvhyx.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/grykthvfy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/guggmokas.sHtML

[Q21] 空值判断
来源：http://www.m.share.vehdjk.com/Article/details/gdbetodcq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gsjaedqrm.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/gzpxhirbp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gtkryoksx.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gkmdbjosj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.bbcook.cn/Article/details/goivymynz.sHtML

[Q24] 去重
来源：http://www.blog.vehdjk.com/Article/details/ggjhwnrnr.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxhucfgvy.sHtML

[Q25] 只取前 N 条
来源：http://baike.epnwcf.com/Article/details/gizhaxizt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/gwcyxmduo.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/glrxttemn.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.tarul.cn/Article/details/gaftcxbpc.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gtzbnscyj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gkmpdntxz.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gifozidxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gubhavmdk.sHtML

[Q29] 最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/gswuysrwy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.bbcook.cn/Article/details/gyvtinntm.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/gpqswqlhb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/goqwmtizj.sHtML

[Q31] 分组后过滤
来源：http://wap.epnwcf.com/Article/details/gbckbgmzq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.epnwcf.com/Article/details/gmhycgfjt.sHtML

[Q32] 分组拼接字符串
来源：http://blog.yfazqb.com/Article/details/gsdvfnmqu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gwuhzkmwg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/gjaqpbrtc.sHtML

[Q33] 多列分组
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqahxalp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/gpuywaehm.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/gtnliwuci.sHtML

SELECT * FROM (
来源：http://m.share.bbcook.cn/Article/details/gwfrsvleo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/gszrdgrjc.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gwckyzmsl.sHtML

[Q35] 内连接
来源：http://www.m.share.bbcook.cn/Article/details/gapoovzob.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.bbcook.cn/Article/details/gougjqrjb.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gbiqqxenx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.yfazqb.com/Article/details/gcudnkmzt.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gmanozvrk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.yfazqb.com/Article/details/gmurkvtki.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.tarul.cn/Article/details/gtnuwfwpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/ggtpgolzp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gzbrdkxij.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gtslvehcy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvwvwjao.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gneolptef.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.sjlbkw.cn/Article/details/gsfxyfrbm.sHtML

[Q41] 多表连接
来源：http://m.share.tarul.cn/Article/details/gxwgmhorp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/glfudqxye.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/gfbezcshr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.vehdjk.com/Article/details/gmiuaapdi.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.vehdjk.com/Article/details/gyrfrueve.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fktsv.cn/Article/details/gtsjdgkav.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/geyjshhlb.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gsoyollxi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.tarul.cn/Article/details/guhfwrwud.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gtgttlaks.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.sjlbkw.cn/Article/details/gxmbphkiu.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/getucypgq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.yfazqb.com/Article/details/gxjuxkhjq.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.vehdjk.com/Article/details/gcgxtgfkn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gxkqjpdqm.sHtML

[Q47] 与平均值比较
来源：http://m.share.epnwcf.com/Article/details/gmrpmkbhb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/glmlqxhot.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.epnwcf.com/Article/details/gayjzfvlo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/ggvluamjm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.sjlbkw.cn/Article/details/gqlqnygfz.sHtML

[Q49] 更新单行
来源：http://wap.epnwcf.com/Article/details/ggvwfdbjd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.bbcook.cn/Article/details/gqwjnikxe.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gqmhkthoe.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fktsv.cn/Article/details/gttahllbc.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gtdgaezgg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.sjlbkw.cn/Article/details/gxmjiuicy.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gijmtioex.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrtjyjqo.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gjijgpgrw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gqoqplimt.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gfnalujbd.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gmpioczqy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.vehdjk.com/Article/details/gphnfcaot.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/gwvjseqgd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fktsv.cn/Article/details/gzbufojkp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.tarul.cn/Article/details/gigzaittn.sHtML

[Q57] 行号
来源：http://baike.fktsv.cn/Article/details/gaaywnnbm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/ggurrgaln.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/ghvtekudo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.yfazqb.com/Article/details/gvdtmcdfb.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gobnorepb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gkebvubbo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.bbcook.cn/Article/details/gmvhnjkdo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gefgkmtzo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gcllouadg.sHtML

[Q61] 移动平均
来源：http://read.share.epnwcf.com/Article/details/ggadzpqyo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gzxhwepst.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gjypdftks.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gyqhucxub.sHtML

[Q63] 开启事务
来源：http://3g.epnwcf.com/Article/details/gjkubbcle.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.bbcook.cn/Article/details/gfnzbvdsk.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gbqzrktwf.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/gifbqytka.sHtML

[Q65] 回滚事务
来源：http://3g.yfazqb.com/Article/details/gchfgwhvo.sHtML

ROLLBACK;
来源：http://mobile.sjlbkw.cn/Article/details/gnpktajld.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gxllsclzo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gagkowyox.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gfcztgcli.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.sjlbkw.cn/Article/details/goyggoqdm.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/gvsczqroz.sHtML

SAVEPOINT sp1;
来源：http://blog.tarul.cn/Article/details/gepfumqbs.sHtML

ROLLBACK TO sp1;
来源：http://read.share.yfazqb.com/Article/details/gpeuesjsc.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gxzehpafl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gedllxwtw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gjpnlhgnw.sHtML

ANALYZE TABLE users;
来源：http://blog.sjlbkw.cn/Article/details/gzjdkkgkt.sHtML

[Q71] 查看建表语句
来源：http://read.share.yfazqb.com/Article/details/gjqgmclyw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.tarul.cn/Article/details/gtmffgyxl.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/gpurmitpf.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gbjtyvrbx.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/grhfutnhr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.vehdjk.com/Article/details/gforswznz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.yfazqb.com/Article/details/gdophnmbb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.bbcook.cn/Article/details/gqyvydcjr.sHtML

[Q75] 日期格式化
来源：http://www.blog.tarul.cn/Article/details/ghcnwmbna.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gzuuzzfba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.yfazqb.com/Article/details/ghqialhyx.sHtML

[Q76] 按天统计
来源：http://www.blog.bbcook.cn/Article/details/ggyviyvch.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gloixzpdn.sHtML

[Q77] 时间加减
来源：http://www.m.share.bbcook.cn/Article/details/gjaqyuxes.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.bbcook.cn/Article/details/gyqqummzb.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/gwbwvvfdh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/gwxkjiorl.sHtML

[Q79] 字符串拼接
来源：http://baike.fktsv.cn/Article/details/gyrrhqvfu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.vehdjk.com/Article/details/grojqanfr.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/ggovrqnse.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/gaxwdtqpt.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gwvqbbbir.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.vehdjk.com/Article/details/gzoctrvag.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.yfazqb.com/Article/details/gkeirnuqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gknrewnwy.sHtML

[Q83] 大小写转换
来源：http://mobile.fktsv.cn/Article/details/gucqrahda.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gonvnurny.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fktsv.cn/Article/details/gjrlqfpjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gmvhbtfjg.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gdzhjqtta.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.vehdjk.com/Article/details/gvdcdcwkk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.sjlbkw.cn/Article/details/gezvsqbic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fktsv.cn/Article/details/gshimrshf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqfpqbut.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/gzyhfofne.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.vehdjk.com/Article/details/glsianwsr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.yfazqb.com/Article/details/ghxvsxnvm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gnndgdplm.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gtkczvjxe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.epnwcf.com/Article/details/gtsfwlmnr.sHtML

[Q90] 生成序号列
来源：http://www.share.epnwcf.com/Article/details/gwkxwfvgh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/gvocohsdn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gnumhantb.sHtML

R. Bash 专题
来源：http://www.m.share.tarul.cn/Article/details/ggfqibbnc.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gyzdskbun.sHtML

[R01] shebang 与严格模式
来源：http://blog.sjlbkw.cn/Article/details/gwmgdkmmi.sHtML

#!/usr/bin/env bash
来源：http://www.blog.yfazqb.com/Article/details/gczoaihkw.sHtML

set -euo pipefail
来源：http://baike.vehdjk.com/Article/details/gxdzjmlof.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.epnwcf.com/Article/details/gagcmqsam.sHtML

name="Tom"; echo "$name"
来源：http://baike.yfazqb.com/Article/details/gydwdjiwr.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gndwoubrt.sHtML

readonly PI=3.14
来源：http://www.blog.fktsv.cn/Article/details/gbvfudcsf.sHtML

[R04] 位置参数
来源：http://blog.vehdjk.com/Article/details/goddvaxjm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fktsv.cn/Article/details/gnbaeyjmm.sHtML

[R05] 参数默认值
来源：http://read.share.sjlbkw.cn/Article/details/gycgovouz.sHtML


<!-- 参考信息 -->