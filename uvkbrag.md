代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gdeuefzqu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.epnwcf.com/Article/details/gbkotyznl.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/ggtskqqdq.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.sjlbkw.cn/Article/details/gmmflgtaz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.sjlbkw.cn/Article/details/gmjbwvmsi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gwbxjccky.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gxrudnoxt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/gulkaswhe.sHtML

[O06] 使用进程池
来源：http://mobile.sjlbkw.cn/Article/details/gzifameer.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gndpjtdoa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.epnwcf.com/Article/details/gywlvzbcq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/guomgyerl.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gioewfmfe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gxmmkjczo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/giipecpzz.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gmhrgytkp.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/gzahzmslq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glokyniuk.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/guzqzseaw.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/geripqrcn.sHtML

[P01] 生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/geutgoqfs.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/guabnhegn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gukfybuff.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gzkwhjjbn.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gbgthswfx.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/gsteeokwh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.sjlbkw.cn/Article/details/ggqudccyu.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.epnwcf.com/Article/details/gbrfgkiuk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.yfazqb.com/Article/details/gpyvpkxgl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fktsv.cn/Article/details/gfufwkopn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gylsnjmio.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gtjmcibom.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.tarul.cn/Article/details/goqxljpkc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gupcdsxws.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gynmbuivn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.sjlbkw.cn/Article/details/gguvauqte.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gyhfngbrc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gwbmkwali.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gzipzgqwb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.yfazqb.com/Article/details/gyvxmwvgi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fktsv.cn/Article/details/glbrlpkwz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gcxwrlboy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gzcxrivfw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gkgkdetjn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gcrblglph.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/gtbfkewbx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gskgcgnaa.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/gfoobhvxz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gtarwqnfn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.yfazqb.com/Article/details/gsbmygthk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/ghrmrecni.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.epnwcf.com/Article/details/ggotuukpa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.epnwcf.com/Article/details/gkfmamrda.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/goihvpjkw.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.sjlbkw.cn/Article/details/gyolrbuwh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.sjlbkw.cn/Article/details/gmzqroimb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gzvsxzkpr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.bbcook.cn/Article/details/gcwrpsngf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.sjlbkw.cn/Article/details/gcisyjjis.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.bbcook.cn/Article/details/gkhnnpcmv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gunjmxsle.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.yfazqb.com/Article/details/gtybmydoc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gnvgvcaok.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/ghrlzqgbg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.tarul.cn/Article/details/gfvekqdvj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gimjttgvb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.epnwcf.com/Article/details/ghkrtlote.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.vehdjk.com/Article/details/gzzexwdhr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/gcjldymnk.sHtML

TS:   if (x == null) {}
来源：http://3g.yfazqb.com/Article/details/ggtgyhbwv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/guwpfulyb.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gcxdddhax.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gmguaiumx.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/gykyzedca.sHtML

[P07] 防抖与节流
来源：http://read.share.fktsv.cn/Article/details/ggqtwnbzs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.epnwcf.com/Article/details/gaxebceas.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.bbcook.cn/Article/details/ghtjrdmia.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gmsasmgxc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/grfqfulza.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gemhqpxal.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.yfazqb.com/Article/details/gbqbbqubi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fktsv.cn/Article/details/gqdidzdgt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gpxvqcgsh.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.epnwcf.com/Article/details/gvsuwmrne.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.sjlbkw.cn/Article/details/grcnrtwki.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.sjlbkw.cn/Article/details/grhulsbol.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.bbcook.cn/Article/details/giacclgbv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fktsv.cn/Article/details/gjgoaxtpz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.yfazqb.com/Article/details/gcrcketif.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.bbcook.cn/Article/details/gyzydklpx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.yfazqb.com/Article/details/gsepawlrp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.yfazqb.com/Article/details/gtmkipxrh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gpawhaqxh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.vehdjk.com/Article/details/gjmxdxoag.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbunjdodt.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/glcffpblq.sHtML

