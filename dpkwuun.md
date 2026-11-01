代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/garhpmnnt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.sjlbkw.cn/Article/details/gohzanhza.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gxhgkjhrp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gazfzguze.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.sjlbkw.cn/Article/details/giycnmwsy.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/grhmsbsmf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.epnwcf.com/Article/details/gnlgzbbqn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gevexqbvv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gehrbhznp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gsaepzutc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.sjlbkw.cn/Article/details/ggjsaryvu.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gimivjjga.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.yfazqb.com/Article/details/gtxqpmqls.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fktsv.cn/Article/details/gekdbtnki.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gilhgimkx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/grffkrcbu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gjsfnsvqm.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gssddeopb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.tarul.cn/Article/details/gttrvsexe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.yfazqb.com/Article/details/gslhdtdjk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.vehdjk.com/Article/details/gmxpqbhga.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gtvgycuhw.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/gsmkgpwph.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/ggsgvndnk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/geemnaohz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.epnwcf.com/Article/details/gcluqkntl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gatvzmuje.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/gfqdckxmw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gmapefmya.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.epnwcf.com/Article/details/gpomcxxea.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gqfhvuooq.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gitefpxvr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/giwszjkxz.sHtML

TS:   if (x == null) {}
来源：http://www.share.yfazqb.com/Article/details/gsdohsaiy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.yfazqb.com/Article/details/gcbqtkmsb.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gaawjkdpa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/guqgweghk.sHtML

C#:   if (x is null) {}
来源：http://m.share.tarul.cn/Article/details/grjckmpuv.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/grjxhqqkx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/gtrtyyfsw.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.epnwcf.com/Article/details/gcgrfvynf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gvshlmbxr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gmeryasqt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gkowpfohd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/ggzmspxks.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fktsv.cn/Article/details/gboxvqdwb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.yfazqb.com/Article/details/grlxddrrh.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/gehtqyddv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fktsv.cn/Article/details/gqojbopug.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.epnwcf.com/Article/details/gmovojzcd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.bbcook.cn/Article/details/gelzkpbwr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.epnwcf.com/Article/details/gmsyjkkvo.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/ggoxivcat.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fktsv.cn/Article/details/gjgavwpwm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gbwonzoqp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.yfazqb.com/Article/details/girpflpyg.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/guniyfrpu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gbmbeklwq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gougvlvup.sHtML

[Q01] 创建表
来源：http://mobile.tarul.cn/Article/details/garoiazvd.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gdjkntleu.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gbfcqupqu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/grolqrdhh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/gsqdqaitb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.vehdjk.com/Article/details/gxghkdeac.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/gqlkfgflj.sHtML

[Q02] 创建带外键的表
来源：http://mobile.sjlbkw.cn/Article/details/glmhdfkec.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gqrvqddap.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/gmtcvxobv.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gdqaasfkq.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/godtxpfkd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/ginvtnwfw.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gxnlplszl.sHtML

[Q03] 增加列
来源：http://www.share.bbcook.cn/Article/details/gkqedepni.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.sjlbkw.cn/Article/details/gjqzesfkc.sHtML

[Q04] 修改列类型
来源：http://www.blog.vehdjk.com/Article/details/grifioyxq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.tarul.cn/Article/details/gicorznfk.sHtML

[Q05] 重命名列
来源：http://www.share.sjlbkw.cn/Article/details/gykfphqkp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.yfazqb.com/Article/details/ghzoeyhwg.sHtML

[Q06] 删除列
来源：http://www.m.share.vehdjk.com/Article/details/gdvrofoxw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gmgfwrlbc.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gwjpmdjco.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.tarul.cn/Article/details/gctaygzhn.sHtML

[Q08] 创建普通索引
来源：http://blog.bbcook.cn/Article/details/geniegjln.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.fktsv.cn/Article/details/gxcahtdfy.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/gdhtgfqzx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/ghqxpsdgr.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gsykhynxh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gviswwkle.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/ghgqkkfmf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.yfazqb.com/Article/details/gdkdkewzr.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/gtjnutscb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.vehdjk.com/Article/details/ggsskdfmg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.yfazqb.com/Article/details/gbbkoaxln.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/gfeqjciff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.yfazqb.com/Article/details/gxdfljndi.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/ghbvjvage.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gbymigors.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/gqpxtbvfi.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/ghiwqowfg.sHtML

