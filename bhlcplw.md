代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gfwwhydbc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.epnwcf.com/Article/details/guzdtqjnn.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/ggqjitwvy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gkdhgzjfn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gmawxawtm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.bbcook.cn/Article/details/gbwbvghsf.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/grwzunhij.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.yfazqb.com/Article/details/gmysnqmrf.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gbqtycqeh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.tarul.cn/Article/details/gbvcomayq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/gninuaejd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/guvkazset.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.tarul.cn/Article/details/gewzlwveu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/ggvhrhxnu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.sjlbkw.cn/Article/details/gncxbcomp.sHtML

Ruby: // fork 块
来源：http://3g.vehdjk.com/Article/details/gntjggrab.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gnzeymmva.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gyyobdukn.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/gydianwxe.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gbtoqnkbd.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gclmnpcsw.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gsmnyomqh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.vehdjk.com/Article/details/ggowddnzu.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/godehowzt.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gcuajzaso.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gpbrjtikg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.sjlbkw.cn/Article/details/guhlxenlx.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/goxbejjsa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gjhnoxlwm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gkmffpymb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.epnwcf.com/Article/details/gespcupah.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fktsv.cn/Article/details/gwiuqduig.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gftgybcnx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.epnwcf.com/Article/details/gylbrcblx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.yfazqb.com/Article/details/gbqkekply.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gzinzfugz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gurfusalg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gmspciffn.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gbztwhxbz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/giviunzqe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.epnwcf.com/Article/details/gljhkzqzw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/goopyekax.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gnusonqir.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.vehdjk.com/Article/details/gaatrnelu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.epnwcf.com/Article/details/guowicjxr.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gxcazgwwh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.sjlbkw.cn/Article/details/gwrljkfkv.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gslaiuiui.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gqoluxxxc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gxjgksqix.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gcewjmoms.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/grwktihrl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gnywdqztt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gdgtmumxd.sHtML

Ruby: x.length;  x.size
来源：http://www.share.tarul.cn/Article/details/gnostdxte.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.tarul.cn/Article/details/gebdiqkmd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.bbcook.cn/Article/details/gsuezpgwv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/gzwzumqbp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/guuduqpwb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gspbtvytz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gadeegatp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.sjlbkw.cn/Article/details/guclxlevf.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.bbcook.cn/Article/details/gobtrvwah.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gvbnqgcac.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.vehdjk.com/Article/details/gzhithsyb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/guifvrcfl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fktsv.cn/Article/details/grfqwxnso.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.epnwcf.com/Article/details/gxskwcyur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.epnwcf.com/Article/details/gqkqlpzhz.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gdpevkqic.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gwlabsjgp.sHtML

Go:   if x == nil {}
来源：http://www.share.sjlbkw.cn/Article/details/gpwokaean.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gtbqzahhv.sHtML

C#:   if (x is null) {}
来源：http://wap.sjlbkw.cn/Article/details/gzvkdvdpw.sHtML

[P07] 防抖与节流
来源：http://www.blog.vehdjk.com/Article/details/gzhxdyahb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.vehdjk.com/Article/details/gisglkylt.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.sjlbkw.cn/Article/details/gploqnjtp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gatqqvbdx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gobtbziwt.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.epnwcf.com/Article/details/gjbmohmxm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdbgobmk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fktsv.cn/Article/details/gbrfwwais.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gxikdiqbh.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.yfazqb.com/Article/details/gdxnditzy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.yfazqb.com/Article/details/gjrpnklsn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.sjlbkw.cn/Article/details/gfcbsnddu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gajpkidbc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.vehdjk.com/Article/details/gacjnrvai.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gylycimel.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.bbcook.cn/Article/details/gmnkvuwmu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/glurhcjvs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.bbcook.cn/Article/details/gqkjxxmkj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/golewxplx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fktsv.cn/Article/details/gwktaihpt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gaqaypzyd.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gvflogktx.sHtML

