代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/ggaefugkh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.epnwcf.com/Article/details/glrardyle.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gaobcrdiy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.vehdjk.com/Article/details/goztmuctj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/gsmycqgop.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.epnwcf.com/Article/details/gejemadzt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gzcdcyvwu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gziadpkvt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.epnwcf.com/Article/details/gfokurtse.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gnfuvznfl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gsscpuhrk.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gczmhgxpe.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.sjlbkw.cn/Article/details/gqtokxxfo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.epnwcf.com/Article/details/gpojaptoe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gaowpehvb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gwhwcebqx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/ghezdficl.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gydtdokko.sHtML

Ruby: x.length;  x.size
来源：http://3g.yfazqb.com/Article/details/garwhnwvt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/gedyizask.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gksnylwps.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/grazayvnx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/gbkpnmmtz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcoearfg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/ggopfnsfs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/gftxdfuah.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gciexbotp.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/gyoalrraa.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gkxlnufuc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gdwiymnkq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gnczaobmo.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gqzrvqyra.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/giuzuoyfb.sHtML

TS:   if (x == null) {}
来源：http://blog.yfazqb.com/Article/details/gfzsbfbwy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gsieskblh.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gxttcpgme.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.tarul.cn/Article/details/glyywkvon.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/gzbsmivug.sHtML

[P07] 防抖与节流
来源：http://wap.fktsv.cn/Article/details/gsdgcvqcq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.vehdjk.com/Article/details/gwidvbbtx.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.vehdjk.com/Article/details/ghcmnvsqc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/gucftztxu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gpczwtuni.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gzdjwgpoy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fktsv.cn/Article/details/gnzmkqhus.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gmrvjagpq.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gyzmjszvd.sHtML

[P08] 处理浮点精度问题
来源：http://3g.yfazqb.com/Article/details/gsrvfuxpb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.yfazqb.com/Article/details/gsckrheju.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.yfazqb.com/Article/details/geaeoeacr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/giemprtla.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/gpycgmqwy.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.epnwcf.com/Article/details/grdsfuwzp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gaxypqhmc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.vehdjk.com/Article/details/gdqjqxnis.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/gawtphpgh.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/ghbvxdlxn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gqjiimdzy.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gffdffqml.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gwktninux.sHtML

