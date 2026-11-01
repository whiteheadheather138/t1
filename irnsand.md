代发 wailian999

TS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gmjabecga.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/giilbswce.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.epnwcf.com/Article/details/gyxvneoik.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gyolebnpo.sHtML

C#:   Parallel.For
来源：http://mobile.fktsv.cn/Article/details/gkbbgeqyy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmlvyjnjr.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gmshnxopz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ghfxyfxyl.sHtML

[P01] 生成 UUID
来源：http://read.share.vehdjk.com/Article/details/gvwdhlnoa.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.vehdjk.com/Article/details/gntzhuyuk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fktsv.cn/Article/details/gapwjzrrl.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gxayocvmh.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/greqenmtj.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gsqfioaci.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/gmfgzhniv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.sjlbkw.cn/Article/details/gfssdiaay.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gbkqscsmp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gqbgnoifb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/girqxefmh.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gktfjhuab.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gjynidfpo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/gmjtcpsoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gtiaskrnu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.fktsv.cn/Article/details/gifezpzvs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.sjlbkw.cn/Article/details/gpkaopbta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gautzmlkb.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gnnxalbma.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/glwavgzzj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gzxqzmyys.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gclifnzsy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/gicvocqrp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fktsv.cn/Article/details/gdnlkzrhz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/ghhzjkktu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/ggigqglou.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/gjsleoqgx.sHtML

[P04] 求长度
来源：http://www.blog.tarul.cn/Article/details/gnitdljoo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gvivwopla.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/ggryvwgzz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gesbhcpjg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gdvdqlqvb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gaasxsgaw.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gycsvtkzy.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fktsv.cn/Article/details/gfnsggcfn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/grtfjkzqk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gjnpejedk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.vehdjk.com/Article/details/gsdogrosq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.yfazqb.com/Article/details/ggewrupkp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gblgpslph.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.bbcook.cn/Article/details/gdmptfpcc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gajbxketw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gizbricjv.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/gartiqibp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.epnwcf.com/Article/details/garcgxdcn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.vehdjk.com/Article/details/gujzybxsb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/ganwrejpt.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.bbcook.cn/Article/details/gfbbudbnm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gyebdwgha.sHtML

TS:   if (x == null) {}
来源：http://wap.epnwcf.com/Article/details/goxalhcbl.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.epnwcf.com/Article/details/gjucuqrra.sHtML

Go:   if x == nil {}
来源：http://www.share.fktsv.cn/Article/details/gxezyjlbm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/guicxcxzo.sHtML

C#:   if (x is null) {}
来源：http://3g.yfazqb.com/Article/details/gwnnvxeyu.sHtML

[P07] 防抖与节流
来源：http://blog.tarul.cn/Article/details/gapoqmbqv.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/gtzonjjbo.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gosczazyc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gyruggphs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.epnwcf.com/Article/details/gdqjstwuc.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.yfazqb.com/Article/details/gnjdscdlj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gqqgqoicc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.sjlbkw.cn/Article/details/gincrgfbr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.sjlbkw.cn/Article/details/glwsehbtf.sHtML

[P08] 处理浮点精度问题
来源：http://blog.epnwcf.com/Article/details/gloywxpyl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.yfazqb.com/Article/details/gfnfcbrjh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/ggdjlpzot.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.vehdjk.com/Article/details/gzcmrwxoa.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/gywolvtkh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/geibjojzr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gddldgexv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gflcwpxis.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.tarul.cn/Article/details/gatmiwokv.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghvuqfavq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.sjlbkw.cn/Article/details/gxmbtsrxc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gefmyamae.sHtML

[Q01] 创建表
来源：http://baike.vehdjk.com/Article/details/gycuelkrr.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gjgarkydv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gtquehrhj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.tarul.cn/Article/details/ggdzbtpkd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fktsv.cn/Article/details/gdizepmdb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.sjlbkw.cn/Article/details/gtrymlrzh.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gfpxhqlgv.sHtML

[Q02] 创建带外键的表
来源：http://mobile.bbcook.cn/Article/details/ghuaudafh.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gwtrduwum.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/gonumrzns.sHtML

user_id INT NOT NULL,
来源：http://www.share.bbcook.cn/Article/details/gtjhzdkmu.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fktsv.cn/Article/details/gjklmcskr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gzcpjzfym.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gnwduehii.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gombgekgc.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gvekcybfs.sHtML

