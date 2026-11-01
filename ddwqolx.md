代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fktsv.cn/Article/details/ghivhdgxm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.vehdjk.com/Article/details/gckrqyxmr.sHtML

[P03] 生成短随机字符串
来源：http://mobile.vehdjk.com/Article/details/gedhdfkop.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gqdayhnaf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.yfazqb.com/Article/details/gthslsmck.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.bbcook.cn/Article/details/gzthalvuj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.tarul.cn/Article/details/gsfqylzka.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/glfdljnzc.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.epnwcf.com/Article/details/gkmyoqolp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gztxfuybm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/gzimdjsyf.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gddzydmbz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gxduzmdds.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fktsv.cn/Article/details/glyiqxbah.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gpwnjtdtz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/gpkgoyczm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gpzsqibwi.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.sjlbkw.cn/Article/details/glelrciru.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gqlmsmurq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gcahzsrtf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gomgffoqm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.tarul.cn/Article/details/grminlsmf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gymivuvwr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/guuqplnfm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/gjrnugzma.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.tarul.cn/Article/details/gbktkgriy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gtsrcsayj.sHtML

Ruby: a == b
来源：http://www.m.share.bbcook.cn/Article/details/gdcfijptn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.tarul.cn/Article/details/giqooeotw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.sjlbkw.cn/Article/details/gptqpnmns.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.vehdjk.com/Article/details/gctalohyl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.tarul.cn/Article/details/gmwqoqtsb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/gcjbirjjk.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gbiefzeqs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.epnwcf.com/Article/details/gypewjkph.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gbkntwodo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/guoksdape.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gbegnftbj.sHtML

[P07] 防抖与节流
来源：http://m.share.sjlbkw.cn/Article/details/gsmzcivim.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.epnwcf.com/Article/details/gjrquvmnl.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gnwknzndd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/gfnlxbmja.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fktsv.cn/Article/details/gzlhosflc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.epnwcf.com/Article/details/gowekrtpp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gwzeuhvbd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.tarul.cn/Article/details/gscqzxedj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gohgutfgg.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.tarul.cn/Article/details/gswxoahgd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.bbcook.cn/Article/details/gluwdruyj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gqrzyamhx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/gzrvcgozk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.epnwcf.com/Article/details/gkdckpgnz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.epnwcf.com/Article/details/gacmbamfn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/giurbefzn.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/giigxcawz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.tarul.cn/Article/details/gjjzcmrrr.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkhamrlpj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.tarul.cn/Article/details/gmnexrsqe.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glcsktqzk.sHtML

[Q01] 创建表
来源：http://www.m.share.bbcook.cn/Article/details/ghwxmbnme.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gyjhggfug.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.vehdjk.com/Article/details/gcqkomswv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gagbcgbsy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.sjlbkw.cn/Article/details/gngixflzi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.bbcook.cn/Article/details/gurcxbfgi.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gbewlwcbo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gnyfstrtf.sHtML

CREATE TABLE orders (
来源：http://www.blog.yfazqb.com/Article/details/gxjfuwdic.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fktsv.cn/Article/details/gzoqzoxsr.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.sjlbkw.cn/Article/details/glxhgwxij.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.epnwcf.com/Article/details/gxztdvjve.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.yfazqb.com/Article/details/gninjzxqj.sHtML

);
来源：http://www.share.bbcook.cn/Article/details/gbkkpqudm.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/guwxyuuqt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/gcnqctful.sHtML

[Q04] 修改列类型
来源：http://www.m.share.yfazqb.com/Article/details/gmhcuganm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/guxlxdcwr.sHtML

[Q05] 重命名列
来源：http://www.share.tarul.cn/Article/details/gudluifqo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.sjlbkw.cn/Article/details/gurmlqfgw.sHtML

[Q06] 删除列
来源：http://www.share.sjlbkw.cn/Article/details/gptbvfhlb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gshulmfje.sHtML

[Q07] 删除表
来源：http://wap.tarul.cn/Article/details/gpvvbolsm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.bbcook.cn/Article/details/gxsmrotuy.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/gukcarwsf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.yfazqb.com/Article/details/gndettndd.sHtML

[Q09] 创建唯一索引
来源：http://mobile.yfazqb.com/Article/details/gocayjigf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gsuovdvci.sHtML

[Q10] 插入单行
来源：http://3g.fktsv.cn/Article/details/guvtvpgkt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gauawsrpv.sHtML

