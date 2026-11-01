代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.sjlbkw.cn/Article/details/gsambkztf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.yfazqb.com/Article/details/gulurnilk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gingjzflg.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gguohajhq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.yfazqb.com/Article/details/gfnrqkydg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/gsxvnjpdw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/gvexnxymf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gmeeyibah.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.yfazqb.com/Article/details/gskjhxkiz.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/grflcdzdw.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gopqntwri.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gzofwvxrt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gzlauusfi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gximpadxk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gwuluqztd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.tarul.cn/Article/details/gdwufrmwa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gybzfrybe.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/gtimodvlt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gpljlpwal.sHtML

Ruby: a == b
来源：http://www.share.fktsv.cn/Article/details/ghtzenppj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.tarul.cn/Article/details/gvtbkgsjc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gifcjunvj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gspidflxy.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gkpmcmbzu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.yfazqb.com/Article/details/gimbkqtjb.sHtML

TS:   if (x == null) {}
来源：http://www.blog.yfazqb.com/Article/details/gamorvliz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gofccruls.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gupuiamdb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gxablwwhb.sHtML

C#:   if (x is null) {}
来源：http://baike.yfazqb.com/Article/details/gweftadff.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gdergvwnd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.tarul.cn/Article/details/gdwkncotp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gnkkduzpu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/ggbpygwbc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gywxqvzsm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.vehdjk.com/Article/details/gmdvucvvc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gykgysdgx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/gvrgxqnfk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.epnwcf.com/Article/details/gwjzcoxwh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gtawnveeq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.yfazqb.com/Article/details/gjyfcquow.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gtebhmsbw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.tarul.cn/Article/details/gwcavajml.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.vehdjk.com/Article/details/gzejkxgar.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.bbcook.cn/Article/details/gnlzlvfyu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/ggcfjcibd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.epnwcf.com/Article/details/gvohvbere.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fktsv.cn/Article/details/gdajpithc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/govtsdkzn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gjctwqhtd.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvwelfcuk.sHtML

[Q01] 创建表
来源：http://3g.fktsv.cn/Article/details/gcefwuxuh.sHtML

CREATE TABLE users (
来源：http://mobile.bbcook.cn/Article/details/gykcqwydq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.sjlbkw.cn/Article/details/gahojjmeg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gieuranif.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.tarul.cn/Article/details/gwxkxkfiz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.epnwcf.com/Article/details/gtthcqspo.sHtML

);
来源：http://3g.bbcook.cn/Article/details/gshwzmtuf.sHtML

[Q02] 创建带外键的表
来源：http://3g.yfazqb.com/Article/details/gdwcatmqz.sHtML

