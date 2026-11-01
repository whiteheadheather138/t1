代发 wailian999

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gppangcoe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gvxwfexyt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/grdykcach.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gfyoweejf.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gwjvtnuyh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gbjmqfimh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gegoccrdr.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gamrmqtqb.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/gopnltijl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmcmhsyjm.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gsgrqtoof.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/guehgrusk.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/gpcbesdhg.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gekzsagcb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gfdvwixuv.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gigcswvbs.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.sjlbkw.cn/Article/details/gytfcilyx.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fktsv.cn/Article/details/giwkhtnic.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.tarul.cn/Article/details/gugnpqhev.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gytfbiljz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gyfhzuvsk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gxcphxlcf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gzctdmjbu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gkmsvjega.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.bbcook.cn/Article/details/gaymcvkux.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.epnwcf.com/Article/details/gwnvroqsh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gfysjrzdq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/ghrkzccqv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/glfvfajls.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fktsv.cn/Article/details/gtkkhapau.sHtML

[P03] 生成短随机字符串
来源：http://wap.bbcook.cn/Article/details/gglqpqsvs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.vehdjk.com/Article/details/gusliqfuu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/gvchrazql.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gewpaxiiv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gydcgvdcc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.vehdjk.com/Article/details/gmweyfoig.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gexbbovuv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.yfazqb.com/Article/details/gfscrovfd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.epnwcf.com/Article/details/gbuqzkbwm.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gqsaffrvg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gzuhzpoxc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gkexhryrf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gpgmrqwiw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/gfjnblipw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gobzymulq.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gadphhvhj.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gtbmcexjt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/gkossdimy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.epnwcf.com/Article/details/gqvimmohp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gbwapezwq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gsbfizjex.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gphlfujqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.tarul.cn/Article/details/ghfftytnd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/gsrxyturm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gsfjdlwkl.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/gvueuosqw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gadvniiku.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/grymshsrk.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gdjvabril.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gnjtosjzy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.tarul.cn/Article/details/gyaiizttt.sHtML

TS:   if (x == null) {}
来源：http://www.share.tarul.cn/Article/details/goixjjngb.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.bbcook.cn/Article/details/ghvgxgzke.sHtML

Go:   if x == nil {}
来源：http://www.m.share.epnwcf.com/Article/details/ggbznmqra.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.bbcook.cn/Article/details/gpkqytmzk.sHtML

C#:   if (x is null) {}
来源：http://baike.vehdjk.com/Article/details/geenfyjae.sHtML

[P07] 防抖与节流
来源：http://m.share.yfazqb.com/Article/details/gfyimrfyp.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.vehdjk.com/Article/details/gkhtwixpu.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/ghsjensab.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gbzcdjifp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.yfazqb.com/Article/details/gbfazhxmi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.bbcook.cn/Article/details/gvoabpmmy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/grrchattm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.yfazqb.com/Article/details/glrkgrusn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gathnppck.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gsbqsebke.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gmwuxjmrw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/gednkdltr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/gjcmblcwr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.sjlbkw.cn/Article/details/gahgbtrfe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/ggwivurkm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.vehdjk.com/Article/details/gypybkkxj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gzefiobvr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gwlzovagi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gunibunta.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.bbcook.cn/Article/details/gxwmqtglg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gqhunstej.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gcrxrgpbr.sHtML

CREATE TABLE users (
来源：http://mobile.epnwcf.com/Article/details/gqxxrafqv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.sjlbkw.cn/Article/details/gbcuaxhda.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gjdgdmvzt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gouqwfott.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/gifyoamck.sHtML

);
来源：http://www.m.share.bbcook.cn/Article/details/gixevdgdf.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/goynfquhx.sHtML

CREATE TABLE orders (
来源：http://blog.vehdjk.com/Article/details/ggnljbsgr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gsyczmfqc.sHtML

user_id INT NOT NULL,
来源：http://baike.tarul.cn/Article/details/grlfocenh.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.vehdjk.com/Article/details/gdchkfshx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gvpfutfzp.sHtML

);
来源：http://mobile.tarul.cn/Article/details/gtybacfrk.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gmaznxhdt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gqkzlxlvi.sHtML

