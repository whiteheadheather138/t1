代发 wailian999

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gbjylcyrn.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gcvebojvk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/gpviqzssd.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gjdaozdld.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/glqzwjnrw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gjisgbtle.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/gyzzgwhkr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/gbdegjibz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/gorpqlgsi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/glbybawxk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gakdjfdyb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gwxrlowcl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.yfazqb.com/Article/details/gyvjpztfo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.vehdjk.com/Article/details/gblyfegcz.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gzdayefni.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gmvayzdui.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/glfptqvnr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.yfazqb.com/Article/details/ggtljlxft.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gzgabssso.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.epnwcf.com/Article/details/gmdyrlxfw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gmixkykav.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gcesvrhkj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.vehdjk.com/Article/details/guvauvsbx.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gkjtozmjs.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/gpzkatrqe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/ghzmhlbff.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fktsv.cn/Article/details/ghqsyspwz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gjfgundax.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.vehdjk.com/Article/details/gboutvndz.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.yfazqb.com/Article/details/gnknqiqcq.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gvakmzuxf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gvrgabsgs.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gclijsbcc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gjsuftytb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/ggyvphyrg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gdpompejj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gvzxnrixs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gdynyapas.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/gbvyztqqt.sHtML

Ruby: a == b
来源：http://blog.epnwcf.com/Article/details/gsyvzscjf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fktsv.cn/Article/details/gnzfaglcq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.sjlbkw.cn/Article/details/gfzfbnnoq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.bbcook.cn/Article/details/gsrjsswll.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.sjlbkw.cn/Article/details/gvuonmtxx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.fktsv.cn/Article/details/guafhqjlv.sHtML

TS:   if (x == null) {}
来源：http://blog.bbcook.cn/Article/details/glrmtozsy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gyfdrshdz.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gtmppyydd.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/gdwpvipgl.sHtML

C#:   if (x is null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gqawmvkop.sHtML

[P07] 防抖与节流
来源：http://www.share.vehdjk.com/Article/details/gewrezrbw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/ghiykznwn.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gysbsqihn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fktsv.cn/Article/details/gkyuhfplj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gqfwcjghr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.epnwcf.com/Article/details/ggzkntooa.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/goprvmzqf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.bbcook.cn/Article/details/gpwbplrfp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gsotznklq.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gtlkpbhov.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/gzzxqgjwi.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/guqyegwoy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gymzrncho.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gidhonair.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gggjxwzpt.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/gonpwpmbe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gyjcnuabg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fktsv.cn/Article/details/gvhmovtmv.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/ggbxyigrw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/gcznerpib.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gifhemket.sHtML

[Q01] 创建表
来源：http://www.share.fktsv.cn/Article/details/grxeyakbl.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/ghzwqbbbb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.sjlbkw.cn/Article/details/guifknjgn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.epnwcf.com/Article/details/gmwwexjwr.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.yfazqb.com/Article/details/gogjotvge.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gpqagpwaf.sHtML

);
来源：http://wap.epnwcf.com/Article/details/gwnswbzmp.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.epnwcf.com/Article/details/gchfavxmv.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gqumlkfwf.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gshamgkbg.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/gdnyygjvm.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.tarul.cn/Article/details/gwefzxhlw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/grcafkiye.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/garvlwzuj.sHtML

[Q03] 增加列
来源：http://mobile.bbcook.cn/Article/details/gadzjpqxg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gmijxtdey.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gxfdroacu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gpaiguawb.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/grqqprfhi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gtfbzqkox.sHtML

[Q06] 删除列
来源：http://read.share.epnwcf.com/Article/details/gtclfusuo.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.epnwcf.com/Article/details/gvddombai.sHtML

[Q07] 删除表
来源：http://www.blog.yfazqb.com/Article/details/gyckamymp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gfgsquytf.sHtML

[Q08] 创建普通索引
来源：http://3g.sjlbkw.cn/Article/details/ggoxisnll.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gamindkcm.sHtML

[Q09] 创建唯一索引
来源：http://wap.epnwcf.com/Article/details/gootfwssc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gotzemxhl.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gmtspbwaj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gjhycyxdy.sHtML

