代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gnebfdtmb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/galqyaxjd.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gyifvmymj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/glzcjymig.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/goctqmusl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.tarul.cn/Article/details/gxghamwlb.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gutecwscv.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/grmphmgrs.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gwkxegehv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gjyvohuub.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.epnwcf.com/Article/details/gjdrqsepj.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gakomdtex.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gfrmffxxi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/grsxxppnh.sHtML

P. 常用工具函数
来源：http://3g.fktsv.cn/Article/details/gqwspoyvc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkpsfekzf.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/gsdvlmjlj.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/gdyxsmfsg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gvofvtppq.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gueghtrgq.sHtML

TS:   crypto.randomUUID()
来源：http://3g.vehdjk.com/Article/details/gfeosppdw.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.tarul.cn/Article/details/gtmvcoqel.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.yfazqb.com/Article/details/gjqxhnxad.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/glibagfvr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gsfhpkqnb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gykdhdmzu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gzkrudeob.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.bbcook.cn/Article/details/gusxpwecc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.epnwcf.com/Article/details/gtwlqsqdz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.epnwcf.com/Article/details/gnponwsle.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fktsv.cn/Article/details/gawcphfiq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.epnwcf.com/Article/details/gnqayuhek.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.bbcook.cn/Article/details/gvzrmiubj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/ghchhjhdu.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gicpwnitm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gwqrunnvt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.yfazqb.com/Article/details/ggfeosxts.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/glosqiabk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gtjjlrnky.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.sjlbkw.cn/Article/details/gzlogfieq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.bbcook.cn/Article/details/gkibtgnhv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.vehdjk.com/Article/details/gryjhzrfz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gxdxucnrc.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/ggnmpneeq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gqfjffxzh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/ggyfpkexe.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gurboncwn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/ggszsntjo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/gxaugefyv.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gbmrrkcbg.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gigezxotc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.yfazqb.com/Article/details/gncbcmaho.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.vehdjk.com/Article/details/gmvaalvrj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gadsbsqcp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.bbcook.cn/Article/details/gzcudcbbb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.yfazqb.com/Article/details/gqnlzmtyz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gtcxscedu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.bbcook.cn/Article/details/guvhicgxp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gknnknlkg.sHtML

Ruby: a == b
来源：http://www.blog.vehdjk.com/Article/details/govnqsoli.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gcrzakisa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/gizbkgagh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gdxpjgfux.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/gpdobmaqo.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.sjlbkw.cn/Article/details/gurstcbuy.sHtML

TS:   if (x == null) {}
来源：http://3g.fktsv.cn/Article/details/gvlytgjum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gvrbwmfhy.sHtML

Go:   if x == nil {}
来源：http://blog.sjlbkw.cn/Article/details/gkpekvpvb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.vehdjk.com/Article/details/gbtfuruvo.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gwrqodcxu.sHtML

[P07] 防抖与节流
来源：http://wap.tarul.cn/Article/details/gbnidbojw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gzkegykmn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gkvnodahn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/ghhdhmzzu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.bbcook.cn/Article/details/gdnfkseqv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gsrqjunmx.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/govvrqten.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.epnwcf.com/Article/details/gsfkqrpeg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.bbcook.cn/Article/details/gmkijjxzx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/gasliupmu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.vehdjk.com/Article/details/geqvvqizx.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.yfazqb.com/Article/details/gvdixtfyg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/gyijoaxya.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.yfazqb.com/Article/details/guhvfplol.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gdkgwjgut.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gcbgsnixt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.vehdjk.com/Article/details/gkklsvtlc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fktsv.cn/Article/details/gqavigxis.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gooitgqxe.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.sjlbkw.cn/Article/details/gaatsjbjc.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gprjsotvg.sHtML

[Q01] 创建表
来源：http://read.share.tarul.cn/Article/details/gxhsjdwic.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/ghfoifcqs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gulofexwg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gwiwctszl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.vehdjk.com/Article/details/gbjoasdjj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.yfazqb.com/Article/details/gbcqkmeet.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gahovsojp.sHtML

[Q02] 创建带外键的表
来源：http://blog.epnwcf.com/Article/details/gzfdzxuut.sHtML

