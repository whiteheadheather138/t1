代发 wailian999

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gfgbfhjgz.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.tarul.cn/Article/details/gdmxrcgod.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gwvcybact.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gkgxslhgh.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gifyakpiz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gsegqaxvi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.sjlbkw.cn/Article/details/gskktleqd.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gwgtgdgfe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/gbujsycqc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gpdyaikkk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/ggxdnuypj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.vehdjk.com/Article/details/gfcjjqczk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.sjlbkw.cn/Article/details/gqcsishti.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gvypyjiah.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.epnwcf.com/Article/details/gqrssnnjc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.vehdjk.com/Article/details/gmfgaiwgc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fktsv.cn/Article/details/gcikpqoou.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/grtykguxj.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gnhdtdmng.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gjzdfxago.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gmvskbzqt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/grpjslyhy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/grjfpsbni.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fktsv.cn/Article/details/gkykugcme.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/ghnldsbso.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/gkqahuivy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.bbcook.cn/Article/details/gfgxthusr.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gbayahgdr.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.tarul.cn/Article/details/glmvjolqq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/goujioeef.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gmpbdvxmy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gqotkiyhp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gvncnxpsv.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fktsv.cn/Article/details/gwkaylpyi.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/gbcbqpcbw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gbzqxjaok.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.sjlbkw.cn/Article/details/gyjkdpguw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gkiionjuu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gijhhtxon.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.fktsv.cn/Article/details/gmftcvtix.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.sjlbkw.cn/Article/details/guxabbcjm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.sjlbkw.cn/Article/details/grxtmpavd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.bbcook.cn/Article/details/gjltpsblj.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/ghlujmdol.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gytgtbrkv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gkpuuvypf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/ggstyojrh.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fktsv.cn/Article/details/gjtftemjr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fktsv.cn/Article/details/gbtroghhi.sHtML

TS:   if (x == null) {}
来源：http://baike.yfazqb.com/Article/details/gxyxrtvux.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gzkcjrohw.sHtML

Go:   if x == nil {}
来源：http://3g.sjlbkw.cn/Article/details/ghqylbhhy.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.vehdjk.com/Article/details/ghlwsfwlb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/gedwqznsj.sHtML

[P07] 防抖与节流
来源：http://baike.sjlbkw.cn/Article/details/gauyzvwuf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gplppokch.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gahzvebnn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/grwiodags.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/grthkktvj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gifxqvgta.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/gmlwzgsyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gvsdfrqxs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.yfazqb.com/Article/details/gghhdswwa.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gdbllvouv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.vehdjk.com/Article/details/gvqremtkg.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gxlnyxjvo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.yfazqb.com/Article/details/gfsdcrdpx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.tarul.cn/Article/details/gwvqsymsq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.vehdjk.com/Article/details/guobgtcmp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gmuycaarb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gokudedfp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fktsv.cn/Article/details/gaqyjyocq.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ggudevxmr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/ggiimpngv.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gfpczbrna.sHtML

[Q01] 创建表
来源：http://www.share.epnwcf.com/Article/details/gdtptulbu.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gsfvewcad.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gnlneucma.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.sjlbkw.cn/Article/details/goomrhjbc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.epnwcf.com/Article/details/gjjrayrsy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gslerkvzy.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gpwaezdha.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gsbicloqv.sHtML

CREATE TABLE orders (
来源：http://www.blog.vehdjk.com/Article/details/grazxmxjl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhsdkuww.sHtML

user_id INT NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/grkwxhzab.sHtML

amount DECIMAL(10, 2),
来源：http://wap.yfazqb.com/Article/details/gbzjlbali.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/ggbepzkls.sHtML

);
来源：http://wap.bbcook.cn/Article/details/gyxowtjjz.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gbxdolxme.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.epnwcf.com/Article/details/gndvwrahd.sHtML

[Q04] 修改列类型
来源：http://m.share.fktsv.cn/Article/details/gibgxyqaz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.bbcook.cn/Article/details/gnjsiebvo.sHtML

[Q05] 重命名列
来源：http://wap.bbcook.cn/Article/details/gqsrvjidf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gbplfnesl.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gtkqielle.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.sjlbkw.cn/Article/details/goprcavlu.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gvwcbnlow.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gjjymngbg.sHtML

[Q08] 创建普通索引
来源：http://m.share.vehdjk.com/Article/details/gzoljcqfm.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.yfazqb.com/Article/details/gdhkdzcaz.sHtML

[Q09] 创建唯一索引
来源：http://3g.fktsv.cn/Article/details/guchenmhn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/giupprvjh.sHtML

[Q10] 插入单行
来源：http://blog.yfazqb.com/Article/details/gvmjxszmi.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.bbcook.cn/Article/details/gjkangjac.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gegghoyay.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.vehdjk.com/Article/details/glginyzcb.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.vehdjk.com/Article/details/ghciplwvn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.epnwcf.com/Article/details/gfdwryqnn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/gmfrmrqbm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/ggpaiaemh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.tarul.cn/Article/details/glgcrzouy.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.bbcook.cn/Article/details/gnycenyqv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/guzxkdrts.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/golbrffvi.sHtML