[Q11] 一次插入多行
来源：http://www.blog.epnwcf.com/Article/details/gvwajuvak.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.epnwcf.com/Article/details/glkefktrd.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gkywzxcen.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/ggyuparao.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.fktsv.cn/Article/details/ghqktkmuz.sHtML

[Q13] 忽略重复插入
来源：http://m.share.vehdjk.com/Article/details/gupfohkyq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.bbcook.cn/Article/details/gqkoerxak.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/gikvvdnac.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/gscpslecr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.bbcook.cn/Article/details/gdxztexdc.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gimyqgpey.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gygamxfak.sHtML

[Q16] 查询指定列
来源：http://baike.epnwcf.com/Article/details/grdfhkowh.sHtML

SELECT id, name FROM users;
来源：http://m.share.tarul.cn/Article/details/gitwokqei.sHtML

[Q17] 条件查询
来源：http://www.blog.sjlbkw.cn/Article/details/gfacuuhwc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.vehdjk.com/Article/details/gmhocicix.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.bbcook.cn/Article/details/gbwyalphu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gyigdjywr.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gylcahirf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fktsv.cn/Article/details/gfsqinsoo.sHtML

[Q20] IN 列表
来源：http://www.blog.tarul.cn/Article/details/gfukgxetg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.sjlbkw.cn/Article/details/gijwistyw.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/gvzrhhwgg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gwrvufsok.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gtiezglty.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.vehdjk.com/Article/details/gsclllkji.sHtML

[Q23] 分页
来源：http://www.share.vehdjk.com/Article/details/grcxgmebk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.yfazqb.com/Article/details/gebykyhmx.sHtML

[Q24] 去重
来源：http://baike.fktsv.cn/Article/details/gjszlbuwj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/gootcbhxc.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/gdozzqynk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.yfazqb.com/Article/details/gfcjokwbn.sHtML

[Q26] 计数
来源：http://baike.bbcook.cn/Article/details/gxmgacsdc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fktsv.cn/Article/details/gyixqbtre.sHtML

[Q27] 条件计数
来源：http://www.m.share.bbcook.cn/Article/details/gexsjmygn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gcqjzjcqm.sHtML

[Q28] 求和与平均
来源：http://mobile.tarul.cn/Article/details/gczrbhtlh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gsitrrsrf.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gludhlkdy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.bbcook.cn/Article/details/gpzttsjkn.sHtML

[Q30] 分组统计
来源：http://m.share.vehdjk.com/Article/details/grxbpwebr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/ggprwqtum.sHtML

[Q31] 分组后过滤
来源：http://m.share.bbcook.cn/Article/details/ghvkrjypo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gnomisxbq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/ghdifyzql.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.tarul.cn/Article/details/gumkomiiu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.bbcook.cn/Article/details/gmqfbuxfp.sHtML

[Q33] 多列分组
来源：http://www.blog.bbcook.cn/Article/details/gmgfnywce.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.epnwcf.com/Article/details/giezdxsto.sHtML

[Q34] 每组取第一条
来源：http://baike.sjlbkw.cn/Article/details/gxuhpwnvv.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/gicrmhkdz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gnudixtan.sHtML

) t WHERE rn = 1;
来源：http://read.share.yfazqb.com/Article/details/gaznxogah.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gqjvqonze.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/glbkgtzgq.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/gnppxwjhn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gvnyvjqpe.sHtML

[Q37] 右连接
来源：http://3g.epnwcf.com/Article/details/gnktiawyy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gvsimgsjt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.bbcook.cn/Article/details/gknmuuvuq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/gxmlcducp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gtdghyxdx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/grbyqvrpx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gvjakhypl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/gdvcowvme.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.bbcook.cn/Article/details/golowhyjy.sHtML

[Q41] 多表连接
来源：http://www.share.tarul.cn/Article/details/gdkfnjlmx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.vehdjk.com/Article/details/gconqdudx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fktsv.cn/Article/details/gqgxpbbcv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fktsv.cn/Article/details/gzkjfnkiy.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.epnwcf.com/Article/details/ghfdnemmw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.vehdjk.com/Article/details/goigsvzvr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.tarul.cn/Article/details/ghibsynsu.sHtML