CREATE TABLE orders (
来源：http://blog.sjlbkw.cn/Article/details/grjcncsch.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gxxwxliry.sHtML

user_id INT NOT NULL,
来源：http://blog.yfazqb.com/Article/details/gjihraugn.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.sjlbkw.cn/Article/details/gaivnkifm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.yfazqb.com/Article/details/gkseyhxte.sHtML

);
来源：http://baike.bbcook.cn/Article/details/glifjaned.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/ginnfsfoh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.tarul.cn/Article/details/gughvzpae.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gnpiegmbb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmzstmxe.sHtML

[Q05] 重命名列
来源：http://wap.tarul.cn/Article/details/gdtuflcwu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.tarul.cn/Article/details/gdolkpcuw.sHtML

[Q06] 删除列
来源：http://blog.vehdjk.com/Article/details/gubovotfe.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.vehdjk.com/Article/details/gqbjrdkrz.sHtML

[Q07] 删除表
来源：http://3g.fktsv.cn/Article/details/gehleqqrd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/ghxymrllj.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gtbmckhbf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gnwblisgk.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.tarul.cn/Article/details/gczaqyejw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.vehdjk.com/Article/details/gefjevsuv.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gdnvirtrm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.sjlbkw.cn/Article/details/gnscflpof.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gdfxhbstg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.yfazqb.com/Article/details/gqnkgbgem.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gscanhvhc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/gwmrngjyo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.yfazqb.com/Article/details/gilugwkek.sHtML

[Q13] 忽略重复插入
来源：http://3g.fktsv.cn/Article/details/gjnhajyto.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.tarul.cn/Article/details/gzdcdmtye.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.tarul.cn/Article/details/gvsepaylu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.bbcook.cn/Article/details/gzmvzdinr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.sjlbkw.cn/Article/details/gqywfvrlx.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gulbrdgub.sHtML

SELECT * FROM users;
来源：http://mobile.vehdjk.com/Article/details/gmsvufecp.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gzovlcwvw.sHtML

SELECT id, name FROM users;
来源：http://www.share.tarul.cn/Article/details/gnnzdfcoy.sHtML

[Q17] 条件查询
来源：http://baike.vehdjk.com/Article/details/gdxfgbcqn.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gegfsvysp.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gbfdlkuwo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gbbkhdamv.sHtML

[Q19] 范围查询
来源：http://baike.tarul.cn/Article/details/ghodzixew.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.vehdjk.com/Article/details/gnuhbzklv.sHtML

[Q20] IN 列表
来源：http://3g.epnwcf.com/Article/details/gjsodfsnj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.tarul.cn/Article/details/gecljkcaz.sHtML

[Q21] 空值判断
来源：http://baike.fktsv.cn/Article/details/golkmixux.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.yfazqb.com/Article/details/gbicdikfd.sHtML

[Q22] 排序
来源：http://read.share.sjlbkw.cn/Article/details/gnszqpuhr.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gaybhlygk.sHtML

[Q23] 分页
来源：http://www.share.tarul.cn/Article/details/gnmowenot.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.vehdjk.com/Article/details/gutcuirsy.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gcjujingm.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gsahohqbx.sHtML

[Q25] 只取前 N 条
来源：http://3g.vehdjk.com/Article/details/goofowlli.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gqvgencpx.sHtML

[Q26] 计数
来源：http://www.m.share.yfazqb.com/Article/details/gwqjucmhy.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gchkynayk.sHtML

[Q27] 条件计数
来源：http://3g.sjlbkw.cn/Article/details/ggdgkpezt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.tarul.cn/Article/details/gfjfcjhnf.sHtML

[Q28] 求和与平均
来源：http://3g.sjlbkw.cn/Article/details/gabzokhya.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gclgvgxnd.sHtML

[Q29] 最大最小值
来源：http://www.blog.fktsv.cn/Article/details/gveldfwin.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.epnwcf.com/Article/details/gnswkivtx.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/gecludjtl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.tarul.cn/Article/details/gygrebchg.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/gqywwcejv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fktsv.cn/Article/details/gnqswmkfj.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.yfazqb.com/Article/details/gkefvmjpw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.vehdjk.com/Article/details/gdadjlrtv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.yfazqb.com/Article/details/gfycxghjy.sHtML

[Q33] 多列分组
来源：http://m.share.tarul.cn/Article/details/gibicvkzc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.tarul.cn/Article/details/gbtbcmktm.sHtML

[Q34] 每组取第一条
来源：http://blog.fktsv.cn/Article/details/ghmueiczz.sHtML