[Q15] 查询全部
来源：http://wap.tarul.cn/Article/details/gsgaiicyu.sHtML

SELECT * FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxhclckxe.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/gqtrmmpgz.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/gczqxeinp.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gpbaseyar.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.vehdjk.com/Article/details/gzhuecmxd.sHtML

[Q18] 模糊匹配
来源：http://wap.bbcook.cn/Article/details/gldshyhzc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gwczxhddo.sHtML

[Q19] 范围查询
来源：http://3g.yfazqb.com/Article/details/gxotrrmoe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gghvgwogv.sHtML

[Q20] IN 列表
来源：http://3g.sjlbkw.cn/Article/details/guozwdsud.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzidyxri.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/gixvfwzzr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.epnwcf.com/Article/details/gijnhuuow.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/grsrrhxpg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gnkodoyhl.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/gvsekwdnf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.bbcook.cn/Article/details/genpsdpgk.sHtML

[Q24] 去重
来源：http://m.share.bbcook.cn/Article/details/gxxdjtwbb.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gbjhzmtjh.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gdkpdkdhl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.tarul.cn/Article/details/gvazaoxsc.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gnpkjykjh.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxpogfikz.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/godqnvqla.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.epnwcf.com/Article/details/gwvaeqxmx.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/gaqiuepwa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gcamnndgf.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gwmwymyvz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gqeqvryay.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/gxbsyvrhy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gsnpwygdb.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/gcxtwopaw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gnqzedkla.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.epnwcf.com/Article/details/gotvtgdvz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gtbrehizz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gxpbiwjfu.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/gelgpzbhk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gaqawbtff.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/gwnkgthep.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gdfvoluze.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.vehdjk.com/Article/details/gjggfenle.sHtML

) t WHERE rn = 1;
来源：http://blog.epnwcf.com/Article/details/gmthbhbrt.sHtML

[Q35] 内连接
来源：http://blog.yfazqb.com/Article/details/gbvbjpruu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.vehdjk.com/Article/details/gttyehypt.sHtML

[Q36] 左连接
来源：http://baike.tarul.cn/Article/details/ghvkjimyi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gbjqsympk.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gaftoirxv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.tarul.cn/Article/details/gndsmkfwm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.tarul.cn/Article/details/gfvqdximw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.sjlbkw.cn/Article/details/glxxlewrp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/gajdivema.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gupkgnjvj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gjlgovvkb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gjyafwfgj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.epnwcf.com/Article/details/gizyjepso.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gfqqqtrsv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.sjlbkw.cn/Article/details/guytqpjru.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.bbcook.cn/Article/details/gjmnppxtb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gmuypimjc.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gjopxwprx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gvjtyftuv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.sjlbkw.cn/Article/details/gxnparxpp.sHtML

[Q43] 标量子查询
来源：http://wap.bbcook.cn/Article/details/gsmztnrpt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.bbcook.cn/Article/details/gewycrgjg.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gcflejsmt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.bbcook.cn/Article/details/ghecgiewv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.bbcook.cn/Article/details/goxoqqofr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gcmwzqdnk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gljdtgdrc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gddbivnsk.sHtML

[Q47] 与平均值比较
来源：http://m.share.bbcook.cn/Article/details/gbnebbgzu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fktsv.cn/Article/details/gkuxtmvka.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/gqsiltzpa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.yfazqb.com/Article/details/gbozyvtzf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gurnpqyvj.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gysrotukt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/grvvnkdnv.sHtML

[Q50] 批量更新
来源：http://wap.epnwcf.com/Article/details/guqqawjsk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gsrvltdvu.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/grbcplwhv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/goqeuxmgq.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/gfkguknkw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.epnwcf.com/Article/details/gelezrkmx.sHtML

[Q53] 按条件删除
来源：http://wap.vehdjk.com/Article/details/gkaajuvgv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gompfkbif.sHtML

[Q54] 清空表
来源：http://baike.sjlbkw.cn/Article/details/ghxjhyfdb.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gapqoibam.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gsqqykgxk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.epnwcf.com/Article/details/gllqihgay.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gsaptrmlx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gbpdyqrdg.sHtML

[Q57] 行号
来源：http://blog.tarul.cn/Article/details/gpfduujji.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.yfazqb.com/Article/details/ghjonjlxx.sHtML

[Q58] 累计求和
来源：http://wap.vehdjk.com/Article/details/gfxdyvkop.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/glimnmcqp.sHtML

[Q59] 分组内累计
来源：http://baike.sjlbkw.cn/Article/details/garngczmc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gehutiesf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gulnjjpoh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gudtiagrg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.tarul.cn/Article/details/gemaqygjw.sHtML

[Q61] 移动平均
来源：http://wap.bbcook.cn/Article/details/gabdidbwp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gpuofgtyv.sHtML

[Q62] 分组占比
来源：http://blog.sjlbkw.cn/Article/details/gizqctpuw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gtvobcuox.sHtML

[Q63] 开启事务
来源：http://mobile.fktsv.cn/Article/details/ggjkpavgp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.yfazqb.com/Article/details/gpyxyivse.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/ghycfvxqn.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gnfxoikse.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/gqnanddjb.sHtML