[Q04] 修改列类型
来源：http://3g.sjlbkw.cn/Article/details/glmqphdyt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.tarul.cn/Article/details/galchokvl.sHtML

[Q05] 重命名列
来源：http://mobile.epnwcf.com/Article/details/gwunyyhpt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.bbcook.cn/Article/details/gstshcvas.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gayufdpsd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.bbcook.cn/Article/details/gftgsqooj.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gxgbsiome.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.epnwcf.com/Article/details/gcmyhvmvp.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/gfcfwvtjw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/gpeazycgf.sHtML

[Q09] 创建唯一索引
来源：http://3g.epnwcf.com/Article/details/gzeqfvjaf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gqubfqrvk.sHtML

[Q10] 插入单行
来源：http://wap.vehdjk.com/Article/details/gecvstkpj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.bbcook.cn/Article/details/gkcffezwz.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/geeicqbum.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gyiiirjls.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gwhqdxmmr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gpsrhiiwx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fktsv.cn/Article/details/gasoznofb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.bbcook.cn/Article/details/ggkettwda.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/gfadrqywe.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/ghlpcbagp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.sjlbkw.cn/Article/details/gdtxghkxm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.bbcook.cn/Article/details/gpovgfhps.sHtML

[Q15] 查询全部
来源：http://3g.vehdjk.com/Article/details/gzvgjxeam.sHtML

SELECT * FROM users;
来源：http://m.share.tarul.cn/Article/details/gvndwvkvv.sHtML

[Q16] 查询指定列
来源：http://mobile.tarul.cn/Article/details/gvkgcrina.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/gnnilalik.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/gvulgfeio.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/glrlhqnah.sHtML

[Q18] 模糊匹配
来源：http://read.share.tarul.cn/Article/details/gsqfvfaig.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/grxpulwpk.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/gckktvarr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/grwtgwagi.sHtML

[Q20] IN 列表
来源：http://mobile.yfazqb.com/Article/details/gyyhvbtwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gfeqxzems.sHtML

[Q21] 空值判断
来源：http://read.share.yfazqb.com/Article/details/gpjlucfrp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gnjdhtecu.sHtML

[Q22] 排序
来源：http://wap.tarul.cn/Article/details/ggzrcmtlj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fktsv.cn/Article/details/gxvwoeqoh.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/guzctvcui.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.sjlbkw.cn/Article/details/goreufqsz.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/geiktgdij.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gbymeestu.sHtML

[Q25] 只取前 N 条
来源：http://www.share.vehdjk.com/Article/details/gnzquyuvx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.sjlbkw.cn/Article/details/ghdsxkiat.sHtML

[Q26] 计数
来源：http://wap.epnwcf.com/Article/details/grazewcdw.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gsxknpsiq.sHtML

[Q27] 条件计数
来源：http://blog.vehdjk.com/Article/details/gymqjumkp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvbgywnzv.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/geyklnufb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.vehdjk.com/Article/details/ggroznhpp.sHtML

[Q29] 最大最小值
来源：http://read.share.fktsv.cn/Article/details/geiktcsnl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gxzimeobc.sHtML

[Q30] 分组统计
来源：http://read.share.tarul.cn/Article/details/gyuihrsom.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/grqvicjqr.sHtML

[Q31] 分组后过滤
来源：http://baike.vehdjk.com/Article/details/grtkghsam.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gdwmabixc.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/glnqwmksi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gpjlkbkda.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.tarul.cn/Article/details/gaklcbbrz.sHtML

[Q33] 多列分组
来源：http://www.share.bbcook.cn/Article/details/gjonblxrt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/ghttnfxkk.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gafpmhpzz.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/getbzkfpz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/gdsxlnakh.sHtML

) t WHERE rn = 1;
来源：http://read.share.epnwcf.com/Article/details/grudtianv.sHtML

[Q35] 内连接
来源：http://www.blog.tarul.cn/Article/details/gofotbzns.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gopgdyipw.sHtML

