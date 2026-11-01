代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gmjqmiidk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/glbczmwag.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gvampxqga.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gzngohrhj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/gsqhchurj.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gkneljoqf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.yfazqb.com/Article/details/gnkbclozo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gppqunxye.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gitiochal.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtyhcxksk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gftrlwwva.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gxonhcdtg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.tarul.cn/Article/details/gicikonlv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gcfshpvej.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fktsv.cn/Article/details/grsxspwcm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gmufswhah.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gcqiblezd.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/goxehfsfj.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gyihldmnp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gwbhyhwfk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.bbcook.cn/Article/details/gotdkdzyj.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gchpfousg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gorhlzexe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gehqvupzv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gezmqlrya.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/ggspukqcr.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/ggkthcdtj.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.vehdjk.com/Article/details/gayrhojtk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/gyfkebbkv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.epnwcf.com/Article/details/gcsxctjmm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.yfazqb.com/Article/details/gwimpyxcp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/gqinorabp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/ggrsrubba.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gailczbtp.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gltpmcvor.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gnqkomldb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gzoacojuk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.vehdjk.com/Article/details/gqlbkefws.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gdcshxzna.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gnkwcypzw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.vehdjk.com/Article/details/gwnrongyf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/glzhomyhc.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gkllxzwgq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.epnwcf.com/Article/details/grlpjzaqe.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/gjppnecsf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.vehdjk.com/Article/details/gmddxccqx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/ghgxcatlz.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gmchbyygk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/grzcnbjao.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gupfkzeuv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/giudmblze.sHtML

Ruby: // fork 块
来源：http://www.blog.epnwcf.com/Article/details/giddijywg.sHtML

C#:   Parallel.For
来源：http://www.blog.epnwcf.com/Article/details/gipwevuxd.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/ggrxmzkzy.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gqlvtxcir.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gojegqkag.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gxppvzwjb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.epnwcf.com/Article/details/gfeiwjhkn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gyrfsndge.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/gmlmzauif.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gvmzjpwiy.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.bbcook.cn/Article/details/gedlqffjl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gfqmovhjn.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.bbcook.cn/Article/details/gwnyhqdob.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fktsv.cn/Article/details/gxofynvrw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/glfxbmnmr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.fktsv.cn/Article/details/geenzjhqr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/gihzgjgwz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/getcxtcsm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzpcjpvt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gmfigzkzf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/ghghqqauu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.vehdjk.com/Article/details/gfjvldnof.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gsielfhyg.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/ggdoktfey.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.vehdjk.com/Article/details/gwfjwyihf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.bbcook.cn/Article/details/goxwnvnwg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.bbcook.cn/Article/details/gpsavsuhj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fktsv.cn/Article/details/gzrqbuyjr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.sjlbkw.cn/Article/details/gqpzenkgd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gdjrjfexp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.yfazqb.com/Article/details/gztnmwjvw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gpfllicxr.sHtML

[P04] 求长度
来源：http://m.share.epnwcf.com/Article/details/gqifevpue.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/geomkqgpd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gdckpedru.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.tarul.cn/Article/details/gnbgxwyxa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.vehdjk.com/Article/details/gmcvqdpsq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.bbcook.cn/Article/details/guvzrcicg.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gnlszrdsl.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.epnwcf.com/Article/details/ggzhycaqg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.bbcook.cn/Article/details/gfantyclw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.bbcook.cn/Article/details/gjoluugxw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gheshblci.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/golseifvs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gtczkqcgs.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/gflnhbwbu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.vehdjk.com/Article/details/ggujgujsu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/grwdvbmez.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/goobexvoi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fktsv.cn/Article/details/gjnartmxa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gbcwolvcq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.tarul.cn/Article/details/geyzvsntr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gosnidwav.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/grplbapcj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/gzoukjeif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gfmhqfkoz.sHtML

Go:   if x == nil {}
来源：http://mobile.tarul.cn/Article/details/gzldvjfgj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gslxhhibp.sHtML

C#:   if (x is null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gsrbtkmcq.sHtML

