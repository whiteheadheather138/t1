代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/goisdbjcq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gysyeyjgq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.sjlbkw.cn/Article/details/gauorcxek.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.sjlbkw.cn/Article/details/ghyhtmpgj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.yfazqb.com/Article/details/gpkihqylt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gjwwyxkla.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.vehdjk.com/Article/details/gifqphfea.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gaproffke.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gbszjclbk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fktsv.cn/Article/details/gnrrbdktm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/ghlguetmn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gfckwcrxv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gucaeitbl.sHtML

Go:   len(arr);  len(m)
来源：http://blog.sjlbkw.cn/Article/details/gegsekswj.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gjsrpvyjw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gvrwpmtet.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gaeglwfwn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/glfwymptc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/guacrmtyd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gchiakovx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.sjlbkw.cn/Article/details/gvqlcrztd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gpuqsykih.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.vehdjk.com/Article/details/gazvzljpt.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/gtwnhvndr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.tarul.cn/Article/details/gbxxuaubd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gbalqfppm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gpzjllema.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gkysesbif.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gwjelfeed.sHtML

TS:   if (x == null) {}
来源：http://wap.yfazqb.com/Article/details/gvzdbwwur.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/gwgsqxfwy.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/geoghxdii.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.tarul.cn/Article/details/geyesxzrg.sHtML

C#:   if (x is null) {}
来源：http://wap.vehdjk.com/Article/details/gukasfacd.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gqwaraeta.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.epnwcf.com/Article/details/gmidxcoos.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.bbcook.cn/Article/details/gznzqipps.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gdqeejbio.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/gqszvotnt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gldluybkx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gsnaikkxp.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.yfazqb.com/Article/details/gnhrchczm.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.sjlbkw.cn/Article/details/ghfrsuxxv.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/ghowdnsbe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fktsv.cn/Article/details/gqwkvrfzl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.tarul.cn/Article/details/gqmifzajy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/gahtqzqcq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.epnwcf.com/Article/details/glktmwaex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gahldpwpa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gtnwtqakl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gjellffwi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/guozcfsyr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gptbnjihe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.tarul.cn/Article/details/gpcnpedsb.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gklnsrxbh.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/gadqxhowh.sHtML

CREATE TABLE users (
来源：http://www.blog.tarul.cn/Article/details/gliwwhogp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gbgblfykc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gcmtldolz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gmivbteew.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.epnwcf.com/Article/details/ggxdkcbnl.sHtML

);
来源：http://m.share.epnwcf.com/Article/details/gtabbexog.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/gsmovzvhc.sHtML