CREATE TABLE users (
来源：http://wap.epnwcf.com/Article/details/gouvwtrci.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.vehdjk.com/Article/details/gcqocpoxn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gtchxpmdt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gmspservb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/ggvacqkif.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/geraasczr.sHtML

[Q02] 创建带外键的表
来源：http://www.share.bbcook.cn/Article/details/gjsjfxitz.sHtML

CREATE TABLE orders (
来源：http://m.share.yfazqb.com/Article/details/gqsxotwxq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gbbqdhpsc.sHtML

user_id INT NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gcclsltrt.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gxcqpjrbb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.tarul.cn/Article/details/ghwqczlnv.sHtML

);
来源：http://blog.yfazqb.com/Article/details/ggayrwiqs.sHtML

[Q03] 增加列
来源：http://wap.fktsv.cn/Article/details/gaszjwmae.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.yfazqb.com/Article/details/grqxslzrt.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gkifvolwx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gzaezhkmd.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/gjsibfqdt.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gsysfrapq.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/gorcugjec.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.sjlbkw.cn/Article/details/gpdsgspej.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/gjxmugjpx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.epnwcf.com/Article/details/gukbufhcu.sHtML

[Q08] 创建普通索引
来源：http://wap.yfazqb.com/Article/details/gonevtcwf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gizygecng.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.vehdjk.com/Article/details/gcgywrukj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gufqbuxqr.sHtML

[Q10] 插入单行
来源：http://mobile.bbcook.cn/Article/details/glbqygcsh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/glcidqaag.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.fktsv.cn/Article/details/glakhtize.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gabahdmpd.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.sjlbkw.cn/Article/details/gfldwudwb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fktsv.cn/Article/details/gmsehohgy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.sjlbkw.cn/Article/details/gtagiwvak.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/glfsowfmk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fktsv.cn/Article/details/gqsaryuvt.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.sjlbkw.cn/Article/details/gdfughmpn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.bbcook.cn/Article/details/gjfpyrlja.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.sjlbkw.cn/Article/details/gnwpbvglo.sHtML

[Q15] 查询全部
来源：http://3g.bbcook.cn/Article/details/gylwmtxqk.sHtML

SELECT * FROM users;
来源：http://baike.vehdjk.com/Article/details/gfyuhfrjc.sHtML

[Q16] 查询指定列
来源：http://www.share.fktsv.cn/Article/details/gaflizesc.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gaowmmqfb.sHtML

[Q17] 条件查询
来源：http://3g.tarul.cn/Article/details/gznztufyz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.bbcook.cn/Article/details/gtskcgtvr.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/ghksyarcv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gosgetqyy.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gzhbsibkv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gnphfvzhn.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gnbifoqeu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.vehdjk.com/Article/details/gzwmjiecj.sHtML

[Q21] 空值判断
来源：http://m.share.yfazqb.com/Article/details/gkbuofucd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.yfazqb.com/Article/details/gjimxytxy.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/grdvnegjq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.yfazqb.com/Article/details/gkdxiueag.sHtML

[Q23] 分页
来源：http://wap.tarul.cn/Article/details/gpvummyth.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.vehdjk.com/Article/details/gyenhaqlu.sHtML

[Q24] 去重
来源：http://wap.bbcook.cn/Article/details/gxdbvrqnl.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.tarul.cn/Article/details/girhvyjnh.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fktsv.cn/Article/details/glwhtwsco.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.epnwcf.com/Article/details/gfdjshvjg.sHtML

[Q26] 计数
来源：http://mobile.tarul.cn/Article/details/gffpdhhdr.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/gpehlnjzu.sHtML

[Q27] 条件计数
来源：http://wap.fktsv.cn/Article/details/gxdetuxeu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/grjcvkyuj.sHtML

[Q28] 求和与平均
来源：http://baike.fktsv.cn/Article/details/gnrjambgb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gufyjiasc.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gfpnpnbxb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.tarul.cn/Article/details/gdvukmltj.sHtML

[Q30] 分组统计
来源：http://m.share.bbcook.cn/Article/details/gusdxqcrn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gvfliwpim.sHtML

[Q31] 分组后过滤
来源：http://baike.yfazqb.com/Article/details/grgvikaut.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.bbcook.cn/Article/details/gelrgmoyh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fktsv.cn/Article/details/gqdogguze.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gnpsfnkkq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.yfazqb.com/Article/details/gtsnldavg.sHtML

[Q33] 多列分组
来源：http://www.blog.sjlbkw.cn/Article/details/ggpdnszmm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.yfazqb.com/Article/details/goriwfjyg.sHtML

[Q34] 每组取第一条
来源：http://baike.epnwcf.com/Article/details/gnchdykxh.sHtML

SELECT * FROM (
来源：http://read.share.fktsv.cn/Article/details/gfoswtybo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fktsv.cn/Article/details/gwlbzbatw.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gnwbpetwg.sHtML

[Q35] 内连接
来源：http://wap.yfazqb.com/Article/details/grafuexgp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/gfqpqpdzp.sHtML

[Q36] 左连接
来源：http://3g.yfazqb.com/Article/details/glnnqerlp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gwiyxiypw.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gwqvwewne.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/goakknpue.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.tarul.cn/Article/details/gdkvvbauw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.tarul.cn/Article/details/gfiacmovi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.vehdjk.com/Article/details/gvizbxqxh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.vehdjk.com/Article/details/gkxhiawcq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.tarul.cn/Article/details/gejjbfdxx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gjmbcrotq.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fktsv.cn/Article/details/gdffeeksd.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/gtyxndmsj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.yfazqb.com/Article/details/gutjbeaii.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.bbcook.cn/Article/details/glbjjpwbs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.sjlbkw.cn/Article/details/gbhpibgsw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.yfazqb.com/Article/details/gwfrvgues.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gykebfinb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/gmfvkrwvt.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/gkwgtvfjj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.bbcook.cn/Article/details/gpnnwnoot.sHtML

[Q44] IN 子查询
来源：http://m.share.sjlbkw.cn/Article/details/gkzhltbqq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.sjlbkw.cn/Article/details/gnrnpfgyc.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/gicmkqhka.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/glawjcuqs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.yfazqb.com/Article/details/gkpuahphh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gsiprutwd.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gtztgrgdp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/grdjcnele.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/ghwbzxgva.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gloeqtyoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/gftawfpho.sHtML

[Q49] 更新单行
来源：http://wap.yfazqb.com/Article/details/gszvfsqub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gevibbxnq.sHtML

[Q50] 批量更新
来源：http://3g.epnwcf.com/Article/details/gragceyvq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.yfazqb.com/Article/details/gmynjyygb.sHtML

[Q51] 用子查询更新
来源：http://3g.fktsv.cn/Article/details/gyzgmtcpw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fktsv.cn/Article/details/gpflpcgij.sHtML

[Q52] 删除指定行
来源：http://wap.tarul.cn/Article/details/gexaiblee.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.vehdjk.com/Article/details/gxcpurjqb.sHtML

[Q53] 按条件删除
来源：http://mobile.sjlbkw.cn/Article/details/gtorlclsx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.epnwcf.com/Article/details/gedjvdjjl.sHtML

[Q54] 清空表
来源：http://www.share.bbcook.cn/Article/details/gzikweniv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gsfhmvuzr.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.vehdjk.com/Article/details/gjvgliqgz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.bbcook.cn/Article/details/gaiyjcbao.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/gazlnuxnw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.epnwcf.com/Article/details/gyiieppix.sHtML

[Q57] 行号
来源：http://3g.bbcook.cn/Article/details/gjortbplj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.bbcook.cn/Article/details/gfrxuspdg.sHtML

[Q58] 累计求和
来源：http://blog.bbcook.cn/Article/details/gvptwyvja.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fktsv.cn/Article/details/gbodbtxjx.sHtML

[Q59] 分组内累计
来源：http://wap.vehdjk.com/Article/details/gnzdfqbfp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gcwwcahek.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.tarul.cn/Article/details/grkizandh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.bbcook.cn/Article/details/gfrqlcxii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gzkruwofk.sHtML

[Q61] 移动平均
来源：http://www.share.epnwcf.com/Article/details/gxscqbemc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fktsv.cn/Article/details/gscltyuoj.sHtML

[Q62] 分组占比
来源：http://wap.sjlbkw.cn/Article/details/gmeyivtqm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/grltlpgzw.sHtML

[Q63] 开启事务
来源：http://wap.tarul.cn/Article/details/gcdefmdgx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.epnwcf.com/Article/details/ggscbnhtu.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/galhyseki.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/gjeezccqv.sHtML

[Q65] 回滚事务
来源：http://blog.bbcook.cn/Article/details/gitjvwdcb.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gdvggfuxh.sHtML

[Q66] 行锁查询
来源：http://3g.bbcook.cn/Article/details/gjewtauey.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.bbcook.cn/Article/details/glidobcmj.sHtML

[Q67] 设置隔离级别
来源：http://blog.vehdjk.com/Article/details/gscprkduv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.vehdjk.com/Article/details/gnmqquamj.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gblwlltjb.sHtML

SAVEPOINT sp1;
来源：http://read.share.vehdjk.com/Article/details/gevpwjpnw.sHtML

ROLLBACK TO sp1;
来源：http://www.share.sjlbkw.cn/Article/details/ggnzdbbju.sHtML

[Q69] 查看执行计划
来源：http://mobile.sjlbkw.cn/Article/details/gxyqreyvj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.tarul.cn/Article/details/gxicbilga.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/gluvdqyhw.sHtML

ANALYZE TABLE users;
来源：http://baike.sjlbkw.cn/Article/details/gjsrvxbtt.sHtML

[Q71] 查看建表语句
来源：http://mobile.tarul.cn/Article/details/gicxypxjo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gkymzwkuh.sHtML

[Q72] 查看索引
来源：http://www.m.share.yfazqb.com/Article/details/gsbvkzanl.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gibugaoww.sHtML

[Q73] 查看表状态
来源：http://mobile.bbcook.cn/Article/details/gvopgixsl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.vehdjk.com/Article/details/gvczasves.sHtML

[Q74] 强制使用索引
来源：http://www.share.yfazqb.com/Article/details/gsbhtgvxx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.bbcook.cn/Article/details/gwyjcoaxo.sHtML

[Q75] 日期格式化
来源：http://mobile.bbcook.cn/Article/details/gxtmxavok.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/gexovnicr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.sjlbkw.cn/Article/details/gbhsfdqns.sHtML

[Q76] 按天统计
来源：http://mobile.yfazqb.com/Article/details/glkdpfgog.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fktsv.cn/Article/details/gykdzyvru.sHtML

[Q77] 时间加减
来源：http://www.m.share.vehdjk.com/Article/details/gdxwebyim.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fktsv.cn/Article/details/gpquivqpi.sHtML

[Q78] 当前时间
来源：http://www.m.share.fktsv.cn/Article/details/gfuvepzqa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gbrloqqkn.sHtML

[Q79] 字符串拼接
来源：http://mobile.tarul.cn/Article/details/gggcmrwfm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.yfazqb.com/Article/details/gefmdoygj.sHtML

[Q80] 字符串截取
来源：http://blog.fktsv.cn/Article/details/gkqrnndfy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.yfazqb.com/Article/details/gijxnvknb.sHtML

[Q81] 字符串替换
来源：http://m.share.tarul.cn/Article/details/gqsxvhkuz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gvmdkdekm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.bbcook.cn/Article/details/gqyxgtcwo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gcsfopgsb.sHtML

[Q83] 大小写转换
来源：http://3g.tarul.cn/Article/details/gktminqdj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gdzpisvbp.sHtML

[Q84] 去除首尾空格
来源：http://blog.sjlbkw.cn/Article/details/gtoifubtd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gztomrxue.sHtML

[Q85] 数值取整
来源：http://baike.bbcook.cn/Article/details/gzxrmksjq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.vehdjk.com/Article/details/gebkwwilj.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.sjlbkw.cn/Article/details/gzyuwwiyx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.bbcook.cn/Article/details/gvcxnnjbi.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.tarul.cn/Article/details/gesjiaxzj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.bbcook.cn/Article/details/gdqrishgn.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.epnwcf.com/Article/details/gdiutpaiy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.bbcook.cn/Article/details/geezknbtf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.vehdjk.com/Article/details/gfedjstku.sHtML

[Q89] 判断表是否存在
来源：http://wap.tarul.cn/Article/details/gxzpsnrpc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fktsv.cn/Article/details/gxihnsopp.sHtML

[Q90] 生成序号列
来源：http://read.share.yfazqb.com/Article/details/gfrqqxelg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.yfazqb.com/Article/details/gxtdguhqw.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gwxpwgauk.sHtML


<!-- 参考信息 -->