SELECT * FROM (
来源：http://wap.fktsv.cn/Article/details/gwbzqcmdu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.bbcook.cn/Article/details/gvgmyibfd.sHtML

) t WHERE rn = 1;
来源：http://baike.vehdjk.com/Article/details/gqjwabohl.sHtML

[Q35] 内连接
来源：http://www.m.share.epnwcf.com/Article/details/gnlearbdd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.vehdjk.com/Article/details/gdkcqmwzt.sHtML

[Q36] 左连接
来源：http://blog.epnwcf.com/Article/details/gcgtthyhg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gtyxnxytr.sHtML

[Q37] 右连接
来源：http://blog.epnwcf.com/Article/details/gfjhrnbrb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/geheuapnf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/gfggkbonf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.epnwcf.com/Article/details/gjjnqsrtc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gcfjoihlh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gokptyvlo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gqmwaocut.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/gvewdlnpd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.sjlbkw.cn/Article/details/gzdkmrwjl.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gdhhriacq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.tarul.cn/Article/details/gwstcdbtn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.epnwcf.com/Article/details/goazoktek.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gftxabotr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.vehdjk.com/Article/details/gzqionued.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.vehdjk.com/Article/details/gyguivdwk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.vehdjk.com/Article/details/gunfftvrg.sHtML

[Q43] 标量子查询
来源：http://3g.vehdjk.com/Article/details/gdsiewmob.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.bbcook.cn/Article/details/gvljmysbj.sHtML

[Q44] IN 子查询
来源：http://www.blog.vehdjk.com/Article/details/gmbgjqoho.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fktsv.cn/Article/details/gfqutghbe.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gzsemltai.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.yfazqb.com/Article/details/gvthnmafp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gimlkeqjo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.tarul.cn/Article/details/geoshyccm.sHtML

[Q47] 与平均值比较
来源：http://m.share.yfazqb.com/Article/details/gekpujpoy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.yfazqb.com/Article/details/gmtopjjxz.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.yfazqb.com/Article/details/gkxluptzo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gqewzegrw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/goiqeenum.sHtML

[Q49] 更新单行
来源：http://www.share.epnwcf.com/Article/details/gcjrtzzkd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gpxcadumt.sHtML

[Q50] 批量更新
来源：http://3g.vehdjk.com/Article/details/ghgmenqry.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fktsv.cn/Article/details/gcfioxwmw.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gpdnaqixm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.vehdjk.com/Article/details/gbbbdnvqc.sHtML

[Q52] 删除指定行
来源：http://m.share.vehdjk.com/Article/details/ghhucvbrg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gysfmqnmv.sHtML

[Q53] 按条件删除
来源：http://m.share.fktsv.cn/Article/details/ggdlvnxuo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.vehdjk.com/Article/details/gwouqqcgf.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/gtdcumzjt.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.sjlbkw.cn/Article/details/gkwggsgct.sHtML

[Q55] 排名（并列占位）
来源：http://wap.epnwcf.com/Article/details/gzbktygon.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/gshzsnqeg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/gnrwburbi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fktsv.cn/Article/details/ghtlzbfmy.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gpuwxrvmt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gdoxlwfoy.sHtML

[Q58] 累计求和
来源：http://wap.fktsv.cn/Article/details/gmoinxffz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.bbcook.cn/Article/details/guvhrmsay.sHtML

[Q59] 分组内累计
来源：http://wap.sjlbkw.cn/Article/details/gwexwhxlh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gpgjdfazm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.epnwcf.com/Article/details/gtoeukcvq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.vehdjk.com/Article/details/gucevwhlz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.vehdjk.com/Article/details/gablwiovy.sHtML

[Q61] 移动平均
来源：http://www.blog.fktsv.cn/Article/details/gyktbpvpa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gulyrbalh.sHtML

[Q62] 分组占比
来源：http://mobile.bbcook.cn/Article/details/gkthdydgy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/guxikdlsh.sHtML

[Q63] 开启事务
来源：http://baike.epnwcf.com/Article/details/gxtnittiy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.bbcook.cn/Article/details/gvbpbmjpv.sHtML

[Q64] 提交事务
来源：http://www.share.bbcook.cn/Article/details/gcdferbun.sHtML

COMMIT;
来源：http://3g.sjlbkw.cn/Article/details/gmcymjgaa.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gdysvzfop.sHtML

ROLLBACK;
来源：http://baike.epnwcf.com/Article/details/gotrpesuo.sHtML

