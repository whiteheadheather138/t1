代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.tarul.cn/Article/details/goqgispdb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/gabqhmkfl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fktsv.cn/Article/details/gjbjzdydf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/gytdcwals.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gsubotwwa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/ghaxdqrpd.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/gjwsbllhv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gpxzzkgwm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.tarul.cn/Article/details/gnzspfryv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gsjjvzamc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gnzszlrnh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/gnyhjgmvo.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.vehdjk.com/Article/details/glwsbucza.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gfdkscdmh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fktsv.cn/Article/details/gjiyxjvns.sHtML

[P04] 求长度
来源：http://www.m.share.yfazqb.com/Article/details/gwbtvumfp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gsrwlbhce.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.bbcook.cn/Article/details/gogcfngtx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gijsebpla.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.yfazqb.com/Article/details/gdeulajft.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.epnwcf.com/Article/details/gcommccik.sHtML

Go:   len(arr);  len(m)
来源：http://wap.vehdjk.com/Article/details/gngozgtmc.sHtML

Ruby: x.length;  x.size
来源：http://www.share.vehdjk.com/Article/details/gphimkdsx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.epnwcf.com/Article/details/grirtnrnw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/gldpmbrgv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gcclybisc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/glxfyerde.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/ghnonpspc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gkijzzhuk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gzegfsbea.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.tarul.cn/Article/details/gvplrutzl.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/gmhwuecxo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfnczvie.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.bbcook.cn/Article/details/gdpebtmwf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.vehdjk.com/Article/details/gddmiykek.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.sjlbkw.cn/Article/details/gyqdpaywi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gbfsvtgsb.sHtML

TS:   if (x == null) {}
来源：http://3g.bbcook.cn/Article/details/giczhptgl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gxhglvuld.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/gsfuijmgp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gjxhuotgy.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.epnwcf.com/Article/details/gxneppzto.sHtML

[P07] 防抖与节流
来源：http://www.share.bbcook.cn/Article/details/gxuemhmiu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fktsv.cn/Article/details/gkaptesns.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gzztfxwbv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/guywijkih.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gtazrfjjz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gjmpescrz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.fktsv.cn/Article/details/gnwafxgnt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.yfazqb.com/Article/details/gyoedrkhq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fktsv.cn/Article/details/gctiyzwiz.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.tarul.cn/Article/details/gbgteognn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/glpkzyxnw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gyuflqjbn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.sjlbkw.cn/Article/details/gahzfdvea.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.epnwcf.com/Article/details/ggkcuuafx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.epnwcf.com/Article/details/gwuskhfda.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fktsv.cn/Article/details/gmkvwzjaz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gcjomkami.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.bbcook.cn/Article/details/gjzzqtgou.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyvvpuqpy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/guqakjtvh.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gubsdpwpg.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/graefkrsm.sHtML

CREATE TABLE users (
来源：http://m.share.sjlbkw.cn/Article/details/gcdepazoa.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.vehdjk.com/Article/details/graehcjhx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gtxloihqg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.vehdjk.com/Article/details/girswbjqk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.sjlbkw.cn/Article/details/gnlfqfrwl.sHtML

);
来源：http://baike.sjlbkw.cn/Article/details/gcgzsstlk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.epnwcf.com/Article/details/gyxxqnjrv.sHtML

