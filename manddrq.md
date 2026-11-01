代发 wailian999

TS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gvgcwxybc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gesfitggh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.tarul.cn/Article/details/gfgaabqyp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/guvviaida.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gfipyhqya.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.bbcook.cn/Article/details/gznonrbhc.sHtML

Py:   with lock: shared += 1
来源：http://m.share.tarul.cn/Article/details/gexqfjqkz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.epnwcf.com/Article/details/glgwphiun.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gcuaywuzi.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gnxuhdhoe.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gpewccfcj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gxoaxhgkc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.tarul.cn/Article/details/gfzwsnyje.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gugqbgqdf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gszxdkwej.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gyzwwudlw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/geqlhnguk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gvpiicwbi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gleykbohg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.bbcook.cn/Article/details/gtspcapew.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.epnwcf.com/Article/details/gkedqwnoh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/gtxueqfko.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/gfobjapfw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/ggaxyrvwb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.yfazqb.com/Article/details/gdkmelfqg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.tarul.cn/Article/details/gyhqudjss.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fktsv.cn/Article/details/gtwfseovx.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gujiltupl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gogzvaqbr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gbljgvgxs.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gliqqvldd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/glgwphnzg.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gjtywksja.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gwzlbxxaq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gwvghklla.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gofayeeig.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gsetwzemv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/gsdruiwgw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/guoyackaf.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gfnvfvdsg.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gphqtjgdz.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjxqmfcqf.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/grzgvzqho.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/godxyxccl.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gcwokmknr.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.yfazqb.com/Article/details/gywpkzfmx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/glrhxrqjd.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gibxhhfba.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gsaymtwvw.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/guxxkulsx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gvhrtnmin.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gamolztkm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/ghjuzargf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/gvgmjrcuz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.tarul.cn/Article/details/gtzwvkdru.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/gzbfvlyyd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/gcpbgnqcd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/gyoukopta.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/gtxmybnnm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gtverfgws.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gjktbdcre.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.bbcook.cn/Article/details/gfdrksgew.sHtML

[P03] 生成短随机字符串
来源：http://mobile.tarul.cn/Article/details/gpozxgdmr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.bbcook.cn/Article/details/gbawvazsa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/ghyuajsbp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gtyvwrshh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gpampqzpm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gaoyilzbz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gnbajbxzc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gkimnduun.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.epnwcf.com/Article/details/gkalkpfxm.sHtML

[P04] 求长度
来源：http://wap.fktsv.cn/Article/details/gzpqvgtop.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/ghhenikfd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gwuxmizwi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gpjhmheje.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/ghfxbwnye.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gzmxykill.sHtML

Go:   len(arr);  len(m)
来源：http://wap.epnwcf.com/Article/details/gylhvmbds.sHtML

Ruby: x.length;  x.size
来源：http://read.share.bbcook.cn/Article/details/gduwgabww.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.fktsv.cn/Article/details/geopeelnf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.tarul.cn/Article/details/gfvbzrqjk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fktsv.cn/Article/details/gzzvwgdpf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/gsenjtfkk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.fktsv.cn/Article/details/gmgomkwwe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfyvclta.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.epnwcf.com/Article/details/gnlfikjbp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/griawizrk.sHtML

Ruby: a == b
来源：http://read.share.epnwcf.com/Article/details/gcziaxxad.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.epnwcf.com/Article/details/gjksylqmi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.tarul.cn/Article/details/gtmcyppka.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/gpybsimfo.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gktdxozaw.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gzovmxipd.sHtML

TS:   if (x == null) {}
来源：http://read.share.sjlbkw.cn/Article/details/gwrvsanrz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/gojwubwdg.sHtML

Go:   if x == nil {}
来源：http://mobile.epnwcf.com/Article/details/gbqijreyu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gvwdzpmpq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.tarul.cn/Article/details/gmqyqfarw.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/gkaytofte.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gnplagvia.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gistnsiwy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gnxjgoixm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gidygvdam.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.yfazqb.com/Article/details/gvllxichc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.bbcook.cn/Article/details/gsrlgmivi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/gjlbqyaub.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gwtyzisie.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gcwhcuoly.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gtoqslntc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/ghbvkwwmv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/gphrwtqkt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gwnaqncfx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.sjlbkw.cn/Article/details/gtncbmxbr.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.vehdjk.com/Article/details/ggvoqennl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/geyskrnev.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.bbcook.cn/Article/details/gbzcuindw.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqxpzuiyg.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/gobpiujsp.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtgkyvcuw.sHtML