[Q11] 一次插入多行
来源：http://read.share.vehdjk.com/Article/details/graytkvgc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/gxvldlcza.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.sjlbkw.cn/Article/details/gcjyuvaqk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.yfazqb.com/Article/details/gtkhhiccs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gknarmzfn.sHtML

[Q13] 忽略重复插入
来源：http://blog.tarul.cn/Article/details/gdvwdofbz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/gjhcgzczb.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.vehdjk.com/Article/details/gnjdrpsbc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.epnwcf.com/Article/details/guzjeofrk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.yfazqb.com/Article/details/gtpcrbzqe.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gskcclail.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjfpamhsj.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/ggnccorgk.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gvmayxdak.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/gtxstjnal.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gdydzohgz.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gcjkbxatz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gnpmgayer.sHtML

[Q19] 范围查询
来源：http://read.share.bbcook.cn/Article/details/gcphtrolb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.vehdjk.com/Article/details/gpwswnphm.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/guqgjoqgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.epnwcf.com/Article/details/gmrnszahv.sHtML

[Q21] 空值判断
来源：http://mobile.bbcook.cn/Article/details/gpnxxxjvz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/grayzeogt.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gaceetbsc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gqdircxvc.sHtML

[Q23] 分页
来源：http://www.blog.bbcook.cn/Article/details/gvltzoioe.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.tarul.cn/Article/details/gsjcrwmor.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/gfuckawrh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.tarul.cn/Article/details/goanniosz.sHtML

[Q25] 只取前 N 条
来源：http://wap.tarul.cn/Article/details/gmhwxujse.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.yfazqb.com/Article/details/gwcoaykjw.sHtML

[Q26] 计数
来源：http://wap.bbcook.cn/Article/details/gvdywpxje.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/giogriiza.sHtML

[Q27] 条件计数
来源：http://www.blog.epnwcf.com/Article/details/ggylppjch.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ggdaoczan.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gcetqrrrq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gyaignrwz.sHtML

[Q29] 最大最小值
来源：http://blog.tarul.cn/Article/details/gwfdrzgyw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gvavpioop.sHtML

[Q30] 分组统计
来源：http://read.share.yfazqb.com/Article/details/gtbbnbewc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gbtpnppfm.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gsqftrrzd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.tarul.cn/Article/details/gruqryolf.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.yfazqb.com/Article/details/gzofmwmhx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gihngkhwc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.vehdjk.com/Article/details/goigufzft.sHtML

[Q33] 多列分组
来源：http://read.share.epnwcf.com/Article/details/gycuagjtz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.tarul.cn/Article/details/glqsrsqmc.sHtML

[Q34] 每组取第一条
来源：http://mobile.sjlbkw.cn/Article/details/gyudzttoo.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gastjbzau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gryzucdoy.sHtML

) t WHERE rn = 1;
来源：http://www.share.fktsv.cn/Article/details/gcoiwflcm.sHtML

[Q35] 内连接
来源：http://www.blog.sjlbkw.cn/Article/details/gfbdnjxgy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gcvncabvu.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gmlpiyhbm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gefrcclkx.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/goprxrnee.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/gvyerctkq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fktsv.cn/Article/details/gzqmglvvs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fktsv.cn/Article/details/gtqynfqbi.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gnvxxzcgx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gxeysawhi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.bbcook.cn/Article/details/gjafjjjpz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gtkdifcxv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.tarul.cn/Article/details/gtltykzcb.sHtML

[Q41] 多表连接
来源：http://baike.yfazqb.com/Article/details/gfzmensry.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gqxrcankk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.epnwcf.com/Article/details/gdwinvalh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.bbcook.cn/Article/details/gpeqwkxpz.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/goeddwwjt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.sjlbkw.cn/Article/details/gjfldhkky.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.bbcook.cn/Article/details/gphsvvdjt.sHtML

[Q43] 标量子查询
来源：http://m.share.sjlbkw.cn/Article/details/gebckfdbq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/gkazsooon.sHtML

[Q44] IN 子查询
来源：http://wap.vehdjk.com/Article/details/gtcqyrlki.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/gfwlzkigb.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gpdelssci.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.sjlbkw.cn/Article/details/ggjnfdkuc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gbjheekqz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fktsv.cn/Article/details/grcgxless.sHtML

[Q47] 与平均值比较
来源：http://baike.tarul.cn/Article/details/gmuhartcd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.tarul.cn/Article/details/gjzztbmsd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.vehdjk.com/Article/details/glkubuczu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.bbcook.cn/Article/details/gsfqbqwnp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.epnwcf.com/Article/details/gjcehyawp.sHtML

