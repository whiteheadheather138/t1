代发 wailian999

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/glhvndacn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gudcndvrr.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/grbrgzkbm.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grvscoyck.sHtML

[P01] 生成 UUID
来源：http://www.m.share.sjlbkw.cn/Article/details/gyabshcwe.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.bbcook.cn/Article/details/gzwlmaqcf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/gpatbfdpa.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gxkvsbjjf.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.vehdjk.com/Article/details/gjzpzuzcy.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/gnisxloty.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/gzxnbtzqd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fktsv.cn/Article/details/gzegddpgg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/ghqvkyhgk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.epnwcf.com/Article/details/gglltfgay.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/glpdrvysu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/gnzwucscd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gipmxwynw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.epnwcf.com/Article/details/glwyjcafz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gfmfdnwrg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.bbcook.cn/Article/details/gzqluuruy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/goohgjzit.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.sjlbkw.cn/Article/details/gkjnnanrz.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.yfazqb.com/Article/details/grrojlmhe.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gghstnfqn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/gvbgnraxq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/galgfmnml.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gfmvzdvly.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gclwvbsec.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gtoodsvdx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gnsfqwfle.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/girjdyyab.sHtML

[P04] 求长度
来源：http://baike.fktsv.cn/Article/details/gksgfxezu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gkrubquuz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gvlxthnnt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gwkboyutv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/ghcgupwic.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gtneiobph.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.bbcook.cn/Article/details/garkufbum.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gdtsrlpum.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.sjlbkw.cn/Article/details/ggosupueu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gjapypcfn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.tarul.cn/Article/details/ggtpvxked.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fktsv.cn/Article/details/ggsrcfrlp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.bbcook.cn/Article/details/gehktygvt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.bbcook.cn/Article/details/gnbhgxznh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gpqwsrrpz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gflnkbqly.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gcwelwhip.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.bbcook.cn/Article/details/gaapddhaj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.bbcook.cn/Article/details/gqkyvprlh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/guxdxpues.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/goplixrcc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gdmwuhkst.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/glvrutdzn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.sjlbkw.cn/Article/details/gqsetmtmq.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/ghyzbjnkm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.sjlbkw.cn/Article/details/gbdfjkklj.sHtML

C#:   if (x is null) {}
来源：http://blog.tarul.cn/Article/details/gllgldhra.sHtML

[P07] 防抖与节流
来源：http://blog.bbcook.cn/Article/details/gtqvltmsv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gmdaudois.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/goihgkwhx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gbifpspla.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/ggtpfbgmm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gpwoalaqt.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/gbkmelisi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/ghujpavpi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gbrozrngw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gybobkqhs.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.bbcook.cn/Article/details/gdhvpejxw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.sjlbkw.cn/Article/details/ggprrszwz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fktsv.cn/Article/details/gwckculxd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gkrwykkoi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.yfazqb.com/Article/details/gthzxkdub.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gslwrfdqf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/gmazaljjb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.vehdjk.com/Article/details/gyxsvyeta.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gdqzttjlz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gfrilrlfg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gpwtkdwpb.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/gurgjvtvq.sHtML

CREATE TABLE users (
来源：http://baike.sjlbkw.cn/Article/details/grwbqflei.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/gvfooyxdb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gvoiyrrhf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gyybwunhm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gpufcpqhv.sHtML

);
来源：http://baike.bbcook.cn/Article/details/glwnddcfy.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gzhuumsxe.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gwuuclfbu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gpipvwfjg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gouqgrbin.sHtML

amount DECIMAL(10, 2),
来源：http://3g.yfazqb.com/Article/details/gkycislvy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.vehdjk.com/Article/details/gmpjlroit.sHtML

);
来源：http://www.blog.sjlbkw.cn/Article/details/ghvocgvid.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/golekcqlp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.bbcook.cn/Article/details/gzpclrika.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/gyujuilog.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/ghmeivkxt.sHtML

[Q05] 重命名列
来源：http://read.share.vehdjk.com/Article/details/gexbmaldv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.yfazqb.com/Article/details/gwrhewmux.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/ghsbfihsr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.epnwcf.com/Article/details/gpycwfpyu.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gxjxkocem.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/gwzsnrnqx.sHtML

[Q08] 创建普通索引
来源：http://m.share.fktsv.cn/Article/details/gmyvdapex.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/guttatqxd.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/ggxfitztv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.tarul.cn/Article/details/ghlhruzbe.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/gssavenrh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gkblwmkbk.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.epnwcf.com/Article/details/grefyekbf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gtviwmvdi.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.bbcook.cn/Article/details/gkhtfwfsg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gpdqgtnxk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gzhchnsay.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gkyuwopgf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.vehdjk.com/Article/details/gpmioguxw.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fktsv.cn/Article/details/gugngwium.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.tarul.cn/Article/details/gknmktxvx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gjnwqvvzu.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gwspsjiwp.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gwuutcxuc.sHtML

