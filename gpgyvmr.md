代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/grmeaoddw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gspxmhdyy.sHtML

[P03] 生成短随机字符串
来源：http://mobile.bbcook.cn/Article/details/grloyaytp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fktsv.cn/Article/details/govxjpzhr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.epnwcf.com/Article/details/ggavbsbwk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gtsnxykmh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gzeknaaba.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gqytwebey.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fktsv.cn/Article/details/gsycblwql.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gbaszytjh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/ggzvztjlv.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gwzwlinxn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gnhcgxyjc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.epnwcf.com/Article/details/grpwajsmi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gywreusew.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gfyvzdkza.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gazvzajbj.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.tarul.cn/Article/details/ghtjnffwi.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gvcjtbnzt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/giyufuhub.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gxezfnbqx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.sjlbkw.cn/Article/details/gphnbihoh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gjrblwlln.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gmrzwzrpc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gjzspwjth.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.vehdjk.com/Article/details/guamhqxjv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.bbcook.cn/Article/details/ggfjjsebr.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gtbzmgjrv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/ghfdjzoss.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.epnwcf.com/Article/details/gxnghaurb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/ggkumiocb.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fktsv.cn/Article/details/gegoktoag.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gpezepxiv.sHtML

TS:   if (x == null) {}
来源：http://baike.bbcook.cn/Article/details/gdnuxbdyc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fktsv.cn/Article/details/ghbmkdyco.sHtML

Go:   if x == nil {}
来源：http://www.m.share.vehdjk.com/Article/details/gotbfldnm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gkokhiler.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gyaqpgigr.sHtML

[P07] 防抖与节流
来源：http://blog.epnwcf.com/Article/details/gpxvsnlah.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/ghpqilhgb.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gipiwblwc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/gdlmiuhdg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/glakwefgn.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.tarul.cn/Article/details/gbuzrbhgp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.epnwcf.com/Article/details/geyekzcvx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/gjqjvndhu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/guqflhues.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.yfazqb.com/Article/details/gcqesxelu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.vehdjk.com/Article/details/gcfjdrthp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gmslhbqyf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.yfazqb.com/Article/details/gmsogueuy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gtirohinr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fktsv.cn/Article/details/gkuddtdxf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.vehdjk.com/Article/details/gsbxlbucs.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/gimreqozo.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.vehdjk.com/Article/details/gyudosnni.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gzrtdoazf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/gxviehjxq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gravndzmu.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/gzyhhpsys.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gduxrncyd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/golcmkamw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gtbebsmmr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.bbcook.cn/Article/details/gjnrjiqkd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.epnwcf.com/Article/details/gvahxbymy.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gjvvdnkag.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gyifbuoyo.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gybzdyrwb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gcjnzdygk.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gjedjqhac.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.vehdjk.com/Article/details/gnmxldhfg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gquyunztt.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/guprdfqec.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gslrzpxeu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.yfazqb.com/Article/details/gcsbjqoom.sHtML

[Q04] 修改列类型
来源：http://www.m.share.bbcook.cn/Article/details/gbtaqnzda.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gakfycagi.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gpblnpizn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.yfazqb.com/Article/details/gjvkjelxo.sHtML

[Q06] 删除列
来源：http://mobile.bbcook.cn/Article/details/gpjgkwxdm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gglxaajyn.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/gyfoduwby.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.vehdjk.com/Article/details/gfhbotoen.sHtML

[Q08] 创建普通索引
来源：http://m.share.epnwcf.com/Article/details/gyxmgleru.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gnmsdstvj.sHtML

[Q09] 创建唯一索引
来源：http://m.share.bbcook.cn/Article/details/gcjbyzsdf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gwhqfflvo.sHtML

[Q10] 插入单行
来源：http://www.m.share.vehdjk.com/Article/details/gfgofzqga.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gvrgibrwm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gibvsyhai.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gvfgasrrj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/ggdwoqsjv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/geehlhjig.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.yfazqb.com/Article/details/gwwqqxzww.sHtML

