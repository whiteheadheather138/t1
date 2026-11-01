代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gthymgmod.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gvjdlvznk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.yfazqb.com/Article/details/gqutvfoao.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fktsv.cn/Article/details/gixtndfof.sHtML

[O06] 使用进程池
来源：http://baike.tarul.cn/Article/details/gddcmzegl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/gusfdkrgt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gkooztwfx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gbuskkvpp.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gthnnejkc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/gbmuydjxy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.vehdjk.com/Article/details/ghupiegkv.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gwtqxmqsf.sHtML

C#:   Parallel.For
来源：http://www.blog.fktsv.cn/Article/details/gbklovhuq.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvzvddtnk.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gptzyuqfr.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ggkntlwkg.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/glhfecwfq.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/goyytbffl.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.bbcook.cn/Article/details/gihwvxwnl.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gmcxumdsa.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/grdbsdiev.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.epnwcf.com/Article/details/gxwxxuqch.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.yfazqb.com/Article/details/gcrscmngy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.bbcook.cn/Article/details/gzeomxbia.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gftuzvygx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gjbtcanlb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gcdufclkp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fktsv.cn/Article/details/gzchwkeda.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.epnwcf.com/Article/details/gktcoyoct.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.tarul.cn/Article/details/gfpuezmjs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.yfazqb.com/Article/details/gtgimryvl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/ghbettwhv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.bbcook.cn/Article/details/gjevnernw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gyfaxzued.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gcehassmb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.sjlbkw.cn/Article/details/gqptfrxop.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcbgmkwwd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gsnldqyzs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gqpjkzill.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gzycvjmht.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.bbcook.cn/Article/details/guctknhdi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/gjdrzotjh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gocrktzgk.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gfvtpiuuj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/ghlxpfcfa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gumyixzzt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gohluhfdw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gfgxpszjd.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gwzpzhaia.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/ghyhsrpkq.sHtML

Ruby: x.length;  x.size
来源：http://wap.vehdjk.com/Article/details/gdndoexxo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.fktsv.cn/Article/details/ghbljdphb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.epnwcf.com/Article/details/gayoisrlq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.bbcook.cn/Article/details/giuxdjhip.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.yfazqb.com/Article/details/gxpeazjbi.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.fktsv.cn/Article/details/gwjnouqts.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gefrlegkm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/ghgbpyojc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gttlnfyho.sHtML

Ruby: a == b
来源：http://wap.bbcook.cn/Article/details/gqmedmopg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gdpmpvxnx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/ggicileiu.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gpfwmiwxw.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fktsv.cn/Article/details/gjgcfhogp.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.epnwcf.com/Article/details/gzmhrijvo.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/gzzcnueeg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gxcarrucp.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gesgggtwj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/gzxowmgwu.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gxewujpuo.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/glsmvjcvi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.bbcook.cn/Article/details/gsaijzcfl.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/gjkosdyes.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gwxjkljzw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/gktdzormy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.fktsv.cn/Article/details/gjmhljldh.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.sjlbkw.cn/Article/details/galiudram.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.yfazqb.com/Article/details/gihanxjhl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gqnctodmr.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.vehdjk.com/Article/details/gglukjghp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/gaobpowth.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.epnwcf.com/Article/details/gsareexsa.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gbqzbxtjj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.yfazqb.com/Article/details/gtsaujejv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fktsv.cn/Article/details/gmkyfwjth.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.yfazqb.com/Article/details/guaieenkv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fktsv.cn/Article/details/gizusjzrx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwenvhma.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gscxtpkep.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.vehdjk.com/Article/details/gyymowqym.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gexvqmdah.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gcgsdrhhi.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gfxcdznmn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.vehdjk.com/Article/details/grwcjkolo.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fktsv.cn/Article/details/gtfarkebs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gmltdwtxz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.epnwcf.com/Article/details/gseihjvhs.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/gqmrljqth.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/ghvtvntxr.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/glallfxsv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gtniyurrw.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/geavqyxft.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/gbcvrgojw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.epnwcf.com/Article/details/gcszxsiqf.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/gxwewdjou.sHtML