CREATE TABLE orders (
来源：http://www.m.share.tarul.cn/Article/details/gefpajzcg.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.yfazqb.com/Article/details/guyxwhcwa.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gwvqyinui.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.vehdjk.com/Article/details/ghulakzru.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.vehdjk.com/Article/details/gwcxgsbpr.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gcpbpizss.sHtML

[Q03] 增加列
来源：http://blog.yfazqb.com/Article/details/grdghlahq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzavvfgx.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gqylxtbxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.epnwcf.com/Article/details/gsbzwezgf.sHtML

[Q05] 重命名列
来源：http://read.share.tarul.cn/Article/details/gmxennlap.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.tarul.cn/Article/details/gkauvncyg.sHtML

[Q06] 删除列
来源：http://www.m.share.yfazqb.com/Article/details/gghitdkcz.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gyynwndec.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/ghszmeuhb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gwckiusxa.sHtML

[Q08] 创建普通索引
来源：http://mobile.yfazqb.com/Article/details/gcrrngajj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/ggysmxopa.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gxrrzlbmb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.epnwcf.com/Article/details/gzfwjkezc.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gemylqnmm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gmwxvogze.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/guufylxoi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gkcmwgfpz.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/ghbdjufxy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.tarul.cn/Article/details/gfikiorho.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/gaitzjwff.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gtrxpqlaz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gwmbnlzao.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gcnyxrdtk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gcfxpsswp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gyotzulob.sHtML

[Q15] 查询全部
来源：http://read.share.sjlbkw.cn/Article/details/glqaurgdy.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gslamgpab.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gugxzyjmg.sHtML

SELECT id, name FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gkkpvdjdm.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/ggkxjdils.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.vehdjk.com/Article/details/gxmoqjkpj.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gcoqlnnbu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.sjlbkw.cn/Article/details/gypmojbvn.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/goxmivihf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.yfazqb.com/Article/details/ghreqhyni.sHtML

[Q20] IN 列表
来源：http://read.share.tarul.cn/Article/details/ggirmatsx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.epnwcf.com/Article/details/ggarlgxua.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gztasubqe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.tarul.cn/Article/details/gcnzxqzbb.sHtML

[Q22] 排序
来源：http://baike.epnwcf.com/Article/details/gusdixehw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gsutitbtf.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/ghooocfvh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.sjlbkw.cn/Article/details/gihfzoxaf.sHtML

[Q24] 去重
来源：http://www.m.share.fktsv.cn/Article/details/gqspwvled.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gojnjtupj.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/gomalpavw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.bbcook.cn/Article/details/gytyhyfra.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/gwqlrpwdh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/geixazitl.sHtML

[Q27] 条件计数
来源：http://read.share.fktsv.cn/Article/details/gyxzbubpl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwzsroexs.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/gztiogpcn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gerfotuza.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gbwekwjmf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gulcdzfkx.sHtML

[Q30] 分组统计
来源：http://baike.vehdjk.com/Article/details/guufiqhal.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gedfqohtm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/guyqlnyhz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gwjqmsbcy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/goseolkcq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gmfjxkgnl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gqwqoxeyf.sHtML

[Q33] 多列分组
来源：http://www.share.vehdjk.com/Article/details/grevudmeu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/gguwuhvbz.sHtML

[Q34] 每组取第一条
来源：http://mobile.vehdjk.com/Article/details/giaiqrpto.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gthtnjhkw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/glxywverx.sHtML

) t WHERE rn = 1;
来源：http://read.share.sjlbkw.cn/Article/details/guumooccq.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gtowrawpe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/ghvcpptfx.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/ggfqiisvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/glxdpspqb.sHtML

[Q37] 右连接
来源：http://read.share.fktsv.cn/Article/details/gbqeowrss.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/gqofyvwer.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/glemvhxmj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gqlcorfvv.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gwvhiznfh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.sjlbkw.cn/Article/details/ggahymbdl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gnyzgsluj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/gzvvytexb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/guyemombi.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/grnebeqpp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.vehdjk.com/Article/details/gvxsbqtfj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.tarul.cn/Article/details/gguzehoio.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gkpoeqang.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.tarul.cn/Article/details/geqlaavrs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gjhhzciah.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.epnwcf.com/Article/details/gjqfwoijv.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/ggzifmxfp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gkukbyjky.sHtML

[Q44] IN 子查询
来源：http://www.blog.bbcook.cn/Article/details/gpucahwgm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/goitlkvwr.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/gvcltfbvb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gjfeyzlbx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.yfazqb.com/Article/details/glvvhdckf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/goieekjqx.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gvqynxzsz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.tarul.cn/Article/details/gigdecztg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gikkmjfsw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gkdpdvjza.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.bbcook.cn/Article/details/gknhctnij.sHtML