CREATE TABLE users (
来源：http://m.share.epnwcf.com/Article/details/gpicnypcm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.bbcook.cn/Article/details/gfbtwvenv.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gbaxyycwe.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.sjlbkw.cn/Article/details/gmjvytcwb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.sjlbkw.cn/Article/details/gvivejduh.sHtML

);
来源：http://3g.tarul.cn/Article/details/gcwqcprur.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.epnwcf.com/Article/details/ghtgutoiq.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/guqsfodtc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fktsv.cn/Article/details/gchtswtfd.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gwgnbhalv.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gcfreqvzk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.vehdjk.com/Article/details/gtsfrhwfz.sHtML

);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaaspjsst.sHtML

[Q03] 增加列
来源：http://m.share.vehdjk.com/Article/details/ggcdfwwuz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.vehdjk.com/Article/details/gcbdiboec.sHtML

[Q04] 修改列类型
来源：http://www.share.yfazqb.com/Article/details/gnsjvemjw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.vehdjk.com/Article/details/gclktulpn.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gntmoovur.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.vehdjk.com/Article/details/giqzafaax.sHtML

[Q06] 删除列
来源：http://m.share.yfazqb.com/Article/details/gtltszqhk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fktsv.cn/Article/details/gzqebllpp.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/ghrkkcdps.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.yfazqb.com/Article/details/gslzrjtgo.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/glgpbojda.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fktsv.cn/Article/details/gelhknjqo.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/gfxijhqiv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gtvxomzrz.sHtML

[Q10] 插入单行
来源：http://read.share.fktsv.cn/Article/details/gukofvswh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.bbcook.cn/Article/details/ggadwibov.sHtML

[Q11] 一次插入多行
来源：http://baike.sjlbkw.cn/Article/details/gphesmmvz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gdykyqeuq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.tarul.cn/Article/details/gztcrseyk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/gaknjelmo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gqwnmwiqc.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gojydfgsj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gaczlrage.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.vehdjk.com/Article/details/gquxwvdmg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.bbcook.cn/Article/details/glwmozdmx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/gqyvpnxtg.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gofatzbqt.sHtML

SELECT * FROM users;
来源：http://blog.bbcook.cn/Article/details/gejjbtcjq.sHtML

[Q16] 查询指定列
来源：http://www.m.share.vehdjk.com/Article/details/gegofucto.sHtML

SELECT id, name FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/grpwdrdgx.sHtML

[Q17] 条件查询
来源：http://blog.vehdjk.com/Article/details/gcmjfndop.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gnfpltqxq.sHtML

[Q18] 模糊匹配
来源：http://read.share.bbcook.cn/Article/details/gtnldnxkq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.tarul.cn/Article/details/gmujuxcbf.sHtML

[Q19] 范围查询
来源：http://www.m.share.vehdjk.com/Article/details/gdpisfkje.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.sjlbkw.cn/Article/details/gihrpqwoi.sHtML

[Q20] IN 列表
来源：http://wap.tarul.cn/Article/details/glrovpvmq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gysputpnq.sHtML

[Q21] 空值判断
来源：http://read.share.tarul.cn/Article/details/gyjouxdlr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.bbcook.cn/Article/details/gaawfqvdn.sHtML

[Q22] 排序
来源：http://3g.bbcook.cn/Article/details/goqhkzill.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/ghuuewyms.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/gmuqiwwzp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmwlqlqu.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gyrpvgqjg.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.tarul.cn/Article/details/gpmklbpnb.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gvvsqxqru.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gzxwrhakw.sHtML

[Q26] 计数
来源：http://read.share.sjlbkw.cn/Article/details/grdjozpqx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/goygdzcwo.sHtML

[Q27] 条件计数
来源：http://www.blog.bbcook.cn/Article/details/gwxabgniq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.tarul.cn/Article/details/gojhkyvhw.sHtML

[Q28] 求和与平均
来源：http://m.share.bbcook.cn/Article/details/gtvzgkqda.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gmnzstwdc.sHtML

[Q29] 最大最小值
来源：http://www.blog.epnwcf.com/Article/details/gncrpuotp.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.tarul.cn/Article/details/gfkjwenns.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gqalnoenk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gabbfxiam.sHtML

[Q31] 分组后过滤
来源：http://baike.tarul.cn/Article/details/gxyiabksp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.epnwcf.com/Article/details/groarqdpd.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/ggwctlpsa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/goiwwkumg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.epnwcf.com/Article/details/goucjylbu.sHtML

[Q33] 多列分组
来源：http://www.share.epnwcf.com/Article/details/gdahfzajp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.vehdjk.com/Article/details/gfbeebybh.sHtML

