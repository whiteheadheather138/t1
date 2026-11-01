代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.tarul.cn/Article/details/gqysuyduu.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gxokedext.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gyocjekxw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gmaiodckv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.vehdjk.com/Article/details/gfpukhzux.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/gfowdbqoq.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gpznsxwlx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/ggfmqisum.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.tarul.cn/Article/details/gpyjhbaqh.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.sjlbkw.cn/Article/details/ghwonzbtm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.vehdjk.com/Article/details/gymdyxvdm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gafjamsvh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gauqlalbn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/gulobhvdu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gvvcnetfr.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gwencalir.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gcvwppbcd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.sjlbkw.cn/Article/details/gnevbcljj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/ghipnlvpd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gdglnocjo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gyymcjaor.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gjdeqqhxa.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/gvvjtgond.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gnjdmvhju.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/ganzwxpup.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gcnkwghrz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/gwlftuvlu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/ggwdranrm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gzbahukle.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.vehdjk.com/Article/details/gczxbiuzd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gxtmrdbdk.sHtML

Ruby: a == b
来源：http://3g.tarul.cn/Article/details/gjlggrewr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gomnqrfwq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gundfxjmg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.sjlbkw.cn/Article/details/gusdretto.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/gphkaztbn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gdtaxajjr.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gurobsioe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/goyglglcr.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gabajpwoe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.epnwcf.com/Article/details/gmesobqgo.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gqevzwpzg.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gkqyxryqw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.sjlbkw.cn/Article/details/gvgnoeccx.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.vehdjk.com/Article/details/gblmwfrks.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gbwcoxypp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gpvgjmpfz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.vehdjk.com/Article/details/gvrvdtyqk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.tarul.cn/Article/details/gcqtkbhtc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fktsv.cn/Article/details/givcrxhlx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/gzvwimgej.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gscndddkg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.tarul.cn/Article/details/gwwpaduaw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/grtbljsbj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fktsv.cn/Article/details/gsdfatnrw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gpystfeia.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.tarul.cn/Article/details/gdbrrzpmg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/gkotlajdj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gxqtiqxlc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.tarul.cn/Article/details/gtwomwkxj.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkltsbqql.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gnbfkknhd.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gquxxwyzb.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gfphuenib.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/ghprvonpj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/glydmqerb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gkskxdnme.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.tarul.cn/Article/details/gqhtxzzth.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gjleflcuv.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gurqbznar.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gwmlohxbx.sHtML

CREATE TABLE orders (
来源：http://www.share.fktsv.cn/Article/details/ggcvfxugd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gukqhzmtj.sHtML

user_id INT NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gsfwycjzs.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gfilosrdb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.vehdjk.com/Article/details/gyjoxjgch.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gvoolqgbp.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/gfqszrhzo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/gqneowruo.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gyubzwhvr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gqyoxtedj.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/gmgucyijx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/gzxrctagl.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gggcygbpq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.epnwcf.com/Article/details/gzkfkqdft.sHtML

[Q07] 删除表
来源：http://wap.sjlbkw.cn/Article/details/gxvxhfczt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.fktsv.cn/Article/details/grodmftim.sHtML

[Q08] 创建普通索引
来源：http://mobile.bbcook.cn/Article/details/glpdzwirb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gmpjucjac.sHtML

[Q09] 创建唯一索引
来源：http://mobile.bbcook.cn/Article/details/gtysfwlbg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gkmtmlobg.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/ggktlwrsj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.epnwcf.com/Article/details/gyfgiacyr.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.tarul.cn/Article/details/gghtmxuhb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gyiconfqo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.bbcook.cn/Article/details/goxbjfqvt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/ggghjqvkb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.tarul.cn/Article/details/gujfyzcpv.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gbaxqmigy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gbeuulzmu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.bbcook.cn/Article/details/gstmvdzgd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/gragwcgbs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.yfazqb.com/Article/details/ggmsnshva.sHtML

[Q15] 查询全部
来源：http://www.share.yfazqb.com/Article/details/gveakkcpr.sHtML

SELECT * FROM users;
来源：http://blog.fktsv.cn/Article/details/geeysznld.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/glkvwdbbx.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gpkofkkbh.sHtML

[Q17] 条件查询
来源：http://mobile.vehdjk.com/Article/details/ggtxlbzve.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gfrmrgxsv.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/ggmezcbbj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gqgwmfepr.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/gzljcyvhr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.bbcook.cn/Article/details/gdzdvbeby.sHtML

[Q20] IN 列表
来源：http://wap.yfazqb.com/Article/details/ghrsclwog.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gkudlwxjk.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gylakromz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.epnwcf.com/Article/details/ggmescnjn.sHtML

[Q22] 排序
来源：http://www.m.share.epnwcf.com/Article/details/gdgsngoul.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/guablykjj.sHtML

[Q23] 分页
来源：http://read.share.bbcook.cn/Article/details/gkqtyeagj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gufiezknv.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gsvelxrpk.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.bbcook.cn/Article/details/ghqdpxdjt.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fktsv.cn/Article/details/gjovbosqm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/glinrnuav.sHtML

[Q26] 计数
来源：http://wap.tarul.cn/Article/details/glziuiakj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.vehdjk.com/Article/details/gixsomahs.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gqlexwhgh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gkmlhjapm.sHtML

[Q28] 求和与平均
来源：http://mobile.bbcook.cn/Article/details/grxspzftv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gglzdaycv.sHtML

[Q29] 最大最小值
来源：http://read.share.epnwcf.com/Article/details/gduvczozx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gfymwkjtz.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gklxigcjy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fktsv.cn/Article/details/gnfqfbbun.sHtML

[Q31] 分组后过滤
来源：http://www.share.tarul.cn/Article/details/gdzfvztpy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.epnwcf.com/Article/details/gqdmtzwae.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gssdhftwn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gkirwnshk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/geasajtdp.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/glpkxkhyv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fktsv.cn/Article/details/gnueralyj.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/gvmhuaqil.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gqplphnrb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gtdnudqtx.sHtML

) t WHERE rn = 1;
来源：http://3g.sjlbkw.cn/Article/details/gstxfphup.sHtML

