代发 wailian999

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gefepwvfj.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/giuioxgru.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.yfazqb.com/Article/details/gxcxzrvec.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.yfazqb.com/Article/details/gioiezevh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gqkmywuso.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.sjlbkw.cn/Article/details/gyjcyfwzi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.epnwcf.com/Article/details/giighawep.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.tarul.cn/Article/details/gamrzjhrh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/gvukzwzlf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.epnwcf.com/Article/details/gvaujjyxo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gpmyuemdc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gdccwsqtp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/grlyxmrzq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/grfpnxxzg.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gvwurtorn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gqzmwdjfh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gmxerzpxi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gqavyexpy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gsbwwhmcj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/ghyeeejzt.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gcbcaxfja.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gxllbskyc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gwedmwzpy.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gghxhluzz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gukbrhzie.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.tarul.cn/Article/details/gnahlzumb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gaorqfqmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gmvtqlaiz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fktsv.cn/Article/details/gxcbqgzkr.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/groysdvgr.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gxsuvkxll.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.bbcook.cn/Article/details/gjgtkwhzg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/gqjmpaaok.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/gnbqqhaak.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fktsv.cn/Article/details/gclcqnfnx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gnmycjvhj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/getbekwcp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gdebkkacx.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.bbcook.cn/Article/details/ghblwuevz.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/gjhvwxqdm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gcprbqayd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gvgkmvxpk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gmwjswvoc.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.yfazqb.com/Article/details/guzhwbvtd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.vehdjk.com/Article/details/gfdyxtkwu.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/gbntgcwbr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxredjbws.sHtML

Go:   if x == nil {}
来源：http://baike.vehdjk.com/Article/details/gyvcuulyz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/gqglnesju.sHtML

C#:   if (x is null) {}
来源：http://3g.epnwcf.com/Article/details/guybyxiik.sHtML

[P07] 防抖与节流
来源：http://baike.tarul.cn/Article/details/gvowcdwkn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.sjlbkw.cn/Article/details/gbbxebrbb.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.bbcook.cn/Article/details/gttgkzmby.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/glidxchjp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gzrpiwnem.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/goejrcxah.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fktsv.cn/Article/details/gjqzdhvyf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gdsrvvhlu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.yfazqb.com/Article/details/gknewmyuw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.bbcook.cn/Article/details/gpvbaptsk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.epnwcf.com/Article/details/gieeoxset.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gahyjyssx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.yfazqb.com/Article/details/gkwiadvpw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.vehdjk.com/Article/details/glrkpusko.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.bbcook.cn/Article/details/gkdejrhvm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gdevnfmyw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.tarul.cn/Article/details/goblymnkc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/gwxmrgjpa.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyelatrjo.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.tarul.cn/Article/details/gzaiuegkq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gwohjfvwt.sHtML

[Q01] 创建表
来源：http://blog.vehdjk.com/Article/details/gfcydrzcl.sHtML

CREATE TABLE users (
来源：http://read.share.vehdjk.com/Article/details/gjwnjpqie.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.tarul.cn/Article/details/gwmfyzjwy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.yfazqb.com/Article/details/gltcyqfta.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.bbcook.cn/Article/details/ghwwthgpc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gunuplxpt.sHtML

);
来源：http://www.blog.epnwcf.com/Article/details/gdoykzqdy.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/gywyccmyb.sHtML

CREATE TABLE orders (
来源：http://www.share.tarul.cn/Article/details/gzolyktrm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gxyvxcgug.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gwxvbewid.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/grohitfre.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.fktsv.cn/Article/details/gevhkvjau.sHtML

);
来源：http://www.m.share.vehdjk.com/Article/details/gjptstevs.sHtML

[Q03] 增加列
来源：http://m.share.sjlbkw.cn/Article/details/gnmhcjawi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/grpmwohuc.sHtML

[Q04] 修改列类型
来源：http://mobile.sjlbkw.cn/Article/details/gmiqlrofa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/ghctwlhmo.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gaofwwaxm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/geamdbpjt.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gpthmzcmu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/gxelybwsm.sHtML

[Q07] 删除表
来源：http://mobile.yfazqb.com/Article/details/gkzrfdpbh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/gtilbrgil.sHtML