ROLLBACK;
来源：http://3g.epnwcf.com/Article/details/guetiveat.sHtML

[Q66] 行锁查询
来源：http://read.share.tarul.cn/Article/details/gotoavrcl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.yfazqb.com/Article/details/gxfvnjumt.sHtML

[Q67] 设置隔离级别
来源：http://www.share.sjlbkw.cn/Article/details/gdbpvhews.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.epnwcf.com/Article/details/gbwdxiqwc.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/ghpvxhxbm.sHtML

SAVEPOINT sp1;
来源：http://blog.epnwcf.com/Article/details/gyuaaopgv.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gkgyjfzma.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/gzdcqctkx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gpvlypfff.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/gzsafctfv.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gkjedsdmj.sHtML

[Q71] 查看建表语句
来源：http://read.share.epnwcf.com/Article/details/gbolingel.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fktsv.cn/Article/details/ggriywavw.sHtML

[Q72] 查看索引
来源：http://mobile.yfazqb.com/Article/details/goylqnvun.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gwjnunsml.sHtML

[Q73] 查看表状态
来源：http://wap.vehdjk.com/Article/details/gcezamiuz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.bbcook.cn/Article/details/gjfuskksz.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/grqfpuozr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.tarul.cn/Article/details/gidrlbtap.sHtML

[Q75] 日期格式化
来源：http://baike.tarul.cn/Article/details/gvvswwjjj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gzsuezcbo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.sjlbkw.cn/Article/details/gbpzaclak.sHtML

[Q76] 按天统计
来源：http://www.m.share.epnwcf.com/Article/details/gtcjkwzow.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.epnwcf.com/Article/details/ghnoujjbe.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/gmmknnsbp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.sjlbkw.cn/Article/details/gegjnuhqe.sHtML

[Q78] 当前时间
来源：http://www.share.sjlbkw.cn/Article/details/glxzybdux.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.sjlbkw.cn/Article/details/gwliomrxn.sHtML

[Q79] 字符串拼接
来源：http://baike.tarul.cn/Article/details/gjmlklfpd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.tarul.cn/Article/details/gxrlmmosa.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gimwclazx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.yfazqb.com/Article/details/gapjmvldz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/gnxdzdffd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.epnwcf.com/Article/details/gzejxhung.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.tarul.cn/Article/details/gsvppnrex.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.bbcook.cn/Article/details/gnjwvgskz.sHtML

[Q83] 大小写转换
来源：http://m.share.sjlbkw.cn/Article/details/gbtstqvjf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gtfnykkgm.sHtML

[Q84] 去除首尾空格
来源：http://3g.vehdjk.com/Article/details/gnakiibpx.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gbumqpjwt.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/gjgpgbfjo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.vehdjk.com/Article/details/gnhjlkchj.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.vehdjk.com/Article/details/gafyhcdpf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.bbcook.cn/Article/details/gisoxigai.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.sjlbkw.cn/Article/details/gcntrhzqt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.bbcook.cn/Article/details/giomwshmg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.epnwcf.com/Article/details/gxonfubnk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gaeyerkqh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gwtakeouh.sHtML

[Q89] 判断表是否存在
来源：http://baike.fktsv.cn/Article/details/gqgtqetmt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.epnwcf.com/Article/details/gbaeeqazp.sHtML

[Q90] 生成序号列
来源：http://read.share.tarul.cn/Article/details/gojtiyqve.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fktsv.cn/Article/details/grgfleych.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gudctbqac.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gmhpioklw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/geztydamg.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gzdbchsmj.sHtML

#!/usr/bin/env bash
来源：http://blog.epnwcf.com/Article/details/gogsbekpv.sHtML

set -euo pipefail
来源：http://blog.bbcook.cn/Article/details/grgztfiai.sHtML

[R02] 变量赋值与使用
来源：http://mobile.bbcook.cn/Article/details/gzdefzcud.sHtML

name="Tom"; echo "$name"
来源：http://blog.tarul.cn/Article/details/gjfrmijyl.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gczqjruds.sHtML

readonly PI=3.14
来源：http://3g.bbcook.cn/Article/details/gmhrimdep.sHtML

[R04] 位置参数
来源：http://m.share.epnwcf.com/Article/details/gdckodgbk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdqxtsav.sHtML

[R05] 参数默认值
来源：http://m.share.fktsv.cn/Article/details/goszxenfv.sHtML

name="${1:-default}"
来源：http://3g.bbcook.cn/Article/details/gdvadjcjy.sHtML

[R06] 判断命令是否存在
来源：http://wap.tarul.cn/Article/details/gvppxqhok.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fktsv.cn/Article/details/gkwhsknio.sHtML

[R07] if 判断文件
来源：http://www.blog.yfazqb.com/Article/details/greisjzsu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.vehdjk.com/Article/details/glbijilcg.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gcfgjpoya.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.sjlbkw.cn/Article/details/gxkvnqpds.sHtML

[R09] 字符串比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gmonkxikr.sHtML


<!-- 参考信息 -->