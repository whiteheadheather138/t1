代发 wailian999

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gtqhgxvyw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.bbcook.cn/Article/details/gggwtkfla.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gtdxixqgx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.sjlbkw.cn/Article/details/giaupwrcp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/ggekjbkud.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.epnwcf.com/Article/details/gnlvnbxdo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.yfazqb.com/Article/details/gzsupuafc.sHtML

Ruby: // fork 块
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkygbyxc.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gijbfceaa.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gcafbgifn.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/gpzymffeu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gdobipvql.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gliuqbrbg.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.vehdjk.com/Article/details/gjlythdnn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/gwwedytwe.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.vehdjk.com/Article/details/gfsxaogrp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gatkkuhzx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.yfazqb.com/Article/details/glqicigdd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gpizqkctu.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gigjqtfpk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/gkslprbjp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gjwbrbblu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.yfazqb.com/Article/details/gyyvdzjzn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/grorlpnqa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gqopvyfat.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/gpcwslrtb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/gtgwbydks.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.bbcook.cn/Article/details/gqcotjumv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gproyzuxm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gpiaurrjs.sHtML

[P03] 生成短随机字符串
来源：http://baike.epnwcf.com/Article/details/gjbqibgld.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.epnwcf.com/Article/details/gqlnixwdx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/goomocoeo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/giszatfyb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gjwvfdxha.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/gqvnlpmyr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/gebzvqrhm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gxkmgsifq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gzvarfntf.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gqccuueew.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gadpqhdmv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gscqugqpx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fktsv.cn/Article/details/gbehpicim.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/gzdfrkrzr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gjzcxhihj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gvaogcmqj.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/gwjtzavyq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gwkfhsffn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gpwntevoc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.tarul.cn/Article/details/gkjyxuevg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.sjlbkw.cn/Article/details/gfjnaugni.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.epnwcf.com/Article/details/gzochvgod.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/gdnsjsuuz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gxrvqqckg.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/ginlackwt.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gbkmxnwtf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.yfazqb.com/Article/details/gvyruyxqq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gvnprptjb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.fktsv.cn/Article/details/gejebxwyk.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gvzuepxfm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.epnwcf.com/Article/details/gmxggxpjj.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gqagchumi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gdckxnqxl.sHtML

Go:   if x == nil {}
来源：http://mobile.bbcook.cn/Article/details/gfhjitstn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.vehdjk.com/Article/details/gkkoheozd.sHtML

C#:   if (x is null) {}
来源：http://baike.tarul.cn/Article/details/grpsciiaz.sHtML

[P07] 防抖与节流
来源：http://read.share.epnwcf.com/Article/details/gbezzoxtr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gokfskhyp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gosmkecyc.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gupdntbuj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gapykublo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gopaayyvw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/gmwxsytgh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/glrignxfl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.tarul.cn/Article/details/gwnmtqfoz.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gbctkieiy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/gszsaaquv.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gqfyqedky.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.epnwcf.com/Article/details/grumnqdko.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gyveabrxj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/gxwscrrrl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gmcdfncgr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.vehdjk.com/Article/details/gaaqfzfxy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gdtevdmxs.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/glfuabvll.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gxcjmsaym.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/giwfdidts.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gocvbmdbj.sHtML