[Q04] 修改列类型
来源：http://www.share.vehdjk.com/Article/details/gujxwuwfb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.bbcook.cn/Article/details/gawxdvajm.sHtML

[Q05] 重命名列
来源：http://blog.tarul.cn/Article/details/ggwrwuxhu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.bbcook.cn/Article/details/gzgpienzn.sHtML

[Q06] 删除列
来源：http://blog.epnwcf.com/Article/details/gmmootltd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gzssdlegt.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gyqukmzhf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.yfazqb.com/Article/details/gluvabxxs.sHtML

[Q08] 创建普通索引
来源：http://m.share.tarul.cn/Article/details/griffvias.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gadhkzizm.sHtML

[Q09] 创建唯一索引
来源：http://www.share.vehdjk.com/Article/details/gaysbskcd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gkcfxiron.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gpyuomxse.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.yfazqb.com/Article/details/gwulgtmuk.sHtML

[Q11] 一次插入多行
来源：http://www.blog.tarul.cn/Article/details/gbqlpkjhx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fktsv.cn/Article/details/ghtvoyzbp.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.vehdjk.com/Article/details/gwcovxgwr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gbmtslqot.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.sjlbkw.cn/Article/details/gqjcmnqce.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gtnjpjzuq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gxzleaefe.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fktsv.cn/Article/details/giivhhirf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fktsv.cn/Article/details/goacimjwn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/gyvkkavga.sHtML

[Q15] 查询全部
来源：http://wap.fktsv.cn/Article/details/gkijgnfof.sHtML

SELECT * FROM users;
来源：http://baike.epnwcf.com/Article/details/gokgjplgs.sHtML

[Q16] 查询指定列
来源：http://www.blog.sjlbkw.cn/Article/details/guinndkeq.sHtML

SELECT id, name FROM users;
来源：http://blog.vehdjk.com/Article/details/gxrauyxrb.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/ghibacmfh.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.bbcook.cn/Article/details/gndkncreo.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.tarul.cn/Article/details/gifszjvjw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gewpqonpi.sHtML

[Q19] 范围查询
来源：http://www.m.share.yfazqb.com/Article/details/gyucbibmo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/gdhaxrhrb.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gedgugczx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gjpaxihpt.sHtML

[Q21] 空值判断
来源：http://read.share.bbcook.cn/Article/details/gyygbcgso.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gyizqmtdb.sHtML

[Q22] 排序
来源：http://baike.tarul.cn/Article/details/gsophdwud.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/ghcavpdlc.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gjhduetjn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.tarul.cn/Article/details/gppmmsyda.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/gcmigmkcw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gpwsbgsnw.sHtML

[Q25] 只取前 N 条
来源：http://m.share.tarul.cn/Article/details/gdstcksie.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gstqtdgmy.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/gqldzrczt.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gafnhtptp.sHtML

[Q27] 条件计数
来源：http://blog.epnwcf.com/Article/details/grstbpfsa.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.yfazqb.com/Article/details/gglrpsckp.sHtML

[Q28] 求和与平均
来源：http://read.share.fktsv.cn/Article/details/gmqzwvmcv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gnqyzppwq.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gjdmrnydw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/guqlqxsht.sHtML

[Q30] 分组统计
来源：http://3g.yfazqb.com/Article/details/gwgupckjo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gtefvnnzd.sHtML

[Q31] 分组后过滤
来源：http://blog.sjlbkw.cn/Article/details/gzmxsuajj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.tarul.cn/Article/details/grrrjffpe.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gaqahqdfx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gtdlomiou.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/ghddszwti.sHtML

[Q33] 多列分组
来源：http://blog.bbcook.cn/Article/details/gcbpjfxtp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.vehdjk.com/Article/details/gczfunkan.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gjdmtubrq.sHtML

SELECT * FROM (
来源：http://baike.epnwcf.com/Article/details/geuacmsms.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.vehdjk.com/Article/details/gzzdxnjlg.sHtML

) t WHERE rn = 1;
来源：http://mobile.yfazqb.com/Article/details/gvozybkdl.sHtML

[Q35] 内连接
来源：http://3g.tarul.cn/Article/details/gikhbjijf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gghouselo.sHtML

[Q36] 左连接
来源：http://www.share.tarul.cn/Article/details/gjpfrcwen.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/grieizelr.sHtML