[Q13] 忽略重复插入
来源：http://blog.fktsv.cn/Article/details/gwriucadt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.tarul.cn/Article/details/gkognalqx.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/gevupzurt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gnjbiigvb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gsdvjevps.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/gsariwrux.sHtML

SELECT * FROM users;
来源：http://m.share.vehdjk.com/Article/details/gemlpueio.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gvyaugrns.sHtML

SELECT id, name FROM users;
来源：http://read.share.yfazqb.com/Article/details/gvkmbwfeo.sHtML

[Q17] 条件查询
来源：http://read.share.epnwcf.com/Article/details/gmsztrlqh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fktsv.cn/Article/details/gylqyqdet.sHtML

[Q18] 模糊匹配
来源：http://m.share.bbcook.cn/Article/details/gwzzaywpa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gyvnubcxr.sHtML

[Q19] 范围查询
来源：http://3g.vehdjk.com/Article/details/gehtywyan.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gxflawyji.sHtML

[Q20] IN 列表
来源：http://read.share.bbcook.cn/Article/details/gjpirkbyc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.bbcook.cn/Article/details/gdyxhpqcm.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gkcxmjxjs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/gqgareyzj.sHtML

[Q22] 排序
来源：http://read.share.vehdjk.com/Article/details/ghojxaxmz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.yfazqb.com/Article/details/gkjthtpzd.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gfbgiomwq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gyhltqkya.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gorhcqqap.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gmptqvqvp.sHtML

[Q25] 只取前 N 条
来源：http://www.share.epnwcf.com/Article/details/gfkwvwjqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/gkqbmgoqu.sHtML

[Q26] 计数
来源：http://www.share.vehdjk.com/Article/details/gjnyesihc.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.bbcook.cn/Article/details/gcqtwamyu.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gtzdstkjg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gbyhjmiio.sHtML

[Q28] 求和与平均
来源：http://mobile.yfazqb.com/Article/details/grwbgszbr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gctvbjjgr.sHtML

[Q29] 最大最小值
来源：http://www.m.share.yfazqb.com/Article/details/gktomjcll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gwhfiqqpd.sHtML

[Q30] 分组统计
来源：http://mobile.yfazqb.com/Article/details/gshmrlcgh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.epnwcf.com/Article/details/glwtcxqgx.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.yfazqb.com/Article/details/gmqhamzwx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/gpuuslrty.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/geuhiryds.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gvdnrdqrt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.tarul.cn/Article/details/gnpzgjqjh.sHtML

[Q33] 多列分组
来源：http://3g.yfazqb.com/Article/details/ggvdkfrzo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.yfazqb.com/Article/details/gzgcloflr.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/gkeksokru.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gsxiwwaii.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.epnwcf.com/Article/details/gvnbrchzg.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gcjkaetgr.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gzbodgtya.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.yfazqb.com/Article/details/gmknboama.sHtML

[Q36] 左连接
来源：http://wap.epnwcf.com/Article/details/gebrdvuqh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gnkkmyzko.sHtML

[Q37] 右连接
来源：http://mobile.fktsv.cn/Article/details/gpnjqnebt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gyotilzmo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gmswktmjw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gaslecusl.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.bbcook.cn/Article/details/gicytbmlb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.sjlbkw.cn/Article/details/gzbndslnu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.sjlbkw.cn/Article/details/gzjaxrxqi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.epnwcf.com/Article/details/ggndokmpt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fktsv.cn/Article/details/giueluovc.sHtML

[Q41] 多表连接
来源：http://m.share.bbcook.cn/Article/details/gtuvmurvi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.sjlbkw.cn/Article/details/gugcqugtk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/ggxjqxtzv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gifavvuvy.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gbbtuppjl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.vehdjk.com/Article/details/gkfpwbjmi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.bbcook.cn/Article/details/gpthalsrz.sHtML

[Q43] 标量子查询
来源：http://m.share.vehdjk.com/Article/details/graccvpja.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fktsv.cn/Article/details/gpqmhrvsb.sHtML

[Q44] IN 子查询
来源：http://m.share.yfazqb.com/Article/details/gnwapwgre.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gecrckizb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fktsv.cn/Article/details/gmysyvsoi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gkwojrmax.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.tarul.cn/Article/details/gvxbrhtmp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gobdyzpdh.sHtML