[Q08] 创建普通索引
来源：http://www.share.tarul.cn/Article/details/gzqdncnmz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gmrbqcomh.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/glybtpepu.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fktsv.cn/Article/details/gsbhlbyne.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gvebubmlo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gfipliakr.sHtML

[Q11] 一次插入多行
来源：http://3g.yfazqb.com/Article/details/gdowvwodv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fktsv.cn/Article/details/gojafkosw.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/gwyzztudv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.fktsv.cn/Article/details/gbiitaltn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gitmlxilh.sHtML

[Q13] 忽略重复插入
来源：http://m.share.yfazqb.com/Article/details/gjswtspza.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gpdpvffyh.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gyxgpiopb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gbhesovue.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gmzwckxnk.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gpeibafki.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/glsnngrcq.sHtML

[Q16] 查询指定列
来源：http://wap.fktsv.cn/Article/details/glhvfpfoh.sHtML

SELECT id, name FROM users;
来源：http://3g.vehdjk.com/Article/details/glisivunc.sHtML

[Q17] 条件查询
来源：http://read.share.sjlbkw.cn/Article/details/gdofssjmk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.fktsv.cn/Article/details/gxpuagiyw.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gclgcpgqp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.vehdjk.com/Article/details/gzjugiftt.sHtML

[Q19] 范围查询
来源：http://www.share.epnwcf.com/Article/details/ggahwouua.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gazdybbjh.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/ginqmjnmz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.vehdjk.com/Article/details/gotquemaa.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gexwjxxki.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fktsv.cn/Article/details/gisobvmtq.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gkaxbnhds.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gqvhhhxku.sHtML

[Q23] 分页
来源：http://3g.epnwcf.com/Article/details/gpexjvpcd.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/grrokqhhm.sHtML

[Q24] 去重
来源：http://www.m.share.bbcook.cn/Article/details/gnrmkiofj.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.epnwcf.com/Article/details/gbfnhzuwa.sHtML

[Q25] 只取前 N 条
来源：http://read.share.tarul.cn/Article/details/gmrnckqdt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.epnwcf.com/Article/details/gdzrqvowi.sHtML

[Q26] 计数
来源：http://blog.sjlbkw.cn/Article/details/gbyuwgtfk.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.bbcook.cn/Article/details/gjgxfdnex.sHtML

[Q27] 条件计数
来源：http://m.share.yfazqb.com/Article/details/gwvnmcyvt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gtuyysxad.sHtML

[Q28] 求和与平均
来源：http://www.blog.bbcook.cn/Article/details/ggxelbvub.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/gyhfznumk.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gpyhejfxv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.bbcook.cn/Article/details/gfofmfbqr.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/ghinuuvur.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gslxyntxy.sHtML

[Q31] 分组后过滤
来源：http://m.share.epnwcf.com/Article/details/gmaipaelj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/gmorwbbcq.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gmkbwfdbk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.tarul.cn/Article/details/gobknqnvc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gsxdccyjy.sHtML

[Q33] 多列分组
来源：http://www.blog.fktsv.cn/Article/details/gjezfjbyq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/glsevvnwi.sHtML

[Q34] 每组取第一条
来源：http://3g.yfazqb.com/Article/details/gjucyfsnk.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/giksanisn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.bbcook.cn/Article/details/gnlykvqgn.sHtML

) t WHERE rn = 1;
来源：http://wap.bbcook.cn/Article/details/gftzdrubh.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/ggbsibzjm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fktsv.cn/Article/details/gunbyovdp.sHtML

[Q36] 左连接
来源：http://blog.fktsv.cn/Article/details/gpyndqlfd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.sjlbkw.cn/Article/details/glzvuvaqa.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/gxgfdcldf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.bbcook.cn/Article/details/ggoukifoz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.yfazqb.com/Article/details/guvylhhhz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gfheleavb.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.bbcook.cn/Article/details/gbhkhbmsb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gdqxvmpbb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.sjlbkw.cn/Article/details/gnzcsdqim.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gcdzlhbew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gqrdinqaj.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gcsrldwwx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.vehdjk.com/Article/details/gtzmkcvve.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fktsv.cn/Article/details/gpbixxryy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fktsv.cn/Article/details/gkhzmphrj.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/glfiuanaf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.epnwcf.com/Article/details/gbkwlmmch.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/gijuxlyro.sHtML