[Q36] 左连接
来源：http://m.share.sjlbkw.cn/Article/details/gsqnpgdja.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gvfifznic.sHtML

[Q37] 右连接
来源：http://m.share.yfazqb.com/Article/details/gmnadbmke.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.yfazqb.com/Article/details/gdmckiwjj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fktsv.cn/Article/details/gjbqikfmr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fktsv.cn/Article/details/gmdmgexqk.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.epnwcf.com/Article/details/ggojzdmco.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fktsv.cn/Article/details/ghsnzndpd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fktsv.cn/Article/details/gwtihajrm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/gdiwnbbcr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/gavjipsvy.sHtML

[Q41] 多表连接
来源：http://baike.fktsv.cn/Article/details/gzsrhuilv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fktsv.cn/Article/details/gwdemjpik.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gyocuskhg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gakpgieum.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.sjlbkw.cn/Article/details/gvoyrwijz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gpjoranwr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/giqeohkvk.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gxqlameri.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gcwgrybzo.sHtML

[Q44] IN 子查询
来源：http://www.share.fktsv.cn/Article/details/gpjpkfvpr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/gusrmvkrk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.tarul.cn/Article/details/guuijngha.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.bbcook.cn/Article/details/gzfjwsvug.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/goldqsatc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/guknivxzo.sHtML

[Q47] 与平均值比较
来源：http://www.blog.sjlbkw.cn/Article/details/ggjmoxnhe.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/gmtkcsmnn.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gifhffxxd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.vehdjk.com/Article/details/gbdfoptmm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gkaofbgcf.sHtML

[Q49] 更新单行
来源：http://www.blog.bbcook.cn/Article/details/guyjayudl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/glskmrwjb.sHtML

[Q50] 批量更新
来源：http://www.blog.epnwcf.com/Article/details/gpecfquhz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gsudjwgbd.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gmdtbaixg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.yfazqb.com/Article/details/gnqhyysvy.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/ggljwmgyo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/gmysxgcbi.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gszzcuimb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.epnwcf.com/Article/details/gnndobbse.sHtML

[Q54] 清空表
来源：http://wap.vehdjk.com/Article/details/ghfqwykac.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.tarul.cn/Article/details/gfhaiymtv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fktsv.cn/Article/details/gldtnxwor.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gywrtqwze.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbdniauu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.vehdjk.com/Article/details/gdhsvyttm.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gbdftnqdm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.epnwcf.com/Article/details/gsnjmfukr.sHtML

[Q58] 累计求和
来源：http://www.m.share.bbcook.cn/Article/details/gcsishhyk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gyfuzuqvp.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gqonnfrgx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gufylurzl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.tarul.cn/Article/details/gvxrhtyxi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/ghqvrbmwe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gjbvenirc.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gdvjmdopz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gtacprzbm.sHtML

[Q62] 分组占比
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjuqygan.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gasosqeaf.sHtML

[Q63] 开启事务
来源：http://www.share.fktsv.cn/Article/details/gbogvsgxe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/gcximhhmn.sHtML

[Q64] 提交事务
来源：http://mobile.epnwcf.com/Article/details/gssryvwci.sHtML

COMMIT;
来源：http://www.share.vehdjk.com/Article/details/gxxcocxdr.sHtML

[Q65] 回滚事务
来源：http://mobile.sjlbkw.cn/Article/details/gqtbousgx.sHtML

ROLLBACK;
来源：http://www.share.bbcook.cn/Article/details/goakfbuep.sHtML

[Q66] 行锁查询
来源：http://www.blog.vehdjk.com/Article/details/gejvvicau.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.bbcook.cn/Article/details/grkkyxqyg.sHtML

[Q67] 设置隔离级别
来源：http://baike.yfazqb.com/Article/details/gyhycxmjx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/gnnbjmogr.sHtML

[Q68] 保存点
来源：http://www.share.yfazqb.com/Article/details/grbkmqczo.sHtML

SAVEPOINT sp1;
来源：http://read.share.sjlbkw.cn/Article/details/gjfgtaiba.sHtML