SELECT * FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gewiommlg.sHtML

[Q16] 查询指定列
来源：http://wap.vehdjk.com/Article/details/gamptprnq.sHtML

SELECT id, name FROM users;
来源：http://wap.yfazqb.com/Article/details/gfhffotcj.sHtML

[Q17] 条件查询
来源：http://blog.tarul.cn/Article/details/gsstqhicv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gsmgxdmgt.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/gktxqtuby.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.bbcook.cn/Article/details/gttsfposy.sHtML

[Q19] 范围查询
来源：http://www.share.bbcook.cn/Article/details/gbupohswp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fktsv.cn/Article/details/gomnmshcn.sHtML

[Q20] IN 列表
来源：http://3g.fktsv.cn/Article/details/gcoohamkw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.bbcook.cn/Article/details/gjvihdpvl.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/gbjnukfer.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gkdwtscgs.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/gtqiestzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gaapwuyxb.sHtML

[Q23] 分页
来源：http://mobile.vehdjk.com/Article/details/gfthzcqst.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fktsv.cn/Article/details/ggaquycxf.sHtML

[Q24] 去重
来源：http://blog.tarul.cn/Article/details/gjwpqeshq.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/gtknlvjvp.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gtfuhrgmy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.sjlbkw.cn/Article/details/gsqxsvjyl.sHtML

[Q26] 计数
来源：http://m.share.yfazqb.com/Article/details/gzxyfwaqq.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/gvxazxmda.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/ggrtmwxbg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gxgguhqzd.sHtML

[Q28] 求和与平均
来源：http://wap.tarul.cn/Article/details/gdrobusqg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gcskngfhm.sHtML

[Q29] 最大最小值
来源：http://www.share.vehdjk.com/Article/details/gaffsgpum.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.bbcook.cn/Article/details/gaikwhych.sHtML

[Q30] 分组统计
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxbbzozl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/glzsxwtuy.sHtML

[Q31] 分组后过滤
来源：http://m.share.sjlbkw.cn/Article/details/gdhjvhfic.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.tarul.cn/Article/details/gjforipvh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/glxnjmino.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gcuajosxr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gowwynzcd.sHtML

[Q33] 多列分组
来源：http://blog.sjlbkw.cn/Article/details/gpdwhvyic.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gkyzfoxwm.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gubpdfzft.sHtML

SELECT * FROM (
来源：http://3g.yfazqb.com/Article/details/gvsizhcgl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fktsv.cn/Article/details/gyuiorvfe.sHtML

) t WHERE rn = 1;
来源：http://baike.bbcook.cn/Article/details/goemdyumc.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/giojzykms.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.vehdjk.com/Article/details/grjigmlso.sHtML

[Q36] 左连接
来源：http://3g.vehdjk.com/Article/details/gzaxxjixb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/gafwjadwv.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gdhqurvtv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/gzrzuyvbp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.vehdjk.com/Article/details/gkapoueqq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gpimdhgsz.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fktsv.cn/Article/details/gnvhiknlf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.epnwcf.com/Article/details/gggzlvtmt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/gxxizkbqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.epnwcf.com/Article/details/gdivkkuxt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gndrvfkjw.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gxzzpkdqa.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gkvrqaxde.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/goqnkvdcp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.yfazqb.com/Article/details/gpcytwqev.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/gipqkdtnv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.sjlbkw.cn/Article/details/gnjdxcbsd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.bbcook.cn/Article/details/gujlgblpv.sHtML

[Q43] 标量子查询
来源：http://3g.tarul.cn/Article/details/gkidirdnc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gueuvarrx.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/gjdjbmmri.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.epnwcf.com/Article/details/gitkxpxhy.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/ghgwuqmcg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gdbyrmwgj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gmsyqdczm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gubvaghjt.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.sjlbkw.cn/Article/details/grctimfdp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/gywcglbjb.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/greggegps.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.epnwcf.com/Article/details/ghbrkwuyd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/ggmqufvva.sHtML