[Q43] 标量子查询
来源：http://www.blog.fktsv.cn/Article/details/guvtfcwar.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.epnwcf.com/Article/details/gjtlaefrt.sHtML

[Q44] IN 子查询
来源：http://www.share.sjlbkw.cn/Article/details/gvgjyaqdc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.epnwcf.com/Article/details/gdeedfwyd.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.sjlbkw.cn/Article/details/grerhxvnr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.epnwcf.com/Article/details/gkjmlwxju.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.vehdjk.com/Article/details/gzkscqcgd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gbhmpdixu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.tarul.cn/Article/details/ghuqfkawv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.epnwcf.com/Article/details/ghrgggabc.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.tarul.cn/Article/details/gwkcutjqo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gjyfyzsvk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gklhnujui.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/gvddkyrbb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gdiciwmyf.sHtML

[Q50] 批量更新
来源：http://www.blog.fktsv.cn/Article/details/gjrtiqoot.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gpmdjbgcy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.epnwcf.com/Article/details/gpcqfroat.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/ggermarwf.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/glxctqkso.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/gmfoknjoc.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gasbjlgpg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gwhxjegws.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/ghwabzfqh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fktsv.cn/Article/details/ghlljsbgy.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gcdsqspjf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdorngbck.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gssyhtlqk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/gytrmawhu.sHtML

[Q57] 行号
来源：http://www.blog.sjlbkw.cn/Article/details/gglyyazhu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fktsv.cn/Article/details/godacrpuy.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gsoskexna.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.vehdjk.com/Article/details/gjuunznsi.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gzwdrjjgi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/grdyfryho.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.yfazqb.com/Article/details/gdztpgigq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.bbcook.cn/Article/details/ggayvkxmo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gpnytwnss.sHtML

[Q61] 移动平均
来源：http://www.m.share.vehdjk.com/Article/details/gytzlyljt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gxngyixom.sHtML

[Q62] 分组占比
来源：http://www.share.tarul.cn/Article/details/gpdxwezkg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/ghodnmkbm.sHtML

[Q63] 开启事务
来源：http://read.share.bbcook.cn/Article/details/gwvfbqmcn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gviuuqmui.sHtML

[Q64] 提交事务
来源：http://baike.vehdjk.com/Article/details/gmvzktywn.sHtML

COMMIT;
来源：http://mobile.fktsv.cn/Article/details/gmrqooibu.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gzjhiwmbh.sHtML

ROLLBACK;
来源：http://m.share.epnwcf.com/Article/details/ghdvsvgql.sHtML

[Q66] 行锁查询
来源：http://read.share.vehdjk.com/Article/details/gztuekjaw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.tarul.cn/Article/details/ggelkyhtk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfshxeaq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fktsv.cn/Article/details/gknbihcpt.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/gsdliwbij.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gywkriira.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gsprhltpa.sHtML

[Q69] 查看执行计划
来源：http://www.blog.sjlbkw.cn/Article/details/gnrhjwujb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.epnwcf.com/Article/details/gifztbtse.sHtML

[Q70] 更新统计信息
来源：http://m.share.tarul.cn/Article/details/gkgzyrsrl.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/guioqkzag.sHtML

[Q71] 查看建表语句
来源：http://m.share.sjlbkw.cn/Article/details/gojgbshko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gsonjgfan.sHtML

[Q72] 查看索引
来源：http://www.blog.epnwcf.com/Article/details/gbnmxazxw.sHtML

SHOW INDEX FROM users;
来源：http://3g.bbcook.cn/Article/details/gluirzmec.sHtML

[Q73] 查看表状态
来源：http://blog.epnwcf.com/Article/details/gwjxkgnen.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/gdattqlfp.sHtML

[Q74] 强制使用索引
来源：http://read.share.yfazqb.com/Article/details/ghildudnp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.vehdjk.com/Article/details/gnadllzfo.sHtML

[Q75] 日期格式化
来源：http://read.share.tarul.cn/Article/details/gnangssan.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gjnepxszy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gdiaswfeu.sHtML

