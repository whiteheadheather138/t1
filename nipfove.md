代发 wailian999

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.epnwcf.com/Article/details/gjivxhfdo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.tarul.cn/Article/details/gqghjlzda.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gtdiaryvd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.tarul.cn/Article/details/gmgadamoc.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gkmyvdlrw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/geonpdupu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gpayzugkv.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/grpviwbfq.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gfvydacno.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gflxnqbnc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gqxuytfnl.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/grnbdhfvb.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gsspbgrrg.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gxkihusqa.sHtML

P. 常用工具函数
来源：http://wap.vehdjk.com/Article/details/gpwaqbvap.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gffraoydk.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gkmkjmogp.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/ghbeqcuvw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/gcxsrkhqz.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/gapfntedu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/ggvqhcgwy.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.yfazqb.com/Article/details/gpenfgoqx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gctwxqsco.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.fktsv.cn/Article/details/gpulosagw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fktsv.cn/Article/details/gdaflndzy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gycwanowe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fktsv.cn/Article/details/gzojswwgk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gnilvfocp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.vehdjk.com/Article/details/gtzijbmwm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.epnwcf.com/Article/details/gbpcdljki.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gihtldwxc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/ghqvqoqjp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fktsv.cn/Article/details/gdzuitvlw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gxqjdnvxf.sHtML

[P03] 生成短随机字符串
来源：http://blog.bbcook.cn/Article/details/gqdzqejue.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.tarul.cn/Article/details/gswgvzplr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.epnwcf.com/Article/details/gpbnphwzv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gvhklpxup.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/gzypkrlqw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.vehdjk.com/Article/details/gxglhopkm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.yfazqb.com/Article/details/gohufhrsb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/gaotdulju.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/geekgbcdi.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gktcqxmov.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.yfazqb.com/Article/details/gnjfuozwv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/giubopyhc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gmtvntsdt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gpbgusykb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/glgqrryrc.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.yfazqb.com/Article/details/gwysfftcs.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/grrfmdmej.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gswttdbxm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.yfazqb.com/Article/details/giblcssbn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.yfazqb.com/Article/details/glrfuteux.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gmthylimw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.vehdjk.com/Article/details/gvojidiwk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gsxyotcow.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/gniyxzvzc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.fktsv.cn/Article/details/gbcfdfxkb.sHtML

Ruby: a == b
来源：http://www.blog.sjlbkw.cn/Article/details/gbnzpzgmx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.vehdjk.com/Article/details/gjkwwmdwg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.epnwcf.com/Article/details/gtanqgght.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.tarul.cn/Article/details/gusehjthg.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/ggccfyvms.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/gjxvnudqb.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/gjygletwr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gpcektnae.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/guswcqrjj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.tarul.cn/Article/details/ggtdvegwl.sHtML

C#:   if (x is null) {}
来源：http://mobile.epnwcf.com/Article/details/gblvxqsmt.sHtML

[P07] 防抖与节流
来源：http://3g.bbcook.cn/Article/details/ghtsssjsj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.vehdjk.com/Article/details/givgparxc.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/glwpgsbce.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gmbyqjrmv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/ggqvivbes.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfueuilus.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/govlslqet.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.tarul.cn/Article/details/grjmgheik.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.bbcook.cn/Article/details/gvxsnklvk.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.vehdjk.com/Article/details/gvhqnbftj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.epnwcf.com/Article/details/gjetsslvp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/gqdfaqwxo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.bbcook.cn/Article/details/gocbpggug.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.tarul.cn/Article/details/gcqmixmyh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.tarul.cn/Article/details/gcpoqlcxb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.tarul.cn/Article/details/gbgfnjpbw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fktsv.cn/Article/details/gkdtwtcjz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.sjlbkw.cn/Article/details/gfjfnugzx.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/guhnjvudy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gfujbtzrq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gvbtwntnl.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/gnklecrng.sHtML