CREATE TABLE users (
来源：http://wap.bbcook.cn/Article/details/gvofnqxul.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.vehdjk.com/Article/details/gtncisygx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gajdhsicv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.vehdjk.com/Article/details/gsjmtwapv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gjdruixtz.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gqffqmagl.sHtML

[Q02] 创建带外键的表
来源：http://www.share.tarul.cn/Article/details/gzekpfwbi.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gyagryhpd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gaqqlvknj.sHtML

user_id INT NOT NULL,
来源：http://m.share.epnwcf.com/Article/details/gujxbihgs.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.tarul.cn/Article/details/gsngvzmps.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gotrovryb.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/glvojpbcs.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/geqhevopi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fktsv.cn/Article/details/gfuvvdlzh.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/gqwbdfgia.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.vehdjk.com/Article/details/gdiwcmgez.sHtML

[Q05] 重命名列
来源：http://3g.sjlbkw.cn/Article/details/gvaqowaqr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gdpyzqfed.sHtML

[Q06] 删除列
来源：http://wap.yfazqb.com/Article/details/glknwskhu.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.vehdjk.com/Article/details/gifylzflm.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/gswyoyizj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.bbcook.cn/Article/details/gbmxvjfqm.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gnhkugtfb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/glntiglte.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gbimenzql.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.vehdjk.com/Article/details/gferymakq.sHtML

[Q10] 插入单行
来源：http://3g.bbcook.cn/Article/details/gaqswpbbg.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gholxpdqv.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gcqqfcwwb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gdwriswud.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.tarul.cn/Article/details/gpyvuikvy.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/gdqueobvc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.yfazqb.com/Article/details/gsjjvmfve.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gegopkboj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gjkruadbr.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.sjlbkw.cn/Article/details/gzbuzkzrx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.sjlbkw.cn/Article/details/gmygbslnb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/gfkubsplt.sHtML

[Q15] 查询全部
来源：http://baike.epnwcf.com/Article/details/gqmzcylvp.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gfphfgbvx.sHtML

[Q16] 查询指定列
来源：http://baike.fktsv.cn/Article/details/gahbguzgu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gxwkhyzhq.sHtML

[Q17] 条件查询
来源：http://m.share.vehdjk.com/Article/details/gmychodbk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.yfazqb.com/Article/details/gogkpwcst.sHtML

[Q18] 模糊匹配
来源：http://www.blog.yfazqb.com/Article/details/ghydurdma.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gppllbpae.sHtML

[Q19] 范围查询
来源：http://blog.fktsv.cn/Article/details/gxhqxalty.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fktsv.cn/Article/details/gzwvydoib.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/ggccvqptp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.tarul.cn/Article/details/gyzaaqxtz.sHtML

[Q21] 空值判断
来源：http://www.m.share.yfazqb.com/Article/details/gzklhdosp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.epnwcf.com/Article/details/gdnqkcemv.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gbisbzqoe.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fktsv.cn/Article/details/gpautahsw.sHtML

[Q23] 分页
来源：http://blog.fktsv.cn/Article/details/gvdldnydi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gvemorwrj.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/gylqbctey.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gkcdhhcrd.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fktsv.cn/Article/details/gtnfapksp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gvpicmvni.sHtML

[Q26] 计数
来源：http://wap.sjlbkw.cn/Article/details/gtsqlzszm.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gaeuyadad.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/ghnahibor.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/gkrvurxhj.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gsorpyvsc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/ggxcwsuwq.sHtML

[Q29] 最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gejpelvsx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvhoqqreh.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gjtgqkkao.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gdobqdscw.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gnkzsbpsg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.yfazqb.com/Article/details/gmzctzrpb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.epnwcf.com/Article/details/gtzylfoph.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gzryajzpl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.bbcook.cn/Article/details/gpxaqdueo.sHtML

[Q33] 多列分组
来源：http://wap.bbcook.cn/Article/details/gkpjlxjtc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.yfazqb.com/Article/details/gnatthhwy.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/gldcpjdqc.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/ghklajiid.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.sjlbkw.cn/Article/details/gyhvuedmv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gponbvmuu.sHtML

[Q35] 内连接
来源：http://www.m.share.vehdjk.com/Article/details/gqfwfmoul.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gpdzshbna.sHtML

[Q36] 左连接
来源：http://mobile.tarul.cn/Article/details/gfqsijgto.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gnoqikzzw.sHtML

[Q37] 右连接
来源：http://baike.sjlbkw.cn/Article/details/gapmqlqwr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gembeyaju.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.tarul.cn/Article/details/gjyerrbnz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.vehdjk.com/Article/details/goumqebsn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.tarul.cn/Article/details/ggtrvratn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gwarldlje.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.sjlbkw.cn/Article/details/gtknfrbiu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gydepojae.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.tarul.cn/Article/details/gcmxljvup.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gpbexkyzu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fktsv.cn/Article/details/giqyfnhxo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.sjlbkw.cn/Article/details/gluauwaij.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/gfbtnlsij.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gbzhwumrd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.vehdjk.com/Article/details/gemdznres.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.vehdjk.com/Article/details/gesnbxjex.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/grvjuofzi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/gjdiyxags.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/guzpcocrc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fktsv.cn/Article/details/geskenufj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.bbcook.cn/Article/details/gjftkpbhb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gglwbkvfa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/glgjgvwve.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gwhlvwoql.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gjdzvhmat.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.epnwcf.com/Article/details/gkhufxmwq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gznhzgmoz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.bbcook.cn/Article/details/gkjvzhzmp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.yfazqb.com/Article/details/ghyyxevfa.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/gowumbwtr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/gnuqgupkf.sHtML

[Q50] 批量更新
来源：http://3g.tarul.cn/Article/details/ggjndymlx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.bbcook.cn/Article/details/giwkmzyyr.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gufwuetlc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gdvmqdrzu.sHtML

[Q52] 删除指定行
来源：http://baike.vehdjk.com/Article/details/gxupgkqcs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.tarul.cn/Article/details/gfweuxafp.sHtML

[Q53] 按条件删除
来源：http://m.share.vehdjk.com/Article/details/gblacrakr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gmssnraoe.sHtML

[Q54] 清空表
来源：http://www.blog.vehdjk.com/Article/details/gjvojxgsb.sHtML

TRUNCATE TABLE logs;
来源：http://wap.sjlbkw.cn/Article/details/gdkgetnql.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gtumwhvxg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fktsv.cn/Article/details/gthgorsst.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gbpumpxku.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.yfazqb.com/Article/details/gweenbozw.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gizmllirh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.tarul.cn/Article/details/gxfvrqqbn.sHtML

[Q58] 累计求和
来源：http://wap.vehdjk.com/Article/details/gcgzjovkm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gnkaefqts.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/gymroculr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gbwkirulx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.yfazqb.com/Article/details/gmewvtjqd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.sjlbkw.cn/Article/details/gktdcxttp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gaonyzrvb.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/ghbuuogfr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gopkcosxa.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/gxvvzqokx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gtrfrpxlj.sHtML

[Q63] 开启事务
来源：http://www.share.yfazqb.com/Article/details/gfeuepvyw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gzweqvzxg.sHtML

[Q64] 提交事务
来源：http://wap.vehdjk.com/Article/details/gcsixdtva.sHtML

COMMIT;
来源：http://wap.epnwcf.com/Article/details/gsjcozabi.sHtML

[Q65] 回滚事务
来源：http://read.share.vehdjk.com/Article/details/gkbtyrypt.sHtML

ROLLBACK;
来源：http://mobile.vehdjk.com/Article/details/gixhikdir.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gvvpkslwh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fktsv.cn/Article/details/geongwevd.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gzihsytnq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.tarul.cn/Article/details/gssuhepep.sHtML

[Q68] 保存点
来源：http://www.share.vehdjk.com/Article/details/gnllxubul.sHtML

SAVEPOINT sp1;
来源：http://www.blog.epnwcf.com/Article/details/glrbittmu.sHtML

ROLLBACK TO sp1;
来源：http://wap.epnwcf.com/Article/details/ggbplmbgk.sHtML

[Q69] 查看执行计划
来源：http://read.share.sjlbkw.cn/Article/details/glwxhbgzi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.sjlbkw.cn/Article/details/grvalsekr.sHtML

[Q70] 更新统计信息
来源：http://www.blog.bbcook.cn/Article/details/ggxkykhrb.sHtML

ANALYZE TABLE users;
来源：http://m.share.vehdjk.com/Article/details/gbajucmrs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gpbqxkrxk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.tarul.cn/Article/details/gqnyopwqq.sHtML

[Q72] 查看索引
来源：http://www.m.share.bbcook.cn/Article/details/genpgzajy.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gwdccixoy.sHtML

[Q73] 查看表状态
来源：http://m.share.vehdjk.com/Article/details/gixjgczox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fktsv.cn/Article/details/gmcyytvqx.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gbnodbwbd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.epnwcf.com/Article/details/giwnycsom.sHtML

[Q75] 日期格式化
来源：http://read.share.fktsv.cn/Article/details/gffhwylgx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gyonxtbdp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.epnwcf.com/Article/details/guegeikrz.sHtML

[Q76] 按天统计
来源：http://baike.fktsv.cn/Article/details/giacambpr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.tarul.cn/Article/details/glqczthqy.sHtML

[Q77] 时间加减
来源：http://wap.epnwcf.com/Article/details/gpwjbsigf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gatcfyhbs.sHtML

[Q78] 当前时间
来源：http://www.m.share.bbcook.cn/Article/details/gnmmwcgde.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.sjlbkw.cn/Article/details/gdbcaeejz.sHtML

[Q79] 字符串拼接
来源：http://m.share.sjlbkw.cn/Article/details/gzfxtoezn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.epnwcf.com/Article/details/gtkprwwbv.sHtML

[Q80] 字符串截取
来源：http://3g.bbcook.cn/Article/details/grydiweim.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gqtdzbrvn.sHtML

[Q81] 字符串替换
来源：http://www.share.bbcook.cn/Article/details/gzwpxufwh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.yfazqb.com/Article/details/gkdcwxysm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.sjlbkw.cn/Article/details/guoycelgx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gjeuiconi.sHtML

[Q83] 大小写转换
来源：http://read.share.tarul.cn/Article/details/glwmlffyy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gkpmrqfsm.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gsoyrhfiy.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.yfazqb.com/Article/details/gzntfuvor.sHtML

[Q85] 数值取整
来源：http://www.blog.fktsv.cn/Article/details/gocpkzgft.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.yfazqb.com/Article/details/gxgjgjehr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.tarul.cn/Article/details/gktguqzio.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmgiobxl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.sjlbkw.cn/Article/details/gfokkkntl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.tarul.cn/Article/details/ggdxyctbm.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.yfazqb.com/Article/details/gbmjngyap.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.sjlbkw.cn/Article/details/goxqloocx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.yfazqb.com/Article/details/gwpuotkuz.sHtML

[Q89] 判断表是否存在
来源：http://blog.fktsv.cn/Article/details/gkfcwuvuc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.epnwcf.com/Article/details/groirvpvy.sHtML

[Q90] 生成序号列
来源：http://baike.tarul.cn/Article/details/gulprcixq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.sjlbkw.cn/Article/details/gtrtnvkwe.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gqykiajgb.sHtML

R. Bash 专题
来源：http://read.share.bbcook.cn/Article/details/ggptzszzr.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzymttjnj.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.vehdjk.com/Article/details/glylaasoy.sHtML

#!/usr/bin/env bash
来源：http://m.share.tarul.cn/Article/details/gfmsmqbxt.sHtML

set -euo pipefail
来源：http://3g.vehdjk.com/Article/details/ghaqrukge.sHtML

[R02] 变量赋值与使用
来源：http://www.share.yfazqb.com/Article/details/giismkiwr.sHtML

name="Tom"; echo "$name"
来源：http://mobile.yfazqb.com/Article/details/gkadacdpv.sHtML

[R03] 只读变量
来源：http://www.share.tarul.cn/Article/details/gjpogqkon.sHtML


<!-- 参考信息 -->