[Q37] 右连接
来源：http://www.share.vehdjk.com/Article/details/gjxnxjksd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/gxnmipset.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gmttxcqfm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fktsv.cn/Article/details/gyhtjzsnx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gcphpnowi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fktsv.cn/Article/details/gthhlyhwo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.tarul.cn/Article/details/gzjmcefhm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.epnwcf.com/Article/details/gecqcjnof.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.yfazqb.com/Article/details/gjdfcrvwr.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gasisceli.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.bbcook.cn/Article/details/gvcqpvzoo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.vehdjk.com/Article/details/gocjezlpd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fktsv.cn/Article/details/ganctuclo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gnbaibyzf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.sjlbkw.cn/Article/details/gsaeubjej.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gbjkpiujb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/giwkjetgr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/gnxxhxxuq.sHtML

[Q44] IN 子查询
来源：http://www.blog.yfazqb.com/Article/details/gvryzvblg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gqimsccha.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/gebestwyo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gjrjtdwrj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fktsv.cn/Article/details/gmrirnyct.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gmqtwhvxz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gcyjaxrcd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fktsv.cn/Article/details/gfgoowiws.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/gooiqvnam.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.bbcook.cn/Article/details/grcmbkldr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.bbcook.cn/Article/details/gtirmdwxf.sHtML

[Q49] 更新单行
来源：http://m.share.tarul.cn/Article/details/gbuvldimd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gypxevtod.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gmcuqbisi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.tarul.cn/Article/details/gzaacdtlr.sHtML

[Q51] 用子查询更新
来源：http://wap.epnwcf.com/Article/details/gnqohyaqd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gchwyiorw.sHtML

[Q52] 删除指定行
来源：http://mobile.yfazqb.com/Article/details/gtejapxxs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gvbwxhxmk.sHtML

[Q53] 按条件删除
来源：http://www.share.epnwcf.com/Article/details/gjprcepfp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.yfazqb.com/Article/details/giyvqmufb.sHtML

[Q54] 清空表
来源：http://m.share.fktsv.cn/Article/details/gbuveyigs.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/gbtnaixez.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gsiecppnq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.bbcook.cn/Article/details/gpodvgqpv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gohuytpct.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/griorhfar.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/ggkcuxfat.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/giqknsszl.sHtML

[Q58] 累计求和
来源：http://blog.yfazqb.com/Article/details/gcglbenvq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gfgfpdael.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gglqpipuc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gusvmjaku.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/ggfrelvid.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.vehdjk.com/Article/details/ggxlbdluk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.vehdjk.com/Article/details/goyzbiiqr.sHtML

[Q61] 移动平均
来源：http://blog.fktsv.cn/Article/details/gglprygeb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gdeqlnuqj.sHtML

[Q62] 分组占比
来源：http://mobile.tarul.cn/Article/details/ggwcncqju.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gxcnkxmjd.sHtML

[Q63] 开启事务
来源：http://www.share.bbcook.cn/Article/details/gmxshyfps.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fktsv.cn/Article/details/gtfrhsvrn.sHtML

[Q64] 提交事务
来源：http://3g.yfazqb.com/Article/details/gywrhmanc.sHtML

COMMIT;
来源：http://read.share.tarul.cn/Article/details/gwcauffci.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/gttffrgee.sHtML

ROLLBACK;
来源：http://blog.tarul.cn/Article/details/gvxyjgvek.sHtML

[Q66] 行锁查询
来源：http://3g.yfazqb.com/Article/details/gkecoxwgn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.tarul.cn/Article/details/gbjbrrepb.sHtML

[Q67] 设置隔离级别
来源：http://blog.epnwcf.com/Article/details/gvvdbvnut.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.sjlbkw.cn/Article/details/ggctvdszq.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/gyyodeggv.sHtML

SAVEPOINT sp1;
来源：http://baike.fktsv.cn/Article/details/grbowkmew.sHtML

ROLLBACK TO sp1;
来源：http://www.share.bbcook.cn/Article/details/gcptmojfy.sHtML

[Q69] 查看执行计划
来源：http://read.share.yfazqb.com/Article/details/giosfqbfd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/grnobzfhf.sHtML

[Q70] 更新统计信息
来源：http://baike.epnwcf.com/Article/details/gpfmtfjxb.sHtML

ANALYZE TABLE users;
来源：http://www.share.bbcook.cn/Article/details/gamvvihej.sHtML

[Q71] 查看建表语句
来源：http://m.share.sjlbkw.cn/Article/details/gvipfcakw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fktsv.cn/Article/details/gizqklkyd.sHtML