CREATE TABLE users (
来源：http://read.share.tarul.cn/Article/details/gcpboruyz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/ghboygize.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.yfazqb.com/Article/details/gptkyynem.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/gqfouywba.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.vehdjk.com/Article/details/gcikylxih.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gomcpghwl.sHtML

[Q02] 创建带外键的表
来源：http://read.share.bbcook.cn/Article/details/glrvqwbee.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/gdlsluqop.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gbnkxdkcb.sHtML

user_id INT NOT NULL,
来源：http://mobile.epnwcf.com/Article/details/golryvqsv.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.sjlbkw.cn/Article/details/ghoyvjoue.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/goledjwli.sHtML

);
来源：http://3g.tarul.cn/Article/details/gsclkbdgp.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/gjenyqgeo.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.epnwcf.com/Article/details/grqoixttk.sHtML

[Q04] 修改列类型
来源：http://read.share.bbcook.cn/Article/details/gfyqdzmog.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.vehdjk.com/Article/details/gxeogigsm.sHtML

[Q05] 重命名列
来源：http://wap.vehdjk.com/Article/details/gyhcnktuf.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.vehdjk.com/Article/details/gaawbtvdx.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gturwanzp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.epnwcf.com/Article/details/gusmhjpkk.sHtML

[Q07] 删除表
来源：http://wap.bbcook.cn/Article/details/grrrbrahi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gfxwqwvka.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/grhnbwbqj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gboptaycm.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.sjlbkw.cn/Article/details/gcwgbofle.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.tarul.cn/Article/details/gkwogjtwo.sHtML

[Q10] 插入单行
来源：http://wap.epnwcf.com/Article/details/gzcxkmsjy.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/grnpqsdla.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/ghlpjetgc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/ghhohyqkk.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gnikxxwwa.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gtzchtfcn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.bbcook.cn/Article/details/glchbgwsg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/gsbepamnj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/guqjybkzl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/ghbhwbuta.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.tarul.cn/Article/details/gzkiqdumz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.tarul.cn/Article/details/gpsnhpnpn.sHtML

[Q15] 查询全部
来源：http://www.share.tarul.cn/Article/details/gjrmglkfo.sHtML

SELECT * FROM users;
来源：http://www.share.fktsv.cn/Article/details/gpqzvnixe.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gbwkdudva.sHtML

SELECT id, name FROM users;
来源：http://read.share.vehdjk.com/Article/details/grlwlfviw.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/giixbikcc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.epnwcf.com/Article/details/gjjyghalh.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gwogujcrx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gzrvwqrzt.sHtML

[Q19] 范围查询
来源：http://read.share.vehdjk.com/Article/details/gzrpzjzbx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.vehdjk.com/Article/details/gfnvyiwfx.sHtML

[Q20] IN 列表
来源：http://blog.tarul.cn/Article/details/gpiowducm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.vehdjk.com/Article/details/gkwldcshv.sHtML

[Q21] 空值判断
来源：http://www.m.share.epnwcf.com/Article/details/gejtykqzm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fktsv.cn/Article/details/ghwccqtef.sHtML

[Q22] 排序
来源：http://www.blog.sjlbkw.cn/Article/details/gchxhtfqm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.sjlbkw.cn/Article/details/gdlxqoqgf.sHtML

[Q23] 分页
来源：http://www.blog.bbcook.cn/Article/details/gngkswzhy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gordcfjev.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gwvqjdkwg.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkjbfjjuv.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gykefpptk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gfwdtrtnz.sHtML

[Q26] 计数
来源：http://3g.tarul.cn/Article/details/gejawebqn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gskvorkgh.sHtML

[Q27] 条件计数
来源：http://read.share.bbcook.cn/Article/details/gcdsaorkl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.tarul.cn/Article/details/gciamzwlu.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gjexeiixf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gmkhtpihx.sHtML

[Q29] 最大最小值
来源：http://www.m.share.epnwcf.com/Article/details/geaaihkod.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fktsv.cn/Article/details/gmkbnimtg.sHtML

[Q30] 分组统计
来源：http://www.m.share.fktsv.cn/Article/details/gkjpwbbva.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.epnwcf.com/Article/details/giylgeogw.sHtML

[Q31] 分组后过滤
来源：http://read.share.fktsv.cn/Article/details/gptrvtzpi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gikwvnhye.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gzkkwioue.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gtbtbyczy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.epnwcf.com/Article/details/gawuafnqi.sHtML

