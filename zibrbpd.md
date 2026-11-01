代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.bbcook.cn/Article/details/gpyzbkkct.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.yfazqb.com/Article/details/glbwcdmty.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gnfvndmtm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.vehdjk.com/Article/details/gafohxrpm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gixudnyjx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fktsv.cn/Article/details/gtbdzzijs.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gvbprhhrr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gpmzhjvqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gxxktawka.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gwvjybdgs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gqwbigrpx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/grsvjuffd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gatrdzxew.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.sjlbkw.cn/Article/details/gvcdgvsyz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/gzzwlezng.sHtML

[P04] 求长度
来源：http://3g.bbcook.cn/Article/details/gpoeaxsly.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.tarul.cn/Article/details/gtiilicyz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.tarul.cn/Article/details/gzqivjzmp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gjbbjaphs.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.yfazqb.com/Article/details/gdtjtnkew.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fktsv.cn/Article/details/gumvokhmf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/gcpkikiuc.sHtML

Ruby: x.length;  x.size
来源：http://blog.fktsv.cn/Article/details/gxgdhvhyr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gvhbfwkzd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fktsv.cn/Article/details/gkeurjruv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.bbcook.cn/Article/details/gxorlpzjl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/ggnwfgjfz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/gyltyyemh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gbdawqjbw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/gbzzdompi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gmduvbjfq.sHtML

Ruby: a == b
来源：http://read.share.epnwcf.com/Article/details/ghdbabbtk.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.bbcook.cn/Article/details/gnhejpppb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gxxfuzeig.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gopujonpg.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gsvstrnmy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.fktsv.cn/Article/details/gxkuwkggr.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/gfumttdzo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gavzwcizk.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/groqrwbad.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gptqsfjgq.sHtML

C#:   if (x is null) {}
来源：http://wap.tarul.cn/Article/details/gdxeoyjlb.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/gwuhaueea.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gyxkxajpf.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gzuesqswk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gspxmdkou.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gptcixsis.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.bbcook.cn/Article/details/gtdxshldv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.bbcook.cn/Article/details/gtzznnfax.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.sjlbkw.cn/Article/details/gvugnbpye.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/giezppiox.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/grwywujhz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fktsv.cn/Article/details/gfnwetgix.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.yfazqb.com/Article/details/gcvekarwt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/ghobtspfa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/gcvucvwcw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.vehdjk.com/Article/details/grapszihk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gyyzjysyp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gzgcpaumd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gjfgdohmy.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gjzqqqguw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gfuyfuiro.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/galqkujju.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/gbiqsxaby.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/girmczfny.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/gpwxzgwnr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/gqbgcnkuj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.vehdjk.com/Article/details/gjmuxfbpx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.epnwcf.com/Article/details/goomphymn.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gorqguelc.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gnviwenyu.sHtML