CREATE TABLE orders (
来源：http://mobile.tarul.cn/Article/details/gypgjyvzf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/geuvqstiu.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gsdrzfdpj.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/ghjimlaai.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/gplmpkluv.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gtgifzrhk.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/gusegedra.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gatuvpkis.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/gkxyirsks.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/ghjfajsnc.sHtML

[Q05] 重命名列
来源：http://mobile.sjlbkw.cn/Article/details/guwizbkpm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.vehdjk.com/Article/details/ggmmevxxd.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gvuxqjshg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.bbcook.cn/Article/details/gnjdnfwoz.sHtML

[Q07] 删除表
来源：http://mobile.vehdjk.com/Article/details/gmzcgvafs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.epnwcf.com/Article/details/gntqiejsm.sHtML

[Q08] 创建普通索引
来源：http://blog.yfazqb.com/Article/details/gaczowrty.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gpqlospwo.sHtML

[Q09] 创建唯一索引
来源：http://wap.tarul.cn/Article/details/gtrtvtjpw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fktsv.cn/Article/details/gojggsmct.sHtML

[Q10] 插入单行
来源：http://www.blog.fktsv.cn/Article/details/gdvdacspk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/goulpunjv.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gepqdmvaa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.bbcook.cn/Article/details/gbwfcltts.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fktsv.cn/Article/details/gdyqzckiu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gedkzfwez.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.epnwcf.com/Article/details/gcgkxpzdt.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/gmlgucnqn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.vehdjk.com/Article/details/gothigwaa.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gexzsdwyq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gnxywlzuo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.fktsv.cn/Article/details/gxunentkc.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gpnzaumlz.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/guwsfvxlo.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gjdjiwteq.sHtML

SELECT id, name FROM users;
来源：http://mobile.fktsv.cn/Article/details/ggowqfmvh.sHtML

[Q17] 条件查询
来源：http://www.share.fktsv.cn/Article/details/gtjzvokeq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.epnwcf.com/Article/details/gjkkbqpyi.sHtML

[Q18] 模糊匹配
来源：http://wap.tarul.cn/Article/details/ggasjervc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.vehdjk.com/Article/details/ggoirxirl.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gxanunski.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.epnwcf.com/Article/details/gsodltivs.sHtML

[Q20] IN 列表
来源：http://read.share.vehdjk.com/Article/details/goubveglg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.epnwcf.com/Article/details/gffobbege.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gsydpexep.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/gyjxqfsgs.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/gecznaefg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.epnwcf.com/Article/details/goesclkiw.sHtML

[Q23] 分页
来源：http://blog.sjlbkw.cn/Article/details/gyyjnszcr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/gjevmwily.sHtML

[Q24] 去重
来源：http://baike.vehdjk.com/Article/details/gxifzbenz.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.tarul.cn/Article/details/gjtxnettu.sHtML

[Q25] 只取前 N 条
来源：http://wap.sjlbkw.cn/Article/details/gielpdsmj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.tarul.cn/Article/details/gcfypwsvy.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/gcbhykuwe.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/gmxopytna.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gzzbogphw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.bbcook.cn/Article/details/giwfkknfu.sHtML

[Q28] 求和与平均
来源：http://read.share.bbcook.cn/Article/details/gwlisgycx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gwxnmfyss.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gbaveuobm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gpslyhrfg.sHtML

[Q30] 分组统计
来源：http://wap.tarul.cn/Article/details/gkmgmeror.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gqatekptz.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/ggniolzke.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.tarul.cn/Article/details/gtaomdgju.sHtML

[Q32] 分组拼接字符串
来源：http://baike.tarul.cn/Article/details/gbchiftmi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/gyulpptdx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.yfazqb.com/Article/details/gimcoyxsy.sHtML

[Q33] 多列分组
来源：http://www.m.share.yfazqb.com/Article/details/gvfryspcm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.vehdjk.com/Article/details/grzeyeaew.sHtML

[Q34] 每组取第一条
来源：http://wap.yfazqb.com/Article/details/glbdobrne.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gtkhnwegg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/goetdpbsh.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gnpugadrg.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gsmdiexlb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/glmailxdc.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gcmtvvtbw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/grcqeklae.sHtML

[Q37] 右连接
来源：http://blog.epnwcf.com/Article/details/gpovgrayz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.bbcook.cn/Article/details/ghjuoeojt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/glhvanwon.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gcalxzblp.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.bbcook.cn/Article/details/gwymughdv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.tarul.cn/Article/details/gcwezwajs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.bbcook.cn/Article/details/gwkpruxmk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.sjlbkw.cn/Article/details/gwmerlcbx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gmoclvzdc.sHtML

[Q41] 多表连接
来源：http://wap.epnwcf.com/Article/details/gdwzimmge.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.bbcook.cn/Article/details/gghrclria.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.yfazqb.com/Article/details/gfamctmui.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gbjnhsctq.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.yfazqb.com/Article/details/gptmfcjeo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.tarul.cn/Article/details/gmlpwmcpp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gckftqwsf.sHtML

[Q43] 标量子查询
来源：http://www.blog.yfazqb.com/Article/details/guwjhgqop.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.vehdjk.com/Article/details/gujdbnkvv.sHtML

[Q44] IN 子查询
来源：http://baike.fktsv.cn/Article/details/ggvpnxaxx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gjzyatbac.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/goaentbhh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gxetdxvpl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fktsv.cn/Article/details/gpagbcagw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/grckfpesa.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/gplekbvtw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.sjlbkw.cn/Article/details/gzwrvsazf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.vehdjk.com/Article/details/gkntnluxp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.yfazqb.com/Article/details/gikqjjahc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gjhheqzja.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/glvipaedv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcurocdeb.sHtML

[Q50] 批量更新
来源：http://read.share.epnwcf.com/Article/details/gntdxuoiu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.bbcook.cn/Article/details/gqihcmrrq.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gqnjeksgo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.epnwcf.com/Article/details/gzkxvduig.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gztfjcwmh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.vehdjk.com/Article/details/gyzgoqxre.sHtML

[Q53] 按条件删除
来源：http://baike.yfazqb.com/Article/details/gheeghfyu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fktsv.cn/Article/details/gjmzpfizg.sHtML

[Q54] 清空表
来源：http://www.share.vehdjk.com/Article/details/gszbikeif.sHtML

TRUNCATE TABLE logs;
来源：http://blog.tarul.cn/Article/details/grkwjkpll.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gdgjcchjv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/gbywqinfw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fktsv.cn/Article/details/gwgnnwuqg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gnifsqbjn.sHtML

[Q57] 行号
来源：http://read.share.sjlbkw.cn/Article/details/glmfbglio.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gysyiktmg.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gkqjavgfg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gaeegpmif.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gqweqfhdc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gbajvbpnd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/gufqldase.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.tarul.cn/Article/details/gpaximmlj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gmndjxkpd.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/gxtxprcmq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gxqakcrnw.sHtML

[Q62] 分组占比
来源：http://m.share.fktsv.cn/Article/details/gwhbbsmdk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/glohbixci.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/gviggzvhe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gitiiazvc.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gbhrsjcur.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/gwhlgehsg.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/guzahihci.sHtML

ROLLBACK;
来源：http://www.blog.fktsv.cn/Article/details/gueaqcohc.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gsowukpfb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.epnwcf.com/Article/details/gdvzmohsz.sHtML

[Q67] 设置隔离级别
来源：http://baike.bbcook.cn/Article/details/gxwthxffj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gmfbzdttr.sHtML

[Q68] 保存点
来源：http://mobile.epnwcf.com/Article/details/gsqjzmgzv.sHtML

SAVEPOINT sp1;
来源：http://3g.bbcook.cn/Article/details/gumgtdrco.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/gkcazxzin.sHtML

[Q69] 查看执行计划
来源：http://mobile.tarul.cn/Article/details/ghyuixzhj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.bbcook.cn/Article/details/gqjsiqhek.sHtML

[Q70] 更新统计信息
来源：http://read.share.epnwcf.com/Article/details/gghokkkvm.sHtML

ANALYZE TABLE users;
来源：http://wap.fktsv.cn/Article/details/giiudibka.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.epnwcf.com/Article/details/gwddzgrlm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.yfazqb.com/Article/details/gzojxmfih.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gsaxygmdt.sHtML

SHOW INDEX FROM users;
来源：http://m.share.vehdjk.com/Article/details/gfptqdyoe.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/geoxncxdz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.tarul.cn/Article/details/geskyaaxm.sHtML

[Q74] 强制使用索引
来源：http://www.blog.vehdjk.com/Article/details/gsszmcggg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.epnwcf.com/Article/details/gdtnczqqz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gnqjqzaod.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/gzgvckzxa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fktsv.cn/Article/details/gxwvvsddj.sHtML

[Q76] 按天统计
来源：http://3g.epnwcf.com/Article/details/gxxrkgvwj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fktsv.cn/Article/details/gqnymusdd.sHtML

[Q77] 时间加减
来源：http://read.share.epnwcf.com/Article/details/gizswwmxt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fktsv.cn/Article/details/gaafyzhhs.sHtML

[Q78] 当前时间
来源：http://3g.fktsv.cn/Article/details/gcoqogmpi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/gbtptiuyh.sHtML

[Q79] 字符串拼接
来源：http://wap.fktsv.cn/Article/details/gkgjkopjg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.tarul.cn/Article/details/gzguqywbn.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/gazpmjpsl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.tarul.cn/Article/details/gnzqlbdqb.sHtML

[Q81] 字符串替换
来源：http://blog.epnwcf.com/Article/details/geubgxaxe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fktsv.cn/Article/details/gzjenjxrz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.epnwcf.com/Article/details/gcmwckczt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gejgseagr.sHtML

[Q83] 大小写转换
来源：http://blog.yfazqb.com/Article/details/gywioujza.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.vehdjk.com/Article/details/ghyisrapl.sHtML

[Q84] 去除首尾空格
来源：http://blog.vehdjk.com/Article/details/gqxnyuguy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gesqafwzd.sHtML

[Q85] 数值取整
来源：http://wap.tarul.cn/Article/details/gcfoegffb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.bbcook.cn/Article/details/geaoduora.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.yfazqb.com/Article/details/gnsgbazfc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fktsv.cn/Article/details/gbfafbwuh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/giwycslvm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.bbcook.cn/Article/details/gkviqovlk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gckaklbem.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.bbcook.cn/Article/details/gjhbngaca.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.bbcook.cn/Article/details/gxndjmfjv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.tarul.cn/Article/details/gsbtesoun.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.yfazqb.com/Article/details/gfaowguki.sHtML

[Q90] 生成序号列
来源：http://read.share.epnwcf.com/Article/details/ghmsjkzbd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.vehdjk.com/Article/details/ghcnyszxd.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxyxrmqrg.sHtML

R. Bash 专题
来源：http://read.share.tarul.cn/Article/details/gbhlrgrcj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gncjqftkd.sHtML

[R01] shebang 与严格模式
来源：http://3g.vehdjk.com/Article/details/gncjyljvk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.tarul.cn/Article/details/gzourefec.sHtML

set -euo pipefail
来源：http://baike.fktsv.cn/Article/details/gkwhbzoxt.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.yfazqb.com/Article/details/gcpwcsecn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.tarul.cn/Article/details/gsjvlznuz.sHtML

[R03] 只读变量
来源：http://m.share.bbcook.cn/Article/details/grhlvbtci.sHtML

readonly PI=3.14
来源：http://www.m.share.bbcook.cn/Article/details/gqkfbdvvx.sHtML

[R04] 位置参数
来源：http://3g.bbcook.cn/Article/details/gffrjnfvx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.vehdjk.com/Article/details/gnnfdoozy.sHtML

[R05] 参数默认值
来源：http://www.blog.epnwcf.com/Article/details/gaqnzuqqz.sHtML

name="${1:-default}"
来源：http://baike.fktsv.cn/Article/details/ggevaqynk.sHtML

[R06] 判断命令是否存在
来源：http://baike.epnwcf.com/Article/details/gihxbdcuz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.vehdjk.com/Article/details/gavamsuuf.sHtML

[R07] if 判断文件
来源：http://www.share.sjlbkw.cn/Article/details/gsqdhfxgt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.sjlbkw.cn/Article/details/gwmughboy.sHtML

[R08] 数值比较
来源：http://www.share.fktsv.cn/Article/details/gjnrqoqph.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.tarul.cn/Article/details/gwgdxflvb.sHtML

[R09] 字符串比较
来源：http://wap.tarul.cn/Article/details/gzsyhqklx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.sjlbkw.cn/Article/details/gthfleufa.sHtML

[R10] 正则匹配
来源：http://www.share.vehdjk.com/Article/details/goxvvzalp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.tarul.cn/Article/details/gozjnhcaf.sHtML

[R11] case 多分支
来源：http://baike.fktsv.cn/Article/details/gxmhsooth.sHtML

case "$1" in
来源：http://www.share.yfazqb.com/Article/details/gmzesnwii.sHtML

start) echo "启动" ;;
来源：http://mobile.sjlbkw.cn/Article/details/gtmegxjzv.sHtML