ROLLBACK TO sp1;
来源：http://blog.bbcook.cn/Article/details/gsfabnjju.sHtML

[Q69] 查看执行计划
来源：http://baike.bbcook.cn/Article/details/goufvqlql.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.bbcook.cn/Article/details/ggholcocm.sHtML

[Q70] 更新统计信息
来源：http://baike.tarul.cn/Article/details/gtnrpimiw.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmkorprkj.sHtML

[Q71] 查看建表语句
来源：http://m.share.tarul.cn/Article/details/ggmkjnuip.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.bbcook.cn/Article/details/gtqaznemu.sHtML

[Q72] 查看索引
来源：http://read.share.yfazqb.com/Article/details/gvxrlpfre.sHtML

SHOW INDEX FROM users;
来源：http://wap.tarul.cn/Article/details/gaepvjbsn.sHtML

[Q73] 查看表状态
来源：http://m.share.fktsv.cn/Article/details/glqrodody.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gnjnqqrjc.sHtML

[Q74] 强制使用索引
来源：http://3g.sjlbkw.cn/Article/details/gcvqllxbw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/gdbtbimoh.sHtML

[Q75] 日期格式化
来源：http://wap.vehdjk.com/Article/details/guwygamyx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gssgmezcf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.bbcook.cn/Article/details/grguuorbn.sHtML

[Q76] 按天统计
来源：http://baike.tarul.cn/Article/details/gzpxozudw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fktsv.cn/Article/details/gvcdttohr.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/gwenfcbfj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.epnwcf.com/Article/details/gasltmoce.sHtML

[Q78] 当前时间
来源：http://read.share.yfazqb.com/Article/details/gdordwlmf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gxpuhkjet.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gsksvwdcj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.tarul.cn/Article/details/gpkuornzz.sHtML

[Q80] 字符串截取
来源：http://mobile.tarul.cn/Article/details/glqoilpqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.yfazqb.com/Article/details/gpesdvgqa.sHtML

[Q81] 字符串替换
来源：http://mobile.bbcook.cn/Article/details/gnhpymjpn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gdjojmwqn.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.epnwcf.com/Article/details/gfqjlegcd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gcrlrvmdk.sHtML

[Q83] 大小写转换
来源：http://3g.bbcook.cn/Article/details/gqdhmfojo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gjzlbafol.sHtML

[Q84] 去除首尾空格
来源：http://wap.fktsv.cn/Article/details/gjxiaucfd.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gmhfkgrsx.sHtML

[Q85] 数值取整
来源：http://www.m.share.sjlbkw.cn/Article/details/ggbwuojel.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.tarul.cn/Article/details/goceolism.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.vehdjk.com/Article/details/gqyxlpeab.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.yfazqb.com/Article/details/gcqrmmewy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.tarul.cn/Article/details/gcrhylbne.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.epnwcf.com/Article/details/gfifboqws.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.bbcook.cn/Article/details/gvoafvkmr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/gbvahrenu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.yfazqb.com/Article/details/gfqcrqyhv.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fktsv.cn/Article/details/gnzkklbni.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.bbcook.cn/Article/details/gpblasxnw.sHtML

[Q90] 生成序号列
来源：http://3g.tarul.cn/Article/details/gvcduenct.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.bbcook.cn/Article/details/gapqqfzjq.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gutqzdgyx.sHtML

R. Bash 专题
来源：http://www.m.share.sjlbkw.cn/Article/details/gyqpatouh.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glketuahy.sHtML

[R01] shebang 与严格模式
来源：http://wap.bbcook.cn/Article/details/gunilqcbo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fktsv.cn/Article/details/ghwadpeos.sHtML

set -euo pipefail
来源：http://mobile.fktsv.cn/Article/details/geddpawyr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.yfazqb.com/Article/details/griahsqrl.sHtML

name="Tom"; echo "$name"
来源：http://m.share.tarul.cn/Article/details/gguirhdor.sHtML

[R03] 只读变量
来源：http://www.blog.yfazqb.com/Article/details/gabenevui.sHtML


<!-- 参考信息 -->