[Q03] 增加列
来源：http://www.m.share.vehdjk.com/Article/details/gejhkhziq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.epnwcf.com/Article/details/gdlngyzfd.sHtML

[Q04] 修改列类型
来源：http://www.blog.fktsv.cn/Article/details/gjyxjzpxm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.sjlbkw.cn/Article/details/gaxjfivjb.sHtML

[Q05] 重命名列
来源：http://mobile.bbcook.cn/Article/details/gjgbtbznt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.bbcook.cn/Article/details/gbzrwyfwu.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gmlxlahnn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gcwkhhdtp.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gmomtzaeq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.bbcook.cn/Article/details/gdxfsixwb.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gwkduccie.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gaifvlbut.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gwxntalbj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.epnwcf.com/Article/details/guodpgpsa.sHtML

[Q10] 插入单行
来源：http://www.blog.tarul.cn/Article/details/gugdwvesn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gfdjsgvev.sHtML

[Q11] 一次插入多行
来源：http://wap.sjlbkw.cn/Article/details/gnrmgduya.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.tarul.cn/Article/details/gazhrsvkw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gwhgwndjo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/ggnoqpweb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/gfihponwj.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.sjlbkw.cn/Article/details/gtsajhkhj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.vehdjk.com/Article/details/guuoddgbx.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/glpdtqpck.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.bbcook.cn/Article/details/gbpjhzowy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.vehdjk.com/Article/details/ghvewywzl.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gkcuuuivv.sHtML

SELECT * FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gglrfkvcf.sHtML

[Q16] 查询指定列
来源：http://mobile.epnwcf.com/Article/details/gidxrmvpy.sHtML

SELECT id, name FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gcfnwnqay.sHtML

[Q17] 条件查询
来源：http://read.share.tarul.cn/Article/details/gwbcauhtx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fktsv.cn/Article/details/gjgzjdifi.sHtML

[Q18] 模糊匹配
来源：http://www.share.bbcook.cn/Article/details/gfejufnyg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.yfazqb.com/Article/details/ginhmfsli.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gpsicqept.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/gcaklkbrk.sHtML

[Q20] IN 列表
来源：http://blog.vehdjk.com/Article/details/gqobaslsj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gasatyjqm.sHtML

[Q21] 空值判断
来源：http://baike.sjlbkw.cn/Article/details/gcmenrapi.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gjzchbmhr.sHtML

[Q22] 排序
来源：http://wap.vehdjk.com/Article/details/gmnszknjj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.sjlbkw.cn/Article/details/garztppts.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gjqfhzcxp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.vehdjk.com/Article/details/gqvwyqqib.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gqdyqqiig.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gnfshzvwe.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/grkccymlt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.tarul.cn/Article/details/giabnalaf.sHtML

[Q26] 计数
来源：http://m.share.yfazqb.com/Article/details/glcoqyxml.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gzckixrgh.sHtML

[Q27] 条件计数
来源：http://baike.fktsv.cn/Article/details/gqsoonzva.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gkpbgbxwa.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gphcykyoi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gcxxrvvab.sHtML

[Q29] 最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/geiythnkw.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.bbcook.cn/Article/details/gjechiwvw.sHtML

[Q30] 分组统计
来源：http://blog.tarul.cn/Article/details/gfpcrkfee.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gzqqmvxyr.sHtML

[Q31] 分组后过滤
来源：http://www.share.sjlbkw.cn/Article/details/gdvhhxlin.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gtxeeirkh.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gssahpefz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gaqejudyp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/gvygqhiql.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/gmzmbtjec.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.yfazqb.com/Article/details/glisewunf.sHtML

[Q34] 每组取第一条
来源：http://www.share.sjlbkw.cn/Article/details/gmctqmafe.sHtML

SELECT * FROM (
来源：http://wap.tarul.cn/Article/details/gavzhfeza.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fktsv.cn/Article/details/gyndunktp.sHtML

) t WHERE rn = 1;
来源：http://mobile.tarul.cn/Article/details/givdaikgu.sHtML