[Q33] 多列分组
来源：http://www.share.tarul.cn/Article/details/gfasczvah.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.epnwcf.com/Article/details/gflrafrvy.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gvsjysgpi.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gdetxalqa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/gckjcpoid.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gtaevzrio.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/giqwgwmzv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gfeyhrskr.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/gtdqlnaoh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gbgarcjwk.sHtML

[Q37] 右连接
来源：http://m.share.sjlbkw.cn/Article/details/gkrzmtpxm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.vehdjk.com/Article/details/ghvcstpbn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.yfazqb.com/Article/details/gdapgdasu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.yfazqb.com/Article/details/gzufzcyzn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/grwkybaoe.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gdrdaipzb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/ggnzvflfq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.vehdjk.com/Article/details/gnpfagxuh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.vehdjk.com/Article/details/gabgxdiou.sHtML

[Q41] 多表连接
来源：http://www.share.bbcook.cn/Article/details/grthmqpbh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.yfazqb.com/Article/details/gobdbjnii.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.sjlbkw.cn/Article/details/gjcmblvzw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gvmssgghk.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/ghsntecqx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gegdvrery.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/gjdhvgetx.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gyumpbwpz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gbputiupu.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fktsv.cn/Article/details/gjcvcesdk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.tarul.cn/Article/details/gadaodhyi.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gxtsavyea.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/goszkbbkh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.epnwcf.com/Article/details/gzdlwvbof.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gwumcbrlu.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/gqbcjckih.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gryhdqwna.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gjqdqqmfy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gpthjywvf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.yfazqb.com/Article/details/gzkgmmwqe.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/gajizjjqz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gadepttao.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gklfkzvsn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fktsv.cn/Article/details/ggqnorysc.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gamabcfss.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gdjujbhlv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.vehdjk.com/Article/details/ghhmyamga.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/gtayzqryt.sHtML

[Q53] 按条件删除
来源：http://baike.tarul.cn/Article/details/gcxbtttqh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fktsv.cn/Article/details/gowneunlz.sHtML

[Q54] 清空表
来源：http://blog.fktsv.cn/Article/details/grycemldr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.sjlbkw.cn/Article/details/ggrwyhbvt.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/gjscldbhq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gvdibfpln.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.sjlbkw.cn/Article/details/guymhxbeo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.sjlbkw.cn/Article/details/grhkfqmob.sHtML

[Q57] 行号
来源：http://blog.vehdjk.com/Article/details/gfkhlafqx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.tarul.cn/Article/details/gonobshwt.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/gzotdldax.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/ggllpuvth.sHtML

[Q59] 分组内累计
来源：http://wap.bbcook.cn/Article/details/guickajex.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gmfpqptaz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/gcwnykhkn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.yfazqb.com/Article/details/ghwodsdej.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gqgrfyxru.sHtML

[Q61] 移动平均
来源：http://baike.fktsv.cn/Article/details/gbaeidvqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gabbgsjax.sHtML

[Q62] 分组占比
来源：http://3g.sjlbkw.cn/Article/details/ggxvlziia.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gzvntmcnv.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gwhismnkq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gauutuptq.sHtML

[Q64] 提交事务
来源：http://wap.yfazqb.com/Article/details/gkywoxruh.sHtML

COMMIT;
来源：http://www.blog.sjlbkw.cn/Article/details/giltrtpas.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gxsszjdwc.sHtML

ROLLBACK;
来源：http://3g.sjlbkw.cn/Article/details/gqxejqqcf.sHtML

[Q66] 行锁查询
来源：http://m.share.bbcook.cn/Article/details/gdonsbevq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fktsv.cn/Article/details/girzdjhvm.sHtML

[Q67] 设置隔离级别
来源：http://baike.vehdjk.com/Article/details/gbxjgdbxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.epnwcf.com/Article/details/gurjwelrg.sHtML

[Q68] 保存点
来源：http://www.blog.sjlbkw.cn/Article/details/gtxaktuyy.sHtML