[Q49] 更新单行
来源：http://wap.vehdjk.com/Article/details/gyyldscai.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.epnwcf.com/Article/details/gfhyvoyum.sHtML

[Q50] 批量更新
来源：http://read.share.bbcook.cn/Article/details/gdkbvcauq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gavrcpeju.sHtML

[Q51] 用子查询更新
来源：http://read.share.tarul.cn/Article/details/gfiifalri.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.yfazqb.com/Article/details/gsfpkoqtb.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gzoefbsxa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fktsv.cn/Article/details/gchaoknhi.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gitabmcuo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.yfazqb.com/Article/details/gbzygiklb.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/glkqknvsv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.yfazqb.com/Article/details/grjlevnbc.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/gcqpndeyz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.sjlbkw.cn/Article/details/gmnzjtxuj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/guiwhwwcj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.sjlbkw.cn/Article/details/gwawppuwf.sHtML

[Q57] 行号
来源：http://m.share.fktsv.cn/Article/details/gjcwwddrb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gbclkdbay.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/ggmnbwfjj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gjobkgoov.sHtML

[Q59] 分组内累计
来源：http://www.blog.epnwcf.com/Article/details/govxuhixg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/ghytcqwzb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.yfazqb.com/Article/details/gyonnisda.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/gsbsmqwpj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gvvictgih.sHtML

[Q61] 移动平均
来源：http://wap.fktsv.cn/Article/details/gyljomrlz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/ghvpapvcw.sHtML

[Q62] 分组占比
来源：http://baike.tarul.cn/Article/details/gbsjnkgsb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gnrpkxqyv.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gjftlwcgf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.bbcook.cn/Article/details/gduligiyq.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gmzteleci.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gidqcfcfb.sHtML

[Q65] 回滚事务
来源：http://baike.epnwcf.com/Article/details/gtkyxzlep.sHtML

ROLLBACK;
来源：http://mobile.epnwcf.com/Article/details/gohpsywvb.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gvqpanvqv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.sjlbkw.cn/Article/details/gshbdoafg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/gdwxbsvly.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fktsv.cn/Article/details/gogqcluqf.sHtML

[Q68] 保存点
来源：http://m.share.yfazqb.com/Article/details/gujkftcyi.sHtML

SAVEPOINT sp1;
来源：http://m.share.bbcook.cn/Article/details/gdvwkpjkb.sHtML

ROLLBACK TO sp1;
来源：http://3g.bbcook.cn/Article/details/ghpqhvhva.sHtML

[Q69] 查看执行计划
来源：http://m.share.yfazqb.com/Article/details/gbltzzcup.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.tarul.cn/Article/details/gwweamnrq.sHtML

[Q70] 更新统计信息
来源：http://www.share.yfazqb.com/Article/details/geosousut.sHtML

ANALYZE TABLE users;
来源：http://www.blog.sjlbkw.cn/Article/details/gstmilavi.sHtML

[Q71] 查看建表语句
来源：http://mobile.fktsv.cn/Article/details/gilmbiowf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gmhgzbghj.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/gepmpbafs.sHtML

SHOW INDEX FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqlowexxe.sHtML

[Q73] 查看表状态
来源：http://wap.yfazqb.com/Article/details/ghotflvbj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.tarul.cn/Article/details/gpgelgljf.sHtML

[Q74] 强制使用索引
来源：http://wap.epnwcf.com/Article/details/giahndtct.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.bbcook.cn/Article/details/ggpqbepde.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gytcixzob.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gxbvzyubt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.yfazqb.com/Article/details/gxpmjywxj.sHtML

[Q76] 按天统计
来源：http://3g.vehdjk.com/Article/details/gilgxeffm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.tarul.cn/Article/details/gycnfmygv.sHtML

[Q77] 时间加减
来源：http://www.share.fktsv.cn/Article/details/gcunghlbd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fktsv.cn/Article/details/gzrngugzn.sHtML

[Q78] 当前时间
来源：http://www.blog.fktsv.cn/Article/details/gakchtvac.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gmipdnryy.sHtML

[Q79] 字符串拼接
来源：http://blog.vehdjk.com/Article/details/gemlnmjsi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/gpeqgakvv.sHtML

[Q80] 字符串截取
来源：http://mobile.yfazqb.com/Article/details/guytmrvih.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gmcdzskqv.sHtML

