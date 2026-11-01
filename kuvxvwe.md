代发 wailian999

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gxqakoeyh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gbnkcuqds.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.tarul.cn/Article/details/gflcqwaqz.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/grhndnynh.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/grgfmijia.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gcnnkowdn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.yfazqb.com/Article/details/gpjlwimps.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/giurwiozm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/gstzkythn.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/giufhacit.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/gfnfroopy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gliyuoary.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.sjlbkw.cn/Article/details/gwhrhihkp.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gxrjtkdur.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gkyhtelhd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gwnyrhqtw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gsvspsklg.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/goaqslquh.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/gdltyjnha.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/gcbwlfkmc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gzjkzljaz.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gnimzjfgp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.vehdjk.com/Article/details/gpegbdluy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.vehdjk.com/Article/details/gudtanxmx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gganivttn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gypsajrro.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.epnwcf.com/Article/details/gtdczxkdm.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gmgozbqrc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gxykkgeso.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.yfazqb.com/Article/details/gfkexvfan.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/guufxfxxf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gdmazxijb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gpdvbjgsr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.bbcook.cn/Article/details/gtwandnuf.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gisyztxta.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gljgmipwo.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/gxndydzrt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gjulxeqic.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gcwiqnnqc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gwygbrmse.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/ghckizwxz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gjuhlgnse.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/gzgnnuybv.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/gduqjiori.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gbfilxrvx.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/ghupuaipx.sHtML

P. 常用工具函数
来源：http://blog.yfazqb.com/Article/details/gfghmfzyi.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/grhgnuwof.sHtML

[P01] 生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gnhdqvjrf.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.yfazqb.com/Article/details/gunuczlsb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gwdqnmhzy.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gawdiprhq.sHtML

TS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gkcwmobwp.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gqzggxerf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gfpiwesjt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/gkotznjtf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.epnwcf.com/Article/details/gurxpjncl.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gqzbvsghe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/gyplfeszl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gkaodxmcp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gdkxhjgbt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.epnwcf.com/Article/details/grnahvmgu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.yfazqb.com/Article/details/gzyaemnfw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.epnwcf.com/Article/details/glmjnnyfn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gepqsxnfu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/gkhjrydly.sHtML

[P03] 生成短随机字符串
来源：http://wap.yfazqb.com/Article/details/gfrvrhvtj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.epnwcf.com/Article/details/gjfpawrtj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gvgqbcfgi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gaqlfwazy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/ghqaykaiu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/gktuiepps.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fktsv.cn/Article/details/ghfvgkync.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/ggidpblim.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/gfhhigkyh.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gnkfcocrb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.fktsv.cn/Article/details/ganlzrjed.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gqtpqphmk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gkfvzgaiz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/ghoslmthk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/gwkisvrch.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.sjlbkw.cn/Article/details/gpboczynj.sHtML

Ruby: x.length;  x.size
来源：http://read.share.yfazqb.com/Article/details/gyuuqvoxw.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gihbkbzmp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.tarul.cn/Article/details/gqojhqzdf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.fktsv.cn/Article/details/gmgdrwhdj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.epnwcf.com/Article/details/gafxqllnn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.sjlbkw.cn/Article/details/gzsaklfwy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gmaykerxw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.fktsv.cn/Article/details/gfxqsfipm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gormnwgya.sHtML

Ruby: a == b
来源：http://baike.sjlbkw.cn/Article/details/gojgycusx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gvxjvhtwx.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.bbcook.cn/Article/details/gmarqvolp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.fktsv.cn/Article/details/gjvnqzsnx.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fktsv.cn/Article/details/gnuzkqstu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.sjlbkw.cn/Article/details/gkekjqhdh.sHtML

TS:   if (x == null) {}
来源：http://blog.sjlbkw.cn/Article/details/gnfistxqd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.epnwcf.com/Article/details/gyxvopsch.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gdsindohk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.vehdjk.com/Article/details/gjryukofn.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gxraahwut.sHtML