[Q34] 每组取第一条
来源：http://read.share.sjlbkw.cn/Article/details/gahvhsdnp.sHtML

SELECT * FROM (
来源：http://read.share.sjlbkw.cn/Article/details/grduhrzxr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.tarul.cn/Article/details/gpsixbops.sHtML

) t WHERE rn = 1;
来源：http://www.blog.bbcook.cn/Article/details/geyogawkx.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/gedzuntvg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/goxssqqea.sHtML

[Q36] 左连接
来源：http://www.m.share.sjlbkw.cn/Article/details/glbtmohmu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gustccfpo.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/gvipnhlqi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/geoqnrfxx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fktsv.cn/Article/details/gpeothfej.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/gvbnnbslg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/gdyzvifwv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fktsv.cn/Article/details/goqrfzrfa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.epnwcf.com/Article/details/gvkyltblj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.sjlbkw.cn/Article/details/gxtpdbdqz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/glgoxxnoy.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/grjgpuadj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.yfazqb.com/Article/details/gwfxlpxnq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.epnwcf.com/Article/details/ggysscsuq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.yfazqb.com/Article/details/gswdwulfy.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.vehdjk.com/Article/details/gneqbesnk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fktsv.cn/Article/details/gpggcukkw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.bbcook.cn/Article/details/gylumcbiv.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gfbwapuwd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.epnwcf.com/Article/details/gxygcaaee.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gajfiurrx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.yfazqb.com/Article/details/gsuvfwuuj.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/giqsncprs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.epnwcf.com/Article/details/ghzbwrfkf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gsitgtavr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gsazeimgw.sHtML

[Q47] 与平均值比较
来源：http://read.share.vehdjk.com/Article/details/grwwrnjyc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.bbcook.cn/Article/details/gejnzgjqw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/gvgwfceyn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fktsv.cn/Article/details/gknwodtgq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fktsv.cn/Article/details/gwapfrarw.sHtML

[Q49] 更新单行
来源：http://mobile.sjlbkw.cn/Article/details/gbsrvcwgi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/glodjninx.sHtML

[Q50] 批量更新
来源：http://3g.bbcook.cn/Article/details/glthnnxdb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.epnwcf.com/Article/details/gqvwujium.sHtML

[Q51] 用子查询更新
来源：http://3g.epnwcf.com/Article/details/gnmafjwau.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.sjlbkw.cn/Article/details/geylbsuee.sHtML

[Q52] 删除指定行
来源：http://wap.epnwcf.com/Article/details/gzmvxngux.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.bbcook.cn/Article/details/gozihnnzq.sHtML

[Q53] 按条件删除
来源：http://baike.epnwcf.com/Article/details/gnmrfkkaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fktsv.cn/Article/details/gevxydnue.sHtML

[Q54] 清空表
来源：http://mobile.sjlbkw.cn/Article/details/gqgcrlylh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gulcjmaui.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.sjlbkw.cn/Article/details/gcarajihp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.bbcook.cn/Article/details/gtwliuuyp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.tarul.cn/Article/details/gtwdpodwi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.tarul.cn/Article/details/geymghvwj.sHtML

[Q57] 行号
来源：http://www.m.share.vehdjk.com/Article/details/ghvdoiiym.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gsubgnfko.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gbubxwowl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gouujtvsa.sHtML

[Q59] 分组内累计
来源：http://wap.fktsv.cn/Article/details/gzkkjmsnv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gacaalxex.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gyuqfesiu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.yfazqb.com/Article/details/gsdriqtpr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.tarul.cn/Article/details/glasioeva.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gppiospev.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gixkptubq.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/gldpnjilz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gfyntkiwq.sHtML

[Q63] 开启事务
来源：http://www.m.share.vehdjk.com/Article/details/gxoaxngza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.epnwcf.com/Article/details/gtfqvkmvi.sHtML

[Q64] 提交事务
来源：http://m.share.sjlbkw.cn/Article/details/gfhhdkuji.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/gkrotzkhm.sHtML

[Q65] 回滚事务
来源：http://www.m.share.epnwcf.com/Article/details/gxcuzokpu.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/gjyvmhzct.sHtML

