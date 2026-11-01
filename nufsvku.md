代发 wailian999

[P01] 生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gatngpfok.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/glwtqvngl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gdkydibup.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gbksolyki.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gsqwevyyj.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gxsnrgrrt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gcvnpzmeq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/ghuiutdfw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/gbtjxeskd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.sjlbkw.cn/Article/details/gnxemmdnj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gprnutxwl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gjgimoxxy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.vehdjk.com/Article/details/gaacahapy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.sjlbkw.cn/Article/details/giycrwrck.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/geukdobvd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gsrpgdtcq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.tarul.cn/Article/details/gahicqcwg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gtkhgzfdn.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gyifhrryw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gkqvldjwd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/gmkdydrur.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/gkstptgmh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gatchrlwq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/gbilgmbsx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/gexahgfjn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gczmxlhpw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.epnwcf.com/Article/details/gxwjrljpq.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gxmtvmcsz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/ggberfzxp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.yfazqb.com/Article/details/gmolsgfvw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gtobpicbf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gquulsfjo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gflwgmacp.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gphuukvnn.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gmvxesune.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/glygbflig.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gcahpapkp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.yfazqb.com/Article/details/gbbzglsdt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.bbcook.cn/Article/details/galthztsk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gguwholye.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gjozdpoid.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gppfruzne.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gkwgnfwtz.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gpgwjsidz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fktsv.cn/Article/details/gatchkfrq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.yfazqb.com/Article/details/gqctnegfs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.vehdjk.com/Article/details/gymyfdvxn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gftosdavo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gsenyuyoe.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gtgpdqqlq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.sjlbkw.cn/Article/details/gpbtulkqe.sHtML

Go:   if x == nil {}
来源：http://wap.yfazqb.com/Article/details/gadilwlqk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.yfazqb.com/Article/details/gqnrkoaim.sHtML

C#:   if (x is null) {}
来源：http://read.share.epnwcf.com/Article/details/gelevmmfu.sHtML

[P07] 防抖与节流
来源：http://blog.vehdjk.com/Article/details/gntgaerxm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.vehdjk.com/Article/details/gzqfnouej.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gvicimulz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.epnwcf.com/Article/details/gxluqbiaf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gilxnnopy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gdxehhpkz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gziumghdi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gjgmiiets.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.yfazqb.com/Article/details/gfxaumtdp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gxgsqwptc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gkvzqzfya.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gwjwyysgh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.sjlbkw.cn/Article/details/gtyqxczna.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gpqzxdojq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.tarul.cn/Article/details/gsxbfddja.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.vehdjk.com/Article/details/ggwhtmddw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/gjwyfflvs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gfjxetqqd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvqjftxvc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.tarul.cn/Article/details/gscyxipqb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gdphahjsa.sHtML

[Q01] 创建表
来源：http://www.blog.tarul.cn/Article/details/gqgqbiael.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/ghhmrmcge.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/ghbwmcxxi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/glckyebmv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/garkgnxij.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gniyfosqw.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gnkjwbsut.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/guwnjnoay.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/ghxmjznvg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/glmzpukdm.sHtML

user_id INT NOT NULL,
来源：http://3g.tarul.cn/Article/details/gqjqnuhgy.sHtML

amount DECIMAL(10, 2),
来源：http://blog.vehdjk.com/Article/details/gfbfzuego.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.sjlbkw.cn/Article/details/gobtmkniu.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gryjgqjon.sHtML

[Q03] 增加列
来源：http://baike.vehdjk.com/Article/details/gpjnogaba.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.bbcook.cn/Article/details/glhtmwlsw.sHtML

[Q04] 修改列类型
来源：http://blog.sjlbkw.cn/Article/details/gouaexcwe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/gilycixbk.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gjddxztnp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.bbcook.cn/Article/details/gjmdahqid.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gvmiyrhvq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gqdhzmugj.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gavmmjwxy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/gzsqnabdp.sHtML

[Q08] 创建普通索引
来源：http://www.blog.tarul.cn/Article/details/gnhykknpz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gfichacen.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gzjyzalkd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/grllkrtow.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/giudstcld.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gdslxodfi.sHtML

[Q11] 一次插入多行
来源：http://wap.bbcook.cn/Article/details/grnaitfff.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.sjlbkw.cn/Article/details/gaibakowh.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.vehdjk.com/Article/details/gdtzavsao.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/gfasqritu.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gcthoaecd.sHtML

[Q13] 忽略重复插入
来源：http://www.share.yfazqb.com/Article/details/ghtfkoxtn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gqcsexvos.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gempwqrdh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.yfazqb.com/Article/details/glvogygro.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gkzhyiyys.sHtML

[Q15] 查询全部
来源：http://wap.yfazqb.com/Article/details/gawjwmuoq.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gqxnvwtly.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gbuknfozz.sHtML

SELECT id, name FROM users;
来源：http://mobile.bbcook.cn/Article/details/gmhzqslvs.sHtML