CREATE TABLE users (
来源：http://www.m.share.yfazqb.com/Article/details/gsuzthvyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.tarul.cn/Article/details/gbncweeol.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/growgtesx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.tarul.cn/Article/details/gyizhlmfk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.sjlbkw.cn/Article/details/gxwcwgvyt.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gpzuqmsxw.sHtML

[Q02] 创建带外键的表
来源：http://read.share.sjlbkw.cn/Article/details/gkwdpzasb.sHtML

CREATE TABLE orders (
来源：http://www.share.yfazqb.com/Article/details/gerrjpknw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gimaqajtx.sHtML

user_id INT NOT NULL,
来源：http://3g.bbcook.cn/Article/details/grlwgyxyc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gbxhsxqgz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gwnlsauyk.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gnqzauhgy.sHtML

[Q03] 增加列
来源：http://3g.fktsv.cn/Article/details/gmgeucggw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gcnddfiwa.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gtplhxyzf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gkociznzb.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/griddosmr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gxcppcoak.sHtML

[Q06] 删除列
来源：http://3g.fktsv.cn/Article/details/gnamihsaj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.yfazqb.com/Article/details/gyvoanbxt.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gmuzghcqb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/gxqgzgnmf.sHtML

[Q08] 创建普通索引
来源：http://blog.bbcook.cn/Article/details/ghhrfmiro.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gyhbgetnn.sHtML

[Q09] 创建唯一索引
来源：http://m.share.epnwcf.com/Article/details/gbntbtizu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gyypjvfkp.sHtML

[Q10] 插入单行
来源：http://3g.sjlbkw.cn/Article/details/gsoluyzgv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gyviarkxx.sHtML

[Q11] 一次插入多行
来源：http://baike.bbcook.cn/Article/details/gonduxlkm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/ggemoiyon.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gkloabxvd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/gakqgimog.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.vehdjk.com/Article/details/grpwyxptt.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gvxozyxxg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/gagjghfje.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.yfazqb.com/Article/details/gcdtyvlxj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gdbltijmc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gunfeoxeg.sHtML

[Q15] 查询全部
来源：http://www.blog.epnwcf.com/Article/details/gynxnemjp.sHtML

SELECT * FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gvrizxykm.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/gwcapvals.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gtfjyqwsx.sHtML

[Q17] 条件查询
来源：http://baike.yfazqb.com/Article/details/gwywojram.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gywprvgth.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.epnwcf.com/Article/details/gijhlwbot.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/gveiunqwk.sHtML

[Q19] 范围查询
来源：http://baike.yfazqb.com/Article/details/gsqbvmopg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/gsgbkyiod.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/garrbzcho.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gugywmeiw.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gjktvrbni.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.epnwcf.com/Article/details/gybjwdmig.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/gvlwplsor.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fktsv.cn/Article/details/gwnsatcbw.sHtML

[Q23] 分页
来源：http://www.share.fktsv.cn/Article/details/gxghbzcdi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.epnwcf.com/Article/details/gthsfryae.sHtML

[Q24] 去重
来源：http://m.share.fktsv.cn/Article/details/gzvechdwq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gbvjunppq.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gkqpidkln.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.yfazqb.com/Article/details/ghvgjwfzq.sHtML

[Q26] 计数
来源：http://www.blog.yfazqb.com/Article/details/gvaadhptq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gbrvamwxj.sHtML

[Q27] 条件计数
来源：http://wap.bbcook.cn/Article/details/gswlqtzsf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.epnwcf.com/Article/details/gyujiuuih.sHtML

[Q28] 求和与平均
来源：http://3g.epnwcf.com/Article/details/gptvycojo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gbriuodpk.sHtML

[Q29] 最大最小值
来源：http://blog.epnwcf.com/Article/details/gkmfoghmw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gzcnwckmu.sHtML

[Q30] 分组统计
来源：http://read.share.fktsv.cn/Article/details/glybbkiyd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/ghysvgatr.sHtML

[Q31] 分组后过滤
来源：http://mobile.epnwcf.com/Article/details/gweryqolj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gcaqirlms.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gpoclnqbk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/grnkxtfuz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gorirhvyp.sHtML

[Q33] 多列分组
来源：http://wap.yfazqb.com/Article/details/gpfumnlmu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/gykzavyto.sHtML

[Q34] 每组取第一条
来源：http://blog.epnwcf.com/Article/details/gmzedovex.sHtML

SELECT * FROM (
来源：http://www.blog.sjlbkw.cn/Article/details/gjdrggwrl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gmmsslazk.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/glhpocjin.sHtML

[Q35] 内连接
来源：http://m.share.bbcook.cn/Article/details/gvbfwmbdi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.sjlbkw.cn/Article/details/gxkxavump.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/gmkulfnmh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.yfazqb.com/Article/details/gdwvkwheh.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/ggqvzialg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.tarul.cn/Article/details/gluycpcxa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.yfazqb.com/Article/details/gavswkeaj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/gkqdsefly.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.yfazqb.com/Article/details/gfxioahzc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.epnwcf.com/Article/details/gmjgyqbis.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gpdhlcmry.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gocluwdcs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.sjlbkw.cn/Article/details/gbhdxunvc.sHtML

[Q41] 多表连接
来源：http://m.share.fktsv.cn/Article/details/gpsaiewck.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gwxswfxds.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/grkpdwmsn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.epnwcf.com/Article/details/grwdxbdiq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gzqhvziqs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.epnwcf.com/Article/details/giynaunhi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/gkrahmmzn.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gsukvaehg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gdgmaolkt.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gjdagqkud.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.tarul.cn/Article/details/gbnabhugb.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.tarul.cn/Article/details/gsgstuwqn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/ghezfuizv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/gqwbhwwtk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gbxdzmjwv.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/gveszndbh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fktsv.cn/Article/details/gowylbhgg.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gavvbbccw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gxgjxcbor.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.vehdjk.com/Article/details/guybgzzsy.sHtML

[Q49] 更新单行
来源：http://m.share.bbcook.cn/Article/details/gjbpaawgz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gilgvefuy.sHtML

[Q50] 批量更新
来源：http://wap.tarul.cn/Article/details/gnyprzddf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gavlxmpgz.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gyuxwcmcx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/gxbmxnpjc.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/grhljfqxz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.sjlbkw.cn/Article/details/gteamrbqk.sHtML

[Q53] 按条件删除
来源：http://www.share.vehdjk.com/Article/details/gbtgjvhru.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.tarul.cn/Article/details/ghmewveyk.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gsheknrmw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/glqzhjvwu.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gthbrljdv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gmlxzokfj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gonuqsuru.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.yfazqb.com/Article/details/gwxxhktws.sHtML

[Q57] 行号
来源：http://baike.bbcook.cn/Article/details/gntokwlva.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/grtnwenuj.sHtML

[Q58] 累计求和
来源：http://blog.tarul.cn/Article/details/gvuxelmrz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.tarul.cn/Article/details/gfizvzgqn.sHtML

[Q59] 分组内累计
来源：http://mobile.tarul.cn/Article/details/gaiyuseks.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ganxoxjgy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.epnwcf.com/Article/details/glvkptggc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.epnwcf.com/Article/details/glaaoduja.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gynwovdph.sHtML

[Q61] 移动平均
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpuqjcmh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gazdgodjb.sHtML

[Q62] 分组占比
来源：http://www.blog.yfazqb.com/Article/details/gnxlcmrjy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gfzonqpkv.sHtML

[Q63] 开启事务
来源：http://wap.fktsv.cn/Article/details/gvdaqkhug.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fktsv.cn/Article/details/gualzgoyz.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/gzyisxedo.sHtML

COMMIT;
来源：http://wap.bbcook.cn/Article/details/gmhdnmntk.sHtML

[Q65] 回滚事务
来源：http://3g.bbcook.cn/Article/details/gdfjjyadl.sHtML

ROLLBACK;
来源：http://mobile.bbcook.cn/Article/details/gbdbtiewc.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/gdkfvobnn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.yfazqb.com/Article/details/gqixrwmdb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gzsbkgzda.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gpmvzvkfk.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/guworfxhr.sHtML

SAVEPOINT sp1;
来源：http://wap.tarul.cn/Article/details/gnabyvayw.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gzxlpzawk.sHtML

[Q69] 查看执行计划
来源：http://www.share.vehdjk.com/Article/details/gyimwdwbl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.tarul.cn/Article/details/gndgybgnj.sHtML

[Q70] 更新统计信息
来源：http://3g.yfazqb.com/Article/details/gqeejhtie.sHtML

ANALYZE TABLE users;
来源：http://www.blog.tarul.cn/Article/details/gnqtlixup.sHtML

[Q71] 查看建表语句
来源：http://mobile.bbcook.cn/Article/details/gpiizzzez.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.bbcook.cn/Article/details/gvflxnpbw.sHtML

[Q72] 查看索引
来源：http://www.share.vehdjk.com/Article/details/gtqitjlph.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gzbuzbpxl.sHtML

[Q73] 查看表状态
来源：http://baike.epnwcf.com/Article/details/gawyydvku.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.sjlbkw.cn/Article/details/gyrjvtchb.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/gbtgdmwve.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.bbcook.cn/Article/details/gegljeunz.sHtML

[Q75] 日期格式化
来源：http://www.share.bbcook.cn/Article/details/givqyazub.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.vehdjk.com/Article/details/ggadebsbq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gqltygtkc.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/ggfywouyl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.epnwcf.com/Article/details/gtsfyudmo.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/ghnkfhqky.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.epnwcf.com/Article/details/gyzwjsqpu.sHtML

[Q78] 当前时间
来源：http://www.m.share.epnwcf.com/Article/details/gsrrpozxb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.sjlbkw.cn/Article/details/gwztxeqgt.sHtML

[Q79] 字符串拼接
来源：http://read.share.vehdjk.com/Article/details/giswbzpmq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.bbcook.cn/Article/details/grpxkgvov.sHtML

[Q80] 字符串截取
来源：http://blog.bbcook.cn/Article/details/gzgpulqjo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmwvriyxq.sHtML

[Q81] 字符串替换
来源：http://wap.epnwcf.com/Article/details/gxzkavxil.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gzebuvutw.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.yfazqb.com/Article/details/gnbtkrwjj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/galogddcb.sHtML

[Q83] 大小写转换
来源：http://baike.epnwcf.com/Article/details/ghbkmbluq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gfkvkxmug.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/gqujasnio.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gpypfskdj.sHtML

[Q85] 数值取整
来源：http://mobile.epnwcf.com/Article/details/gfofyacjb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.bbcook.cn/Article/details/glorimwwa.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/ghgmzripl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.bbcook.cn/Article/details/gahrnxfxk.sHtML

[Q87] JSON 字段做条件
来源：http://blog.epnwcf.com/Article/details/gsesprmsg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.sjlbkw.cn/Article/details/gfbgwfaoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gvoofbowm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.yfazqb.com/Article/details/gqdqfajsf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fktsv.cn/Article/details/gsqiikfxn.sHtML

[Q89] 判断表是否存在
来源：http://mobile.yfazqb.com/Article/details/gxuwbepyv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/grnvvnffk.sHtML

[Q90] 生成序号列
来源：http://3g.vehdjk.com/Article/details/gtopidswe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.yfazqb.com/Article/details/gkshcqdxs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmqkfezcb.sHtML

R. Bash 专题
来源：http://read.share.vehdjk.com/Article/details/ggbilquob.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzhzymkmy.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.tarul.cn/Article/details/gecedyrxj.sHtML

#!/usr/bin/env bash
来源：http://3g.epnwcf.com/Article/details/gkincfzez.sHtML

set -euo pipefail
来源：http://wap.epnwcf.com/Article/details/ghplwrjnw.sHtML

[R02] 变量赋值与使用
来源：http://baike.vehdjk.com/Article/details/gjymtdrod.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gjfaztnyi.sHtML

[R03] 只读变量
来源：http://baike.bbcook.cn/Article/details/grodkodbr.sHtML

readonly PI=3.14
来源：http://www.m.share.epnwcf.com/Article/details/gdjxluhae.sHtML

[R04] 位置参数
来源：http://3g.sjlbkw.cn/Article/details/gvjeaulmh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fktsv.cn/Article/details/gkzvvdfcd.sHtML

[R05] 参数默认值
来源：http://www.share.yfazqb.com/Article/details/gxcuibipu.sHtML

name="${1:-default}"
来源：http://wap.tarul.cn/Article/details/gyrqswohe.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/gdzsfzbil.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.vehdjk.com/Article/details/gavnpuwnb.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gzcwfadus.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.vehdjk.com/Article/details/ggrnhpiar.sHtML

[R08] 数值比较
来源：http://baike.fktsv.cn/Article/details/gnpzujabc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fktsv.cn/Article/details/gbvldhxfa.sHtML

[R09] 字符串比较
来源：http://wap.fktsv.cn/Article/details/gsekfjode.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.tarul.cn/Article/details/gbatuyssd.sHtML

[R10] 正则匹配
来源：http://www.m.share.fktsv.cn/Article/details/gpjtkvymd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.tarul.cn/Article/details/gqjhxfrvr.sHtML

[R11] case 多分支
来源：http://blog.tarul.cn/Article/details/glctjbgxo.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/griabgzue.sHtML

start) echo "启动" ;;
来源：http://www.share.tarul.cn/Article/details/gzfywfnmy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.yfazqb.com/Article/details/gkuuvndku.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fktsv.cn/Article/details/gioakyvsr.sHtML

esac
来源：http://wap.fktsv.cn/Article/details/gqdydoqlq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.vehdjk.com/Article/details/gffhozjyo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fktsv.cn/Article/details/gjeakjazm.sHtML

[R13] for 计数循环
来源：http://mobile.yfazqb.com/Article/details/grgwrzbne.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.vehdjk.com/Article/details/guagryskf.sHtML

[R14] C 风格 for
来源：http://m.share.epnwcf.com/Article/details/gtbgiiqbe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.sjlbkw.cn/Article/details/goqeewhsd.sHtML

[R15] while 逐行读文件
来源：http://www.share.epnwcf.com/Article/details/gdxvjkmrx.sHtML


<!-- 参考信息 -->