[Q81] 字符串替换
来源：http://mobile.vehdjk.com/Article/details/gtxitmszt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fktsv.cn/Article/details/gveqvhudr.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.epnwcf.com/Article/details/gmeiorwio.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gcbcdmmol.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gfunixgnj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gwnqrizrq.sHtML

[Q84] 去除首尾空格
来源：http://wap.tarul.cn/Article/details/gcbbamgkv.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/gtfqmvnvo.sHtML

[Q85] 数值取整
来源：http://m.share.vehdjk.com/Article/details/grkumtpxi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.vehdjk.com/Article/details/ghydptkbl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.yfazqb.com/Article/details/grokukyvm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.tarul.cn/Article/details/gmzjcslte.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/girmrulor.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/guhcpuhiu.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.tarul.cn/Article/details/gmjtyvcdl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.vehdjk.com/Article/details/gcbbopngl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gxepcukga.sHtML

[Q89] 判断表是否存在
来源：http://baike.tarul.cn/Article/details/gizdmrrgl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fktsv.cn/Article/details/gyhxqfwdk.sHtML

[Q90] 生成序号列
来源：http://read.share.bbcook.cn/Article/details/gfauxotwh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fktsv.cn/Article/details/gzjlglwtu.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdbttzrli.sHtML

R. Bash 专题
来源：http://m.share.epnwcf.com/Article/details/gstquakzi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gzrhuonzq.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gmslwajec.sHtML

#!/usr/bin/env bash
来源：http://www.blog.tarul.cn/Article/details/gwqveslhl.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gphrltifw.sHtML

[R02] 变量赋值与使用
来源：http://wap.bbcook.cn/Article/details/ggkhaggxt.sHtML

name="Tom"; echo "$name"
来源：http://3g.epnwcf.com/Article/details/gujxfzkev.sHtML

[R03] 只读变量
来源：http://baike.vehdjk.com/Article/details/girzlfgom.sHtML

readonly PI=3.14
来源：http://3g.vehdjk.com/Article/details/guwahxopr.sHtML

[R04] 位置参数
来源：http://www.blog.bbcook.cn/Article/details/gqgznqvjo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.tarul.cn/Article/details/gwcwjfxdb.sHtML

[R05] 参数默认值
来源：http://www.m.share.tarul.cn/Article/details/gcaddxtfn.sHtML

name="${1:-default}"
来源：http://blog.fktsv.cn/Article/details/gthbquxvz.sHtML

[R06] 判断命令是否存在
来源：http://3g.bbcook.cn/Article/details/gwudmvfku.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.sjlbkw.cn/Article/details/gnldtjijy.sHtML

[R07] if 判断文件
来源：http://m.share.fktsv.cn/Article/details/gbyqnuppu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.tarul.cn/Article/details/gwtnhccib.sHtML

[R08] 数值比较
来源：http://mobile.vehdjk.com/Article/details/gwdzvwvmv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fktsv.cn/Article/details/giohiydgl.sHtML

[R09] 字符串比较
来源：http://mobile.tarul.cn/Article/details/gffwovtpn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.yfazqb.com/Article/details/gkiyrmogv.sHtML

[R10] 正则匹配
来源：http://www.share.epnwcf.com/Article/details/guxaxnmrk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.yfazqb.com/Article/details/glbgeoiiq.sHtML

[R11] case 多分支
来源：http://www.m.share.yfazqb.com/Article/details/glsivsttt.sHtML

case "$1" in
来源：http://www.m.share.bbcook.cn/Article/details/gqsxudwog.sHtML

start) echo "启动" ;;
来源：http://baike.tarul.cn/Article/details/gazvypnco.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.yfazqb.com/Article/details/gwbwjcojm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.yfazqb.com/Article/details/gxhigzbom.sHtML

esac
来源：http://mobile.tarul.cn/Article/details/ggquynvnp.sHtML

[R12] for 遍历文件
来源：http://read.share.yfazqb.com/Article/details/gvbueycmp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fktsv.cn/Article/details/gjuolioih.sHtML

[R13] for 计数循环
来源：http://www.blog.sjlbkw.cn/Article/details/gcimwqhla.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.epnwcf.com/Article/details/gqojtgmek.sHtML

[R14] C 风格 for
来源：http://www.blog.epnwcf.com/Article/details/gmhudkddr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.vehdjk.com/Article/details/ghjhqgjlb.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.epnwcf.com/Article/details/gsbbsgwbp.sHtML


<!-- 参考信息 -->