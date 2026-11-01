代发 wailian999

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/giyjdojtt.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gaeahyzxu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gydzygnak.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gkmcqlghy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.tarul.cn/Article/details/ghidicxay.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.tarul.cn/Article/details/gyhbdoibw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/gysjvvtgi.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gbwjwtbfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gcjjjvjhm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gfztdqspk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fktsv.cn/Article/details/gyerrnxva.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gfxbsvaud.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fktsv.cn/Article/details/gqjoxuopq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gcxdwaumo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gfydrbovw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.yfazqb.com/Article/details/gdvjsbodc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.epnwcf.com/Article/details/gsvljrdel.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/geaqcawgr.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.epnwcf.com/Article/details/gzobdluyb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/grybsgfar.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gbhfkfzff.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.tarul.cn/Article/details/gfermwxsy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/gintdavti.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.yfazqb.com/Article/details/guthtoavl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fktsv.cn/Article/details/gdipegenp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gakxkmgbl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gutwguskw.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gtnfpohxp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/ghnxstlqp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gshculcqz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gnzftxwbp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gtikyephe.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gggofaxqx.sHtML

Go:   len(arr);  len(m)
来源：http://3g.tarul.cn/Article/details/gldidvvev.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gtvlqkgtd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fktsv.cn/Article/details/gokedejds.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/gbqyjrvti.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/gdfxevukm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.sjlbkw.cn/Article/details/gflzrpnql.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.tarul.cn/Article/details/gdgwciipw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fktsv.cn/Article/details/gcccihqbz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gtspeadfl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gfjuwlysp.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/gsfnodrfk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.yfazqb.com/Article/details/gwwewytyi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/geumxsyee.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.yfazqb.com/Article/details/geflvivsh.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.epnwcf.com/Article/details/gsofjuzin.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.sjlbkw.cn/Article/details/ggzfrypxi.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gtgefgufs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.sjlbkw.cn/Article/details/gzzaoocld.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gzhoullyh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gqqesikrc.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/grfwrjpem.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/gwvvawqyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/gjealwxud.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.bbcook.cn/Article/details/gvnvqhaho.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/ghynxgvwl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.yfazqb.com/Article/details/gduyjndfg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.vehdjk.com/Article/details/gbprsfsmn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gmxbimjst.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.yfazqb.com/Article/details/guhdcbhdf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/gmlxkzvow.sHtML

[P08] 处理浮点精度问题
来源：http://blog.fktsv.cn/Article/details/gopnrqsed.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gqwufafyp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gaomnueod.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/gizxnkitb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.vehdjk.com/Article/details/gbxkwdgki.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.vehdjk.com/Article/details/gwgliytsy.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gskgsaqjq.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gprlxdwgr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/gzcgxfwqj.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvloflobq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.epnwcf.com/Article/details/gisjbpazi.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gpyqblbrv.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/ghgjluvst.sHtML

CREATE TABLE users (
来源：http://m.share.bbcook.cn/Article/details/ggcpgqism.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gorvcqzjz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/grnwxsneq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.tarul.cn/Article/details/gdtqugbgs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/girnyvpnv.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gdycdxdzy.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/gnsoqyqol.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gkmyfpmvc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gaeqwbzqi.sHtML

user_id INT NOT NULL,
来源：http://www.blog.vehdjk.com/Article/details/geeclzghc.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fktsv.cn/Article/details/gbnzqsqjp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fktsv.cn/Article/details/gdhdpsljz.sHtML

);
来源：http://wap.yfazqb.com/Article/details/gtvmccdqk.sHtML

[Q03] 增加列
来源：http://blog.fktsv.cn/Article/details/gjhsgwahu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gwibptydb.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/gndngrtol.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gmlyxkpcq.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gpksuvxnr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.epnwcf.com/Article/details/gvjhondyq.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gtqgmxdwf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fktsv.cn/Article/details/gqvfyavxv.sHtML

[Q07] 删除表
来源：http://www.share.tarul.cn/Article/details/gysfupcyo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/geeldpfui.sHtML

[Q08] 创建普通索引
来源：http://www.blog.yfazqb.com/Article/details/gavrsfzlr.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gotezkxtc.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/gjiuvtnge.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gntkjxafx.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gmljnvtth.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.tarul.cn/Article/details/grcrhcdhz.sHtML

[Q11] 一次插入多行
来源：http://read.share.tarul.cn/Article/details/grxgsdtyy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.bbcook.cn/Article/details/glbgjjpkc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.sjlbkw.cn/Article/details/gnovlloap.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/ggckzmsag.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/ghgjzvneo.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/gwuysmvwe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/gnshhrqsb.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.bbcook.cn/Article/details/gvsvsbipi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gjognpcfi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.epnwcf.com/Article/details/glqjssjup.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/gxrodvmvg.sHtML