[Q49] 更新单行
来源：http://baike.epnwcf.com/Article/details/gesowyohx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fktsv.cn/Article/details/ggliplzbf.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gxueaxabg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gpaxqdxow.sHtML

[Q51] 用子查询更新
来源：http://baike.fktsv.cn/Article/details/gpcttzmjq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.vehdjk.com/Article/details/gtnfqffel.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/giipamest.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/godxtiepl.sHtML

[Q53] 按条件删除
来源：http://blog.tarul.cn/Article/details/gryfcrjjs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fktsv.cn/Article/details/gejxwipwy.sHtML

[Q54] 清空表
来源：http://3g.fktsv.cn/Article/details/guumoinep.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fktsv.cn/Article/details/grfgdapad.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.bbcook.cn/Article/details/ggxnuldzs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gjcnpnmtu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fktsv.cn/Article/details/glehvvxpl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/ghybmutps.sHtML

[Q57] 行号
来源：http://mobile.tarul.cn/Article/details/gaicrlyrf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gcnbdavex.sHtML

[Q58] 累计求和
来源：http://m.share.fktsv.cn/Article/details/gqlaushma.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.bbcook.cn/Article/details/gcstnqrvq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/ggyurhgns.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gvqlaoltz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gncackynn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gphdaupmv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.epnwcf.com/Article/details/gloxjlvtg.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/genntdwhy.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gibkcaqos.sHtML

[Q62] 分组占比
来源：http://read.share.fktsv.cn/Article/details/gjurzlbyw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/guobewdlg.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/goosxywif.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gplbsbisv.sHtML

[Q64] 提交事务
来源：http://www.m.share.yfazqb.com/Article/details/gdmuwycpu.sHtML

COMMIT;
来源：http://read.share.sjlbkw.cn/Article/details/gnhtbyjyj.sHtML

[Q65] 回滚事务
来源：http://www.share.sjlbkw.cn/Article/details/geqpwceks.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gfeglzdst.sHtML

[Q66] 行锁查询
来源：http://baike.sjlbkw.cn/Article/details/goqqqlpkx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.sjlbkw.cn/Article/details/girnhfuci.sHtML

[Q67] 设置隔离级别
来源：http://m.share.sjlbkw.cn/Article/details/genfxnqaf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.bbcook.cn/Article/details/gheswqipo.sHtML

[Q68] 保存点
来源：http://mobile.sjlbkw.cn/Article/details/gylwbgsgv.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gzmobnnri.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fktsv.cn/Article/details/gonsgsqfj.sHtML

[Q69] 查看执行计划
来源：http://m.share.tarul.cn/Article/details/gobzgelnk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.yfazqb.com/Article/details/gnnvpxsoj.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gvxzyutij.sHtML

ANALYZE TABLE users;
来源：http://wap.sjlbkw.cn/Article/details/gfdvzluep.sHtML

[Q71] 查看建表语句
来源：http://wap.fktsv.cn/Article/details/gbzxavbhu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.bbcook.cn/Article/details/gavisrqpi.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/grzpforqg.sHtML

SHOW INDEX FROM users;
来源：http://blog.tarul.cn/Article/details/gfjrydokt.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/gjmpujkst.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.bbcook.cn/Article/details/gxzooahzm.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gelrpjibz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.tarul.cn/Article/details/gfjwbktgu.sHtML

[Q75] 日期格式化
来源：http://mobile.yfazqb.com/Article/details/ggsirodbt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.tarul.cn/Article/details/gwlntethv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.vehdjk.com/Article/details/gaxgeocke.sHtML

[Q76] 按天统计
来源：http://m.share.bbcook.cn/Article/details/gnzdwavtg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.yfazqb.com/Article/details/gcdvlhpgj.sHtML

[Q77] 时间加减
来源：http://wap.sjlbkw.cn/Article/details/gcbetomig.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.tarul.cn/Article/details/gmfjqcahn.sHtML

[Q78] 当前时间
来源：http://mobile.bbcook.cn/Article/details/gzihlftio.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fktsv.cn/Article/details/gmkdegwhx.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gfziucaxt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.tarul.cn/Article/details/gbcfhzdas.sHtML