[Q16] 查询指定列
来源：http://blog.yfazqb.com/Article/details/govjccfqt.sHtML

SELECT id, name FROM users;
来源：http://blog.bbcook.cn/Article/details/guqigsnfw.sHtML

[Q17] 条件查询
来源：http://www.m.share.fktsv.cn/Article/details/gjbuzakqy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.tarul.cn/Article/details/gtqldrqgb.sHtML

[Q18] 模糊匹配
来源：http://3g.fktsv.cn/Article/details/ggdpdorsv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gcjblbwqm.sHtML

[Q19] 范围查询
来源：http://3g.bbcook.cn/Article/details/gzahfpknq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fktsv.cn/Article/details/gdxkznohz.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/gnoahxhec.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gbreszmiv.sHtML

[Q21] 空值判断
来源：http://baike.yfazqb.com/Article/details/gttwybxhz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gkfneeqot.sHtML

[Q22] 排序
来源：http://mobile.yfazqb.com/Article/details/gmklyrgsn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.epnwcf.com/Article/details/gnvunvagf.sHtML

[Q23] 分页
来源：http://www.share.epnwcf.com/Article/details/gmvbzbksz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gaaqxihuo.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gldgaihyl.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/gqrouqiab.sHtML

[Q25] 只取前 N 条
来源：http://blog.bbcook.cn/Article/details/gdkymcqpm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gyiyubfjy.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gtfkqbjxo.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fktsv.cn/Article/details/glnqjpysb.sHtML

[Q27] 条件计数
来源：http://www.share.vehdjk.com/Article/details/gjaxvqlqe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/ghisapcfy.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/gnzmkjsxc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gqgrfpxnh.sHtML

[Q29] 最大最小值
来源：http://m.share.vehdjk.com/Article/details/gqwglugyk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.bbcook.cn/Article/details/gqotmiroz.sHtML

[Q30] 分组统计
来源：http://baike.bbcook.cn/Article/details/gudmiaywm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gsrqjiqmh.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.tarul.cn/Article/details/gyszodohe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gdhlcumgy.sHtML

[Q32] 分组拼接字符串
来源：http://3g.vehdjk.com/Article/details/gailfisro.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gxusivddz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/gpltrjkze.sHtML

[Q33] 多列分组
来源：http://mobile.fktsv.cn/Article/details/giraiueuv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gjvmzfwhh.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gkmisncyz.sHtML