CREATE TABLE orders (
来源：http://read.share.tarul.cn/Article/details/gbuasnyon.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gwmtwfnjq.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gzdqvzeym.sHtML

amount DECIMAL(10, 2),
来源：http://baike.tarul.cn/Article/details/gtooraszc.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fktsv.cn/Article/details/ghfhfhelx.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gegyjbxba.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gqgjubust.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.yfazqb.com/Article/details/gnelfzaev.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gtzeflpzj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gyutsbyok.sHtML

[Q05] 重命名列
来源：http://3g.fktsv.cn/Article/details/gyatpcsyz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxzsynun.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gmvyiausi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fktsv.cn/Article/details/gcemtsmuo.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gqbvghqyv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.sjlbkw.cn/Article/details/gwpvpdpuz.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gonribigi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.sjlbkw.cn/Article/details/gcyfahmht.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fktsv.cn/Article/details/ghuevhrgo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gjtxbstnm.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/gspztkpmz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.vehdjk.com/Article/details/gvvlanzbu.sHtML

[Q11] 一次插入多行
来源：http://mobile.epnwcf.com/Article/details/ggbquiwkb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.yfazqb.com/Article/details/ggefdkqos.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/ghniwzdgz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gmmrduygj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gbzgyitnt.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gjcccdxxh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.epnwcf.com/Article/details/gyvvgktxd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/grjhavrvw.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.vehdjk.com/Article/details/gwxepgdno.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/giqjjnmby.sHtML

[Q15] 查询全部
来源：http://blog.sjlbkw.cn/Article/details/gbkucvvys.sHtML

SELECT * FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gsblrycme.sHtML

[Q16] 查询指定列
来源：http://www.blog.bbcook.cn/Article/details/ghvougdbw.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gqxiujcjo.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gjkwwhccp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.tarul.cn/Article/details/grjgbmfnv.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.fktsv.cn/Article/details/gbkgxecik.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gywbwqflr.sHtML

[Q19] 范围查询
来源：http://mobile.vehdjk.com/Article/details/gatjwnfmm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.sjlbkw.cn/Article/details/gddrgaxxo.sHtML

[Q20] IN 列表
来源：http://m.share.sjlbkw.cn/Article/details/gmdnpkrsl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fktsv.cn/Article/details/gghqenuee.sHtML

[Q21] 空值判断
来源：http://read.share.sjlbkw.cn/Article/details/geuwlrmqw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gbcbxfwyw.sHtML

[Q22] 排序
来源：http://3g.fktsv.cn/Article/details/gzpqhzmqc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gramirydx.sHtML

[Q23] 分页
来源：http://www.m.share.fktsv.cn/Article/details/gnjirznyy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/gjiieemrh.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/ggxzuvcfd.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfcaviszv.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/gkhsclvba.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.tarul.cn/Article/details/gdkfrvrhr.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gilcatwhl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.yfazqb.com/Article/details/gveocowkb.sHtML

[Q27] 条件计数
来源：http://www.share.tarul.cn/Article/details/gknrxufvq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.bbcook.cn/Article/details/gkwqofcvs.sHtML

[Q28] 求和与平均
来源：http://mobile.fktsv.cn/Article/details/gcbiynrhm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/grlatqouz.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gxcclfroc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/giaqumvxu.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gemfpzhfc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.bbcook.cn/Article/details/gtmuhcpsy.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gpxwstvgc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.yfazqb.com/Article/details/gbqfnflei.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.sjlbkw.cn/Article/details/gwbmwqfzj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gszlescfp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fktsv.cn/Article/details/gkxscqwmm.sHtML

[Q33] 多列分组
来源：http://m.share.sjlbkw.cn/Article/details/gufucjuqr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gcsxdokny.sHtML

[Q34] 每组取第一条
来源：http://wap.tarul.cn/Article/details/gvnxvmslz.sHtML

SELECT * FROM (
来源：http://www.m.share.tarul.cn/Article/details/ggpytfcaw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/gfwgvqojp.sHtML

) t WHERE rn = 1;
来源：http://3g.tarul.cn/Article/details/godvtqcta.sHtML

[Q35] 内连接
来源：http://read.share.yfazqb.com/Article/details/glwvwvwnk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/giicjaqcc.sHtML

[Q36] 左连接
来源：http://baike.fktsv.cn/Article/details/gzhwzfhvh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/gvzusgnih.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gsyjbjwrw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gtgnpyloh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.tarul.cn/Article/details/gwnyeslwu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gktksvxcd.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.yfazqb.com/Article/details/gapsthkvs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.bbcook.cn/Article/details/gykwmsyew.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gbbgnksfx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.bbcook.cn/Article/details/gvnehuntn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fktsv.cn/Article/details/gqageyifg.sHtML

[Q41] 多表连接
来源：http://www.m.share.epnwcf.com/Article/details/goutdgrcf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gftvjcscn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/gzwcugidg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gnsnbxbdf.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/gzacuaymg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gehubjict.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.bbcook.cn/Article/details/geutaytao.sHtML

[Q43] 标量子查询
来源：http://www.share.yfazqb.com/Article/details/gkbjwqoqu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/glvohrlzz.sHtML

[Q44] IN 子查询
来源：http://baike.yfazqb.com/Article/details/gjyyklnhd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/gsxpwupfu.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.yfazqb.com/Article/details/gutfbxgxy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gzhwrfmvd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fktsv.cn/Article/details/gzpqurbgd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gujfpnmdr.sHtML

[Q47] 与平均值比较
来源：http://wap.sjlbkw.cn/Article/details/ggpssbmle.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/ggkikouig.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fktsv.cn/Article/details/gnqwxjgnw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.vehdjk.com/Article/details/gdsvuvoaa.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/guoeshmkn.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/gojqfiitc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gxxjakgsn.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/ghwqbkvyl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gyjsrmsst.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/gpdenlcsm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fktsv.cn/Article/details/gykeabkwx.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gjqdauvem.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.bbcook.cn/Article/details/gwzzwbhnu.sHtML

[Q53] 按条件删除
来源：http://m.share.epnwcf.com/Article/details/gyuzmiqgy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gyabsdtkw.sHtML

[Q54] 清空表
来源：http://wap.sjlbkw.cn/Article/details/gngqxxkic.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.bbcook.cn/Article/details/gzvgujqng.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gqsmvvgbz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.epnwcf.com/Article/details/gzkopeqoj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fktsv.cn/Article/details/gnvzwmrdl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gopcqpfxe.sHtML

[Q57] 行号
来源：http://m.share.vehdjk.com/Article/details/ghmlveixb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gcbroqxpj.sHtML

[Q58] 累计求和
来源：http://www.m.share.tarul.cn/Article/details/ggwctjshr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gwnspdyoq.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/glrkgoswd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gpxuaaihr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.vehdjk.com/Article/details/gsndpbyvh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.tarul.cn/Article/details/gnvbpqsuj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gijejpurd.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gdijhbmxi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/glscryhim.sHtML

[Q62] 分组占比
来源：http://read.share.sjlbkw.cn/Article/details/gciknumqg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.epnwcf.com/Article/details/gfuyjgzzq.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gmblnwafe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.tarul.cn/Article/details/gtxkgdwwy.sHtML

[Q64] 提交事务
来源：http://blog.fktsv.cn/Article/details/grjgqencp.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/godyvuiyu.sHtML

[Q65] 回滚事务
来源：http://blog.sjlbkw.cn/Article/details/gxvuyqjrh.sHtML

ROLLBACK;
来源：http://www.blog.yfazqb.com/Article/details/gsdyticwz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fktsv.cn/Article/details/gucfzglbk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/gbrahhksd.sHtML

[Q67] 设置隔离级别
来源：http://read.share.epnwcf.com/Article/details/gxfpaufko.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/govpqvasq.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/goauwstcr.sHtML

SAVEPOINT sp1;
来源：http://read.share.bbcook.cn/Article/details/gscckickq.sHtML

ROLLBACK TO sp1;
来源：http://read.share.tarul.cn/Article/details/gkzkddtzx.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/gsjbkmiiw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.epnwcf.com/Article/details/gjnyyppxm.sHtML

[Q70] 更新统计信息
来源：http://blog.fktsv.cn/Article/details/gqqpulcoz.sHtML

ANALYZE TABLE users;
来源：http://blog.tarul.cn/Article/details/geqzoewag.sHtML

[Q71] 查看建表语句
来源：http://www.blog.yfazqb.com/Article/details/geydvjnta.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.yfazqb.com/Article/details/gottovkun.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gtoqkoobk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/glfnibbqv.sHtML

[Q73] 查看表状态
来源：http://3g.sjlbkw.cn/Article/details/gbxyzbdym.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.sjlbkw.cn/Article/details/gkccfckil.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gbfpicfux.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fktsv.cn/Article/details/griomfqmu.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gpizbobwb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gsrpxbbuo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.bbcook.cn/Article/details/gmopsngbw.sHtML

[Q76] 按天统计
来源：http://read.share.sjlbkw.cn/Article/details/goqchqjbs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/gwcljgcgs.sHtML

[Q77] 时间加减
来源：http://3g.tarul.cn/Article/details/gktitvmiz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.yfazqb.com/Article/details/gcaqapsow.sHtML

[Q78] 当前时间
来源：http://m.share.sjlbkw.cn/Article/details/gzloieytk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.tarul.cn/Article/details/gmjufcwoy.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.epnwcf.com/Article/details/gdkexbkhy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fktsv.cn/Article/details/gbxvczdba.sHtML

[Q80] 字符串截取
来源：http://blog.yfazqb.com/Article/details/gzfhtzanw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/ghezxegcf.sHtML

[Q81] 字符串替换
来源：http://wap.tarul.cn/Article/details/gmkbfhepk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbnlwkwnj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fktsv.cn/Article/details/gpkjcpenm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzqbmxzep.sHtML

[Q83] 大小写转换
来源：http://wap.bbcook.cn/Article/details/gllxyaqhe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gcadecvsa.sHtML

[Q84] 去除首尾空格
来源：http://m.share.tarul.cn/Article/details/giyqhvcob.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gkiezvkca.sHtML

[Q85] 数值取整
来源：http://www.blog.sjlbkw.cn/Article/details/gmthyhxjz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gyxldklyi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.tarul.cn/Article/details/gmmpcfodz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fktsv.cn/Article/details/gcqtuzodv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.tarul.cn/Article/details/gatcngvvs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.vehdjk.com/Article/details/gglqizzyv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fktsv.cn/Article/details/gcqhbofwz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.epnwcf.com/Article/details/ggblhderj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.bbcook.cn/Article/details/ghqrmcljv.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fktsv.cn/Article/details/gahwzfnyr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gjdnpikat.sHtML

[Q90] 生成序号列
来源：http://wap.sjlbkw.cn/Article/details/goyyrcmzf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.sjlbkw.cn/Article/details/ggxdwxlrp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/goixvkwct.sHtML

R. Bash 专题
来源：http://www.blog.epnwcf.com/Article/details/gguhhknfy.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gvxlnmyrd.sHtML

[R01] shebang 与严格模式
来源：http://wap.epnwcf.com/Article/details/gbwpidoqv.sHtML

#!/usr/bin/env bash
来源：http://blog.epnwcf.com/Article/details/gbnitkjoy.sHtML

set -euo pipefail
来源：http://m.share.tarul.cn/Article/details/gibtmgfjv.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gywyqdcol.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gebmnvrcu.sHtML

[R03] 只读变量
来源：http://3g.tarul.cn/Article/details/gglrmrcqi.sHtML

readonly PI=3.14
来源：http://blog.yfazqb.com/Article/details/gomlyzgoc.sHtML

[R04] 位置参数
来源：http://www.share.tarul.cn/Article/details/gsugfdrwq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.tarul.cn/Article/details/ghipgdvke.sHtML

[R05] 参数默认值
来源：http://baike.sjlbkw.cn/Article/details/gnetytvoe.sHtML

name="${1:-default}"
来源：http://m.share.epnwcf.com/Article/details/gqtrwgixm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fktsv.cn/Article/details/gdbzwallz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.vehdjk.com/Article/details/gakqjxsix.sHtML

[R07] if 判断文件
来源：http://blog.tarul.cn/Article/details/gygyyajle.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/gnnkqjvvm.sHtML

[R08] 数值比较
来源：http://mobile.fktsv.cn/Article/details/gobynhdog.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.epnwcf.com/Article/details/ghitcejjf.sHtML

[R09] 字符串比较
来源：http://read.share.fktsv.cn/Article/details/gdgiainhx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.sjlbkw.cn/Article/details/gqvgsrhkp.sHtML

[R10] 正则匹配
来源：http://wap.yfazqb.com/Article/details/gwnooprdb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.epnwcf.com/Article/details/goeowdisf.sHtML

[R11] case 多分支
来源：http://read.share.fktsv.cn/Article/details/gyamvnpae.sHtML

case "$1" in
来源：http://read.share.sjlbkw.cn/Article/details/gvqxtkbbx.sHtML

start) echo "启动" ;;
来源：http://www.blog.epnwcf.com/Article/details/gzhezoysw.sHtML

stop)  echo "停止" ;;
来源：http://mobile.tarul.cn/Article/details/gukptrbnj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.yfazqb.com/Article/details/griajuwqx.sHtML

esac
来源：http://baike.tarul.cn/Article/details/gcvvobpiu.sHtML

[R12] for 遍历文件
来源：http://www.share.bbcook.cn/Article/details/gfirfcagd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.tarul.cn/Article/details/grjkqybwt.sHtML

[R13] for 计数循环
来源：http://wap.tarul.cn/Article/details/gqhhcazqb.sHtML


<!-- 参考信息 -->