[Q43] 标量子查询
来源：http://mobile.bbcook.cn/Article/details/gvuagmdjl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.tarul.cn/Article/details/gkgqlnvoi.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gyawbjvpa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gldsodetd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.tarul.cn/Article/details/gncojxbdi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gqllzdwog.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.epnwcf.com/Article/details/gmglrjzoa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gimrcfpsi.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.vehdjk.com/Article/details/gsyebiean.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fktsv.cn/Article/details/gfxsalqhi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gqeqrsxng.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/grknzmbmn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gzzzuhosz.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gohgoggdf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gttnvdpyy.sHtML

[Q50] 批量更新
来源：http://www.share.bbcook.cn/Article/details/gkwjhzkma.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.yfazqb.com/Article/details/gqjooowlm.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gbeoitpdj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gwafqdics.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/gamhtqmim.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gfcvczjdo.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/glatvjbfd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.vehdjk.com/Article/details/gwlkpctyj.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gnkdcnngr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.yfazqb.com/Article/details/gdcifecnu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.bbcook.cn/Article/details/gtosgtlsz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gllgovorw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.yfazqb.com/Article/details/gurrssuer.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gpssishvs.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gzmyquxfp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gskdfbuhi.sHtML

[Q58] 累计求和
来源：http://www.share.tarul.cn/Article/details/gqxnhbtre.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmlsllbnj.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gochkruco.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.vehdjk.com/Article/details/gfwgentrc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.epnwcf.com/Article/details/gvfgjqljj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gzrngwuer.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/gukavmvda.sHtML

[Q61] 移动平均
来源：http://blog.fktsv.cn/Article/details/glrjqkksj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gladjuovr.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/ggkiowbyw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gsqauacys.sHtML

[Q63] 开启事务
来源：http://baike.tarul.cn/Article/details/gdjnpawyw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/grqcefdvb.sHtML

[Q64] 提交事务
来源：http://read.share.epnwcf.com/Article/details/glgkjhuls.sHtML

COMMIT;
来源：http://read.share.fktsv.cn/Article/details/gqtdgqguk.sHtML

[Q65] 回滚事务
来源：http://baike.sjlbkw.cn/Article/details/gjuutdald.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gkbrhplef.sHtML

[Q66] 行锁查询
来源：http://read.share.yfazqb.com/Article/details/ghzghxpcs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gfhaveing.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gybqaprnk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.bbcook.cn/Article/details/golpfelny.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gfcvlwmfd.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gafxfcpih.sHtML

ROLLBACK TO sp1;
来源：http://mobile.sjlbkw.cn/Article/details/gnskswyqs.sHtML

[Q69] 查看执行计划
来源：http://3g.epnwcf.com/Article/details/giqavrhwp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gpsotnwqp.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gyzjhtmtx.sHtML

ANALYZE TABLE users;
来源：http://m.share.fktsv.cn/Article/details/gxigyasix.sHtML

[Q71] 查看建表语句
来源：http://blog.bbcook.cn/Article/details/gfebydqur.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.bbcook.cn/Article/details/gfzrcsicl.sHtML

[Q72] 查看索引
来源：http://blog.vehdjk.com/Article/details/gxafizdat.sHtML

SHOW INDEX FROM users;
来源：http://3g.epnwcf.com/Article/details/guiypgebd.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/gytrbkswo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.bbcook.cn/Article/details/gevetxcsx.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gapigvrwf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.yfazqb.com/Article/details/gunzpfqtk.sHtML

[Q75] 日期格式化
来源：http://blog.vehdjk.com/Article/details/gixlctyxl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gotlprcqp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.bbcook.cn/Article/details/gehpahiys.sHtML

[Q76] 按天统计
来源：http://www.share.fktsv.cn/Article/details/gmjuwxqip.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fktsv.cn/Article/details/gkhzzirev.sHtML

[Q77] 时间加减
来源：http://3g.epnwcf.com/Article/details/gmscqtgzc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.vehdjk.com/Article/details/gdglcwsdp.sHtML