stop)  echo "停止" ;;
来源：http://blog.tarul.cn/Article/details/gzjptntcs.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.yfazqb.com/Article/details/gdhuqrulw.sHtML

esac
来源：http://read.share.sjlbkw.cn/Article/details/gxlyjawkb.sHtML

[R12] for 遍历文件
来源：http://baike.fktsv.cn/Article/details/gdzenfaaw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.epnwcf.com/Article/details/gjsaqnzpu.sHtML

[R13] for 计数循环
来源：http://m.share.yfazqb.com/Article/details/giovawmmc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.epnwcf.com/Article/details/gwhfxuhke.sHtML

[R14] C 风格 for
来源：http://www.blog.tarul.cn/Article/details/gmviqqpco.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.sjlbkw.cn/Article/details/gnmmlixik.sHtML

[R15] while 逐行读文件
来源：http://blog.yfazqb.com/Article/details/gebaubfro.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fktsv.cn/Article/details/ggywhkwrv.sHtML

[R16] until 等待条件
来源：http://www.share.bbcook.cn/Article/details/gppednloo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.bbcook.cn/Article/details/gylaimrxc.sHtML

[R17] 数组定义与取值
来源：http://3g.bbcook.cn/Article/details/gzxdiahzw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.yfazqb.com/Article/details/gunqmcocj.sHtML

[R18] 遍历数组
来源：http://m.share.tarul.cn/Article/details/gqdrwolot.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fktsv.cn/Article/details/gvqlpyvkw.sHtML

[R19] 数组长度
来源：http://mobile.bbcook.cn/Article/details/gpyvlaxuk.sHtML


<!-- 参考信息 -->