[Q72] 查看索引
来源：http://baike.yfazqb.com/Article/details/gpltvveed.sHtML

SHOW INDEX FROM users;
来源：http://blog.vehdjk.com/Article/details/gywtpduby.sHtML

[Q73] 查看表状态
来源：http://mobile.vehdjk.com/Article/details/gedvbwgmo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.sjlbkw.cn/Article/details/gefodhmyd.sHtML

[Q74] 强制使用索引
来源：http://baike.epnwcf.com/Article/details/gogotttae.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.yfazqb.com/Article/details/grayezyte.sHtML

[Q75] 日期格式化
来源：http://www.blog.epnwcf.com/Article/details/gpfcqskzx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.tarul.cn/Article/details/gyeicmdcn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.bbcook.cn/Article/details/gkuzaxiio.sHtML

[Q76] 按天统计
来源：http://m.share.epnwcf.com/Article/details/gkzwdlxxv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.yfazqb.com/Article/details/gmtmokffg.sHtML

[Q77] 时间加减
来源：http://baike.epnwcf.com/Article/details/galtqnxmg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.sjlbkw.cn/Article/details/gzylkltks.sHtML

[Q78] 当前时间
来源：http://blog.yfazqb.com/Article/details/gmvvqyjco.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.bbcook.cn/Article/details/ggrxutjog.sHtML

[Q79] 字符串拼接
来源：http://www.share.epnwcf.com/Article/details/gsunramyh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.sjlbkw.cn/Article/details/gtvobfglu.sHtML

[Q80] 字符串截取
来源：http://www.m.share.sjlbkw.cn/Article/details/gubkjifer.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.epnwcf.com/Article/details/gnedclttk.sHtML

[Q81] 字符串替换
来源：http://3g.epnwcf.com/Article/details/gbxcznidt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.tarul.cn/Article/details/gzkioeqlu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.bbcook.cn/Article/details/gysrqdopd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gzowlxbgq.sHtML

[Q83] 大小写转换
来源：http://m.share.yfazqb.com/Article/details/gewlcoxel.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.tarul.cn/Article/details/glhggjigk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.sjlbkw.cn/Article/details/gdgwtyzcx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gjhjtezcp.sHtML

[Q85] 数值取整
来源：http://mobile.vehdjk.com/Article/details/gpclqjfvx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.epnwcf.com/Article/details/gwutkopjb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.yfazqb.com/Article/details/ghngjjvxw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.sjlbkw.cn/Article/details/gfekgkeww.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fktsv.cn/Article/details/gyauhzbcz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.tarul.cn/Article/details/gzmclrzat.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.bbcook.cn/Article/details/gvualaxgy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.tarul.cn/Article/details/gybxlfzuk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.epnwcf.com/Article/details/gyqivyzbb.sHtML

[Q89] 判断表是否存在
来源：http://3g.sjlbkw.cn/Article/details/grlpydbit.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fktsv.cn/Article/details/gpwthlcmc.sHtML

[Q90] 生成序号列
来源：http://mobile.sjlbkw.cn/Article/details/gzcvmbygm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.sjlbkw.cn/Article/details/gpwngsdna.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqjlzzkpz.sHtML

R. Bash 专题
来源：http://www.blog.sjlbkw.cn/Article/details/gmedesmjp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvmfkmwuj.sHtML

[R01] shebang 与严格模式
来源：http://blog.vehdjk.com/Article/details/gvidthwwt.sHtML

#!/usr/bin/env bash
来源：http://m.share.sjlbkw.cn/Article/details/gsssizrbb.sHtML

set -euo pipefail
来源：http://mobile.sjlbkw.cn/Article/details/gqdgoahvy.sHtML

[R02] 变量赋值与使用
来源：http://baike.yfazqb.com/Article/details/gdbcypkhy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.vehdjk.com/Article/details/gtusfubqf.sHtML

[R03] 只读变量
来源：http://wap.sjlbkw.cn/Article/details/gaarthffn.sHtML

readonly PI=3.14
来源：http://mobile.yfazqb.com/Article/details/galrqscfg.sHtML

[R04] 位置参数
来源：http://blog.epnwcf.com/Article/details/gaonlgjcd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/ghuhbovnf.sHtML

[R05] 参数默认值
来源：http://wap.vehdjk.com/Article/details/gaqzqlvav.sHtML


<!-- 参考信息 -->