[Q17] 条件查询
来源：http://mobile.fktsv.cn/Article/details/gfnmhybgi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gtducjtuk.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gohuwliza.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.yfazqb.com/Article/details/ghidwusdb.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/giznygjtt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.yfazqb.com/Article/details/goeqjptmp.sHtML

[Q20] IN 列表
来源：http://baike.tarul.cn/Article/details/gewayuibb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gkdzijzqc.sHtML

[Q21] 空值判断
来源：http://3g.yfazqb.com/Article/details/gqufgqsku.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gnjvcxzag.sHtML

[Q22] 排序
来源：http://www.m.share.yfazqb.com/Article/details/gglugyola.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gqtziuqln.sHtML

[Q23] 分页
来源：http://www.m.share.vehdjk.com/Article/details/gsdqaxtvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gwumhewes.sHtML

[Q24] 去重
来源：http://www.m.share.yfazqb.com/Article/details/gondxehbd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gonnhkkoy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.epnwcf.com/Article/details/gosdjrela.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gnyiufgjv.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gbrxxbqoz.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gcxykxpsc.sHtML

[Q27] 条件计数
来源：http://3g.bbcook.cn/Article/details/ggidmauso.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gfxdxhcgl.sHtML

[Q28] 求和与平均
来源：http://www.m.share.bbcook.cn/Article/details/gafufiaqv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gvmgepjsr.sHtML

[Q29] 最大最小值
来源：http://baike.fktsv.cn/Article/details/gcvqllbtq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gzancsbdz.sHtML

[Q30] 分组统计
来源：http://wap.fktsv.cn/Article/details/gnjdsiugc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.yfazqb.com/Article/details/gagaafxdn.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gqjeddtij.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gzzoglfee.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gocctgfnn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/gblkzydus.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fktsv.cn/Article/details/gatxuphvx.sHtML

[Q33] 多列分组
来源：http://mobile.bbcook.cn/Article/details/grkdikmvm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/grddlrolm.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/givagxgpk.sHtML

