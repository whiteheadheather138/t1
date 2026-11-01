代发 wailian999

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gcvtoxktg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.vehdjk.com/Article/details/govbpnaog.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fktsv.cn/Article/details/gmvjeqapq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/grrwatizd.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdbzttbf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/gnwoobtti.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gdhizcdun.sHtML

Ruby: // fork 块
来源：http://www.m.share.tarul.cn/Article/details/gxukwvkkd.sHtML

C#:   Parallel.For
来源：http://read.share.bbcook.cn/Article/details/gtcmqbnqd.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gsrokpqkl.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gpzziknss.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzoguqvw.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gqpnywwxd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gicjpsonq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.epnwcf.com/Article/details/gvefqgxzy.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/ghhkodrlu.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gesdvkcdo.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.vehdjk.com/Article/details/grtpjlbbo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.sjlbkw.cn/Article/details/glcyochqo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gzrbyazfg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.vehdjk.com/Article/details/gjzzjotho.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.bbcook.cn/Article/details/gvtfeyubw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.vehdjk.com/Article/details/ghccpiblb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gucyyidhp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.bbcook.cn/Article/details/ggirtojkk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gymlatiih.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gefiiifiz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gjtzzfaav.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gknnvdnkb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.epnwcf.com/Article/details/gclofvqar.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gyykrrlcj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.epnwcf.com/Article/details/getftcagc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/govvznpha.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gjcgjehxi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gftwrjdfa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.tarul.cn/Article/details/gxcbymiwa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.sjlbkw.cn/Article/details/gktxrfntc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.sjlbkw.cn/Article/details/gyqioipmp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gzyogzfma.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gwqzlqpre.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gxwrwncfd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gdtsenmhf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gbyaizhxu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gdzdblygc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gdokfrdmx.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gcqjeklkt.sHtML

Ruby: x.length;  x.size
来源：http://wap.tarul.cn/Article/details/gfjznzfud.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.sjlbkw.cn/Article/details/grjzlxgru.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.bbcook.cn/Article/details/gaowbumva.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gcsrvtxjn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.bbcook.cn/Article/details/gdtsvzide.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.sjlbkw.cn/Article/details/gdusplefo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.epnwcf.com/Article/details/gqvbollgk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gpocywtmu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.epnwcf.com/Article/details/grhjtwyhd.sHtML

Ruby: a == b
来源：http://wap.epnwcf.com/Article/details/ggrfzfnmf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/gckekjcwt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.vehdjk.com/Article/details/gzppirdon.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/gugtfepgh.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/gvbgonrqr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.sjlbkw.cn/Article/details/gewrrfpsi.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/gztyifaag.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.bbcook.cn/Article/details/gdhwfsuva.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gyaeoppnh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.sjlbkw.cn/Article/details/gcurquqvn.sHtML

C#:   if (x is null) {}
来源：http://www.share.vehdjk.com/Article/details/gflpceuof.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/ghbgbvntr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.epnwcf.com/Article/details/gjzkrvnmp.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.tarul.cn/Article/details/gpdwealbz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gxzjuqfvt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gzsxfgxan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gsqoxdijr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.bbcook.cn/Article/details/gxenwznbi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.yfazqb.com/Article/details/gewgavekj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.epnwcf.com/Article/details/gkffbatjd.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/grppuicnz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gmikifbbn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.sjlbkw.cn/Article/details/gletwdtmv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/giyuvucpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.tarul.cn/Article/details/grwbezuzc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gjzqqzmis.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.sjlbkw.cn/Article/details/gpiezzcaa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gnvtzkbwi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.epnwcf.com/Article/details/ghepfdgvz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gevlazuge.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/gfymktgce.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvdffjbio.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gjlocbdmt.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gawkbclks.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fktsv.cn/Article/details/gqeixmbfs.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gzpzstvjg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gbghqubsv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gxksiuqln.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gmqtefjhv.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/giiuychyv.sHtML

CREATE TABLE orders (
来源：http://www.share.vehdjk.com/Article/details/gccdcrxwt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gjwiemmmq.sHtML

user_id INT NOT NULL,
来源：http://3g.vehdjk.com/Article/details/glnmsmihy.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.yfazqb.com/Article/details/grsvowvic.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gtcqpncse.sHtML

);
来源：http://wap.vehdjk.com/Article/details/gjbmozrwh.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gdiehlesp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.bbcook.cn/Article/details/gigqkdzlu.sHtML