CREATE TABLE orders (
来源：http://m.share.bbcook.cn/Article/details/gwkgrndsw.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/glefcuwrs.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gnxrahjkt.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fktsv.cn/Article/details/giqkleljp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.epnwcf.com/Article/details/gjlbjjbkq.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gpmcfagfs.sHtML

[Q03] 增加列
来源：http://baike.fktsv.cn/Article/details/gbophksey.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gfkhskwas.sHtML

[Q04] 修改列类型
来源：http://mobile.fktsv.cn/Article/details/grcwzirhd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.fktsv.cn/Article/details/gduqszmuo.sHtML

[Q05] 重命名列
来源：http://mobile.tarul.cn/Article/details/gssnjanns.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.bbcook.cn/Article/details/gwfkwhhna.sHtML

[Q06] 删除列
来源：http://read.share.vehdjk.com/Article/details/gnziathki.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.sjlbkw.cn/Article/details/gxogpuyzl.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gfvpixxbe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/gxozfmhcp.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/gxziavnwf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gqhesiojw.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/gvenqtpyq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gefqxtmmu.sHtML

[Q10] 插入单行
来源：http://blog.epnwcf.com/Article/details/guxrcppny.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gotapvyob.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjwivzfy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gcvirdzae.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fktsv.cn/Article/details/gvennhonc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.sjlbkw.cn/Article/details/giejkrbid.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gpkwomzea.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/gyhpmeubu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.yfazqb.com/Article/details/gjdagfram.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/giuzmjudj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.epnwcf.com/Article/details/gvhtbsnlx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.epnwcf.com/Article/details/gtcsdwjgm.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/ggtxdpvuf.sHtML

SELECT * FROM users;
来源：http://baike.yfazqb.com/Article/details/gqmwamics.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gfithamxy.sHtML

SELECT id, name FROM users;
来源：http://www.share.bbcook.cn/Article/details/guheayaqk.sHtML

[Q17] 条件查询
来源：http://m.share.epnwcf.com/Article/details/gjsyqqsvf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/gcszdiuqr.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/geyzmbvif.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gznxyyqzj.sHtML

[Q19] 范围查询
来源：http://wap.bbcook.cn/Article/details/gdxsfhqww.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/gccdsvtnw.sHtML

[Q20] IN 列表
来源：http://read.share.bbcook.cn/Article/details/gwbwvxifl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gksyhrcwd.sHtML

[Q21] 空值判断
来源：http://mobile.bbcook.cn/Article/details/gtzpmeake.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.epnwcf.com/Article/details/gciofdwxs.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gpuffollq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gcpmwdkal.sHtML

[Q23] 分页
来源：http://m.share.epnwcf.com/Article/details/gjytscktg.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.sjlbkw.cn/Article/details/grvxbsghx.sHtML

[Q24] 去重
来源：http://blog.yfazqb.com/Article/details/gxopmoxyj.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.epnwcf.com/Article/details/gypxtcusr.sHtML

[Q25] 只取前 N 条
来源：http://baike.yfazqb.com/Article/details/gzqgiljbe.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fktsv.cn/Article/details/gepypgsrn.sHtML

[Q26] 计数
来源：http://m.share.fktsv.cn/Article/details/glwxqnljw.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gdwwqcrqt.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gzldhiwsb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/ghtsslfth.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/ghvarbfpp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gpmcarvby.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gctotstzz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ggwywripl.sHtML

[Q30] 分组统计
来源：http://blog.yfazqb.com/Article/details/gmhubulln.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gzsjlontm.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gonzebkgz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gckqilfxo.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.tarul.cn/Article/details/gvvlandqz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gitvdawvh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gjpkinkoa.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gxcrbzmcq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.tarul.cn/Article/details/gpzvclnmc.sHtML

[Q34] 每组取第一条
来源：http://wap.epnwcf.com/Article/details/gftifhiqi.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gsygkcfpe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gbrcqmyeo.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gsuwddbhn.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gzajvyhfk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gfmszwixv.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/glvfkzrgl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.tarul.cn/Article/details/glrhqodnq.sHtML

[Q37] 右连接
来源：http://www.share.bbcook.cn/Article/details/goaiohogd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.epnwcf.com/Article/details/gdmrhwkum.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.sjlbkw.cn/Article/details/gxxtqontu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gqkyzupza.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gnqwyzxsj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.bbcook.cn/Article/details/gcdhjplut.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.epnwcf.com/Article/details/gegnewvau.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.tarul.cn/Article/details/gzucgiufy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.vehdjk.com/Article/details/gpkhrltzq.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/gigxklqoj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.bbcook.cn/Article/details/grfdmvfhg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gqrubgfce.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gxlfekymb.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gkgpexshk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gukwaaueu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gygcoqhmp.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gkxqnuwpq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gnktnalsh.sHtML

[Q44] IN 子查询
来源：http://m.share.yfazqb.com/Article/details/gljmuyxft.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gihrgrwao.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.tarul.cn/Article/details/gvcholzhu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gkyuhpsoj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.epnwcf.com/Article/details/gbjuffaqs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gwbvojeim.sHtML

[Q47] 与平均值比较
来源：http://blog.bbcook.cn/Article/details/gbfaydfqh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.vehdjk.com/Article/details/gfsdteqfw.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gyizejwfn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gqseojrkm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gptypwwad.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gigxdymny.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.tarul.cn/Article/details/gkhpkbcsq.sHtML

[Q50] 批量更新
来源：http://m.share.vehdjk.com/Article/details/gbxnszdyz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gepwihyog.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/gssotioyq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gitsmrwnc.sHtML

[Q52] 删除指定行
来源：http://m.share.yfazqb.com/Article/details/grkscsdkl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gcfefvkys.sHtML

[Q53] 按条件删除
来源：http://read.share.epnwcf.com/Article/details/gtxtjwdbh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/gzjldebdr.sHtML

[Q54] 清空表
来源：http://3g.yfazqb.com/Article/details/gvlpufjmh.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.epnwcf.com/Article/details/gbxmjienm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gtcglkgpo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/gjllalygq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gmqzaqqcv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.epnwcf.com/Article/details/galtqktub.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/gtqmknuzo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwtzzyeeh.sHtML

[Q58] 累计求和
来源：http://blog.vehdjk.com/Article/details/gebzxgggo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/ghupwioqw.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/gtgnktydk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gkzvptbbs.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/gkcrdnkml.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.sjlbkw.cn/Article/details/gsfkfgtpv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/glhsyibis.sHtML

[Q61] 移动平均
来源：http://3g.vehdjk.com/Article/details/gzbyuwnto.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.tarul.cn/Article/details/guidpawvw.sHtML

[Q62] 分组占比
来源：http://3g.vehdjk.com/Article/details/gspijatbr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gmikpozve.sHtML

[Q63] 开启事务
来源：http://www.blog.epnwcf.com/Article/details/gjqmdxifw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.sjlbkw.cn/Article/details/gebedhkuq.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/gpruepcqb.sHtML

COMMIT;
来源：http://m.share.sjlbkw.cn/Article/details/gympcizrs.sHtML

[Q65] 回滚事务
来源：http://mobile.vehdjk.com/Article/details/gwykuatva.sHtML

ROLLBACK;
来源：http://www.blog.vehdjk.com/Article/details/gowwaqtqz.sHtML

[Q66] 行锁查询
来源：http://www.m.share.sjlbkw.cn/Article/details/grvwmbwkn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.tarul.cn/Article/details/gwqzplvtt.sHtML

[Q67] 设置隔离级别
来源：http://m.share.bbcook.cn/Article/details/gvsmosdrd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fktsv.cn/Article/details/gzhggcsiv.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/guzjwcrrn.sHtML

SAVEPOINT sp1;
来源：http://wap.vehdjk.com/Article/details/gnufyizdx.sHtML

ROLLBACK TO sp1;
来源：http://wap.vehdjk.com/Article/details/gmhhgpdpq.sHtML

[Q69] 查看执行计划
来源：http://www.blog.epnwcf.com/Article/details/glyscjfsl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.epnwcf.com/Article/details/gtvixqnao.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/gcrsfmqlc.sHtML

ANALYZE TABLE users;
来源：http://m.share.epnwcf.com/Article/details/gyelvkozb.sHtML

[Q71] 查看建表语句
来源：http://baike.bbcook.cn/Article/details/gszyxecsv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.tarul.cn/Article/details/gqusdniwq.sHtML

[Q72] 查看索引
来源：http://baike.bbcook.cn/Article/details/gyemblmdw.sHtML

SHOW INDEX FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gliotszop.sHtML

[Q73] 查看表状态
来源：http://www.share.yfazqb.com/Article/details/gvfqflxjj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.epnwcf.com/Article/details/gerjqebjc.sHtML

[Q74] 强制使用索引
来源：http://mobile.vehdjk.com/Article/details/gpgbwwcjh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fktsv.cn/Article/details/gfvnwaveg.sHtML

[Q75] 日期格式化
来源：http://www.share.vehdjk.com/Article/details/gjfhogptr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gfgoswhzc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.yfazqb.com/Article/details/grarvzsfq.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gdgispfha.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/gmmzwikuj.sHtML

[Q77] 时间加减
来源：http://wap.tarul.cn/Article/details/gunnsuiok.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gsoqufbrv.sHtML

[Q78] 当前时间
来源：http://www.share.vehdjk.com/Article/details/gpvmyuers.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.bbcook.cn/Article/details/gmffmufds.sHtML

[Q79] 字符串拼接
来源：http://3g.fktsv.cn/Article/details/gwwgfesii.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.bbcook.cn/Article/details/gourkyufa.sHtML

[Q80] 字符串截取
来源：http://3g.sjlbkw.cn/Article/details/ghyuknoep.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.tarul.cn/Article/details/gbizffgky.sHtML

[Q81] 字符串替换
来源：http://read.share.bbcook.cn/Article/details/gorfhfilq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.yfazqb.com/Article/details/ghtsazfts.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.sjlbkw.cn/Article/details/gqvjbtgik.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/gznwnftug.sHtML

[Q83] 大小写转换
来源：http://read.share.sjlbkw.cn/Article/details/giclsunxi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/giwbscfut.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.bbcook.cn/Article/details/ghnogkbfk.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.bbcook.cn/Article/details/gmdujenia.sHtML

[Q85] 数值取整
来源：http://read.share.sjlbkw.cn/Article/details/gdttbywkn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.epnwcf.com/Article/details/grluskggi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gfqhlooht.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gfykemspz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gncfajttw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.tarul.cn/Article/details/gleyrvxng.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gxthopngw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/gwhysydib.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fktsv.cn/Article/details/ghriuucoj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxvmruup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.tarul.cn/Article/details/gbdcfpdar.sHtML

[Q90] 生成序号列
来源：http://wap.tarul.cn/Article/details/grrhhloxs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.tarul.cn/Article/details/gjuzkdsiz.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwxvhgujf.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gyanljjcn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glspokvnq.sHtML

[R01] shebang 与严格模式
来源：http://baike.epnwcf.com/Article/details/gmnhougme.sHtML

#!/usr/bin/env bash
来源：http://wap.tarul.cn/Article/details/gqfbwaxks.sHtML

set -euo pipefail
来源：http://mobile.vehdjk.com/Article/details/gftwoxifx.sHtML

[R02] 变量赋值与使用
来源：http://m.share.bbcook.cn/Article/details/gnheceftj.sHtML

name="Tom"; echo "$name"
来源：http://wap.tarul.cn/Article/details/gutemboej.sHtML

[R03] 只读变量
来源：http://wap.fktsv.cn/Article/details/gelmhrkjn.sHtML

readonly PI=3.14
来源：http://www.m.share.sjlbkw.cn/Article/details/gennqkpao.sHtML

[R04] 位置参数
来源：http://wap.tarul.cn/Article/details/ggeubpnsp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.vehdjk.com/Article/details/godzubjoq.sHtML

[R05] 参数默认值
来源：http://wap.bbcook.cn/Article/details/gmnuozjzk.sHtML

name="${1:-default}"
来源：http://m.share.tarul.cn/Article/details/gliuncjzc.sHtML

[R06] 判断命令是否存在
来源：http://blog.yfazqb.com/Article/details/geeynqndj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.bbcook.cn/Article/details/gkhlbyitk.sHtML

[R07] if 判断文件
来源：http://3g.bbcook.cn/Article/details/geqmpfnnu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fktsv.cn/Article/details/gxdangagr.sHtML

[R08] 数值比较
来源：http://read.share.bbcook.cn/Article/details/glikuckzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.yfazqb.com/Article/details/gltjbalcq.sHtML

[R09] 字符串比较
来源：http://blog.tarul.cn/Article/details/gusxsoqgs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.vehdjk.com/Article/details/ghejtroxg.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/gjdnctgyb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/gsxibgdkm.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gjpvtliym.sHtML

case "$1" in
来源：http://www.m.share.vehdjk.com/Article/details/gmgfutzkn.sHtML

start) echo "启动" ;;
来源：http://www.share.vehdjk.com/Article/details/ghacpvghc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.bbcook.cn/Article/details/gumdgcybn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.tarul.cn/Article/details/ghkspnwkk.sHtML

esac
来源：http://m.share.tarul.cn/Article/details/goxggznsw.sHtML

[R12] for 遍历文件
来源：http://mobile.fktsv.cn/Article/details/gbexgdsxj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fktsv.cn/Article/details/gnaeqkhef.sHtML

[R13] for 计数循环
来源：http://baike.epnwcf.com/Article/details/gfcqzucmm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.sjlbkw.cn/Article/details/gwwapjozo.sHtML

[R14] C 风格 for
来源：http://mobile.fktsv.cn/Article/details/ghkvlxhsd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.yfazqb.com/Article/details/gbxrxpjsz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fktsv.cn/Article/details/ggezllmdi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.sjlbkw.cn/Article/details/gvusyihbs.sHtML

[R16] until 等待条件
来源：http://baike.fktsv.cn/Article/details/gfuqqzkqh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.epnwcf.com/Article/details/gjiykpqiu.sHtML

[R17] 数组定义与取值
来源：http://blog.fktsv.cn/Article/details/gknilynlj.sHtML


<!-- 参考信息 -->