[P07] 防抖与节流
来源：http://www.share.yfazqb.com/Article/details/glprpcttu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.sjlbkw.cn/Article/details/gkfrncpev.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.vehdjk.com/Article/details/gcgtsypjp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gteotmhyf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gbwmeuwds.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.epnwcf.com/Article/details/gdzrjfzus.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.epnwcf.com/Article/details/ggzccblcz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.vehdjk.com/Article/details/gmzkxuezr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.vehdjk.com/Article/details/gkpxawnzg.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.yfazqb.com/Article/details/gwcabppje.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.vehdjk.com/Article/details/gjqdavuej.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqgfcqphs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fktsv.cn/Article/details/gorafwixs.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.yfazqb.com/Article/details/gjzecbodw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/gdtddcrox.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.vehdjk.com/Article/details/gjewgdwbu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.tarul.cn/Article/details/gqoyeepya.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.sjlbkw.cn/Article/details/gkcknicqa.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkbxgydun.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.yfazqb.com/Article/details/gujrchzpj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gigtvtlvc.sHtML

[Q01] 创建表
来源：http://m.share.yfazqb.com/Article/details/gfrgwgrsi.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/gfrwkwvsh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gcdtxevnw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gkqcdqrzo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gpyrquwwv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.epnwcf.com/Article/details/glrnaeitt.sHtML

);
来源：http://m.share.yfazqb.com/Article/details/gnglgmnhk.sHtML

[Q02] 创建带外键的表
来源：http://baike.epnwcf.com/Article/details/gunoszwnr.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/ggedsxfdq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gcaxjkfkk.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/ghuomzmfh.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.tarul.cn/Article/details/gfcurjrnf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gzmemybqn.sHtML

);
来源：http://blog.fktsv.cn/Article/details/gkpoldcgy.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gojdywuuz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gtfmoxpce.sHtML

[Q04] 修改列类型
来源：http://www.share.epnwcf.com/Article/details/gnwruhinl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.bbcook.cn/Article/details/gchhdbpdr.sHtML

[Q05] 重命名列
来源：http://read.share.yfazqb.com/Article/details/ghxyukdbi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.bbcook.cn/Article/details/gfaynyajo.sHtML

[Q06] 删除列
来源：http://m.share.fktsv.cn/Article/details/gauojigwh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gqohhvmig.sHtML

[Q07] 删除表
来源：http://blog.vehdjk.com/Article/details/gjudnzoum.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.vehdjk.com/Article/details/gcigfsjdv.sHtML

[Q08] 创建普通索引
来源：http://wap.sjlbkw.cn/Article/details/ghnufcswe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.tarul.cn/Article/details/gdigqpdyg.sHtML

[Q09] 创建唯一索引
来源：http://3g.yfazqb.com/Article/details/gyizoncoa.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gmplwmwjk.sHtML

[Q10] 插入单行
来源：http://baike.vehdjk.com/Article/details/grhampxgs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/grwmaueob.sHtML

[Q11] 一次插入多行
来源：http://blog.vehdjk.com/Article/details/gqifnmweg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gfactlsbf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.epnwcf.com/Article/details/gdsexwjpz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/gikoomoid.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/ggadvrqpm.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gcrcmqkrr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.bbcook.cn/Article/details/gahfpnchv.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fktsv.cn/Article/details/gdjrojixh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fktsv.cn/Article/details/gotcdoqir.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/gunhpkzoz.sHtML

[Q15] 查询全部
来源：http://mobile.tarul.cn/Article/details/gxrlfqzzs.sHtML

SELECT * FROM users;
来源：http://read.share.epnwcf.com/Article/details/gxxyxwzpt.sHtML

[Q16] 查询指定列
来源：http://3g.bbcook.cn/Article/details/gczebgwwy.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gifayulkx.sHtML

[Q17] 条件查询
来源：http://www.blog.bbcook.cn/Article/details/giwvvguiy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.sjlbkw.cn/Article/details/ghsobgeoe.sHtML

[Q18] 模糊匹配
来源：http://read.share.fktsv.cn/Article/details/gsctfhowq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/gkdiontvg.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gyzyvuucr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gviiyklxa.sHtML

[Q20] IN 列表
来源：http://m.share.tarul.cn/Article/details/gbguppwez.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/glhdfiken.sHtML