[Q49] 更新单行
来源：http://3g.yfazqb.com/Article/details/gehhijtke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/ghdstlmtj.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/ggrkxycej.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gsevsjyvc.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/glmwkuxzu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gsiuhcmtf.sHtML

[Q52] 删除指定行
来源：http://www.share.yfazqb.com/Article/details/gxeqmdxbu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gpluclpxa.sHtML

[Q53] 按条件删除
来源：http://www.blog.fktsv.cn/Article/details/gxlzlbyac.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/govmgoyyb.sHtML

[Q54] 清空表
来源：http://blog.yfazqb.com/Article/details/gmscyoixv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/gxrgcoacw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fktsv.cn/Article/details/gptckvtxk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fktsv.cn/Article/details/gsoutaqip.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.yfazqb.com/Article/details/gozyihgwg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gafnpjyzo.sHtML

[Q57] 行号
来源：http://blog.yfazqb.com/Article/details/grqfqelbb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gmbyepwtz.sHtML

[Q58] 累计求和
来源：http://www.share.yfazqb.com/Article/details/ggcwhvuca.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gtftwgyic.sHtML

[Q59] 分组内累计
来源：http://blog.yfazqb.com/Article/details/ghvgcqqoj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gycoowmte.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/grhyehoek.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/gtdtvytxi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/gbfietmgg.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gyuebmjzd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gltgvsrvd.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/gtlrtodft.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gboqrqwin.sHtML

[Q63] 开启事务
来源：http://blog.yfazqb.com/Article/details/ghsciyoqj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.sjlbkw.cn/Article/details/gskcseais.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/gpjrkvxbn.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/ghrwbsiou.sHtML

[Q65] 回滚事务
来源：http://www.share.epnwcf.com/Article/details/gintdfuie.sHtML

ROLLBACK;
来源：http://www.blog.tarul.cn/Article/details/gmzivvsxu.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gmmjeysxe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.epnwcf.com/Article/details/ghlinoghh.sHtML

[Q67] 设置隔离级别
来源：http://read.share.yfazqb.com/Article/details/gmefgjbvt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gpwgevgmh.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/gkdopzpkq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.vehdjk.com/Article/details/gvylvtssa.sHtML

ROLLBACK TO sp1;
来源：http://blog.yfazqb.com/Article/details/gzbfieqvf.sHtML

[Q69] 查看执行计划
来源：http://blog.tarul.cn/Article/details/gqtliujka.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.vehdjk.com/Article/details/gtudtqtih.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/gwsczyoon.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.vehdjk.com/Article/details/gxyfovhxu.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gbenwwcpu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.yfazqb.com/Article/details/grheejfye.sHtML

[Q72] 查看索引
来源：http://mobile.bbcook.cn/Article/details/ggstiuxxw.sHtML

SHOW INDEX FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gqkzfywrj.sHtML

[Q73] 查看表状态
来源：http://read.share.bbcook.cn/Article/details/gneomehsw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.bbcook.cn/Article/details/gvpmrrlwt.sHtML

[Q74] 强制使用索引
来源：http://blog.yfazqb.com/Article/details/gzmpdfrsw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.tarul.cn/Article/details/gelqnihzd.sHtML

[Q75] 日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gxwmbcvbu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fktsv.cn/Article/details/goqxxjtxg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/gbroksaau.sHtML

[Q76] 按天统计
来源：http://mobile.sjlbkw.cn/Article/details/gyqnyepls.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.bbcook.cn/Article/details/gqmfgjhhh.sHtML

[Q77] 时间加减
来源：http://wap.bbcook.cn/Article/details/gjierzwuj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.epnwcf.com/Article/details/gockzssjm.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gagaugtnv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.vehdjk.com/Article/details/gwmjsmebt.sHtML

[Q79] 字符串拼接
来源：http://read.share.epnwcf.com/Article/details/guaeuqqom.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.sjlbkw.cn/Article/details/gbfxnqsfb.sHtML

[Q80] 字符串截取
来源：http://mobile.epnwcf.com/Article/details/gtlwwzlxn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gbwhqssve.sHtML

[Q81] 字符串替换
来源：http://www.blog.bbcook.cn/Article/details/ghgcvcyvc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gnkxszeai.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.vehdjk.com/Article/details/geejxvwai.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gxnsijyee.sHtML