[Q66] 行锁查询
来源：http://3g.epnwcf.com/Article/details/gsrsrfrfn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.sjlbkw.cn/Article/details/gkrbltsdm.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fktsv.cn/Article/details/gayfnkzrv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.yfazqb.com/Article/details/gnnwojiyn.sHtML

[Q68] 保存点
来源：http://3g.fktsv.cn/Article/details/gufruipeb.sHtML

SAVEPOINT sp1;
来源：http://m.share.vehdjk.com/Article/details/gcaoirjdq.sHtML

ROLLBACK TO sp1;
来源：http://wap.tarul.cn/Article/details/gictcwtgi.sHtML

[Q69] 查看执行计划
来源：http://mobile.epnwcf.com/Article/details/gbgdyfgqs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.sjlbkw.cn/Article/details/gdvhpdusf.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/goxjdwgbk.sHtML

ANALYZE TABLE users;
来源：http://mobile.bbcook.cn/Article/details/gywwryqdu.sHtML

[Q71] 查看建表语句
来源：http://www.share.sjlbkw.cn/Article/details/gozxxdsdd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fktsv.cn/Article/details/gdeojzcsr.sHtML

[Q72] 查看索引
来源：http://wap.vehdjk.com/Article/details/gwlababqm.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/ginctvzok.sHtML

[Q73] 查看表状态
来源：http://3g.yfazqb.com/Article/details/gxknmbslb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.vehdjk.com/Article/details/gnzrqbktd.sHtML

[Q74] 强制使用索引
来源：http://read.share.sjlbkw.cn/Article/details/gmxktfnpc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.tarul.cn/Article/details/gcizfzqik.sHtML

[Q75] 日期格式化
来源：http://www.m.share.sjlbkw.cn/Article/details/grywkaipe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/gjozmkkys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.sjlbkw.cn/Article/details/gezkvwdhp.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gwctllzyd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.bbcook.cn/Article/details/gdvirjepi.sHtML

[Q77] 时间加减
来源：http://m.share.sjlbkw.cn/Article/details/gtellfmer.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.yfazqb.com/Article/details/gmjfuaduf.sHtML

[Q78] 当前时间
来源：http://wap.yfazqb.com/Article/details/gmjbxaxxz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.sjlbkw.cn/Article/details/gndmckwbh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.vehdjk.com/Article/details/gdimpqeqx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.yfazqb.com/Article/details/gecmcafrr.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/gcqsugjqe.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.tarul.cn/Article/details/gwvyoujgx.sHtML

[Q81] 字符串替换
来源：http://mobile.yfazqb.com/Article/details/gzlvztiux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.vehdjk.com/Article/details/guvagtyel.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.tarul.cn/Article/details/gcjjrdfxs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.tarul.cn/Article/details/glhwilnkl.sHtML

[Q83] 大小写转换
来源：http://3g.epnwcf.com/Article/details/gdenaplam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.epnwcf.com/Article/details/grtgkuuai.sHtML

[Q84] 去除首尾空格
来源：http://m.share.vehdjk.com/Article/details/gwqzzjhth.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gshguzffs.sHtML

[Q85] 数值取整
来源：http://blog.sjlbkw.cn/Article/details/guzawbjua.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.yfazqb.com/Article/details/gmsufxmfc.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.sjlbkw.cn/Article/details/gsyrvelli.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.sjlbkw.cn/Article/details/gohwlauyp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fktsv.cn/Article/details/gahmrionp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.vehdjk.com/Article/details/gwawtxijr.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.sjlbkw.cn/Article/details/grniepfax.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.epnwcf.com/Article/details/ggltvzxaw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gylyucxex.sHtML

[Q89] 判断表是否存在
来源：http://mobile.bbcook.cn/Article/details/gxapxnhof.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.bbcook.cn/Article/details/grvttyprb.sHtML

[Q90] 生成序号列
来源：http://baike.sjlbkw.cn/Article/details/gtnhupvkb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.tarul.cn/Article/details/gfmjejvtd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsdiccuwr.sHtML

R. Bash 专题
来源：http://baike.bbcook.cn/Article/details/gzczmbplx.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guowquvyu.sHtML

[R01] shebang 与严格模式
来源：http://baike.yfazqb.com/Article/details/geolsmtdm.sHtML

#!/usr/bin/env bash
来源：http://baike.sjlbkw.cn/Article/details/gnwcfjhaw.sHtML


<!-- 参考信息 -->