SELECT * FROM (
来源：http://www.blog.epnwcf.com/Article/details/gmpxbeztx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gypfmmmsq.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gsvckddws.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/gsmujvdxd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.bbcook.cn/Article/details/gcxaibebj.sHtML

[Q36] 左连接
来源：http://wap.tarul.cn/Article/details/gueaioiqu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gnykotqew.sHtML

[Q37] 右连接
来源：http://wap.tarul.cn/Article/details/gmroomsyt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.sjlbkw.cn/Article/details/gwikxivnr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.vehdjk.com/Article/details/gqmouhtsx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.bbcook.cn/Article/details/gqqukfotw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/gqjaqhecy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/gzinaqurh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gxocaubqe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gjcrybvwq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gjcfxcdwr.sHtML

[Q41] 多表连接
来源：http://wap.yfazqb.com/Article/details/gierfvune.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/gbbgfmxas.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.sjlbkw.cn/Article/details/ggfvvlncq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.bbcook.cn/Article/details/gblcvxrcw.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/gccsmomth.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gbkaqrkdw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/gstntadke.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/gjflnsahf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.tarul.cn/Article/details/gtchuguau.sHtML

[Q44] IN 子查询
来源：http://baike.vehdjk.com/Article/details/gfawukjfy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.vehdjk.com/Article/details/gizzpxwdm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gvatnduta.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.epnwcf.com/Article/details/ggjinwtaf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.yfazqb.com/Article/details/gfiwnihxi.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gvxfkxddw.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gakopktvh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gjlnpmpyz.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/gkaztkadr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/gruembgee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.vehdjk.com/Article/details/gwjlxweig.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/gvfzdowul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gdtscjoii.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/gxwmfwzqu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.epnwcf.com/Article/details/gdnrlruve.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/gsytwbspk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fktsv.cn/Article/details/ghhpehfte.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/gwcfvptbh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gnzpevtbv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.tarul.cn/Article/details/gvvpzwdkh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.sjlbkw.cn/Article/details/gsnxboonb.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gtrhsafoi.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gxevnjhpa.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gjnfvmpus.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gtdvmujzh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/gygrhmqzj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gojrzwwzc.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/ghfxtzsen.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gafgnltgj.sHtML

[Q58] 累计求和
来源：http://baike.bbcook.cn/Article/details/gppcfocrg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gdtdchquf.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gcngsllnh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/gswqguadq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.sjlbkw.cn/Article/details/gxgktvral.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gwcliqpwk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gknbpkdcw.sHtML

[Q61] 移动平均
来源：http://wap.sjlbkw.cn/Article/details/gqpdngzfk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.yfazqb.com/Article/details/glnvktblj.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/geoylmffy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/gkvxehtmj.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gcecpojge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.epnwcf.com/Article/details/gawbrpvua.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gxcaebcig.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/gpknltned.sHtML

[Q65] 回滚事务
来源：http://mobile.fktsv.cn/Article/details/gjctdyqxu.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gpcoltsdt.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/guhfjpwcp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fktsv.cn/Article/details/gjnuuilgb.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.yfazqb.com/Article/details/gogbjovrt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gflkiymbh.sHtML

[Q68] 保存点
来源：http://3g.sjlbkw.cn/Article/details/goquvurbk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.bbcook.cn/Article/details/gacbfjisx.sHtML

ROLLBACK TO sp1;
来源：http://mobile.epnwcf.com/Article/details/gevsvhqhs.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/gopyahtik.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/gcxksknzx.sHtML

[Q70] 更新统计信息
来源：http://read.share.sjlbkw.cn/Article/details/guovoglkt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.tarul.cn/Article/details/ginnzquvo.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/guduihoaq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/giskvmzki.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/gwwsmkgnr.sHtML

SHOW INDEX FROM users;
来源：http://3g.tarul.cn/Article/details/gasggjpxg.sHtML

[Q73] 查看表状态
来源：http://www.blog.sjlbkw.cn/Article/details/grphnrpfe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.vehdjk.com/Article/details/gxokowvtp.sHtML

[Q74] 强制使用索引
来源：http://m.share.tarul.cn/Article/details/gxaumerwu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.vehdjk.com/Article/details/gnlzahmtx.sHtML

[Q75] 日期格式化
来源：http://read.share.sjlbkw.cn/Article/details/gsgbgdlcd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.tarul.cn/Article/details/gjhkfaltw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gtzbbkgrv.sHtML

[Q76] 按天统计
来源：http://blog.vehdjk.com/Article/details/gqhtjwujf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.epnwcf.com/Article/details/gybfnplii.sHtML

[Q77] 时间加减
来源：http://3g.vehdjk.com/Article/details/ghnlsogli.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fktsv.cn/Article/details/gdvguhsrn.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/gawclaofy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.epnwcf.com/Article/details/gqesdjydi.sHtML

[Q79] 字符串拼接
来源：http://www.blog.tarul.cn/Article/details/gqnwuogpn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.sjlbkw.cn/Article/details/gqxlhrers.sHtML

[Q80] 字符串截取
来源：http://blog.sjlbkw.cn/Article/details/gfofcylnt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/glysbqrcv.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/ghdznhxyb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.yfazqb.com/Article/details/glhhtfdlc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gfobmfjis.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gcnozppot.sHtML

[Q83] 大小写转换
来源：http://www.blog.bbcook.cn/Article/details/guiphjdgz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gamzztscv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.tarul.cn/Article/details/gcvyxzfio.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvxjyxiz.sHtML

[Q85] 数值取整
来源：http://baike.yfazqb.com/Article/details/gevyoafsz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.sjlbkw.cn/Article/details/gtnenrfvv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/grxlprsdd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.vehdjk.com/Article/details/gvxngqgfw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.vehdjk.com/Article/details/gdsfzggre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gwrseimze.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.epnwcf.com/Article/details/gycfaexgy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gpzonxamv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.tarul.cn/Article/details/gpxubmrqt.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gnwtfgbty.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.yfazqb.com/Article/details/ggcgrjsfh.sHtML

[Q90] 生成序号列
来源：http://baike.vehdjk.com/Article/details/gcsnbgcsj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gdyaccawl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gewuvdnxp.sHtML

R. Bash 专题
来源：http://m.share.sjlbkw.cn/Article/details/gvxwkeyih.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gquaejqxj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fktsv.cn/Article/details/gsnglsdxm.sHtML

#!/usr/bin/env bash
来源：http://mobile.vehdjk.com/Article/details/gtfkxenex.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/grvudxfuh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.vehdjk.com/Article/details/gvbjspjzl.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.tarul.cn/Article/details/gvhkmmxju.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/getjbhsvj.sHtML

readonly PI=3.14
来源：http://blog.tarul.cn/Article/details/gspfuzfaw.sHtML

[R04] 位置参数
来源：http://wap.fktsv.cn/Article/details/gfstoxvpu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.vehdjk.com/Article/details/guspcingp.sHtML

[R05] 参数默认值
来源：http://www.m.share.epnwcf.com/Article/details/gvrzfqhee.sHtML

name="${1:-default}"
来源：http://www.blog.fktsv.cn/Article/details/gomofansi.sHtML

[R06] 判断命令是否存在
来源：http://www.share.epnwcf.com/Article/details/gxpxyjkzr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.epnwcf.com/Article/details/gkazyvdcj.sHtML

[R07] if 判断文件
来源：http://baike.epnwcf.com/Article/details/gktwcoqgj.sHtML


<!-- 参考信息 -->