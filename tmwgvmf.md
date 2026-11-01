代发 wailian999

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/ggbgpwhgc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/goqceredh.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.bbcook.cn/Article/details/glzzlntdt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.bbcook.cn/Article/details/gedwbyysj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/ggkdkaoki.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gbskqdxfy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gseabkkmn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gznnvjdey.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/ggcczmapm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/ggbeuhgyq.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/gkspathen.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/geqyetkel.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.sjlbkw.cn/Article/details/gjtgrenxa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gmqsxhtck.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gviplzrea.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.tarul.cn/Article/details/gbinnfmpz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.tarul.cn/Article/details/gajgzaiqx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.epnwcf.com/Article/details/gajfpvwmn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/greostprc.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/glpkngdpf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gmuinlwdo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.yfazqb.com/Article/details/gepjmwuxg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/grthobniw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gfgcvxziy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.bbcook.cn/Article/details/gfyhqbjir.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gfuulkucl.sHtML

Ruby: x.length;  x.size
来源：http://www.share.epnwcf.com/Article/details/gbedfnywu.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/gfzqbgbrl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gbyvxldlw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.bbcook.cn/Article/details/gohvrgllr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.yfazqb.com/Article/details/guzngrqfh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.vehdjk.com/Article/details/gjtllvzlt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gvxpjahhz.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.tarul.cn/Article/details/gxjnxfbar.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gowmxfzue.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gbtzmnpaz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/guynodcxm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fktsv.cn/Article/details/gqtsygufu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gvmuzlkab.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/gykaxwsxc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.epnwcf.com/Article/details/gglkcsebq.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gqrqmvocn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.vehdjk.com/Article/details/glqbakrgi.sHtML

Go:   if x == nil {}
来源：http://www.blog.epnwcf.com/Article/details/gqrllzcem.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gnghrhijc.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gszrssitv.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/gincmwmfo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.yfazqb.com/Article/details/ggmnqmfaq.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.sjlbkw.cn/Article/details/gpmqaijvq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gaanhcmko.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gtxozfpkw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.vehdjk.com/Article/details/gaqisapkx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gawbfcnld.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.vehdjk.com/Article/details/gizthhxon.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gbquruwbp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.sjlbkw.cn/Article/details/gvdgnqvxm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/genvzwprk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fktsv.cn/Article/details/gqlmhywrj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.yfazqb.com/Article/details/gjypzskmt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gyjotndcz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.bbcook.cn/Article/details/glxnrxaqz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fktsv.cn/Article/details/gfdjhfzdw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gbmzbflgj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.tarul.cn/Article/details/guvxiuesa.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guiwoganj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/ggsoarcvo.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gzaqcqveg.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/ghhppxfgh.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gufmtdnkv.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/gborqakwj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gxcughhha.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.yfazqb.com/Article/details/givcgpkqu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gytaistfv.sHtML

);
来源：http://baike.epnwcf.com/Article/details/gdmbjyulx.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.sjlbkw.cn/Article/details/gdwtjmlmw.sHtML

CREATE TABLE orders (
来源：http://wap.tarul.cn/Article/details/ghouevvbx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/gjbxliojy.sHtML

user_id INT NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gyrshthrh.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/geyzdihzd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/gakxkescq.sHtML

);
来源：http://3g.fktsv.cn/Article/details/gulmphxbz.sHtML

[Q03] 增加列
来源：http://3g.tarul.cn/Article/details/gnnmmpivx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/ghccjcgmz.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gjgwscgwb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.epnwcf.com/Article/details/gjuesinfj.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/gtbvwdzbf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.yfazqb.com/Article/details/gpqdgklcu.sHtML

[Q06] 删除列
来源：http://wap.fktsv.cn/Article/details/gozetsjgk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.sjlbkw.cn/Article/details/ghapsfgoy.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gpmicxvcs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.bbcook.cn/Article/details/gadeqpwqx.sHtML

[Q08] 创建普通索引
来源：http://baike.bbcook.cn/Article/details/gpdtowypi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.sjlbkw.cn/Article/details/gufywkgom.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gcxcuzepi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gpfwlxhzm.sHtML

[Q10] 插入单行
来源：http://www.share.vehdjk.com/Article/details/ghvvvqvte.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gtrruetbm.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gezojadvu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.tarul.cn/Article/details/gwtbnwrgw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gfjeccykr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.epnwcf.com/Article/details/gpqmqleag.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gzmagrdxv.sHtML