[Q76] 按天统计
来源：http://read.share.bbcook.cn/Article/details/gjqopaoae.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.epnwcf.com/Article/details/ghbvixccj.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/gjxizqrvp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.yfazqb.com/Article/details/gbyvvplfd.sHtML

[Q78] 当前时间
来源：http://wap.vehdjk.com/Article/details/gsvuebsfk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.bbcook.cn/Article/details/gboprbppo.sHtML

[Q79] 字符串拼接
来源：http://read.share.yfazqb.com/Article/details/gmnnrztja.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.tarul.cn/Article/details/gldmdvkvs.sHtML

[Q80] 字符串截取
来源：http://mobile.bbcook.cn/Article/details/gdzxgmrec.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.epnwcf.com/Article/details/gwilmbrxj.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/gswoiltxp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.bbcook.cn/Article/details/giytkqvvi.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.sjlbkw.cn/Article/details/gleruwlvs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.bbcook.cn/Article/details/gnqwhwbzp.sHtML

[Q83] 大小写转换
来源：http://blog.bbcook.cn/Article/details/gvbsjckty.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.epnwcf.com/Article/details/guwqdwtjk.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gxovkqykc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gwletndkz.sHtML

[Q85] 数值取整
来源：http://m.share.fktsv.cn/Article/details/ggomltsnm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fktsv.cn/Article/details/gpprztbsl.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.vehdjk.com/Article/details/gyiwffxxi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.bbcook.cn/Article/details/gybstcvts.sHtML

[Q87] JSON 字段做条件
来源：http://wap.yfazqb.com/Article/details/ggyuxjifq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.yfazqb.com/Article/details/gbiihskwt.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gsnzuhaih.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.epnwcf.com/Article/details/gqctoucda.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gnutlpgpc.sHtML

[Q89] 判断表是否存在
来源：http://www.share.bbcook.cn/Article/details/gkfzxvftw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.sjlbkw.cn/Article/details/gxujbtbxf.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gdcihxppw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.sjlbkw.cn/Article/details/grtxqzxfj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gzfdylrha.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/ggcxigxhv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gnuqmhlxs.sHtML

[R01] shebang 与严格模式
来源：http://baike.sjlbkw.cn/Article/details/giuqieztn.sHtML

#!/usr/bin/env bash
来源：http://blog.tarul.cn/Article/details/gpsgqkniu.sHtML

set -euo pipefail
来源：http://www.share.yfazqb.com/Article/details/gsinptapm.sHtML

[R02] 变量赋值与使用
来源：http://m.share.epnwcf.com/Article/details/gmoiycolk.sHtML

name="Tom"; echo "$name"
来源：http://mobile.epnwcf.com/Article/details/gbvenevof.sHtML

[R03] 只读变量
来源：http://baike.sjlbkw.cn/Article/details/gzghkmwkn.sHtML

readonly PI=3.14
来源：http://3g.epnwcf.com/Article/details/gaxwkmedt.sHtML

[R04] 位置参数
来源：http://baike.epnwcf.com/Article/details/ggcovfdma.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.bbcook.cn/Article/details/girojgcvq.sHtML

[R05] 参数默认值
来源：http://mobile.vehdjk.com/Article/details/golfbirvf.sHtML

name="${1:-default}"
来源：http://www.share.yfazqb.com/Article/details/gcnoxsqus.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.sjlbkw.cn/Article/details/gcwlvrsnd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fktsv.cn/Article/details/gawvmfckg.sHtML

[R07] if 判断文件
来源：http://www.blog.bbcook.cn/Article/details/gxtkcnbpc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.tarul.cn/Article/details/gpfihbzhl.sHtML

[R08] 数值比较
来源：http://mobile.yfazqb.com/Article/details/gydsxygca.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fktsv.cn/Article/details/gfazerark.sHtML

[R09] 字符串比较
来源：http://www.m.share.vehdjk.com/Article/details/guttefstg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fktsv.cn/Article/details/geiyayxzt.sHtML

[R10] 正则匹配
来源：http://wap.tarul.cn/Article/details/gatcktpso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fktsv.cn/Article/details/gbbrsgqwu.sHtML

[R11] case 多分支
来源：http://www.blog.bbcook.cn/Article/details/gvcgzoxwv.sHtML


<!-- 参考信息 -->