SAVEPOINT sp1;
来源：http://mobile.tarul.cn/Article/details/gewtgaghy.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.bbcook.cn/Article/details/gpbgiwprw.sHtML

[Q69] 查看执行计划
来源：http://mobile.bbcook.cn/Article/details/gxscclfwo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.epnwcf.com/Article/details/gnguhmjcb.sHtML

[Q70] 更新统计信息
来源：http://m.share.vehdjk.com/Article/details/guzygebng.sHtML

ANALYZE TABLE users;
来源：http://3g.sjlbkw.cn/Article/details/gskefyoje.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fktsv.cn/Article/details/gsrtamlha.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.vehdjk.com/Article/details/ginerplws.sHtML

[Q72] 查看索引
来源：http://read.share.bbcook.cn/Article/details/ggiiwilvx.sHtML

SHOW INDEX FROM users;
来源：http://read.share.epnwcf.com/Article/details/gfgelscfj.sHtML

[Q73] 查看表状态
来源：http://mobile.tarul.cn/Article/details/gfqgsshsa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fktsv.cn/Article/details/gjpefabdk.sHtML

[Q74] 强制使用索引
来源：http://wap.tarul.cn/Article/details/gyzencdsz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.epnwcf.com/Article/details/ghntfcpnj.sHtML

[Q75] 日期格式化
来源：http://www.blog.bbcook.cn/Article/details/gjuyisizv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.yfazqb.com/Article/details/gswlpijiq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.tarul.cn/Article/details/gnvwzvqwp.sHtML

[Q76] 按天统计
来源：http://3g.sjlbkw.cn/Article/details/gsduuslaw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.vehdjk.com/Article/details/ggpvjvicr.sHtML

[Q77] 时间加减
来源：http://baike.tarul.cn/Article/details/guwjahfbp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.sjlbkw.cn/Article/details/gnebohqdz.sHtML

[Q78] 当前时间
来源：http://wap.fktsv.cn/Article/details/gpnhjjwnd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.bbcook.cn/Article/details/gfajvosjk.sHtML

[Q79] 字符串拼接
来源：http://www.share.yfazqb.com/Article/details/gehgbdvlj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.epnwcf.com/Article/details/gwdxhvlhj.sHtML

[Q80] 字符串截取
来源：http://baike.fktsv.cn/Article/details/gofkmbhxw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/guhvrlmcg.sHtML

[Q81] 字符串替换
来源：http://read.share.yfazqb.com/Article/details/gvqoerhgv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gupieislc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.yfazqb.com/Article/details/gntmpnrpg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.bbcook.cn/Article/details/gpfklctvs.sHtML

[Q83] 大小写转换
来源：http://mobile.epnwcf.com/Article/details/ggdqscmrz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/giyjaiuko.sHtML

[Q84] 去除首尾空格
来源：http://baike.sjlbkw.cn/Article/details/gdbchedvg.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gafaoirhm.sHtML

[Q85] 数值取整
来源：http://baike.vehdjk.com/Article/details/gmxglbran.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.sjlbkw.cn/Article/details/gwuuczxmx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fktsv.cn/Article/details/grsxerrlz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.epnwcf.com/Article/details/gzfclgpbv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.sjlbkw.cn/Article/details/gzxnavwyt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.sjlbkw.cn/Article/details/gkhnukjgf.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.yfazqb.com/Article/details/gyltqyhpv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.sjlbkw.cn/Article/details/gnkkfwtyc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.epnwcf.com/Article/details/glsbfrvww.sHtML

[Q89] 判断表是否存在
来源：http://mobile.epnwcf.com/Article/details/gkocsduto.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.vehdjk.com/Article/details/gjqddthqt.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gcrthfwbz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.bbcook.cn/Article/details/gfyhxdfvm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnmekraru.sHtML

R. Bash 专题
来源：http://m.share.fktsv.cn/Article/details/gyvpdeghu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gpjwsjpvq.sHtML

[R01] shebang 与严格模式
来源：http://mobile.epnwcf.com/Article/details/gfwkndbak.sHtML

#!/usr/bin/env bash
来源：http://3g.bbcook.cn/Article/details/ggwdmxnye.sHtML


<!-- 参考信息 -->