[Q47] 与平均值比较
来源：http://www.blog.bbcook.cn/Article/details/gruzjphgn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gpydimhdk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gfpwmoiwh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.tarul.cn/Article/details/gujtpmnmu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gfvgnfeie.sHtML

[Q49] 更新单行
来源：http://blog.yfazqb.com/Article/details/gvjpwemki.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.yfazqb.com/Article/details/gbowjfcma.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/guzgdocch.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.vehdjk.com/Article/details/guxchtueb.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gdedvoeed.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gdqxyhblu.sHtML

[Q52] 删除指定行
来源：http://3g.tarul.cn/Article/details/gtdulmksi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.vehdjk.com/Article/details/gputmvuup.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gjiipzhgq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fktsv.cn/Article/details/gviybvzbi.sHtML

[Q54] 清空表
来源：http://blog.tarul.cn/Article/details/gyljzsxui.sHtML

TRUNCATE TABLE logs;
来源：http://wap.epnwcf.com/Article/details/gtztlnrqf.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/glkzenjnv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gjravajjk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.vehdjk.com/Article/details/gvkiixogx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gqqjwllwy.sHtML

[Q57] 行号
来源：http://3g.vehdjk.com/Article/details/gjkjomvnw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gbjbgpjem.sHtML

[Q58] 累计求和
来源：http://3g.vehdjk.com/Article/details/gekfwidci.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gxqilpkhg.sHtML

[Q59] 分组内累计
来源：http://baike.bbcook.cn/Article/details/gxnjgcvxq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.tarul.cn/Article/details/gyrcdtxqq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gnkeqprez.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gmqxhvgan.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gzxnnxxjb.sHtML

[Q61] 移动平均
来源：http://m.share.vehdjk.com/Article/details/gkrrmrcmj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fktsv.cn/Article/details/gqxziwqlm.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/goadluofy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gnmxyvghu.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gtbndwjhg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.yfazqb.com/Article/details/gyzixscvk.sHtML

[Q64] 提交事务
来源：http://3g.fktsv.cn/Article/details/gqviwjdlp.sHtML

COMMIT;
来源：http://read.share.epnwcf.com/Article/details/gdszjcxpz.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gevlayryb.sHtML

ROLLBACK;
来源：http://3g.yfazqb.com/Article/details/gpxmvsyrj.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gzyeickpe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gojmmqqsu.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gksyyyush.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gbzsdgfjj.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gosycwgst.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/gopyrbzmz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/goxvalehf.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/gfzpwtcjd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.vehdjk.com/Article/details/gtafpzhbl.sHtML

[Q70] 更新统计信息
来源：http://www.share.bbcook.cn/Article/details/grypdfipz.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gksntjjyk.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/grfdwxwcu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.vehdjk.com/Article/details/gdkjqoboh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fktsv.cn/Article/details/gqpwjdrzy.sHtML

SHOW INDEX FROM users;
来源：http://www.share.vehdjk.com/Article/details/gcgcykvqn.sHtML

[Q73] 查看表状态
来源：http://read.share.yfazqb.com/Article/details/gsixwtyfn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gslmgzzvc.sHtML

[Q74] 强制使用索引
来源：http://mobile.yfazqb.com/Article/details/gvddllbmc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/gpukobsrp.sHtML

[Q75] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gblxkxgkp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gwzzlgxce.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.epnwcf.com/Article/details/gajuktlnv.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/gmpoiudxi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.yfazqb.com/Article/details/gofzlpxug.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gorsnoily.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.sjlbkw.cn/Article/details/gmmioatqt.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gvefmircf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.yfazqb.com/Article/details/gkhevlqyh.sHtML

[Q79] 字符串拼接
来源：http://wap.yfazqb.com/Article/details/gxenogbcr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gtokckgsl.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gwudkklbw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.tarul.cn/Article/details/gcrwqejez.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gttslgtnm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.vehdjk.com/Article/details/ghmhrlewb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.epnwcf.com/Article/details/gzlziqznq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gwmtgidtw.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gojviktmn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gzhuwbomv.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.vehdjk.com/Article/details/ghilsnuwu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/ggyrqblov.sHtML