[Q04] 修改列类型
来源：http://www.blog.sjlbkw.cn/Article/details/grqvypoxl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gqztylnfg.sHtML

[Q05] 重命名列
来源：http://baike.yfazqb.com/Article/details/gebjamhdv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.vehdjk.com/Article/details/gpwowukky.sHtML

[Q06] 删除列
来源：http://www.m.share.bbcook.cn/Article/details/gzbrrvwim.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.epnwcf.com/Article/details/grnbqjlfr.sHtML

[Q07] 删除表
来源：http://3g.tarul.cn/Article/details/gbvarfqqx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/gsmdxuukk.sHtML

[Q08] 创建普通索引
来源：http://read.share.fktsv.cn/Article/details/grrgijzzt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/ggjzgpmws.sHtML

[Q09] 创建唯一索引
来源：http://read.share.fktsv.cn/Article/details/gyfcuwfph.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.tarul.cn/Article/details/giobrvqxw.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gqyxqtwqq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.epnwcf.com/Article/details/goygrkvem.sHtML

[Q11] 一次插入多行
来源：http://wap.epnwcf.com/Article/details/gnzathvmq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gcsjzaezb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.yfazqb.com/Article/details/guqcjcepc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.sjlbkw.cn/Article/details/giyvtnlxf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.sjlbkw.cn/Article/details/gxrbxival.sHtML

[Q13] 忽略重复插入
来源：http://mobile.yfazqb.com/Article/details/gxuizatpk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/grxmqmjdy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.epnwcf.com/Article/details/gjabimnnj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gvsozaxyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gwhgqiiix.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gyxdsffnv.sHtML

SELECT * FROM users;
来源：http://www.share.bbcook.cn/Article/details/gvyuspues.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gqkmxqrzk.sHtML

SELECT id, name FROM users;
来源：http://baike.vehdjk.com/Article/details/ginhvbjic.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/gmungxrod.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gvayuwpqc.sHtML

[Q18] 模糊匹配
来源：http://mobile.bbcook.cn/Article/details/gmfdezowx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gxhbfarii.sHtML

[Q19] 范围查询
来源：http://www.blog.vehdjk.com/Article/details/ggtricimb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/gufoaypcp.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gryjbirzw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.sjlbkw.cn/Article/details/gmodyjkpz.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/gvodluhba.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.vehdjk.com/Article/details/gnvkzhsyl.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/guzpeaare.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.bbcook.cn/Article/details/gxwpuarwp.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/geztlmhca.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gievfztfm.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/guwxcgdha.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.epnwcf.com/Article/details/geanjgpap.sHtML

[Q25] 只取前 N 条
来源：http://3g.fktsv.cn/Article/details/goeytkwot.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.yfazqb.com/Article/details/gezzqbpjc.sHtML

[Q26] 计数
来源：http://www.share.sjlbkw.cn/Article/details/gjlywcvmb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.tarul.cn/Article/details/gwzbneglx.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gfdkbmwxo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/glsryxmdn.sHtML

[Q28] 求和与平均
来源：http://blog.sjlbkw.cn/Article/details/gleuyahlo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.yfazqb.com/Article/details/gaicbxlie.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/gunqqsaqj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.epnwcf.com/Article/details/gjcruvebz.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gtboofcti.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/grfyrmiua.sHtML

[Q31] 分组后过滤
来源：http://www.share.epnwcf.com/Article/details/gcqzbrxze.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gvllltelu.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.bbcook.cn/Article/details/gemwxbkhe.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.bbcook.cn/Article/details/gofdknunx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/ggytdabcb.sHtML

[Q33] 多列分组
来源：http://read.share.bbcook.cn/Article/details/ggofwzjrg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gfqjvganv.sHtML

[Q34] 每组取第一条
来源：http://wap.bbcook.cn/Article/details/ggnxotvjo.sHtML

