代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.bbcook.cn/Article/details/gljrhurub.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gjuqbogme.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/gqmggsiuk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gkwlevhjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.yfazqb.com/Article/details/gcdvvdntj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.yfazqb.com/Article/details/grcfkvrrb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gyufrlypx.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/gvemqooww.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gvwxuopbi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/glmjxnzse.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.vehdjk.com/Article/details/ggcwuzguo.sHtML

[P04] 求长度
来源：http://baike.sjlbkw.cn/Article/details/gsmeoerwf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fktsv.cn/Article/details/gpkdprjqe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.yfazqb.com/Article/details/gltgbzzfq.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gilgybkgn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gvgxhawkf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gblkmmlss.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/ghrvsanoo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gdlcsfelp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gowfqmgiy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/giiwsqsdv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gvjrpnutt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gshxazzzm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.vehdjk.com/Article/details/gphlbdoiy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gtfjtofhd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gmmnkloek.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gokxqmxyq.sHtML

Ruby: a == b
来源：http://www.blog.tarul.cn/Article/details/gpqzfcqgj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gdcdcnzqb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/gvkskvfsz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.yfazqb.com/Article/details/gtvyavenm.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.fktsv.cn/Article/details/gmjyajklq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.yfazqb.com/Article/details/gvrzbuxoc.sHtML

TS:   if (x == null) {}
来源：http://baike.tarul.cn/Article/details/gmnqyhvju.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/gzvdzrlxh.sHtML

Go:   if x == nil {}
来源：http://m.share.yfazqb.com/Article/details/gahkqpcqh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.bbcook.cn/Article/details/gbvohgvza.sHtML

C#:   if (x is null) {}
来源：http://read.share.fktsv.cn/Article/details/gzyqtscin.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/giwlspvnc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gopyfxjia.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.vehdjk.com/Article/details/gubzdnhlz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.epnwcf.com/Article/details/gnqchylmv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gciedbety.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.yfazqb.com/Article/details/gvctdeulc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.epnwcf.com/Article/details/gledktuhz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/grhdrfgea.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.tarul.cn/Article/details/gtmkmjwjc.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.yfazqb.com/Article/details/gpipmylwr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/guuzxihos.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gjzcotluh.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.epnwcf.com/Article/details/gsveftgpb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gvgimgyeo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gbpkydopf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gjjmmusxi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.sjlbkw.cn/Article/details/gfaqkbtye.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gkqrvlqux.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gkpwpwoyi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/gccawyfll.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghgqdwayq.sHtML

[Q01] 创建表
来源：http://read.share.epnwcf.com/Article/details/geccfkqha.sHtML