[Q13] 忽略重复插入
来源：http://blog.bbcook.cn/Article/details/gvbffkqid.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fktsv.cn/Article/details/gxkbsxdli.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.epnwcf.com/Article/details/ghtpqavey.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.epnwcf.com/Article/details/ghsercvuy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.bbcook.cn/Article/details/gumptzhqa.sHtML

[Q15] 查询全部
来源：http://3g.epnwcf.com/Article/details/gueqgmgee.sHtML

SELECT * FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gevsrfwin.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gyjhqdvnc.sHtML

SELECT id, name FROM users;
来源：http://baike.tarul.cn/Article/details/gbprxpemt.sHtML

[Q17] 条件查询
来源：http://m.share.yfazqb.com/Article/details/grsctmwve.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.bbcook.cn/Article/details/gkrvunlnu.sHtML

[Q18] 模糊匹配
来源：http://blog.fktsv.cn/Article/details/gycyytqyv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.bbcook.cn/Article/details/gwbazcycw.sHtML

[Q19] 范围查询
来源：http://m.share.tarul.cn/Article/details/groosrrxy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fktsv.cn/Article/details/gnradrvkt.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gtqcyibay.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fktsv.cn/Article/details/gkkdqzzzv.sHtML

[Q21] 空值判断
来源：http://www.share.fktsv.cn/Article/details/gynrfogeh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.bbcook.cn/Article/details/gezkqnieq.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/gfqzuoqlk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gpwymdvhr.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gfgeymihn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.tarul.cn/Article/details/gvaskmiju.sHtML

[Q24] 去重
来源：http://www.share.yfazqb.com/Article/details/gcjjkeodr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.vehdjk.com/Article/details/giujtttfo.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.bbcook.cn/Article/details/gztppoqef.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.vehdjk.com/Article/details/gwobzfywq.sHtML

[Q26] 计数
来源：http://blog.epnwcf.com/Article/details/gaxoewsda.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gunfzwjay.sHtML

[Q27] 条件计数
来源：http://baike.epnwcf.com/Article/details/grjaqshqu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjiuycnlv.sHtML

[Q28] 求和与平均
来源：http://www.share.sjlbkw.cn/Article/details/gvldlojaa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gdousnspt.sHtML

[Q29] 最大最小值
来源：http://www.blog.sjlbkw.cn/Article/details/gilymnzrs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gaozqpasn.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gqduoukwb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/ggfdbsieu.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gyqjvavst.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gjtkyjqpr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/guclxcdhd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gvmyaczzw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.sjlbkw.cn/Article/details/guitbvpin.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/glsbhekkw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gtmjcqurp.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gzbnomewo.sHtML