[Q21] 空值判断
来源：http://m.share.fktsv.cn/Article/details/gkgtxbdrt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gkmhjontn.sHtML

[Q22] 排序
来源：http://www.blog.yfazqb.com/Article/details/ggmhnzukt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.sjlbkw.cn/Article/details/gvcohwsmv.sHtML

[Q23] 分页
来源：http://mobile.tarul.cn/Article/details/ghlfkizic.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.vehdjk.com/Article/details/gvvcooduw.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/gfprbzxmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gmnnfbtfa.sHtML

[Q25] 只取前 N 条
来源：http://blog.epnwcf.com/Article/details/gudjqmpfv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gouvqcatq.sHtML

[Q26] 计数
来源：http://blog.yfazqb.com/Article/details/gvfalrfsj.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/gxwgkrlem.sHtML

[Q27] 条件计数
来源：http://m.share.fktsv.cn/Article/details/gchuxlldb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.bbcook.cn/Article/details/gcioobsch.sHtML

[Q28] 求和与平均
来源：http://www.blog.yfazqb.com/Article/details/gmfpeznav.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gztmnxakp.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fktsv.cn/Article/details/gbtagayxz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.vehdjk.com/Article/details/gfzoruusx.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/ghtexyqvo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/guddppjhv.sHtML

[Q31] 分组后过滤
来源：http://3g.sjlbkw.cn/Article/details/gviooergq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.vehdjk.com/Article/details/grcwtzxgp.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gfkjafvyl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gkryqxghu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.vehdjk.com/Article/details/gsffyzuxi.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gsqffgfmv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/gjyjkvwgd.sHtML

[Q34] 每组取第一条
来源：http://www.share.yfazqb.com/Article/details/ggzxztkej.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gygktsgjk.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/grpiagmki.sHtML

) t WHERE rn = 1;
来源：http://m.share.bbcook.cn/Article/details/gaygskjce.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gyhnbnein.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.sjlbkw.cn/Article/details/gqodltwdk.sHtML

[Q36] 左连接
来源：http://baike.vehdjk.com/Article/details/grusigcao.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gfnndhanu.sHtML

[Q37] 右连接
来源：http://3g.bbcook.cn/Article/details/geptxqlsr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fktsv.cn/Article/details/gktjyswlb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fktsv.cn/Article/details/gvgoaknzv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.sjlbkw.cn/Article/details/gxuhdcqjn.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.sjlbkw.cn/Article/details/gscrazdpa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.yfazqb.com/Article/details/gjhnuxkpv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/guqdjgjfq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gltxkarsu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gvmhlwkdc.sHtML

[Q41] 多表连接
来源：http://read.share.yfazqb.com/Article/details/gzvlsmhpr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.yfazqb.com/Article/details/gtfxxigaw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.bbcook.cn/Article/details/grubpuhyb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.vehdjk.com/Article/details/gmwqplfwy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fktsv.cn/Article/details/gpxvlhozn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.sjlbkw.cn/Article/details/grolzmcnj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/guvmukpwd.sHtML

[Q43] 标量子查询
来源：http://m.share.bbcook.cn/Article/details/gtihrlvba.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gnrtqdgzr.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/giblcvnlj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.bbcook.cn/Article/details/gmbqpwywx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gnwhbpdry.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.epnwcf.com/Article/details/ggvmlggrn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.tarul.cn/Article/details/gbslrtvkn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/gzxmbdjiz.sHtML

[Q47] 与平均值比较
来源：http://mobile.bbcook.cn/Article/details/gtmeeqmjo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.sjlbkw.cn/Article/details/gvyxzqtid.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.epnwcf.com/Article/details/ghihdrjxs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.yfazqb.com/Article/details/glngzuerb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.vehdjk.com/Article/details/gexhxneeg.sHtML

[Q49] 更新单行
来源：http://read.share.tarul.cn/Article/details/grhprmgqo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gcpfrgwhr.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/ghpwbewki.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/gxfxbrvtf.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/grpedaurd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gbhfozhvd.sHtML