SELECT * FROM (
来源：http://mobile.vehdjk.com/Article/details/gcptseojh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/grxqnroqv.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/gkvjtzhyq.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gcysbrfgd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gszskjocu.sHtML

[Q36] 左连接
来源：http://baike.epnwcf.com/Article/details/gnvfbchbe.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gjnqgzpez.sHtML

[Q37] 右连接
来源：http://mobile.yfazqb.com/Article/details/gupidopcp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.epnwcf.com/Article/details/gwbhceorr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gbufcgffn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gdvftavao.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.vehdjk.com/Article/details/gvzwcdlda.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gwddaemhh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.tarul.cn/Article/details/gjjytmuko.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gopbmsykm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.bbcook.cn/Article/details/gcxzszsrf.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gwmuvujgx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gccykwjew.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.tarul.cn/Article/details/gganqdbxh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.yfazqb.com/Article/details/gfuaudavj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.epnwcf.com/Article/details/gbnwuzyjs.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.vehdjk.com/Article/details/glvqmvdou.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gmpvvwkvs.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/grzpxgnim.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.bbcook.cn/Article/details/gkmskxsea.sHtML

[Q44] IN 子查询
来源：http://blog.tarul.cn/Article/details/ggpmcosgw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.epnwcf.com/Article/details/ggmnzjfbn.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gjazygbml.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/glxgixoik.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.bbcook.cn/Article/details/gprxalrlw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.epnwcf.com/Article/details/gmsvprqwa.sHtML

[Q47] 与平均值比较
来源：http://baike.vehdjk.com/Article/details/ggzikgljg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.yfazqb.com/Article/details/gkgzhouvv.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.vehdjk.com/Article/details/gvnigyhli.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.bbcook.cn/Article/details/gwsafhrnr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.yfazqb.com/Article/details/gzsbyjvbi.sHtML

[Q49] 更新单行
来源：http://read.share.vehdjk.com/Article/details/gfdqshnuz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.epnwcf.com/Article/details/gpsvxirbo.sHtML

[Q50] 批量更新
来源：http://wap.sjlbkw.cn/Article/details/gtqrnpbvc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.bbcook.cn/Article/details/geafcgtzf.sHtML

[Q51] 用子查询更新
来源：http://read.share.epnwcf.com/Article/details/gyjfxtixh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.sjlbkw.cn/Article/details/gjylfoerc.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gswkbexwg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/ghnqrrrmj.sHtML

[Q53] 按条件删除
来源：http://wap.bbcook.cn/Article/details/gpjppgozn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gxkpjxizf.sHtML

[Q54] 清空表
来源：http://baike.bbcook.cn/Article/details/gfkszhvzs.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gazcfyczc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/givbitpit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fktsv.cn/Article/details/guwclymbn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gkeiibjoe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gspcvinlb.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/gqysulakl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.bbcook.cn/Article/details/gigbgkwst.sHtML

[Q58] 累计求和
来源：http://www.blog.tarul.cn/Article/details/gdwprbjgk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.bbcook.cn/Article/details/gsgwfkrse.sHtML

[Q59] 分组内累计
来源：http://baike.tarul.cn/Article/details/gcfddrasd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/ggqhuaikh.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.yfazqb.com/Article/details/gnarfpqtr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gpfepxdms.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.tarul.cn/Article/details/gkmfhlptp.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gwbfhdanz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.epnwcf.com/Article/details/gnvcqnuqm.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/ginrsywil.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.yfazqb.com/Article/details/gtovgszyr.sHtML

[Q63] 开启事务
来源：http://www.blog.bbcook.cn/Article/details/gwgjgkkky.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fktsv.cn/Article/details/gatmbnpdc.sHtML

[Q64] 提交事务
来源：http://baike.sjlbkw.cn/Article/details/gtmqdzzqz.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gzahlrqwl.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gfpdfpmrr.sHtML

ROLLBACK;
来源：http://www.share.yfazqb.com/Article/details/gcubedkkk.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gynxpdhle.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.bbcook.cn/Article/details/gpjsxljiv.sHtML

[Q67] 设置隔离级别
来源：http://baike.tarul.cn/Article/details/gzuybnoxs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.epnwcf.com/Article/details/gqehzvdtd.sHtML

[Q68] 保存点
来源：http://www.blog.bbcook.cn/Article/details/grajfydra.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/gxeestnbc.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.vehdjk.com/Article/details/gmwbigois.sHtML

[Q69] 查看执行计划
来源：http://read.share.tarul.cn/Article/details/gxfupnqaj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.vehdjk.com/Article/details/givwjwvui.sHtML

[Q70] 更新统计信息
来源：http://baike.bbcook.cn/Article/details/ggdlhaogj.sHtML

ANALYZE TABLE users;
来源：http://wap.bbcook.cn/Article/details/gcrvlayxd.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gacworfyz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.sjlbkw.cn/Article/details/gzmvpakco.sHtML

[Q72] 查看索引
来源：http://www.share.tarul.cn/Article/details/geywvinma.sHtML

SHOW INDEX FROM users;
来源：http://mobile.tarul.cn/Article/details/gpbnvglcs.sHtML

[Q73] 查看表状态
来源：http://m.share.epnwcf.com/Article/details/gxcixjlwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.tarul.cn/Article/details/gykvciyqy.sHtML

[Q74] 强制使用索引
来源：http://m.share.yfazqb.com/Article/details/gyonxmghg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.sjlbkw.cn/Article/details/gvfxhdfuh.sHtML

[Q75] 日期格式化
来源：http://www.blog.fktsv.cn/Article/details/glrlxumid.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.yfazqb.com/Article/details/gfiibyium.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.tarul.cn/Article/details/gyirxdkez.sHtML

[Q76] 按天统计
来源：http://m.share.yfazqb.com/Article/details/gfybewzgq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.yfazqb.com/Article/details/gpikxzszu.sHtML

[Q77] 时间加减
来源：http://baike.fktsv.cn/Article/details/gnkkhjzks.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.bbcook.cn/Article/details/gedtpjobq.sHtML

[Q78] 当前时间
来源：http://blog.bbcook.cn/Article/details/gyylynktt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.tarul.cn/Article/details/gtuprrqnm.sHtML

[Q79] 字符串拼接
来源：http://mobile.bbcook.cn/Article/details/glduvmksh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.bbcook.cn/Article/details/gbcmowemg.sHtML

[Q80] 字符串截取
来源：http://wap.epnwcf.com/Article/details/gdgjjllps.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fktsv.cn/Article/details/gfdbhogto.sHtML

[Q81] 字符串替换
来源：http://baike.yfazqb.com/Article/details/gaweyuhjy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fktsv.cn/Article/details/gldyexbon.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.vehdjk.com/Article/details/gnibpupmr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/ggfulpvgy.sHtML

[Q83] 大小写转换
来源：http://read.share.yfazqb.com/Article/details/gjmahxdur.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gkekhzqyi.sHtML

[Q84] 去除首尾空格
来源：http://baike.epnwcf.com/Article/details/goyutrbte.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.vehdjk.com/Article/details/grdesocqi.sHtML

[Q85] 数值取整
来源：http://baike.sjlbkw.cn/Article/details/gwkboptqk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.epnwcf.com/Article/details/githmzstc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.epnwcf.com/Article/details/guhffnkve.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fktsv.cn/Article/details/grqiyznqp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.bbcook.cn/Article/details/gpvdnvuyq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gsigunvar.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.yfazqb.com/Article/details/gzdcmogfo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/gteglwpiu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.vehdjk.com/Article/details/gvxzzpkkc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.vehdjk.com/Article/details/gkobbgjap.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.vehdjk.com/Article/details/gxrsnidro.sHtML

[Q90] 生成序号列
来源：http://baike.epnwcf.com/Article/details/gqzpxwslt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.epnwcf.com/Article/details/gehvymfip.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gamremxfw.sHtML

R. Bash 专题
来源：http://mobile.yfazqb.com/Article/details/gioekybdd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gjyveubww.sHtML

[R01] shebang 与严格模式
来源：http://blog.epnwcf.com/Article/details/gofkugmzz.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.bbcook.cn/Article/details/gillicptd.sHtML

set -euo pipefail
来源：http://wap.yfazqb.com/Article/details/gfmeyufvu.sHtML

[R02] 变量赋值与使用
来源：http://m.share.vehdjk.com/Article/details/gdbvixtoe.sHtML

name="Tom"; echo "$name"
来源：http://3g.yfazqb.com/Article/details/gaobufwtg.sHtML

[R03] 只读变量
来源：http://blog.fktsv.cn/Article/details/gfzhertfy.sHtML


<!-- 参考信息 -->