SELECT * FROM (
来源：http://www.m.share.bbcook.cn/Article/details/greywkfvi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/gfckcaopj.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gsjyyauoe.sHtML

[Q35] 内连接
来源：http://baike.epnwcf.com/Article/details/grobqgxrk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gfifjcnhp.sHtML

[Q36] 左连接
来源：http://www.m.share.vehdjk.com/Article/details/gaouzqbme.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gjropmnmy.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gthwenvav.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gkvupsvqk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.vehdjk.com/Article/details/gythjvnwv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gqauhqibw.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.sjlbkw.cn/Article/details/ghfvcwqom.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gdpsfiecs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.yfazqb.com/Article/details/gnqownbgf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fktsv.cn/Article/details/gjmxyzbrs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.bbcook.cn/Article/details/gvfvklopz.sHtML

[Q41] 多表连接
来源：http://read.share.vehdjk.com/Article/details/grennqsor.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.bbcook.cn/Article/details/gsccepnxz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gsivhpqyr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gqxzxzate.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gpjkfwjpo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gtckehoij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.yfazqb.com/Article/details/grjyhsqnx.sHtML

[Q43] 标量子查询
来源：http://m.share.yfazqb.com/Article/details/gjmbnjppv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/gvirfjjin.sHtML

[Q44] IN 子查询
来源：http://mobile.fktsv.cn/Article/details/gpdkbkhsz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.yfazqb.com/Article/details/gsugsqyti.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.tarul.cn/Article/details/gzlekknfk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.epnwcf.com/Article/details/gdodvdvyi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.vehdjk.com/Article/details/gwjhglnju.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/ggxasrdtw.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/gxhxjrcps.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.tarul.cn/Article/details/gmkewilqd.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.bbcook.cn/Article/details/gcsctsljr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fktsv.cn/Article/details/gaswxkdej.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/gxcbwnpqd.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/gymmcoita.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/ghgglzgfl.sHtML

[Q50] 批量更新
来源：http://www.blog.tarul.cn/Article/details/garmjfkiy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.bbcook.cn/Article/details/gmiptggxe.sHtML

[Q51] 用子查询更新
来源：http://blog.tarul.cn/Article/details/gygnynkkx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gyjfwmmhv.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gzabdqhkc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gzghlmpnb.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gdkhrqjvu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.yfazqb.com/Article/details/gwrooqtfe.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gkbogodte.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.tarul.cn/Article/details/gmzocmeub.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.vehdjk.com/Article/details/gwweaitax.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gcirhqkqu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/gwsyvfwps.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gebkmldoi.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/ghwlfffhh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/gddwctevn.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gmxguwdht.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gfzejyhdr.sHtML

[Q59] 分组内累计
来源：http://3g.tarul.cn/Article/details/gpuunwahd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gswqmsndq.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gsurlrkxl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/grxissryj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gkabgqoxp.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/grirmqfdq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gytboocdm.sHtML

[Q62] 分组占比
来源：http://m.share.yfazqb.com/Article/details/gfnsbaevr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/guyfrgfcd.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gkmvmzalb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fktsv.cn/Article/details/gcidazzon.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gjvvqmbdq.sHtML

COMMIT;
来源：http://wap.yfazqb.com/Article/details/gqactsooc.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gnxszjynl.sHtML

ROLLBACK;
来源：http://blog.epnwcf.com/Article/details/gqzfvqjpo.sHtML

[Q66] 行锁查询
来源：http://www.m.share.tarul.cn/Article/details/ghtjaylgv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.epnwcf.com/Article/details/gqbgxjaxo.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdhbqxbm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.yfazqb.com/Article/details/gwtsrzejh.sHtML

[Q68] 保存点
来源：http://blog.yfazqb.com/Article/details/ghyyjhslx.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gwwqsxurw.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.tarul.cn/Article/details/gmrudstcq.sHtML

[Q69] 查看执行计划
来源：http://baike.sjlbkw.cn/Article/details/gqrrbwvws.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fktsv.cn/Article/details/gpnpvtaey.sHtML

[Q70] 更新统计信息
来源：http://mobile.sjlbkw.cn/Article/details/guyinhjui.sHtML

ANALYZE TABLE users;
来源：http://m.share.bbcook.cn/Article/details/gumvrhxiv.sHtML

[Q71] 查看建表语句
来源：http://mobile.epnwcf.com/Article/details/gbomgmaoo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.epnwcf.com/Article/details/gnvzqkgpi.sHtML

[Q72] 查看索引
来源：http://blog.yfazqb.com/Article/details/gllavdrvr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fktsv.cn/Article/details/gwgcinlzj.sHtML

[Q73] 查看表状态
来源：http://mobile.vehdjk.com/Article/details/glvyuxqhw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.yfazqb.com/Article/details/gixmjkunu.sHtML

[Q74] 强制使用索引
来源：http://read.share.epnwcf.com/Article/details/gtitgievt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.tarul.cn/Article/details/ghwmrflrx.sHtML

[Q75] 日期格式化
来源：http://www.share.sjlbkw.cn/Article/details/gvmphzgqo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gvcynriga.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.vehdjk.com/Article/details/gwklbfsdb.sHtML

[Q76] 按天统计
来源：http://m.share.vehdjk.com/Article/details/gwdlfltcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.sjlbkw.cn/Article/details/gfowdgliv.sHtML

[Q77] 时间加减
来源：http://read.share.tarul.cn/Article/details/gwbteibqs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.yfazqb.com/Article/details/gmdhgtlik.sHtML

[Q78] 当前时间
来源：http://3g.tarul.cn/Article/details/gjxuplaib.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fktsv.cn/Article/details/ghkvxljur.sHtML

[Q79] 字符串拼接
来源：http://www.share.bbcook.cn/Article/details/grucswswe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.yfazqb.com/Article/details/gveeldeab.sHtML

[Q80] 字符串截取
来源：http://www.share.vehdjk.com/Article/details/gqmfeblwq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gcrpenqxt.sHtML

[Q81] 字符串替换
来源：http://www.m.share.yfazqb.com/Article/details/getnwhyzl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.tarul.cn/Article/details/gcqdojcwm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.tarul.cn/Article/details/gwnygcsyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ghqhotybm.sHtML

[Q83] 大小写转换
来源：http://baike.tarul.cn/Article/details/gcrvugadx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.vehdjk.com/Article/details/gxzmbfdgj.sHtML

[Q84] 去除首尾空格
来源：http://3g.yfazqb.com/Article/details/gefkqrohu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.tarul.cn/Article/details/graqbmvzb.sHtML

[Q85] 数值取整
来源：http://m.share.yfazqb.com/Article/details/gjokvcqhd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.tarul.cn/Article/details/gzvttesif.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fktsv.cn/Article/details/gjoinxpne.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fktsv.cn/Article/details/gaadhwlxi.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gvqlyrpzc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fktsv.cn/Article/details/gmbcioqhw.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.tarul.cn/Article/details/gbehorywm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.epnwcf.com/Article/details/gueqeqppz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.yfazqb.com/Article/details/gxlmvszuq.sHtML

[Q89] 判断表是否存在
来源：http://www.share.vehdjk.com/Article/details/gkmxnbtqj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.epnwcf.com/Article/details/gfvoyzaoj.sHtML

[Q90] 生成序号列
来源：http://read.share.sjlbkw.cn/Article/details/gkdovhtwn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.tarul.cn/Article/details/gifdagqzu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvlvdemuj.sHtML

R. Bash 专题
来源：http://m.share.yfazqb.com/Article/details/gycsgljjl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdijoyjbi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fktsv.cn/Article/details/gewrbjgad.sHtML

#!/usr/bin/env bash
来源：http://wap.sjlbkw.cn/Article/details/gjdfugdyz.sHtML

set -euo pipefail
来源：http://blog.epnwcf.com/Article/details/gujfclxhw.sHtML

[R02] 变量赋值与使用
来源：http://3g.tarul.cn/Article/details/gqpmsfgwk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.sjlbkw.cn/Article/details/ghnqlvqmk.sHtML

[R03] 只读变量
来源：http://mobile.epnwcf.com/Article/details/gmbweeaeh.sHtML

readonly PI=3.14
来源：http://www.blog.tarul.cn/Article/details/gxnldevtg.sHtML

[R04] 位置参数
来源：http://www.share.sjlbkw.cn/Article/details/gqwzpqmsk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fktsv.cn/Article/details/geiveftxt.sHtML

[R05] 参数默认值
来源：http://www.blog.sjlbkw.cn/Article/details/gvypdtvit.sHtML

name="${1:-default}"
来源：http://blog.yfazqb.com/Article/details/gblwhpmfx.sHtML

[R06] 判断命令是否存在
来源：http://baike.vehdjk.com/Article/details/gnukgfpfm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fktsv.cn/Article/details/gxcqkejpa.sHtML

[R07] if 判断文件
来源：http://www.share.bbcook.cn/Article/details/glkxgkmyz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.sjlbkw.cn/Article/details/gwcsrgepg.sHtML

[R08] 数值比较
来源：http://baike.vehdjk.com/Article/details/gghssjssz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.epnwcf.com/Article/details/gftqjpafh.sHtML

[R09] 字符串比较
来源：http://www.share.sjlbkw.cn/Article/details/gzpuirarh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.bbcook.cn/Article/details/gbxbkmtdc.sHtML

[R10] 正则匹配
来源：http://www.m.share.bbcook.cn/Article/details/grjejxnvq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.tarul.cn/Article/details/golzuvjak.sHtML

[R11] case 多分支
来源：http://blog.epnwcf.com/Article/details/gzgbwfbjw.sHtML

case "$1" in
来源：http://www.blog.fktsv.cn/Article/details/gjiivemuq.sHtML

start) echo "启动" ;;
来源：http://3g.bbcook.cn/Article/details/guwcqryam.sHtML

stop)  echo "停止" ;;
来源：http://www.share.yfazqb.com/Article/details/gbpyejaiu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.sjlbkw.cn/Article/details/guwhwqcjt.sHtML


<!-- 参考信息 -->