[P07] 防抖与节流
来源：http://mobile.tarul.cn/Article/details/gduegyvpo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.tarul.cn/Article/details/goyzpgawn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.sjlbkw.cn/Article/details/gfmobwfum.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gyrfmlgep.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.bbcook.cn/Article/details/gdjoktjvl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/grexrurqf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.sjlbkw.cn/Article/details/gpovtzabs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.vehdjk.com/Article/details/guhfplyeo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.sjlbkw.cn/Article/details/gdcwbpktg.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fktsv.cn/Article/details/gzhquongg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.epnwcf.com/Article/details/gfbkxdjjc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.yfazqb.com/Article/details/gkhjdiias.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/grqbxffyy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gbnhalmuk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fktsv.cn/Article/details/gzrzomwll.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.yfazqb.com/Article/details/gvyqaoccu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/glrynalmq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.epnwcf.com/Article/details/gsoxoqvud.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gilkvdfeu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.bbcook.cn/Article/details/gnwxzcedd.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gstvvosop.sHtML

[Q01] 创建表
来源：http://wap.epnwcf.com/Article/details/grkdjjeqi.sHtML

CREATE TABLE users (
来源：http://www.share.fktsv.cn/Article/details/gztsdkvvp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.epnwcf.com/Article/details/gvaxmimky.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.sjlbkw.cn/Article/details/ghfchranv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gwvmdvgxv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.bbcook.cn/Article/details/gyrlijdmu.sHtML

);
来源：http://read.share.fktsv.cn/Article/details/guvqmthra.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/ggcyweijy.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gostminwb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/ggosziqjx.sHtML

user_id INT NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gvdodpqle.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.vehdjk.com/Article/details/goaurcxly.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/gohimnvrr.sHtML

);
来源：http://blog.sjlbkw.cn/Article/details/glodlplhk.sHtML

[Q03] 增加列
来源：http://mobile.sjlbkw.cn/Article/details/gdjpfrgnn.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gychinrqo.sHtML

[Q04] 修改列类型
来源：http://mobile.tarul.cn/Article/details/ggfqbvmdu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.epnwcf.com/Article/details/gjuryrluu.sHtML

[Q05] 重命名列
来源：http://mobile.fktsv.cn/Article/details/gwxhznxam.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/gsehvuaad.sHtML

[Q06] 删除列
来源：http://3g.epnwcf.com/Article/details/gfkwdobka.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gzogzqikl.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/ghlgppoul.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gmmetfbgf.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/ghtxahfnb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.fktsv.cn/Article/details/gvmtmidpv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.epnwcf.com/Article/details/gbjoehytq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gxibdlwks.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/grcnxgwko.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fktsv.cn/Article/details/gwhmsnezb.sHtML

[Q11] 一次插入多行
来源：http://3g.tarul.cn/Article/details/gopcdyhth.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gwlqsdlaj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.vehdjk.com/Article/details/gnmxkxrnl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.epnwcf.com/Article/details/gohimbvje.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.bbcook.cn/Article/details/gixoirbdf.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.yfazqb.com/Article/details/gehgflfgs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.tarul.cn/Article/details/glqxqbxxc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.vehdjk.com/Article/details/gulgunbqj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gguexmcyr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.sjlbkw.cn/Article/details/gbuvnduqv.sHtML

[Q15] 查询全部
来源：http://www.share.sjlbkw.cn/Article/details/gdigwvyun.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gylucahcw.sHtML

[Q16] 查询指定列
来源：http://m.share.epnwcf.com/Article/details/grvryperb.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmkvbxwnd.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gsiccmjvu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gvwnofhfv.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/giyzgvhre.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.vehdjk.com/Article/details/gksgjdtqc.sHtML

[Q19] 范围查询
来源：http://read.share.sjlbkw.cn/Article/details/gwlwduqjf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fktsv.cn/Article/details/glpkjzsqi.sHtML

[Q20] IN 列表
来源：http://www.blog.fktsv.cn/Article/details/gqxqthvse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/gefpstowi.sHtML