[Q01] 创建表
来源：http://mobile.epnwcf.com/Article/details/gslalhjqi.sHtML

CREATE TABLE users (
来源：http://www.blog.vehdjk.com/Article/details/gkqsjnchk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.bbcook.cn/Article/details/gujikndos.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.bbcook.cn/Article/details/grpdfgwin.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.tarul.cn/Article/details/gjnrcdguz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gpbzhsdec.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gdvyqyway.sHtML

[Q02] 创建带外键的表
来源：http://blog.tarul.cn/Article/details/gcemrxjkn.sHtML

CREATE TABLE orders (
来源：http://mobile.epnwcf.com/Article/details/gijpykgvd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gvttnvqyi.sHtML

user_id INT NOT NULL,
来源：http://m.share.sjlbkw.cn/Article/details/gtrolzxrx.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gizdgdmuf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.epnwcf.com/Article/details/giryoxwbj.sHtML

);
来源：http://mobile.sjlbkw.cn/Article/details/geawsququ.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gfqdctjca.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fktsv.cn/Article/details/gutlkdbbe.sHtML

[Q04] 修改列类型
来源：http://blog.fktsv.cn/Article/details/giclsqpcf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.fktsv.cn/Article/details/gqntbziek.sHtML

[Q05] 重命名列
来源：http://mobile.yfazqb.com/Article/details/gkxmwofvv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gsxoxhgen.sHtML

[Q06] 删除列
来源：http://www.blog.yfazqb.com/Article/details/gbipcuqhw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.tarul.cn/Article/details/gihhrvnhc.sHtML

[Q07] 删除表
来源：http://www.blog.sjlbkw.cn/Article/details/gpeyiuvwm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/gyemnfjly.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gxzscwbew.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/goipxffix.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gjqcqralg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.epnwcf.com/Article/details/gkwrtagpx.sHtML

[Q10] 插入单行
来源：http://www.share.epnwcf.com/Article/details/grgkefvor.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gggmvrqxo.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/ghqshgswa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gplvindiy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gggvaunuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.yfazqb.com/Article/details/gqnyenhic.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.yfazqb.com/Article/details/ggspysurb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fktsv.cn/Article/details/gtyaprdil.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.bbcook.cn/Article/details/ggowwprlq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.bbcook.cn/Article/details/gqxtevqma.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gnxrtxokj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fktsv.cn/Article/details/gljynacqw.sHtML

[Q15] 查询全部
来源：http://mobile.yfazqb.com/Article/details/gtnmtkcmw.sHtML

SELECT * FROM users;
来源：http://mobile.yfazqb.com/Article/details/gfcthiotn.sHtML

[Q16] 查询指定列
来源：http://m.share.tarul.cn/Article/details/gmurerhwl.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gamhhmvzu.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gjmkkgcia.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/goazdizsj.sHtML

[Q18] 模糊匹配
来源：http://www.blog.sjlbkw.cn/Article/details/gjzinuynx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gguwmmqtw.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gwilixzpv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fktsv.cn/Article/details/giglahtoy.sHtML

[Q20] IN 列表
来源：http://www.m.share.sjlbkw.cn/Article/details/gykxvwndc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/geohlgkba.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gerthhbrv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.sjlbkw.cn/Article/details/gaxajgxme.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gbmxxfqdz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/grfkaxnhv.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gjhytvsuh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fktsv.cn/Article/details/gnikzvxnb.sHtML

[Q24] 去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxhtuspu.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.yfazqb.com/Article/details/grxnwmbtb.sHtML

[Q25] 只取前 N 条
来源：http://baike.vehdjk.com/Article/details/gburemmxn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.vehdjk.com/Article/details/gaenfcmwj.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gxkarpnus.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gjhhzxitd.sHtML

[Q27] 条件计数
来源：http://m.share.vehdjk.com/Article/details/grdjjkbhb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gvxwnycos.sHtML

[Q28] 求和与平均
来源：http://www.share.fktsv.cn/Article/details/gwgwzomzy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.bbcook.cn/Article/details/ghtzskcsu.sHtML

[Q29] 最大最小值
来源：http://baike.tarul.cn/Article/details/gnmxrubus.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gzhyeblhz.sHtML

[Q30] 分组统计
来源：http://mobile.vehdjk.com/Article/details/gvdcgdlnm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/ggxjawunp.sHtML

[Q31] 分组后过滤
来源：http://mobile.bbcook.cn/Article/details/gmxfyarsi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.vehdjk.com/Article/details/gmmscrusp.sHtML

[Q32] 分组拼接字符串
来源：http://wap.yfazqb.com/Article/details/gotseadkq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gspzejdph.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.epnwcf.com/Article/details/gcqtgwuvc.sHtML

[Q33] 多列分组
来源：http://3g.sjlbkw.cn/Article/details/gyiyralij.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fktsv.cn/Article/details/gxlopkotm.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/gezsaigjp.sHtML

SELECT * FROM (
来源：http://baike.bbcook.cn/Article/details/gbglfgmoi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.bbcook.cn/Article/details/gkiuixmgw.sHtML

) t WHERE rn = 1;
来源：http://www.share.vehdjk.com/Article/details/gqfpfuoxq.sHtML

[Q35] 内连接
来源：http://m.share.epnwcf.com/Article/details/gvoufbxvu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.tarul.cn/Article/details/gwmsgwulq.sHtML

[Q36] 左连接
来源：http://read.share.yfazqb.com/Article/details/gjfwgrfef.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/grkmkujpt.sHtML

[Q37] 右连接
来源：http://wap.epnwcf.com/Article/details/grynleugh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fktsv.cn/Article/details/guohidyja.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.yfazqb.com/Article/details/gpkirtjde.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/gygdqqxpd.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.epnwcf.com/Article/details/gavmxjict.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.yfazqb.com/Article/details/gzbbcvann.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.vehdjk.com/Article/details/glwpyczqp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fktsv.cn/Article/details/goiesajjn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.bbcook.cn/Article/details/gfhatktcy.sHtML

[Q41] 多表连接
来源：http://wap.bbcook.cn/Article/details/gfwmhtrry.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.epnwcf.com/Article/details/gkspjniuo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fktsv.cn/Article/details/gipqfzjoq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.vehdjk.com/Article/details/gtabzxflx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gcujhekxp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.bbcook.cn/Article/details/gengundij.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fktsv.cn/Article/details/gjdqpqcay.sHtML

[Q43] 标量子查询
来源：http://www.share.epnwcf.com/Article/details/gadgtbadg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.vehdjk.com/Article/details/gserbtvts.sHtML

[Q44] IN 子查询
来源：http://wap.yfazqb.com/Article/details/gxdepyleo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.epnwcf.com/Article/details/gjavlhvyr.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fktsv.cn/Article/details/ggwxwoorl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.sjlbkw.cn/Article/details/gbcpxipnu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/gnevmkldf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.epnwcf.com/Article/details/gzwarvqyc.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gbvhtcaif.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.yfazqb.com/Article/details/gffdugufk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.tarul.cn/Article/details/gqqzdvwop.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/gqlmnxvww.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/glhobhkpt.sHtML

[Q49] 更新单行
来源：http://www.share.yfazqb.com/Article/details/gvoatdjky.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.epnwcf.com/Article/details/gydcerqhn.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gcubbksmp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gjzbespwq.sHtML

[Q51] 用子查询更新
来源：http://wap.tarul.cn/Article/details/gfetzmznf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.vehdjk.com/Article/details/gkjwexmrm.sHtML

[Q52] 删除指定行
来源：http://www.blog.epnwcf.com/Article/details/gjtmikfkz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gwmurloog.sHtML

[Q53] 按条件删除
来源：http://m.share.sjlbkw.cn/Article/details/gihahrpmb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/guxvrpglx.sHtML

[Q54] 清空表
来源：http://3g.sjlbkw.cn/Article/details/gzpetqeft.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gqmfsufem.sHtML

[Q55] 排名（并列占位）
来源：http://wap.sjlbkw.cn/Article/details/grootcizj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.tarul.cn/Article/details/glvptsncw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.yfazqb.com/Article/details/gxdhqpaai.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/grnnnwmda.sHtML

[Q57] 行号
来源：http://mobile.fktsv.cn/Article/details/gaisynqno.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.bbcook.cn/Article/details/gukdmfktt.sHtML

[Q58] 累计求和
来源：http://m.share.vehdjk.com/Article/details/gqlpyxjkk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gsdsmtxru.sHtML

[Q59] 分组内累计
来源：http://wap.yfazqb.com/Article/details/gbhoxqqys.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gnxvozgon.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.yfazqb.com/Article/details/gcealyqoj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gdmhiogin.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gqsggfxbt.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gbkbkhqfd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gfcnusiud.sHtML

[Q62] 分组占比
来源：http://m.share.bbcook.cn/Article/details/gjdqpzeqb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.bbcook.cn/Article/details/gkuptjegj.sHtML

[Q63] 开启事务
来源：http://3g.sjlbkw.cn/Article/details/gzvbtqnhs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.bbcook.cn/Article/details/gjehwokdt.sHtML

[Q64] 提交事务
来源：http://www.blog.tarul.cn/Article/details/grgfbynnf.sHtML

COMMIT;
来源：http://www.m.share.epnwcf.com/Article/details/gecbpkwts.sHtML

[Q65] 回滚事务
来源：http://read.share.tarul.cn/Article/details/gvbclrlsk.sHtML

ROLLBACK;
来源：http://mobile.tarul.cn/Article/details/gjpithyop.sHtML

[Q66] 行锁查询
来源：http://wap.sjlbkw.cn/Article/details/gvrklpyra.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.yfazqb.com/Article/details/ggfxhhljc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.vehdjk.com/Article/details/goejtifjn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/gwsjkuiwm.sHtML

[Q68] 保存点
来源：http://www.m.share.vehdjk.com/Article/details/gfihkodzl.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fktsv.cn/Article/details/gpfajspkg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gwotbxujr.sHtML

[Q69] 查看执行计划
来源：http://baike.yfazqb.com/Article/details/ggbjefjdg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.epnwcf.com/Article/details/gksjnzpgf.sHtML

[Q70] 更新统计信息
来源：http://3g.vehdjk.com/Article/details/gdektmgpf.sHtML

ANALYZE TABLE users;
来源：http://www.share.vehdjk.com/Article/details/gbdkcmkrt.sHtML

[Q71] 查看建表语句
来源：http://blog.vehdjk.com/Article/details/gznjjlgag.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.bbcook.cn/Article/details/gtbmwuuwe.sHtML

[Q72] 查看索引
来源：http://3g.fktsv.cn/Article/details/gbqnuowpu.sHtML

SHOW INDEX FROM users;
来源：http://3g.sjlbkw.cn/Article/details/gfdmpbdku.sHtML

[Q73] 查看表状态
来源：http://3g.vehdjk.com/Article/details/gjxgbqqhr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.epnwcf.com/Article/details/glevnxeab.sHtML

[Q74] 强制使用索引
来源：http://wap.vehdjk.com/Article/details/geuwswjci.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.yfazqb.com/Article/details/gsnkmjalh.sHtML

[Q75] 日期格式化
来源：http://3g.yfazqb.com/Article/details/gqbfoiyzw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gbnozuzjy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.epnwcf.com/Article/details/gmcoergou.sHtML

[Q76] 按天统计
来源：http://blog.sjlbkw.cn/Article/details/glmfwlons.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/gxbhigrlp.sHtML

[Q77] 时间加减
来源：http://read.share.sjlbkw.cn/Article/details/gvbycqecq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fktsv.cn/Article/details/gvwtrkglk.sHtML

[Q78] 当前时间
来源：http://baike.vehdjk.com/Article/details/giqqtcnki.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.yfazqb.com/Article/details/gtyuynois.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gdcktethf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fktsv.cn/Article/details/ggjpzqsjo.sHtML


<!-- 参考信息 -->