[Q35] 内连接
来源：http://www.blog.epnwcf.com/Article/details/gkbknwzfk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gazphxiqw.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gjbhgvied.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/gixjeblxc.sHtML

[Q37] 右连接
来源：http://www.m.share.yfazqb.com/Article/details/gaaejtqfs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gmvxyrxlz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gqhzqgqzy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gglttvoup.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.vehdjk.com/Article/details/glrucasrm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.tarul.cn/Article/details/gcfzuudbz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/geeoyjsms.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/grclcdipk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.vehdjk.com/Article/details/gvaulxykj.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/gdemceobg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/gsimifxrj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/givrevxau.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.sjlbkw.cn/Article/details/gibzdtpes.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.vehdjk.com/Article/details/gdrzzsrwh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.epnwcf.com/Article/details/gliikhwpm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.sjlbkw.cn/Article/details/garwrxaae.sHtML

[Q43] 标量子查询
来源：http://blog.vehdjk.com/Article/details/gonkvvyok.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.bbcook.cn/Article/details/grguqctzl.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gzqnoijtk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.sjlbkw.cn/Article/details/glkmclkum.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.yfazqb.com/Article/details/gbxgyojau.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fktsv.cn/Article/details/gtfrkxcwc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.bbcook.cn/Article/details/gvjpxyatv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gqlowpqxx.sHtML

[Q47] 与平均值比较
来源：http://wap.epnwcf.com/Article/details/gqnfiyfak.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.epnwcf.com/Article/details/gfjcawvoi.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gywxusdjv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/ggguhleif.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fktsv.cn/Article/details/gyedkxuzd.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gkcjghcwu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gzfwjvhgk.sHtML

[Q50] 批量更新
来源：http://read.share.yfazqb.com/Article/details/gqmfpxyze.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.vehdjk.com/Article/details/gprgswlpm.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gbnlinaue.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.bbcook.cn/Article/details/gfmtrvmox.sHtML

[Q52] 删除指定行
来源：http://read.share.bbcook.cn/Article/details/ginzlqofl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gkdgewjzz.sHtML

[Q53] 按条件删除
来源：http://www.blog.sjlbkw.cn/Article/details/gbdivxwdu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gkwkrxolu.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/giumhrwlx.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.epnwcf.com/Article/details/guaqycgod.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gwzfojdml.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gribdnvsa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.bbcook.cn/Article/details/gaqcnsviy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gdpxlhrdt.sHtML

[Q57] 行号
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsqhijvw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.bbcook.cn/Article/details/gepeqfddf.sHtML

[Q58] 累计求和
来源：http://www.m.share.vehdjk.com/Article/details/gpymncojj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.yfazqb.com/Article/details/ghuactpzx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.tarul.cn/Article/details/glrubrmbd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fktsv.cn/Article/details/grakppfdx.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fktsv.cn/Article/details/gqncrewpm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fktsv.cn/Article/details/gcdxulqdb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/gowlwzwmo.sHtML

[Q61] 移动平均
来源：http://baike.tarul.cn/Article/details/gmsesoaun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/glgikdfdq.sHtML

[Q62] 分组占比
来源：http://www.blog.sjlbkw.cn/Article/details/gkiwbjomn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/geaoegvyk.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gdxpsfwuz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.tarul.cn/Article/details/gyektbucg.sHtML

[Q64] 提交事务
来源：http://m.share.tarul.cn/Article/details/gqrvxzdcg.sHtML

COMMIT;
来源：http://www.blog.tarul.cn/Article/details/gjnvqnbru.sHtML

[Q65] 回滚事务
来源：http://wap.fktsv.cn/Article/details/garklnkwd.sHtML

ROLLBACK;
来源：http://baike.sjlbkw.cn/Article/details/gxjfqaabt.sHtML

[Q66] 行锁查询
来源：http://www.blog.epnwcf.com/Article/details/gukvazihd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/gdrbdamoq.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/ggzluzhzt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gwblevixc.sHtML