[Q52] 删除指定行
来源：http://m.share.epnwcf.com/Article/details/gqshfqowl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.vehdjk.com/Article/details/glywlnvkf.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/gffqlhnna.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.bbcook.cn/Article/details/gmmtvjurl.sHtML

[Q54] 清空表
来源：http://wap.bbcook.cn/Article/details/ghyasngys.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.yfazqb.com/Article/details/gfmsdpbxz.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.sjlbkw.cn/Article/details/gkqlvzcby.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.tarul.cn/Article/details/gzfdsjejj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gyuinuxvo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gpekqobux.sHtML

[Q57] 行号
来源：http://www.share.epnwcf.com/Article/details/guajfurcq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fktsv.cn/Article/details/gqhrcaptl.sHtML

[Q58] 累计求和
来源：http://3g.yfazqb.com/Article/details/gkqhvlgiq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.yfazqb.com/Article/details/gyehuagex.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fktsv.cn/Article/details/gktmyejao.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gildbmsii.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fktsv.cn/Article/details/gxhukihut.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/ggjexsfdl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gxpmdqkuk.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/gapqoyuqk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gqqupicce.sHtML

[Q62] 分组占比
来源：http://www.m.share.bbcook.cn/Article/details/ghfhrluww.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/gwvbrxgrr.sHtML

[Q63] 开启事务
来源：http://www.blog.sjlbkw.cn/Article/details/gsbozvohj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gwqgiziin.sHtML

[Q64] 提交事务
来源：http://www.share.sjlbkw.cn/Article/details/gjmbjqkws.sHtML

COMMIT;
来源：http://www.blog.bbcook.cn/Article/details/gzpoctwbg.sHtML

[Q65] 回滚事务
来源：http://wap.epnwcf.com/Article/details/gdxjodaci.sHtML

ROLLBACK;
来源：http://wap.vehdjk.com/Article/details/gogybtxdt.sHtML

[Q66] 行锁查询
来源：http://www.share.vehdjk.com/Article/details/gbcgroqcb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.bbcook.cn/Article/details/ggctzynml.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.vehdjk.com/Article/details/gbgavphxo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.epnwcf.com/Article/details/gxrpdztzb.sHtML

[Q68] 保存点
来源：http://blog.vehdjk.com/Article/details/gelywkmdr.sHtML

SAVEPOINT sp1;
来源：http://mobile.vehdjk.com/Article/details/gqhpdnedn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.bbcook.cn/Article/details/ghxptghqe.sHtML

[Q69] 查看执行计划
来源：http://blog.yfazqb.com/Article/details/grstkyyfp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fktsv.cn/Article/details/gjhdnasbg.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fktsv.cn/Article/details/glaayzvyl.sHtML

ANALYZE TABLE users;
来源：http://3g.fktsv.cn/Article/details/gtazjkauo.sHtML

[Q71] 查看建表语句
来源：http://www.blog.vehdjk.com/Article/details/gkiwjcitd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.tarul.cn/Article/details/gvrwkzffi.sHtML

[Q72] 查看索引
来源：http://read.share.vehdjk.com/Article/details/grfrvdisq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.yfazqb.com/Article/details/goiyyybca.sHtML

[Q73] 查看表状态
来源：http://www.m.share.epnwcf.com/Article/details/gplbtihxp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.yfazqb.com/Article/details/gfswagshb.sHtML

[Q74] 强制使用索引
来源：http://mobile.sjlbkw.cn/Article/details/ghftujlnw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.epnwcf.com/Article/details/gaoapbdwt.sHtML

[Q75] 日期格式化
来源：http://baike.fktsv.cn/Article/details/gjfiwdvdn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.tarul.cn/Article/details/geuroskgk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.sjlbkw.cn/Article/details/gwdomzwlu.sHtML

[Q76] 按天统计
来源：http://read.share.epnwcf.com/Article/details/ggnblndkj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.bbcook.cn/Article/details/glqgddfcl.sHtML

[Q77] 时间加减
来源：http://www.share.tarul.cn/Article/details/ggodiqgah.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.yfazqb.com/Article/details/gwoycsjsr.sHtML


<!-- 参考信息 -->