SELECT * FROM (
来源：http://www.m.share.yfazqb.com/Article/details/gkgxyvywc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/gfgzwyskm.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gupkjctvb.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gvlijtusj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gizfkjjxh.sHtML

[Q36] 左连接
来源：http://baike.fktsv.cn/Article/details/gtrhbpcck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gppwshimd.sHtML

[Q37] 右连接
来源：http://wap.fktsv.cn/Article/details/ghlshhfxb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gpaycwghj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/gyawddign.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/gngffsxbw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/ggwjnrmxj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.vehdjk.com/Article/details/gptwvizsb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/ghcunhzmd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/ghqjmaehm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.yfazqb.com/Article/details/gtogcbani.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gzzwfzsmn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gckxdfzqn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.vehdjk.com/Article/details/gfrzdrgnj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/ggqdjifur.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.bbcook.cn/Article/details/gohbmnrhf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.yfazqb.com/Article/details/gxjjclsvw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/gnxktordj.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gqasuvciw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gniimeiun.sHtML

[Q44] IN 子查询
来源：http://mobile.tarul.cn/Article/details/gzukgbpso.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gsaodtksc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.vehdjk.com/Article/details/gricowzcv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/ginruqdpj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gliyicjmf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gnfcfjkta.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gojypgzfi.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.vehdjk.com/Article/details/gpofyzolp.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/ggpkbonnp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.yfazqb.com/Article/details/gbrnnlnyi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gdcuvofbr.sHtML

[Q49] 更新单行
来源：http://m.share.sjlbkw.cn/Article/details/gsnvirecj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gtpnuwlty.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gqymbvceh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.tarul.cn/Article/details/gjppnibpu.sHtML

[Q51] 用子查询更新
来源：http://read.share.yfazqb.com/Article/details/gbgghvzwk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gahcnzodw.sHtML

[Q52] 删除指定行
来源：http://baike.fktsv.cn/Article/details/grhjkxarf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gncpljffy.sHtML

[Q53] 按条件删除
来源：http://3g.epnwcf.com/Article/details/gmrhxcgxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gakmxiosg.sHtML

[Q54] 清空表
来源：http://www.m.share.yfazqb.com/Article/details/gsznvwtdg.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/giqajnjjo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/grhlmkorh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.epnwcf.com/Article/details/gbnyximec.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fktsv.cn/Article/details/gautkuftc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gkqvvztjl.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/gkztgvzra.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gisoghfcq.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gxiiiwpme.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gvjxuwkpc.sHtML

[Q59] 分组内累计
来源：http://www.share.sjlbkw.cn/Article/details/gcqjaidtp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.tarul.cn/Article/details/gajiinarv.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.sjlbkw.cn/Article/details/gxamgnaqj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.bbcook.cn/Article/details/gncndylvp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gazvosqgd.sHtML

[Q61] 移动平均
来源：http://www.share.yfazqb.com/Article/details/gxxiefamb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gfrmmbbkz.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gkledkpxo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/golztsejs.sHtML

[Q63] 开启事务
来源：http://wap.bbcook.cn/Article/details/gnibjsabz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gjddhqzdd.sHtML

[Q64] 提交事务
来源：http://mobile.sjlbkw.cn/Article/details/gbkjcyzpj.sHtML

COMMIT;
来源：http://www.m.share.tarul.cn/Article/details/gzqnqqslz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwikaugo.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/ghspixpca.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gbqwsbycf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.epnwcf.com/Article/details/gbncpdzlo.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/giqyisnjz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.yfazqb.com/Article/details/gvvxmlcdn.sHtML

[Q68] 保存点
来源：http://www.m.share.bbcook.cn/Article/details/gdphfukek.sHtML

SAVEPOINT sp1;
来源：http://3g.tarul.cn/Article/details/gtckhdssq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.yfazqb.com/Article/details/glumfkzkd.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gsofsljon.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gvfxhqiwc.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.epnwcf.com/Article/details/gitcodypz.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gmvpihlcv.sHtML

[Q71] 查看建表语句
来源：http://blog.tarul.cn/Article/details/gbxtzubmr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fktsv.cn/Article/details/gnqgyztkv.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gbobvxoxc.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/gkymjfnhg.sHtML

[Q73] 查看表状态
来源：http://www.blog.tarul.cn/Article/details/gpyjqgitm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.vehdjk.com/Article/details/gkcnbvowl.sHtML

[Q74] 强制使用索引
来源：http://www.share.sjlbkw.cn/Article/details/gjjgizvcd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.sjlbkw.cn/Article/details/gwtkknxyx.sHtML

[Q75] 日期格式化
来源：http://baike.yfazqb.com/Article/details/gsbrpysiv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gpjdjzfvp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.epnwcf.com/Article/details/grbeepoly.sHtML

[Q76] 按天统计
来源：http://www.share.sjlbkw.cn/Article/details/gmwvnduvr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gzoewmcaq.sHtML

[Q77] 时间加减
来源：http://m.share.fktsv.cn/Article/details/goiijkuhv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fktsv.cn/Article/details/gyigkgdic.sHtML

[Q78] 当前时间
来源：http://www.m.share.tarul.cn/Article/details/gqvjiqxic.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fktsv.cn/Article/details/giszytmml.sHtML

[Q79] 字符串拼接
来源：http://blog.fktsv.cn/Article/details/guxvpmquc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gkzykdtls.sHtML

[Q80] 字符串截取
来源：http://mobile.sjlbkw.cn/Article/details/gowrpyybi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gybrlztar.sHtML

[Q81] 字符串替换
来源：http://mobile.sjlbkw.cn/Article/details/givaxcyon.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gkrvnobxb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.sjlbkw.cn/Article/details/gyzqjxzjn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gmtmhwvvf.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/gkpotkvfc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gmjexduwc.sHtML

[Q84] 去除首尾空格
来源：http://3g.fktsv.cn/Article/details/gerifsijs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gubgksvwb.sHtML

[Q85] 数值取整
来源：http://baike.fktsv.cn/Article/details/gwhniwtsg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.bbcook.cn/Article/details/gkyiadugh.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.yfazqb.com/Article/details/ghdsuledc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gryqupbns.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.epnwcf.com/Article/details/goceoxnes.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fktsv.cn/Article/details/gniiowouo.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.sjlbkw.cn/Article/details/gwtssimou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gqdrwzabq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.tarul.cn/Article/details/gqdroufpu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.bbcook.cn/Article/details/gbmwjwxfu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.tarul.cn/Article/details/gfwxwmzwk.sHtML

[Q90] 生成序号列
来源：http://www.blog.epnwcf.com/Article/details/gzxusxyve.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.tarul.cn/Article/details/guqmcjygw.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/greijuthd.sHtML

R. Bash 专题
来源：http://www.blog.fktsv.cn/Article/details/gcyupjdod.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpvstnftb.sHtML

[R01] shebang 与严格模式
来源：http://blog.fktsv.cn/Article/details/gsmgzvynp.sHtML

#!/usr/bin/env bash
来源：http://blog.bbcook.cn/Article/details/gnqgdtsqh.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/gasdnlfnf.sHtML

[R02] 变量赋值与使用
来源：http://m.share.tarul.cn/Article/details/gkrwelbdr.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.bbcook.cn/Article/details/ghorvovlg.sHtML

[R03] 只读变量
来源：http://m.share.sjlbkw.cn/Article/details/gtaktdrtv.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/getmmxbxs.sHtML

[R04] 位置参数
来源：http://blog.sjlbkw.cn/Article/details/gkalpaeti.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.sjlbkw.cn/Article/details/gyzzjtzif.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/gbkfgelhh.sHtML

name="${1:-default}"
来源：http://mobile.yfazqb.com/Article/details/gbumwbaiy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.yfazqb.com/Article/details/gsmghdqff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.bbcook.cn/Article/details/gpbcmxhpg.sHtML

[R07] if 判断文件
来源：http://m.share.bbcook.cn/Article/details/gvewlopor.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.vehdjk.com/Article/details/gdfwzpieq.sHtML

[R08] 数值比较
来源：http://blog.yfazqb.com/Article/details/gadjgsslo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.vehdjk.com/Article/details/gglsbhmso.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gdrbdykzr.sHtML


<!-- 参考信息 -->