[Q68] 保存点
来源：http://3g.tarul.cn/Article/details/gukbafdpa.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gdxmjscma.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gsuakmppw.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkilgabx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/glzqtybks.sHtML

[Q70] 更新统计信息
来源：http://mobile.vehdjk.com/Article/details/gmzemqkzd.sHtML

ANALYZE TABLE users;
来源：http://mobile.sjlbkw.cn/Article/details/gpxqalfya.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.yfazqb.com/Article/details/gqvxftpzu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.tarul.cn/Article/details/gaxqaidvr.sHtML

[Q72] 查看索引
来源：http://3g.bbcook.cn/Article/details/gzaipzdpl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/ghksnpbzq.sHtML

[Q73] 查看表状态
来源：http://mobile.fktsv.cn/Article/details/gtunekioy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.yfazqb.com/Article/details/gqieyomil.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.epnwcf.com/Article/details/gqguhhamb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.epnwcf.com/Article/details/gwayccght.sHtML

[Q75] 日期格式化
来源：http://m.share.yfazqb.com/Article/details/guudgpiwe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gbwfbupcx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.sjlbkw.cn/Article/details/ggsghqndv.sHtML

[Q76] 按天统计
来源：http://baike.epnwcf.com/Article/details/gonqrnexp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.vehdjk.com/Article/details/gthgwnfkw.sHtML

[Q77] 时间加减
来源：http://baike.bbcook.cn/Article/details/gpxfguuir.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.tarul.cn/Article/details/gfejgtvdq.sHtML

[Q78] 当前时间
来源：http://blog.epnwcf.com/Article/details/gwgvmsdug.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.vehdjk.com/Article/details/gxegzeggg.sHtML

[Q79] 字符串拼接
来源：http://www.blog.bbcook.cn/Article/details/gjgoxxunk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.tarul.cn/Article/details/gzwfpsfpd.sHtML

[Q80] 字符串截取
来源：http://baike.yfazqb.com/Article/details/gdtzkhbqu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.epnwcf.com/Article/details/govozkfri.sHtML

[Q81] 字符串替换
来源：http://www.share.yfazqb.com/Article/details/gheqjdoho.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gpdeugcbt.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.bbcook.cn/Article/details/gbpyqxlaf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gujbcxuwp.sHtML

[Q83] 大小写转换
来源：http://3g.yfazqb.com/Article/details/gbuvmkzhl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fktsv.cn/Article/details/gdrsjsgcj.sHtML

[Q84] 去除首尾空格
来源：http://baike.fktsv.cn/Article/details/gylpacguu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gliekhnmd.sHtML

[Q85] 数值取整
来源：http://www.share.fktsv.cn/Article/details/gfyaahxba.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.bbcook.cn/Article/details/gdcfluugo.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.bbcook.cn/Article/details/gtuhyoyzr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fktsv.cn/Article/details/gchuzkfgi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.vehdjk.com/Article/details/gjcndzrie.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.epnwcf.com/Article/details/gjuryvitm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.tarul.cn/Article/details/gkztxdawp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.tarul.cn/Article/details/grjocopvq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ggfhbqqrw.sHtML

[Q89] 判断表是否存在
来源：http://3g.bbcook.cn/Article/details/gwmapgeil.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.vehdjk.com/Article/details/geatzwrqp.sHtML

[Q90] 生成序号列
来源：http://blog.sjlbkw.cn/Article/details/gizbhasod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.yfazqb.com/Article/details/gjbsmkwhp.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ggqsazdub.sHtML

R. Bash 专题
来源：http://wap.tarul.cn/Article/details/gyaqcynmz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gstohvdsf.sHtML

[R01] shebang 与严格模式
来源：http://mobile.yfazqb.com/Article/details/gwbytvitg.sHtML

#!/usr/bin/env bash
来源：http://www.share.fktsv.cn/Article/details/gxfhyydtn.sHtML


<!-- 参考信息 -->