[Q85] 数值取整
来源：http://blog.tarul.cn/Article/details/gbzqmgidv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/ggngipjlz.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.tarul.cn/Article/details/geqzudbvf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fktsv.cn/Article/details/gxqbbldus.sHtML

[Q87] JSON 字段做条件
来源：http://blog.sjlbkw.cn/Article/details/gijzkigdc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.sjlbkw.cn/Article/details/gacqxvmsa.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.sjlbkw.cn/Article/details/goycnkqja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.tarul.cn/Article/details/gxkebtluv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fktsv.cn/Article/details/gilhbdwnf.sHtML

[Q89] 判断表是否存在
来源：http://read.share.epnwcf.com/Article/details/gahsjcmzu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.bbcook.cn/Article/details/gyotiiept.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/geayrpxfq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.vehdjk.com/Article/details/ghilbjmwt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gclfuuodk.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gqcobkxgv.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gdxyiystq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.bbcook.cn/Article/details/gfogkeoqy.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/gfxncxczu.sHtML

set -euo pipefail
来源：http://baike.bbcook.cn/Article/details/germzlaum.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.bbcook.cn/Article/details/gzqpaxocd.sHtML

name="Tom"; echo "$name"
来源：http://wap.yfazqb.com/Article/details/guaxrzpar.sHtML

[R03] 只读变量
来源：http://wap.tarul.cn/Article/details/gpmgnkdci.sHtML

readonly PI=3.14
来源：http://m.share.sjlbkw.cn/Article/details/gzifdfxug.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/glvuzbcms.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gfuptoofb.sHtML

[R05] 参数默认值
来源：http://www.share.epnwcf.com/Article/details/gbevqqwic.sHtML

name="${1:-default}"
来源：http://www.blog.bbcook.cn/Article/details/ggnqtqrud.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.tarul.cn/Article/details/glyoqoazl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.bbcook.cn/Article/details/geircjyxz.sHtML

[R07] if 判断文件
来源：http://www.share.tarul.cn/Article/details/geidutdvg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.yfazqb.com/Article/details/gyeujlkrp.sHtML

[R08] 数值比较
来源：http://www.share.bbcook.cn/Article/details/gpvyikicp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.yfazqb.com/Article/details/gqvshhjwn.sHtML

[R09] 字符串比较
来源：http://www.blog.fktsv.cn/Article/details/gtkbqkvyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.bbcook.cn/Article/details/gqwqdmmpm.sHtML

[R10] 正则匹配
来源：http://blog.epnwcf.com/Article/details/gyircvwin.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.bbcook.cn/Article/details/gidbiyqld.sHtML

[R11] case 多分支
来源：http://www.blog.epnwcf.com/Article/details/gxhxibidv.sHtML

case "$1" in
来源：http://3g.bbcook.cn/Article/details/gjqflspom.sHtML

start) echo "启动" ;;
来源：http://www.share.sjlbkw.cn/Article/details/gdzsezgfr.sHtML

stop)  echo "停止" ;;
来源：http://baike.sjlbkw.cn/Article/details/goeziootr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.yfazqb.com/Article/details/glsdyinpe.sHtML

esac
来源：http://baike.fktsv.cn/Article/details/ghcrmzzdf.sHtML

[R12] for 遍历文件
来源：http://www.blog.yfazqb.com/Article/details/ghhltfiyn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.epnwcf.com/Article/details/gdwfugtkk.sHtML

[R13] for 计数循环
来源：http://www.blog.yfazqb.com/Article/details/gwhmdyqio.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.epnwcf.com/Article/details/gmsutyswg.sHtML

[R14] C 风格 for
来源：http://baike.tarul.cn/Article/details/gjaydcqyk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.yfazqb.com/Article/details/gnnvpwgfq.sHtML

[R15] while 逐行读文件
来源：http://blog.sjlbkw.cn/Article/details/ggmamuefz.sHtML


<!-- 参考信息 -->