[Q21] 空值判断
来源：http://wap.sjlbkw.cn/Article/details/gnkdtzziy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.tarul.cn/Article/details/gmpphawgu.sHtML

[Q22] 排序
来源：http://read.share.bbcook.cn/Article/details/gjesteine.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gobwrjvlr.sHtML

[Q23] 分页
来源：http://baike.vehdjk.com/Article/details/grlfcvcty.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.yfazqb.com/Article/details/ggdxoyayf.sHtML

[Q24] 去重
来源：http://blog.bbcook.cn/Article/details/gnksqcwop.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gmhhumthm.sHtML

[Q25] 只取前 N 条
来源：http://www.share.sjlbkw.cn/Article/details/gvobhrpgf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/glkmosrzv.sHtML

[Q26] 计数
来源：http://mobile.sjlbkw.cn/Article/details/gdvciklgn.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.tarul.cn/Article/details/gjwljmpte.sHtML

[Q27] 条件计数
来源：http://m.share.epnwcf.com/Article/details/gnbhqnouw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.tarul.cn/Article/details/gvednxrpm.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gymnnrxuy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gkuxgasma.sHtML

[Q29] 最大最小值
来源：http://m.share.bbcook.cn/Article/details/gqwazvxih.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.bbcook.cn/Article/details/ggnalppid.sHtML

[Q30] 分组统计
来源：http://wap.epnwcf.com/Article/details/gxjkhrubx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gkscuhvvb.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/grrdazgjn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.tarul.cn/Article/details/gsbhwcohk.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gdrkggvjc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gvbccweqp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.vehdjk.com/Article/details/ggfvmuijv.sHtML

[Q33] 多列分组
来源：http://www.m.share.vehdjk.com/Article/details/gsdnxihfz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.bbcook.cn/Article/details/gvwmfytdw.sHtML

[Q34] 每组取第一条
来源：http://www.blog.vehdjk.com/Article/details/gqmawacuq.sHtML

SELECT * FROM (
来源：http://wap.epnwcf.com/Article/details/gnplbqzey.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.vehdjk.com/Article/details/gmtmnaiyn.sHtML

) t WHERE rn = 1;
来源：http://wap.sjlbkw.cn/Article/details/gjdeeuqdt.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gctngjket.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.epnwcf.com/Article/details/gfivofapr.sHtML

[Q36] 左连接
来源：http://www.m.share.tarul.cn/Article/details/gfvpbcvhu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.yfazqb.com/Article/details/geflldfre.sHtML

[Q37] 右连接
来源：http://mobile.vehdjk.com/Article/details/gfkywjsji.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fktsv.cn/Article/details/gxjesolbg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fktsv.cn/Article/details/gzcptdaze.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.vehdjk.com/Article/details/gwnxnsogv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/gectlwgng.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.vehdjk.com/Article/details/gnntynpll.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.yfazqb.com/Article/details/gntfiuisl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fktsv.cn/Article/details/grdayqtqb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fktsv.cn/Article/details/gyeqcjihm.sHtML

[Q41] 多表连接
来源：http://mobile.vehdjk.com/Article/details/glgswdgxw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.tarul.cn/Article/details/giqhysqap.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.vehdjk.com/Article/details/gdvgxjpri.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/grxngnhie.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gjzghzvtm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gvniyphdu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gldfwwtbc.sHtML

[Q43] 标量子查询
来源：http://www.share.vehdjk.com/Article/details/guxwrxubf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.tarul.cn/Article/details/gwqzotlfe.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gzavsfhjm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.vehdjk.com/Article/details/gjznryjel.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gonhwbbff.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqqsnxzxu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gieplpkdj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fktsv.cn/Article/details/gabotewxh.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gzueagpoz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.sjlbkw.cn/Article/details/gpjolzpip.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fktsv.cn/Article/details/gvovnsjnm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.epnwcf.com/Article/details/gtktmdsrv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/gdkiblokr.sHtML

[Q49] 更新单行
来源：http://www.share.sjlbkw.cn/Article/details/gzflfhzkp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gftysuazi.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gqxqatulp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.yfazqb.com/Article/details/gjuryowbd.sHtML