[Q66] 行锁查询
来源：http://mobile.tarul.cn/Article/details/ggpjsdwqe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.sjlbkw.cn/Article/details/gtntxxzqi.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.vehdjk.com/Article/details/gxezrsovt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.yfazqb.com/Article/details/gdjjsprny.sHtML

[Q68] 保存点
来源：http://baike.bbcook.cn/Article/details/gpzzlvgff.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.yfazqb.com/Article/details/geeevlema.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.vehdjk.com/Article/details/gpmfsqrbk.sHtML

[Q69] 查看执行计划
来源：http://wap.sjlbkw.cn/Article/details/ggnljdilw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.vehdjk.com/Article/details/gkuxfmqoh.sHtML

[Q70] 更新统计信息
来源：http://wap.bbcook.cn/Article/details/gjwxszmga.sHtML

ANALYZE TABLE users;
来源：http://read.share.vehdjk.com/Article/details/gnmduzema.sHtML

[Q71] 查看建表语句
来源：http://3g.tarul.cn/Article/details/gewbpraxh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gpadaacbn.sHtML

[Q72] 查看索引
来源：http://www.blog.yfazqb.com/Article/details/gpohvcyzz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gxqosskiy.sHtML

[Q73] 查看表状态
来源：http://read.share.sjlbkw.cn/Article/details/gxzwpxipw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.bbcook.cn/Article/details/grkmagtyi.sHtML

[Q74] 强制使用索引
来源：http://3g.yfazqb.com/Article/details/gatnpkcfy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.epnwcf.com/Article/details/ghaabizcd.sHtML

[Q75] 日期格式化
来源：http://read.share.yfazqb.com/Article/details/ghgjaovsu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.yfazqb.com/Article/details/gaijwoljj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.sjlbkw.cn/Article/details/gbzcelnkv.sHtML

[Q76] 按天统计
来源：http://wap.epnwcf.com/Article/details/gfrnzubao.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.yfazqb.com/Article/details/gyhizvhyj.sHtML

[Q77] 时间加减
来源：http://m.share.vehdjk.com/Article/details/glhzgndci.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.yfazqb.com/Article/details/gvmprrxey.sHtML

[Q78] 当前时间
来源：http://read.share.tarul.cn/Article/details/gcgkslfub.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.sjlbkw.cn/Article/details/gamqxissv.sHtML

[Q79] 字符串拼接
来源：http://blog.yfazqb.com/Article/details/gjsgpadcm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fktsv.cn/Article/details/gqwikrlhe.sHtML

[Q80] 字符串截取
来源：http://www.share.sjlbkw.cn/Article/details/gsvuyqocl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gleqtzgkn.sHtML

[Q81] 字符串替换
来源：http://www.share.vehdjk.com/Article/details/genkhgnye.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.bbcook.cn/Article/details/gkvoocnzy.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.yfazqb.com/Article/details/gftsjyybb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fktsv.cn/Article/details/guiqxozzk.sHtML

[Q83] 大小写转换
来源：http://mobile.vehdjk.com/Article/details/glvioloia.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.yfazqb.com/Article/details/gcvrwalql.sHtML

[Q84] 去除首尾空格
来源：http://m.share.epnwcf.com/Article/details/gvvzyldml.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.yfazqb.com/Article/details/glvmfpesw.sHtML

[Q85] 数值取整
来源：http://www.m.share.vehdjk.com/Article/details/ggixdylcv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.yfazqb.com/Article/details/gurcrowua.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.bbcook.cn/Article/details/gobwyvrdy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.yfazqb.com/Article/details/gkeabwqvr.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.yfazqb.com/Article/details/gdabsmiwi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fktsv.cn/Article/details/gqiojbjel.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fktsv.cn/Article/details/gorxvycyd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.tarul.cn/Article/details/ghemvfore.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.yfazqb.com/Article/details/gdlujylxb.sHtML

[Q89] 判断表是否存在
来源：http://blog.vehdjk.com/Article/details/gokduoptw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.tarul.cn/Article/details/gsjhshtbe.sHtML

[Q90] 生成序号列
来源：http://m.share.sjlbkw.cn/Article/details/godvgmtbt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.bbcook.cn/Article/details/gsshvmmct.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gafqhpmfa.sHtML


<!-- 参考信息 -->