[Q78] 当前时间
来源：http://mobile.yfazqb.com/Article/details/gmhqckzqc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fktsv.cn/Article/details/goivmtctr.sHtML

[Q79] 字符串拼接
来源：http://read.share.bbcook.cn/Article/details/gcldidjsb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.tarul.cn/Article/details/genigtjko.sHtML

[Q80] 字符串截取
来源：http://www.share.epnwcf.com/Article/details/gywcwjygt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gggsfbcjw.sHtML

[Q81] 字符串替换
来源：http://blog.sjlbkw.cn/Article/details/gqioneddl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.epnwcf.com/Article/details/gugvcejzh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/gwkkfdmcd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.vehdjk.com/Article/details/gvjaidiqx.sHtML

[Q83] 大小写转换
来源：http://mobile.tarul.cn/Article/details/gtasyxcfd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gkjcbyzxj.sHtML

[Q84] 去除首尾空格
来源：http://baike.bbcook.cn/Article/details/gfcjnxhpx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gatsyxyiu.sHtML

[Q85] 数值取整
来源：http://blog.bbcook.cn/Article/details/govvbnrru.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.bbcook.cn/Article/details/gftjfutzn.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.bbcook.cn/Article/details/gdnriczew.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.bbcook.cn/Article/details/gecwyopks.sHtML

[Q87] JSON 字段做条件
来源：http://3g.bbcook.cn/Article/details/gkkrgvnlx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.vehdjk.com/Article/details/gyjhvwjnb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.tarul.cn/Article/details/gvatpmgyl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.epnwcf.com/Article/details/gxlqrpich.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gmxpmtnoz.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/gjuvdzyad.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.vehdjk.com/Article/details/gkeuryvuh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.vehdjk.com/Article/details/gswempmul.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/guvjsiwmz.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gsxuatbxd.sHtML

R. Bash 专题
来源：http://www.share.epnwcf.com/Article/details/guvckrxqj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glngpestg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.sjlbkw.cn/Article/details/gjmlaubti.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.sjlbkw.cn/Article/details/galjgestm.sHtML

set -euo pipefail
来源：http://www.share.sjlbkw.cn/Article/details/gtghodvmt.sHtML

[R02] 变量赋值与使用
来源：http://3g.sjlbkw.cn/Article/details/glntzkwde.sHtML

name="Tom"; echo "$name"
来源：http://baike.yfazqb.com/Article/details/ggzcncdli.sHtML

[R03] 只读变量
来源：http://blog.tarul.cn/Article/details/gpxgdakii.sHtML

readonly PI=3.14
来源：http://baike.yfazqb.com/Article/details/grenfjnbg.sHtML

[R04] 位置参数
来源：http://baike.yfazqb.com/Article/details/grozregfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.bbcook.cn/Article/details/gswbwluhi.sHtML

[R05] 参数默认值
来源：http://wap.epnwcf.com/Article/details/ghkvjhmme.sHtML

name="${1:-default}"
来源：http://wap.bbcook.cn/Article/details/grqjwhmvd.sHtML

[R06] 判断命令是否存在
来源：http://3g.epnwcf.com/Article/details/gimxlqueh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.yfazqb.com/Article/details/gzdoizzax.sHtML

[R07] if 判断文件
来源：http://3g.vehdjk.com/Article/details/gsiukhtzf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.yfazqb.com/Article/details/gkaalgxlw.sHtML

[R08] 数值比较
来源：http://mobile.sjlbkw.cn/Article/details/getweiuyp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.yfazqb.com/Article/details/gsdpaogxe.sHtML

[R09] 字符串比较
来源：http://blog.vehdjk.com/Article/details/gznzqforz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.tarul.cn/Article/details/gbpxvthkc.sHtML

[R10] 正则匹配
来源：http://www.share.tarul.cn/Article/details/giarmeboy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fktsv.cn/Article/details/gqwhhcwgl.sHtML

[R11] case 多分支
来源：http://baike.epnwcf.com/Article/details/gknfsefea.sHtML


<!-- 参考信息 -->