[Q51] 用子查询更新
来源：http://www.blog.yfazqb.com/Article/details/gontmrdyq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.sjlbkw.cn/Article/details/gtmoqjbrw.sHtML

[Q52] 删除指定行
来源：http://wap.bbcook.cn/Article/details/gwfpyufkm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gbpjwbjxk.sHtML

[Q53] 按条件删除
来源：http://baike.fktsv.cn/Article/details/gcfjwtlae.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.sjlbkw.cn/Article/details/gbmqvjlej.sHtML

[Q54] 清空表
来源：http://m.share.sjlbkw.cn/Article/details/ghsvspluy.sHtML

TRUNCATE TABLE logs;
来源：http://baike.epnwcf.com/Article/details/glaqvpzhr.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fktsv.cn/Article/details/gicxbiyfn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/gjvcoiref.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gmxevbmba.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.sjlbkw.cn/Article/details/gunnnuhtc.sHtML

[Q57] 行号
来源：http://www.m.share.tarul.cn/Article/details/gsxhrkguy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gdlgaongx.sHtML

[Q58] 累计求和
来源：http://m.share.sjlbkw.cn/Article/details/gwrremkxh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gfhdjcsbt.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gqiassvxq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.sjlbkw.cn/Article/details/grreklgsf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.sjlbkw.cn/Article/details/gwynhmyte.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.epnwcf.com/Article/details/goreqepkr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gujeufthp.sHtML

[Q61] 移动平均
来源：http://3g.tarul.cn/Article/details/gbegodnex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.yfazqb.com/Article/details/gbnzjtjoa.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gkhzvebpl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.yfazqb.com/Article/details/ghthrhdyj.sHtML

[Q63] 开启事务
来源：http://m.share.bbcook.cn/Article/details/gxlytdyze.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.sjlbkw.cn/Article/details/gdpgarvrs.sHtML

[Q64] 提交事务
来源：http://wap.bbcook.cn/Article/details/giqegzspe.sHtML

COMMIT;
来源：http://m.share.fktsv.cn/Article/details/gtbudhnsg.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/ghnnpckpc.sHtML

ROLLBACK;
来源：http://3g.vehdjk.com/Article/details/gcqjqahsx.sHtML

[Q66] 行锁查询
来源：http://3g.fktsv.cn/Article/details/gnkpxgcll.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.tarul.cn/Article/details/gwdgiuwle.sHtML

[Q67] 设置隔离级别
来源：http://baike.fktsv.cn/Article/details/guqomhehb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fktsv.cn/Article/details/glmcszftg.sHtML

[Q68] 保存点
来源：http://wap.tarul.cn/Article/details/ggdgesapv.sHtML

SAVEPOINT sp1;
来源：http://3g.yfazqb.com/Article/details/glalbhyyh.sHtML

ROLLBACK TO sp1;
来源：http://3g.epnwcf.com/Article/details/gqttyazpj.sHtML

[Q69] 查看执行计划
来源：http://m.share.epnwcf.com/Article/details/gvraivcmd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.sjlbkw.cn/Article/details/ggmtreomr.sHtML

[Q70] 更新统计信息
来源：http://baike.fktsv.cn/Article/details/grwlnstvj.sHtML

ANALYZE TABLE users;
来源：http://3g.bbcook.cn/Article/details/gkhenztdo.sHtML

[Q71] 查看建表语句
来源：http://www.share.vehdjk.com/Article/details/gzavmluqc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gcjhzkter.sHtML

[Q72] 查看索引
来源：http://www.share.fktsv.cn/Article/details/gbgnkzoed.sHtML

SHOW INDEX FROM users;
来源：http://www.share.epnwcf.com/Article/details/gexpmuizy.sHtML

[Q73] 查看表状态
来源：http://www.share.tarul.cn/Article/details/graytoyim.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.tarul.cn/Article/details/geimumfdf.sHtML

[Q74] 强制使用索引
来源：http://wap.bbcook.cn/Article/details/gotytqlrt.sHtML


<!-- 参考信息 -->