[Q35] 内连接
来源：http://baike.sjlbkw.cn/Article/details/gyfdlnltu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gqatohlvq.sHtML

[Q36] 左连接
来源：http://blog.sjlbkw.cn/Article/details/gjcoybgmv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gbvvxnzkw.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/glbdbgker.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.bbcook.cn/Article/details/gjvlemfqs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gdkpmdeal.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.yfazqb.com/Article/details/ghnuufrln.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gioxmpdlf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gzyhkfcuy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.yfazqb.com/Article/details/gxkrkgfvx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.epnwcf.com/Article/details/gjnzxelcu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gzmchmsqu.sHtML

[Q41] 多表连接
来源：http://blog.epnwcf.com/Article/details/gabqmyrbc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/ghqyihyry.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.tarul.cn/Article/details/gsbouhmop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fktsv.cn/Article/details/gnsswztdl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.sjlbkw.cn/Article/details/gkyfakquw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/goytqgbtv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.yfazqb.com/Article/details/guniskslv.sHtML

[Q43] 标量子查询
来源：http://wap.epnwcf.com/Article/details/gulragfee.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fktsv.cn/Article/details/gbuxhgaqh.sHtML

[Q44] IN 子查询
来源：http://www.blog.sjlbkw.cn/Article/details/gpsvhhinz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gnshpuivz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gltkmqnws.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.yfazqb.com/Article/details/gjspgnihb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/givwelkee.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gvvonlruv.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/gmcxomctj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gobunopcz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.epnwcf.com/Article/details/gwquhwlam.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gmapqufrq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gslycnxgs.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/gegbgpimx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gywzdyopu.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/geuormewr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gzmlovoke.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/gwgyakgmx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.sjlbkw.cn/Article/details/gxqhnboil.sHtML

[Q52] 删除指定行
来源：http://m.share.bbcook.cn/Article/details/gvloztuli.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gujmsqkok.sHtML

[Q53] 按条件删除
来源：http://mobile.fktsv.cn/Article/details/gdwyswgqr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gldavtnwr.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/gqiueratb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.yfazqb.com/Article/details/gpmphrqcn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gincxcjqb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gqrdpbdhd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gseihdhcb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gfqwagdmx.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/gekrslprt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gtwihtpcs.sHtML

[Q58] 累计求和
来源：http://baike.epnwcf.com/Article/details/gfqrlqjwo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gmtahqcqs.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gxmjksmdk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gngimyyqk.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.bbcook.cn/Article/details/glzwwybhh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.yfazqb.com/Article/details/gssrdgabp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fktsv.cn/Article/details/gocmseadk.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gsongxjxv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gmonlpqzc.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gdtqizgur.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gybsfsdgt.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gqicvnodc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.sjlbkw.cn/Article/details/gwyzedikv.sHtML

[Q64] 提交事务
来源：http://www.share.epnwcf.com/Article/details/gxwwcmysq.sHtML

COMMIT;
来源：http://blog.bbcook.cn/Article/details/gjpdzpovb.sHtML

[Q65] 回滚事务
来源：http://www.blog.yfazqb.com/Article/details/gqmtalgww.sHtML

ROLLBACK;
来源：http://www.share.epnwcf.com/Article/details/gpcnupdaz.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gtxvuxjov.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gvtbxdodk.sHtML

[Q67] 设置隔离级别
来源：http://www.share.epnwcf.com/Article/details/gqifqckir.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gegxkpmlt.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/gbxsoqzgs.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/glgfskxtf.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/glofuaczq.sHtML

[Q69] 查看执行计划
来源：http://wap.bbcook.cn/Article/details/gfeaycxuv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.tarul.cn/Article/details/godkbazdk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.yfazqb.com/Article/details/gidqmxbcz.sHtML

ANALYZE TABLE users;
来源：http://read.share.yfazqb.com/Article/details/gqkadrikw.sHtML

[Q71] 查看建表语句
来源：http://wap.bbcook.cn/Article/details/gifqfplds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.vehdjk.com/Article/details/girpjprlm.sHtML