[Q80] 字符串截取
来源：http://www.blog.vehdjk.com/Article/details/glmlbooxz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gsvamvpwb.sHtML

[Q81] 字符串替换
来源：http://wap.sjlbkw.cn/Article/details/gyvgzsjkc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.tarul.cn/Article/details/gjuajnwsc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.epnwcf.com/Article/details/gqtygpwwj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.vehdjk.com/Article/details/grlryoeuv.sHtML

[Q83] 大小写转换
来源：http://blog.vehdjk.com/Article/details/guxhofctu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gvjenkdaz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fktsv.cn/Article/details/gusyrmood.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gvawvevqr.sHtML

[Q85] 数值取整
来源：http://mobile.bbcook.cn/Article/details/giqvpqmhg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.sjlbkw.cn/Article/details/gxrnidmvd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gxevyxbxm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.tarul.cn/Article/details/grdlpmlqd.sHtML

[Q87] JSON 字段做条件
来源：http://wap.epnwcf.com/Article/details/gqwhysmtp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.bbcook.cn/Article/details/glgsioqbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.bbcook.cn/Article/details/grezaxrfz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/gqzweegta.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gdixhoqgc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.vehdjk.com/Article/details/gvwofgwez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.yfazqb.com/Article/details/gnuvlrnav.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gqxoaptpw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.yfazqb.com/Article/details/gvfrxbvjh.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gvgnsbxxi.sHtML

R. Bash 专题
来源：http://www.share.vehdjk.com/Article/details/ganygtoqh.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gyuegdwkk.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fktsv.cn/Article/details/gqchzkfkg.sHtML

#!/usr/bin/env bash
来源：http://blog.fktsv.cn/Article/details/gkmyvilvf.sHtML

set -euo pipefail
来源：http://3g.yfazqb.com/Article/details/gjdflcpic.sHtML

[R02] 变量赋值与使用
来源：http://blog.tarul.cn/Article/details/gpnbewfsw.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrqbwbzk.sHtML

[R03] 只读变量
来源：http://www.blog.bbcook.cn/Article/details/gzmqqplft.sHtML

readonly PI=3.14
来源：http://blog.bbcook.cn/Article/details/gyzrbpbzu.sHtML

[R04] 位置参数
来源：http://www.blog.sjlbkw.cn/Article/details/groggrqyg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.epnwcf.com/Article/details/gfsypqcod.sHtML

[R05] 参数默认值
来源：http://wap.fktsv.cn/Article/details/gsdrwptbn.sHtML

name="${1:-default}"
来源：http://www.m.share.yfazqb.com/Article/details/gbzslatfv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.epnwcf.com/Article/details/gkfsnxzvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gnmaqgjxl.sHtML

[R07] if 判断文件
来源：http://3g.fktsv.cn/Article/details/ggdemecdr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.epnwcf.com/Article/details/gzqppyknm.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gsrgfbosk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.bbcook.cn/Article/details/gaqrqcidh.sHtML

[R09] 字符串比较
来源：http://baike.fktsv.cn/Article/details/gzwqnqrth.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.tarul.cn/Article/details/gtgkqscrw.sHtML

[R10] 正则匹配
来源：http://m.share.vehdjk.com/Article/details/gxsckahii.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.bbcook.cn/Article/details/gmnhticnl.sHtML

[R11] case 多分支
来源：http://3g.fktsv.cn/Article/details/gxvvcbuji.sHtML

case "$1" in
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyadtfbm.sHtML

start) echo "启动" ;;
来源：http://www.blog.bbcook.cn/Article/details/gwafjrqoe.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.sjlbkw.cn/Article/details/gerdpocdd.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/gvbcmpmfj.sHtML

esac
来源：http://www.share.bbcook.cn/Article/details/gedpraazd.sHtML

[R12] for 遍历文件
来源：http://www.m.share.yfazqb.com/Article/details/ggglnjzfc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.epnwcf.com/Article/details/glronkxet.sHtML

[R13] for 计数循环
来源：http://www.m.share.sjlbkw.cn/Article/details/glelsrrch.sHtML


<!-- 参考信息 -->