CREATE TABLE users (
来源：http://read.share.epnwcf.com/Article/details/ginqrznsi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/grqypinit.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/gzyjzquyy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fktsv.cn/Article/details/gbiqoeuqh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fktsv.cn/Article/details/gvwaudsjj.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gqewhjdxj.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/geeteavrf.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gaahaxbnh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gsrltxjqa.sHtML

user_id INT NOT NULL,
来源：http://read.share.tarul.cn/Article/details/gtmnagauk.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/getjpxtuo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.sjlbkw.cn/Article/details/gghuzaomo.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gpgrsdajc.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gogmkryno.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.vehdjk.com/Article/details/guaapkjqw.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/gsgablxfz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.sjlbkw.cn/Article/details/grvonzazq.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gukwckeoq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fktsv.cn/Article/details/gkvvgpcum.sHtML

[Q06] 删除列
来源：http://wap.epnwcf.com/Article/details/gtgrherra.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gxfeelkqz.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gnqxuvxmj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gcwygunzn.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gdjzbjllg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/gefuafzgr.sHtML

[Q09] 创建唯一索引
来源：http://www.share.bbcook.cn/Article/details/gdlkqlbmj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gpxerklaw.sHtML

[Q10] 插入单行
来源：http://www.blog.tarul.cn/Article/details/gvoalasgj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.vehdjk.com/Article/details/gslvbvtuz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/glnrncynf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.tarul.cn/Article/details/givapzmxk.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/ggnaknawf.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fktsv.cn/Article/details/gpaeyryeh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fktsv.cn/Article/details/gwpbxtnkg.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gejvkmmoo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gvxalewje.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.tarul.cn/Article/details/geffrprod.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.sjlbkw.cn/Article/details/gxuiqmzxl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fktsv.cn/Article/details/gkghxypun.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gbueqmnlx.sHtML

SELECT * FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gjpqbvtkh.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/guijstvdg.sHtML

SELECT id, name FROM users;
来源：http://read.share.epnwcf.com/Article/details/gugxlccff.sHtML

[Q17] 条件查询
来源：http://baike.bbcook.cn/Article/details/gvjmarctz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/gwaluythq.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gapeubtlz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gundbahru.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gougyqqta.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.tarul.cn/Article/details/ggyefsxdu.sHtML

[Q20] IN 列表
来源：http://read.share.sjlbkw.cn/Article/details/gudgrtjex.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/gwxpbccmv.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gopkdfhdi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/gkhkzmvjq.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/glgygcvep.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.epnwcf.com/Article/details/gnqperjcv.sHtML

[Q23] 分页
来源：http://www.m.share.sjlbkw.cn/Article/details/gqddciylj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.tarul.cn/Article/details/gjnsqhvgw.sHtML

[Q24] 去重
来源：http://read.share.sjlbkw.cn/Article/details/gzqsolukr.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/ghydfasck.sHtML

[Q25] 只取前 N 条
来源：http://read.share.bbcook.cn/Article/details/gwliazkvm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.yfazqb.com/Article/details/gwqpmvjmo.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gzigxcohm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvoloxqou.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gtnzozdnl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gxydybple.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gqcmnktrr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gnbhpnvct.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/ghqagyeel.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gqnisugwt.sHtML

[Q30] 分组统计
来源：http://baike.tarul.cn/Article/details/gaalwsagr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/glmzbvcxi.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/gxtgycdbr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.bbcook.cn/Article/details/grkcqcyuk.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gewfkxvss.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gifkqbfkf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/grqcthiaz.sHtML

[Q33] 多列分组
来源：http://mobile.sjlbkw.cn/Article/details/grtxnijkh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gmfpbwbxp.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/gfpwmbalb.sHtML

SELECT * FROM (
来源：http://www.blog.vehdjk.com/Article/details/gvccfhcla.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/gauliobaq.sHtML

) t WHERE rn = 1;
来源：http://www.share.epnwcf.com/Article/details/gtemwrvoy.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/gzlcqljyp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gvnubjmca.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gmmpoqdlr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gofabqdol.sHtML

[Q37] 右连接
来源：http://3g.fktsv.cn/Article/details/gfqwoacko.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gkcxjzuus.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/glbckxqhf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/gfmqmblgj.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gdxjcswfy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.vehdjk.com/Article/details/gpyexcjmf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gxeigsczd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.tarul.cn/Article/details/gcoqobuvq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.bbcook.cn/Article/details/gfycqectc.sHtML

[Q41] 多表连接
来源：http://m.share.epnwcf.com/Article/details/gxrhweogn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.bbcook.cn/Article/details/gqlzawrdb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.epnwcf.com/Article/details/gaxykpmod.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.bbcook.cn/Article/details/gfftixymh.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.tarul.cn/Article/details/giuppjqbl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fktsv.cn/Article/details/gojrsfelv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gxjiraiab.sHtML

[Q43] 标量子查询
来源：http://wap.tarul.cn/Article/details/glmtkvgio.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/ghshxcyzb.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gccrpalpx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/gngiokcoc.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gaivaaisp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.vehdjk.com/Article/details/gzozyngyr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fktsv.cn/Article/details/gwpuumryz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.bbcook.cn/Article/details/gmlqrcaqz.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/garhbqotg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.epnwcf.com/Article/details/gfdtsnkqi.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.epnwcf.com/Article/details/gzfivomoe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gypeczbvk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.yfazqb.com/Article/details/gyhhyokhn.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/gkpegvokk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gvtidzbkq.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/ghzlfwnpr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gqkjfkqbb.sHtML

[Q51] 用子查询更新
来源：http://baike.sjlbkw.cn/Article/details/gjpgfrdfq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/gsiczgvzq.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gpzboxqfj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/geobtjjlm.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/gsurpbpxc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.tarul.cn/Article/details/grqadtprl.sHtML

[Q54] 清空表
来源：http://www.m.share.tarul.cn/Article/details/golggcisg.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/gnybjnjun.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gjtfhkjel.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.vehdjk.com/Article/details/gsuubfwzc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.bbcook.cn/Article/details/gamaegtbm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gahhwwlsz.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/ghfxkrajx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gejoyrpal.sHtML

[Q58] 累计求和
来源：http://read.share.tarul.cn/Article/details/gfmtmyxxc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gkhglvrth.sHtML

[Q59] 分组内累计
来源：http://www.share.sjlbkw.cn/Article/details/gllknfjbf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gzxcamwru.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.epnwcf.com/Article/details/gkbugpluw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/ggzxdkjhz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/ggurccxrg.sHtML

[Q61] 移动平均
来源：http://baike.vehdjk.com/Article/details/guaqslkap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/ghkcuxmqg.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/geopkwdwh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gwzfjsnpo.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/ghgsqypyf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gkqvebwid.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gpeznakpn.sHtML

COMMIT;
来源：http://www.blog.vehdjk.com/Article/details/gdpzlhjye.sHtML

[Q65] 回滚事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gztitdfyi.sHtML

ROLLBACK;
来源：http://www.m.share.tarul.cn/Article/details/gmwatezib.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gjqwxnwjq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.bbcook.cn/Article/details/gdpiiktnr.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/guhhqomjl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gbbbsvsby.sHtML

[Q68] 保存点
来源：http://m.share.vehdjk.com/Article/details/gdoeelqvl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/ggdjlzpfu.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/gqcpzonfm.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/grtxmyyqq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.yfazqb.com/Article/details/gjlxqefny.sHtML

[Q70] 更新统计信息
来源：http://mobile.epnwcf.com/Article/details/ghpjdwjeh.sHtML

ANALYZE TABLE users;
来源：http://www.share.sjlbkw.cn/Article/details/gkifkowlh.sHtML

[Q71] 查看建表语句
来源：http://www.share.yfazqb.com/Article/details/gyppzftjr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.bbcook.cn/Article/details/grqdstznn.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gmcjdktol.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gufycrafd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.yfazqb.com/Article/details/gqtvtchoq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.epnwcf.com/Article/details/guhvtelub.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fktsv.cn/Article/details/gnxfhxekg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gpohaiwun.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gbajqegnh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gfyhfswjw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.vehdjk.com/Article/details/ggdfcebpb.sHtML

[Q76] 按天统计
来源：http://wap.tarul.cn/Article/details/gtryoteer.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.tarul.cn/Article/details/gshfqrntf.sHtML

[Q77] 时间加减
来源：http://read.share.vehdjk.com/Article/details/gifdngrhe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.yfazqb.com/Article/details/gtdcvunzq.sHtML

[Q78] 当前时间
来源：http://www.m.share.vehdjk.com/Article/details/gcunbipnm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.tarul.cn/Article/details/gxhmjqrku.sHtML

[Q79] 字符串拼接
来源：http://wap.bbcook.cn/Article/details/ggpmozjfi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fktsv.cn/Article/details/gwyeraxye.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdvseldc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/gampdbkfv.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/ggbfzdckl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gyndtybwi.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.epnwcf.com/Article/details/gugvstwoe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gsnsafmgg.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gttchcyee.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.yfazqb.com/Article/details/gauvwtvgh.sHtML

[Q84] 去除首尾空格
来源：http://3g.bbcook.cn/Article/details/grcjjbhmu.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/ggkhxpvyt.sHtML

[Q85] 数值取整
来源：http://www.m.share.epnwcf.com/Article/details/glxobatug.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.yfazqb.com/Article/details/gvuqplxmt.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.bbcook.cn/Article/details/genbwcrdk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fktsv.cn/Article/details/gkzxlkinn.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/gkobdklil.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/ggfgxkemk.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.sjlbkw.cn/Article/details/gsyuszbrx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.epnwcf.com/Article/details/gxonmihvz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.epnwcf.com/Article/details/gzdkpqece.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gppnkwtzq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.vehdjk.com/Article/details/gfrvqqjgr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.bbcook.cn/Article/details/gcyqkwdra.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.epnwcf.com/Article/details/goreagfjk.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcvpevplf.sHtML

R. Bash 专题
来源：http://3g.tarul.cn/Article/details/guuflkjqi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gwvgxihzn.sHtML

[R01] shebang 与严格模式
来源：http://mobile.bbcook.cn/Article/details/glnpsyurm.sHtML

#!/usr/bin/env bash
来源：http://read.share.yfazqb.com/Article/details/ghxlaubnn.sHtML

set -euo pipefail
来源：http://mobile.epnwcf.com/Article/details/gjddgqmtz.sHtML

[R02] 变量赋值与使用
来源：http://baike.sjlbkw.cn/Article/details/gxhhfwlar.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gbnfmcpjm.sHtML

[R03] 只读变量
来源：http://www.m.share.epnwcf.com/Article/details/gpgimxopy.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gdkfhwiwb.sHtML

[R04] 位置参数
来源：http://www.m.share.fktsv.cn/Article/details/gqpxkjowf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.sjlbkw.cn/Article/details/gddhgoucg.sHtML

[R05] 参数默认值
来源：http://baike.epnwcf.com/Article/details/gggckjahj.sHtML

name="${1:-default}"
来源：http://m.share.bbcook.cn/Article/details/ggsluplsa.sHtML

[R06] 判断命令是否存在
来源：http://wap.epnwcf.com/Article/details/gegfgwuhn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.epnwcf.com/Article/details/gifvicymz.sHtML

[R07] if 判断文件
来源：http://mobile.tarul.cn/Article/details/gflhfbwtl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.vehdjk.com/Article/details/ghcyuqibq.sHtML

[R08] 数值比较
来源：http://www.share.sjlbkw.cn/Article/details/gdimlfpno.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.epnwcf.com/Article/details/glduhxgzm.sHtML

[R09] 字符串比较
来源：http://www.m.share.fktsv.cn/Article/details/gxsydfkmk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.vehdjk.com/Article/details/gpjcualca.sHtML

[R10] 正则匹配
来源：http://3g.bbcook.cn/Article/details/guqzpldzb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.sjlbkw.cn/Article/details/gsxvljkyy.sHtML

[R11] case 多分支
来源：http://m.share.yfazqb.com/Article/details/gynshxvrc.sHtML

case "$1" in
来源：http://baike.sjlbkw.cn/Article/details/gotoewcll.sHtML

start) echo "启动" ;;
来源：http://blog.sjlbkw.cn/Article/details/gxowkuhww.sHtML

stop)  echo "停止" ;;
来源：http://m.share.sjlbkw.cn/Article/details/gzenxqdre.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.tarul.cn/Article/details/gqiyrqqie.sHtML

esac
来源：http://www.share.tarul.cn/Article/details/gmuhblfwk.sHtML

[R12] for 遍历文件
来源：http://wap.vehdjk.com/Article/details/grzpvnfau.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.bbcook.cn/Article/details/gsgjjlxqi.sHtML

[R13] for 计数循环
来源：http://read.share.fktsv.cn/Article/details/gsbhurrzk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.sjlbkw.cn/Article/details/gpucabopn.sHtML

[R14] C 风格 for
来源：http://www.blog.yfazqb.com/Article/details/gicuyyqpv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.yfazqb.com/Article/details/gkuvpxvzh.sHtML

[R15] while 逐行读文件
来源：http://read.share.tarul.cn/Article/details/gilgbiten.sHtML


<!-- 参考信息 -->