[Q72] 查看索引
来源：http://www.m.share.vehdjk.com/Article/details/glwaxmbgf.sHtML

SHOW INDEX FROM users;
来源：http://baike.epnwcf.com/Article/details/gzvraflaq.sHtML

[Q73] 查看表状态
来源：http://baike.yfazqb.com/Article/details/ghuzahxsj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/gnthutukm.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gdvpxrgco.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.vehdjk.com/Article/details/ggchutvnb.sHtML

[Q75] 日期格式化
来源：http://wap.fktsv.cn/Article/details/grjbijpyl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gbgtbkyxe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.sjlbkw.cn/Article/details/gexlwrrmv.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gnffgvypz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fktsv.cn/Article/details/gvoprfolf.sHtML

[Q77] 时间加减
来源：http://www.blog.yfazqb.com/Article/details/gigbhwkfn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.vehdjk.com/Article/details/gwajtkroh.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/gtfzczhkm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.sjlbkw.cn/Article/details/gswivcplc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.yfazqb.com/Article/details/glihgdtxz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.bbcook.cn/Article/details/gdazvcdzl.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gmcfxkjzm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.epnwcf.com/Article/details/grihypiov.sHtML

[Q81] 字符串替换
来源：http://baike.tarul.cn/Article/details/gpdpwtvbg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.yfazqb.com/Article/details/gmqebzxkh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.bbcook.cn/Article/details/glbafwxvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gaidlpbeg.sHtML

[Q83] 大小写转换
来源：http://www.share.tarul.cn/Article/details/gnxhgaaeb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gvjnlrfpz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.sjlbkw.cn/Article/details/gphrsxhit.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gjfqgzfhd.sHtML

[Q85] 数值取整
来源：http://wap.fktsv.cn/Article/details/gvjhzqwrx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fktsv.cn/Article/details/ggtqpejpu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/gnwskqrjh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.yfazqb.com/Article/details/gyggxwwtt.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fktsv.cn/Article/details/gifhaterr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.vehdjk.com/Article/details/gvahmfqfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gifxnxvit.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.sjlbkw.cn/Article/details/gbwftgind.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.tarul.cn/Article/details/gxkyvkexu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.vehdjk.com/Article/details/gpmxghdec.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.epnwcf.com/Article/details/gzvcxzkng.sHtML

[Q90] 生成序号列
来源：http://www.share.sjlbkw.cn/Article/details/gygxwtzui.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.vehdjk.com/Article/details/gqhxlpzmp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqtepkhef.sHtML

R. Bash 专题
来源：http://3g.epnwcf.com/Article/details/gbcgombpe.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gumgraiov.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fktsv.cn/Article/details/gdfmlruax.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.yfazqb.com/Article/details/gwwlndhbb.sHtML

set -euo pipefail
来源：http://www.share.tarul.cn/Article/details/goszoggls.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gxajffvjo.sHtML

name="Tom"; echo "$name"
来源：http://www.share.sjlbkw.cn/Article/details/gszqsfezd.sHtML

[R03] 只读变量
来源：http://mobile.vehdjk.com/Article/details/gdadrkwmo.sHtML

readonly PI=3.14
来源：http://3g.fktsv.cn/Article/details/gvhsurlir.sHtML

[R04] 位置参数
来源：http://www.share.vehdjk.com/Article/details/gqjyzncvf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.tarul.cn/Article/details/gwdsusivb.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gmdtiicbw.sHtML

name="${1:-default}"
来源：http://mobile.sjlbkw.cn/Article/details/gaueedczk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fktsv.cn/Article/details/gjiyxpuar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fktsv.cn/Article/details/gbrdsqtad.sHtML

[R07] if 判断文件
来源：http://baike.yfazqb.com/Article/details/gxrxlctpv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gcwuqoazi.sHtML

[R08] 数值比较
来源：http://www.share.vehdjk.com/Article/details/gkctibgdi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.bbcook.cn/Article/details/gjzoflmvt.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/geslkbvdg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.vehdjk.com/Article/details/gcsspmhnt.sHtML

[R10] 正则匹配
来源：http://blog.sjlbkw.cn/Article/details/gspdwrsye.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.epnwcf.com/Article/details/gbvkzultd.sHtML

[R11] case 多分支
来源：http://www.m.share.sjlbkw.cn/Article/details/gcutoegyw.sHtML

case "$1" in
来源：http://www.blog.epnwcf.com/Article/details/geflofplq.sHtML

start) echo "启动" ;;
来源：http://www.blog.vehdjk.com/Article/details/gdcvttkrk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fktsv.cn/Article/details/gkadawnvc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.tarul.cn/Article/details/gciqnjncp.sHtML

esac
来源：http://blog.yfazqb.com/Article/details/gmubczpyg.sHtML

[R12] for 遍历文件
来源：http://m.share.tarul.cn/Article/details/gnqglhnld.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.vehdjk.com/Article/details/gbinupfwj.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gdvttzkgx.sHtML


<!-- 参考信息 -->