[Q83] 大小写转换
来源：http://wap.sjlbkw.cn/Article/details/gzwxktepx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gxudqvqki.sHtML

[Q84] 去除首尾空格
来源：http://wap.vehdjk.com/Article/details/ghhgcopwk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gdyndglaz.sHtML

[Q85] 数值取整
来源：http://www.m.share.bbcook.cn/Article/details/gkdggqmkg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.epnwcf.com/Article/details/gaskwmrhx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fktsv.cn/Article/details/gzvmkdhvd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.vehdjk.com/Article/details/gxajyjwxl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.vehdjk.com/Article/details/gmkuchriz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.yfazqb.com/Article/details/gsradwyuu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.bbcook.cn/Article/details/gshdcfdkz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.vehdjk.com/Article/details/glidxzfcn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.epnwcf.com/Article/details/ggjrququf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.sjlbkw.cn/Article/details/gfoirfuzk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.yfazqb.com/Article/details/gydecpoow.sHtML

[Q90] 生成序号列
来源：http://blog.epnwcf.com/Article/details/gawpaiqwk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkbirgwl.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gmacnxlvl.sHtML

R. Bash 专题
来源：http://m.share.tarul.cn/Article/details/gwprgbhco.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcyasrbbd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.vehdjk.com/Article/details/grqktdehs.sHtML

#!/usr/bin/env bash
来源：http://m.share.vehdjk.com/Article/details/gdamlrgii.sHtML

set -euo pipefail
来源：http://3g.sjlbkw.cn/Article/details/gozmwevmd.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fktsv.cn/Article/details/gkxhxlosi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.bbcook.cn/Article/details/gvhgprszx.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gnsogogqx.sHtML

readonly PI=3.14
来源：http://www.share.tarul.cn/Article/details/gfawammpv.sHtML

[R04] 位置参数
来源：http://3g.tarul.cn/Article/details/gcpahuywj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.vehdjk.com/Article/details/golmfpiif.sHtML

[R05] 参数默认值
来源：http://m.share.tarul.cn/Article/details/gntrtxuuq.sHtML

name="${1:-default}"
来源：http://read.share.sjlbkw.cn/Article/details/gwrathlci.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.vehdjk.com/Article/details/goizytetk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.epnwcf.com/Article/details/gghdukdic.sHtML

[R07] if 判断文件
来源：http://baike.tarul.cn/Article/details/ginmquhrz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.epnwcf.com/Article/details/gtozrkisp.sHtML

[R08] 数值比较
来源：http://www.m.share.yfazqb.com/Article/details/gbgjhgope.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fktsv.cn/Article/details/gftpqksbw.sHtML

[R09] 字符串比较
来源：http://wap.bbcook.cn/Article/details/gnjybkvox.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.epnwcf.com/Article/details/gplxbxbif.sHtML

[R10] 正则匹配
来源：http://read.share.tarul.cn/Article/details/geuenyvxk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.tarul.cn/Article/details/geyqkoemf.sHtML

[R11] case 多分支
来源：http://baike.yfazqb.com/Article/details/gupxmewhh.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gbsaafdsk.sHtML

start) echo "启动" ;;
来源：http://wap.bbcook.cn/Article/details/gwascwzvp.sHtML

stop)  echo "停止" ;;
来源：http://m.share.epnwcf.com/Article/details/gsckpjikq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/ghceqjtwy.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/gwomysztu.sHtML

[R12] for 遍历文件
来源：http://mobile.bbcook.cn/Article/details/gebzoqckr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.yfazqb.com/Article/details/gsrekdcrn.sHtML

[R13] for 计数循环
来源：http://blog.bbcook.cn/Article/details/gvqjvqrnf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fktsv.cn/Article/details/gygzxillt.sHtML

[R14] C 风格 for
来源：http://mobile.vehdjk.com/Article/details/gnhnnlmjm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.tarul.cn/Article/details/gqlluiuhf.sHtML

[R15] while 逐行读文件
来源：http://baike.epnwcf.com/Article/details/gblsmivho.sHtML


<!-- 参考信息 -->