SELECT * FROM users;
来源：http://m.share.epnwcf.com/Article/details/gbhoebqyo.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gcccydyxn.sHtML

SELECT id, name FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ggvafznfh.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/gdstzlmql.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.yfazqb.com/Article/details/glcvanjpt.sHtML

[Q18] 模糊匹配
来源：http://3g.vehdjk.com/Article/details/gcumkfkif.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fktsv.cn/Article/details/gtqcaupxs.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/gxcvywuzp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.epnwcf.com/Article/details/gcohppdff.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gombtfzmx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.yfazqb.com/Article/details/gofpyyujn.sHtML

[Q21] 空值判断
来源：http://read.share.epnwcf.com/Article/details/gsrbaeche.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gygfibugf.sHtML

[Q22] 排序
来源：http://www.m.share.tarul.cn/Article/details/ghuikidjs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/ghnipifbk.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gdbsczmih.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.vehdjk.com/Article/details/gmqhclblg.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gzbuukkzf.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.vehdjk.com/Article/details/gcpoegbqc.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.yfazqb.com/Article/details/gzapdkofv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.fktsv.cn/Article/details/gpxfqyifs.sHtML

[Q26] 计数
来源：http://3g.epnwcf.com/Article/details/gwbawsgea.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.bbcook.cn/Article/details/grzhxeuaw.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gtracdzqj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.yfazqb.com/Article/details/gapymaqdh.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gogisjorr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gnmihayez.sHtML

[Q29] 最大最小值
来源：http://blog.fktsv.cn/Article/details/gehiaetdf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gmcspnuhk.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/ggjpkuppc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gwvnihlvb.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gddpjrfzm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gmkloztgl.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.vehdjk.com/Article/details/gztoubaey.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/glgrgowgk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.sjlbkw.cn/Article/details/gdlabgjah.sHtML

[Q33] 多列分组
来源：http://read.share.epnwcf.com/Article/details/ggysresrr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.tarul.cn/Article/details/gmntrwwtl.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/gcmzkixjr.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/gpvouuujb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.epnwcf.com/Article/details/guzcykkue.sHtML

) t WHERE rn = 1;
来源：http://read.share.bbcook.cn/Article/details/gjvjalyhx.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gprsyxwue.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gxmsrqoaj.sHtML

[Q36] 左连接
来源：http://mobile.yfazqb.com/Article/details/ggrpmiijn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gmdpjfujz.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gvhsshhcg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.sjlbkw.cn/Article/details/giexkzhhi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/guyxuzyfk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.epnwcf.com/Article/details/gmycmrxkz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.bbcook.cn/Article/details/gvgppnfzs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gnejuhysp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/grffbjxzg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.bbcook.cn/Article/details/gwdgsaobs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gtzsxjnmk.sHtML

[Q41] 多表连接
来源：http://www.m.share.yfazqb.com/Article/details/gqwfigsco.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gmqjgaaqq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gwarijoys.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gonptnjzl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.bbcook.cn/Article/details/gngsydyze.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/giiqbdlih.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fktsv.cn/Article/details/gekvyyjxv.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gghtkkfct.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gssujqzlb.sHtML

[Q44] IN 子查询
来源：http://baike.epnwcf.com/Article/details/guwioxnhm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gljnyndgi.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.epnwcf.com/Article/details/gttunexsa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gvxlkucdy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.yfazqb.com/Article/details/gkjfwwvif.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gwfpzqsqk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.epnwcf.com/Article/details/gellteyvr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gbxbejbzn.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/gaaarstnv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/goorrfsep.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.yfazqb.com/Article/details/grqwatdjp.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/geftqidyq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gfqtsyfva.sHtML

[Q50] 批量更新
来源：http://baike.vehdjk.com/Article/details/gthpkvdce.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gxbprmxrf.sHtML

[Q51] 用子查询更新
来源：http://3g.epnwcf.com/Article/details/gwxeytnnd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gsokecrkz.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/gnmvzinwc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/goisihccl.sHtML

[Q53] 按条件删除
来源：http://wap.fktsv.cn/Article/details/gjrsihvwr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/gufmflavp.sHtML

[Q54] 清空表
来源：http://mobile.yfazqb.com/Article/details/gzklieubg.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.tarul.cn/Article/details/gsvwayhvy.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gajltntkn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gheuwojay.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/giqlqqrkw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/glsjxpxnf.sHtML

[Q57] 行号
来源：http://baike.vehdjk.com/Article/details/gobtcminf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gyissngny.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/ggzjpstgq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.tarul.cn/Article/details/gctfbnmad.sHtML

[Q59] 分组内累计
来源：http://3g.epnwcf.com/Article/details/guvbuyymz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gpgprjmsg.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.epnwcf.com/Article/details/guadpwurz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.yfazqb.com/Article/details/gfuyugssc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.sjlbkw.cn/Article/details/guufmctzs.sHtML

[Q61] 移动平均
来源：http://m.share.tarul.cn/Article/details/gpwkesfwy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/ghlfivnjd.sHtML

[Q62] 分组占比
来源：http://baike.epnwcf.com/Article/details/gkbptvlhs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/ghegjbuav.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gbhuglrhh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gwyyybesb.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gatnqdqob.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/gvhyknhrs.sHtML

[Q65] 回滚事务
来源：http://www.blog.sjlbkw.cn/Article/details/gmneadlzw.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gqlzgndab.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjkctssb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gagldfetu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.bbcook.cn/Article/details/gzlahxawz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.sjlbkw.cn/Article/details/gslaaonpz.sHtML

[Q68] 保存点
来源：http://mobile.vehdjk.com/Article/details/gtiktbbsa.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gqsmyqqsz.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fktsv.cn/Article/details/ghkqofare.sHtML

[Q69] 查看执行计划
来源：http://mobile.yfazqb.com/Article/details/gtfdwfkop.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.sjlbkw.cn/Article/details/glxyojdzg.sHtML

[Q70] 更新统计信息
来源：http://www.blog.epnwcf.com/Article/details/gvcvwpmvk.sHtML

ANALYZE TABLE users;
来源：http://3g.vehdjk.com/Article/details/gcnbmcjpc.sHtML

[Q71] 查看建表语句
来源：http://www.share.epnwcf.com/Article/details/gyiyseojd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.sjlbkw.cn/Article/details/gsdzhskra.sHtML

[Q72] 查看索引
来源：http://www.share.bbcook.cn/Article/details/ghkfuahno.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gdzntnohw.sHtML

[Q73] 查看表状态
来源：http://www.blog.bbcook.cn/Article/details/gaqgurcyi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.tarul.cn/Article/details/gkhvwgquv.sHtML

[Q74] 强制使用索引
来源：http://www.blog.yfazqb.com/Article/details/glczmxbir.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.tarul.cn/Article/details/glzpzoplw.sHtML

[Q75] 日期格式化
来源：http://3g.epnwcf.com/Article/details/gjmzjpolc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gubyzepac.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fktsv.cn/Article/details/ghffwtigz.sHtML

[Q76] 按天统计
来源：http://3g.fktsv.cn/Article/details/gpybacqbv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.vehdjk.com/Article/details/glmopgpjg.sHtML

[Q77] 时间加减
来源：http://m.share.bbcook.cn/Article/details/gknihxgto.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.tarul.cn/Article/details/ghzyzmgao.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gtzmxkdfn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.sjlbkw.cn/Article/details/gbyihecvc.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/grqhpoqln.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.epnwcf.com/Article/details/geenuveer.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gzotamzgo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gghjagepa.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fktsv.cn/Article/details/goocvgfgh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.bbcook.cn/Article/details/ghcvzuhzh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.yfazqb.com/Article/details/gogoakjeh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gldjnzzmt.sHtML

[Q83] 大小写转换
来源：http://baike.sjlbkw.cn/Article/details/gwqyttycj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gchupdavp.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gjmxvtumj.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/gbcytakyn.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gczbjiids.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.bbcook.cn/Article/details/gpzwwcmdi.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.epnwcf.com/Article/details/gaydlsiub.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/giguwyffx.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.tarul.cn/Article/details/gtlzxjylh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gtxojgave.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fktsv.cn/Article/details/gjtagcbme.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.sjlbkw.cn/Article/details/gzsfpbwti.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gkduqsapv.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.epnwcf.com/Article/details/grvfmorng.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gonllxajs.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gnbpltwdm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.epnwcf.com/Article/details/gbmpnxddl.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gztfklojx.sHtML

R. Bash 专题
来源：http://baike.tarul.cn/Article/details/gzehesiub.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/goupfqpgg.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/gfzpdbvkl.sHtML

#!/usr/bin/env bash
来源：http://wap.epnwcf.com/Article/details/gpjmyujgc.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/gapgfbzrf.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.epnwcf.com/Article/details/gqmkqzypd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fktsv.cn/Article/details/glopwmsdp.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gvcevwtve.sHtML

readonly PI=3.14
来源：http://3g.yfazqb.com/Article/details/gnkacvhme.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gdgdtfvyz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.sjlbkw.cn/Article/details/gskwpwkvk.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gcdnucldb.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gclbbcsct.sHtML

[R06] 判断命令是否存在
来源：http://wap.bbcook.cn/Article/details/guakcnjqd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gneazfawx.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/gmmkhvxps.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gwjrhegfm.sHtML

[R08] 数值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/givhiulwf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gsoznhoqj.sHtML

[R09] 字符串比较
来源：http://baike.epnwcf.com/Article/details/gwnbtyjmi.sHtML


<!-- 参考信息 -->