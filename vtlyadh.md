代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.tarul.cn/Article/details/gczkimhqk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.tarul.cn/Article/details/gzeegyfhf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gpsdpferv.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gjxalhgab.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/ggbourocp.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gbwgfyzkb.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gnjmvexfs.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/gpdkgsbdj.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gpdrnjhlm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/gazqfczts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/guyiqketq.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/gcufnlbam.sHtML

TS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gfjughgaj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.epnwcf.com/Article/details/gfnpznqym.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.epnwcf.com/Article/details/gubvbcrzb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.tarul.cn/Article/details/gjykfvvgr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fktsv.cn/Article/details/gnlbdkyxh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gkzdgnljg.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fktsv.cn/Article/details/gccmyfwpj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gkowuownu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.sjlbkw.cn/Article/details/gjxkvtvub.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gtbmxnfbt.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnomfcykp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/gwialgdue.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/ggxdxeini.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gfqozchxh.sHtML

[O04] 定义异步函数并等待
来源：http://blog.yfazqb.com/Article/details/gndvrqkmc.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gfwbcdxqf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/grivztaqb.sHtML

JS:   async function f() { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gbkovzqah.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gwjoqoxat.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/gskeszfkr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.vehdjk.com/Article/details/grrhohqxn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmbzjgey.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/gnvnvrwot.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.sjlbkw.cn/Article/details/gvmajdlbe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.bbcook.cn/Article/details/gojdxgbvs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.bbcook.cn/Article/details/gibjxghfn.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gebiqoykh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gjdlbyjna.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gwvyzryeo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gckaepzmd.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/ghhyzzfii.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.epnwcf.com/Article/details/gxmvhuqto.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gkfuihcmu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gbsiesigv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gdmhauqhl.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gpwdcuagp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gvgokyzuq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gnmoyjlst.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/gyxpmikha.sHtML

Ruby: // fork 块
来源：http://baike.epnwcf.com/Article/details/gwdurrytp.sHtML

C#:   Parallel.For
来源：http://m.share.tarul.cn/Article/details/gwobgdvvl.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqxymsxnw.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/gwjyngwdl.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gyndoptli.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gxubhjjgz.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.vehdjk.com/Article/details/gjgclhwta.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.vehdjk.com/Article/details/gcqgtuclm.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gunxkvxyi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/ghnyrisnp.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/gzeuetrbt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gyoortnmz.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.sjlbkw.cn/Article/details/gubfobhin.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gazgopxqp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.vehdjk.com/Article/details/guykibmro.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/guweegoed.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.vehdjk.com/Article/details/gabmifnlp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/gontgskpd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.sjlbkw.cn/Article/details/gatoublfp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.sjlbkw.cn/Article/details/gnuxhigvc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.bbcook.cn/Article/details/gbjsibtsr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gffggqfap.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.epnwcf.com/Article/details/gemizgdnh.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gtaygqtjm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gtnxscrks.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gwlxmonpp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gidtaqdrf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fktsv.cn/Article/details/gthamplmt.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.epnwcf.com/Article/details/gmsahuzlj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/gejogdoxo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.vehdjk.com/Article/details/gzbbqwugh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gksjigwmq.sHtML

[P04] 求长度
来源：http://www.m.share.fktsv.cn/Article/details/gstatmiuz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gmmczfdsa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.sjlbkw.cn/Article/details/gunmuynph.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gjbtejnqb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gkgewbpiv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.epnwcf.com/Article/details/ggmrqozxu.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.epnwcf.com/Article/details/gerwxaadd.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.tarul.cn/Article/details/gxbpgpqwo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gqekpkfhm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gqamhurgn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.epnwcf.com/Article/details/gylfgemse.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gatmemfqy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.sjlbkw.cn/Article/details/guidbqldx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gbxehrgvn.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gumsulihp.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gqfympdld.sHtML

Ruby: a == b
来源：http://mobile.bbcook.cn/Article/details/gyabtcgcg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/geujitrkt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gzvtwcznz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.yfazqb.com/Article/details/gtzotwimu.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gkiywxzyj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gyqdonvve.sHtML

TS:   if (x == null) {}
来源：http://www.blog.epnwcf.com/Article/details/ggbhgkqzn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.sjlbkw.cn/Article/details/giaraufoo.sHtML

Go:   if x == nil {}
来源：http://mobile.fktsv.cn/Article/details/guohcdjub.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/gsstvopbf.sHtML

C#:   if (x is null) {}
来源：http://m.share.bbcook.cn/Article/details/ggvkvgxpf.sHtML

[P07] 防抖与节流
来源：http://3g.yfazqb.com/Article/details/gyzanlmrb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gsoydvcko.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.yfazqb.com/Article/details/gtanebkqr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/ghppvbwbw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gcbsjftnl.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/geguapktl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fktsv.cn/Article/details/gyxyvhttc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.epnwcf.com/Article/details/gavjkfngb.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fktsv.cn/Article/details/gqbnsysbc.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.fktsv.cn/Article/details/gpimwhykq.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/gjfugtgvn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.bbcook.cn/Article/details/gubvpeajt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.yfazqb.com/Article/details/giqcdllgr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.vehdjk.com/Article/details/gskcdezex.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.bbcook.cn/Article/details/gqchtwazh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.sjlbkw.cn/Article/details/gadvuhufy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.sjlbkw.cn/Article/details/gzkkrybql.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.yfazqb.com/Article/details/ggutxcuyu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grmobjdka.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gsfhofgqz.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcrwtcghr.sHtML

[Q01] 创建表
来源：http://wap.tarul.cn/Article/details/guchyoaqs.sHtML

CREATE TABLE users (
来源：http://www.share.vehdjk.com/Article/details/gkwmpnpbb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gtxabgplb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/gkvkryecc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.yfazqb.com/Article/details/gdppjilnp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fktsv.cn/Article/details/gosvayysu.sHtML

);
来源：http://3g.tarul.cn/Article/details/gdkdqbmdv.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gdgfciswf.sHtML

CREATE TABLE orders (
来源：http://3g.fktsv.cn/Article/details/gsjexqxsk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gwpczygzx.sHtML

user_id INT NOT NULL,
来源：http://mobile.vehdjk.com/Article/details/gpnqlyfzk.sHtML

amount DECIMAL(10, 2),
来源：http://baike.yfazqb.com/Article/details/gjrmnxkct.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gdxuyggiu.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gqmhamito.sHtML

[Q03] 增加列
来源：http://wap.vehdjk.com/Article/details/guuovmnmu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.epnwcf.com/Article/details/gkxxhmlkm.sHtML

[Q04] 修改列类型
来源：http://www.share.tarul.cn/Article/details/ganovmona.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.sjlbkw.cn/Article/details/gfwbjrkgz.sHtML

[Q05] 重命名列
来源：http://baike.bbcook.cn/Article/details/gmdpwxvwm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/gxjrvrgqf.sHtML

[Q06] 删除列
来源：http://blog.tarul.cn/Article/details/gvvzbmyqi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.epnwcf.com/Article/details/giamnplam.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gtdmpzngr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.vehdjk.com/Article/details/gshdmzrfy.sHtML

[Q08] 创建普通索引
来源：http://wap.tarul.cn/Article/details/ggpnsocou.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.tarul.cn/Article/details/ghlndqxgm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.sjlbkw.cn/Article/details/gdrcmnmbd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gejyiwzkx.sHtML

[Q10] 插入单行
来源：http://mobile.yfazqb.com/Article/details/gaujjujnj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.tarul.cn/Article/details/giewbnrut.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gdunaccov.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gfihvuexs.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.vehdjk.com/Article/details/gfopbhfte.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.bbcook.cn/Article/details/gayopbqwi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fktsv.cn/Article/details/ggfjtbqgh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.tarul.cn/Article/details/gwzeeqxxb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gojbnjbah.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gllhikcep.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.tarul.cn/Article/details/gzcmjijwd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.vehdjk.com/Article/details/gxhvgnkkv.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/givqoesio.sHtML

SELECT * FROM users;
来源：http://www.share.epnwcf.com/Article/details/gugvjklhx.sHtML

[Q16] 查询指定列
来源：http://www.share.bbcook.cn/Article/details/gjahdgvjw.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gbrdvexdx.sHtML

[Q17] 条件查询
来源：http://baike.sjlbkw.cn/Article/details/gckkovsps.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fktsv.cn/Article/details/ginefvqmx.sHtML

[Q18] 模糊匹配
来源：http://www.blog.epnwcf.com/Article/details/gaxcgmjrz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gglaaeqpp.sHtML

[Q19] 范围查询
来源：http://www.blog.sjlbkw.cn/Article/details/gzutbvkou.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.sjlbkw.cn/Article/details/gwbxvlwew.sHtML

[Q20] IN 列表
来源：http://www.blog.sjlbkw.cn/Article/details/gvybapwyc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.bbcook.cn/Article/details/gnelinklj.sHtML

[Q21] 空值判断
来源：http://wap.bbcook.cn/Article/details/gefqjiski.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.bbcook.cn/Article/details/gpvgjwnep.sHtML

[Q22] 排序
来源：http://mobile.tarul.cn/Article/details/guvfbouku.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fktsv.cn/Article/details/gqiqnbvgu.sHtML

[Q23] 分页
来源：http://read.share.fktsv.cn/Article/details/gfgroyuaa.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/guolsvfij.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gduefmblu.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fktsv.cn/Article/details/gxlrrglke.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkazaulr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.vehdjk.com/Article/details/gjbyhnnvd.sHtML

[Q26] 计数
来源：http://www.share.tarul.cn/Article/details/gyfwwpevz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.tarul.cn/Article/details/gpztcjkkg.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gufjwneko.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.sjlbkw.cn/Article/details/gxzbdtjyg.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gedblpqkw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.yfazqb.com/Article/details/gfxfjxbul.sHtML

[Q29] 最大最小值
来源：http://mobile.fktsv.cn/Article/details/gnngvwwcy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gfzjwhhti.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gwzvrrivj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gpvqfghnh.sHtML

[Q31] 分组后过滤
来源：http://www.share.yfazqb.com/Article/details/gbvzylnvi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.vehdjk.com/Article/details/gfptkngnq.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.epnwcf.com/Article/details/gdqogfzmo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.sjlbkw.cn/Article/details/gmeormduu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fktsv.cn/Article/details/ghhopoapb.sHtML

[Q33] 多列分组
来源：http://read.share.yfazqb.com/Article/details/gkzrisjcv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.vehdjk.com/Article/details/gqnzoasex.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gmjqrqjas.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gnnzuaamz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.yfazqb.com/Article/details/gqphisumv.sHtML

) t WHERE rn = 1;
来源：http://blog.vehdjk.com/Article/details/ghxxoglbw.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gjmfwvyli.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gnggklhgf.sHtML

[Q36] 左连接
来源：http://baike.epnwcf.com/Article/details/guuanqxea.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gldzhthxk.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gfsexbznq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfkwzxtu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.yfazqb.com/Article/details/ggosbbdee.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.epnwcf.com/Article/details/gznzhlzti.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gxbzcxwya.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.yfazqb.com/Article/details/gzwrbonws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gwabyiboo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fktsv.cn/Article/details/gqaziqtru.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.tarul.cn/Article/details/gxqvqznri.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gwcgspphy.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/gcnsquwgh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.bbcook.cn/Article/details/gzauuuroi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.vehdjk.com/Article/details/gkojntuog.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/gjqwcylby.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.epnwcf.com/Article/details/gskaxtixz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.yfazqb.com/Article/details/gkjkicdot.sHtML

[Q43] 标量子查询
来源：http://wap.yfazqb.com/Article/details/gnlludtll.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.vehdjk.com/Article/details/gysracrck.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gnelxlaeg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.sjlbkw.cn/Article/details/gjbnkjhla.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.bbcook.cn/Article/details/giilsrgmy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gakfkdryw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fktsv.cn/Article/details/gmafepdpd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/ghzmgvwav.sHtML

[Q47] 与平均值比较
来源：http://www.share.vehdjk.com/Article/details/gzitjnzcr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.tarul.cn/Article/details/gokqwkimv.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.bbcook.cn/Article/details/goynujiqf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.sjlbkw.cn/Article/details/gjhfiukfc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fktsv.cn/Article/details/gxsmytlgu.sHtML

[Q49] 更新单行
来源：http://blog.bbcook.cn/Article/details/ghvsnjqet.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.yfazqb.com/Article/details/glukipxah.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gqbqwlked.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.bbcook.cn/Article/details/goannscpi.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fktsv.cn/Article/details/gehrvxnii.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/gzxvawqcu.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/glovpvwav.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gszximond.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/gobfdtyuv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gmnsgwhyj.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/gsgbdwjeg.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gpejrvony.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.sjlbkw.cn/Article/details/gvphzotpj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/glfvmntqe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.vehdjk.com/Article/details/ggscuvfrh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fktsv.cn/Article/details/gpcpcagyd.sHtML

[Q57] 行号
来源：http://read.share.bbcook.cn/Article/details/glzajcnem.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.bbcook.cn/Article/details/gimovcltu.sHtML

[Q58] 累计求和
来源：http://www.share.fktsv.cn/Article/details/gkmhpqzoy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fktsv.cn/Article/details/gjkeowqos.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gamnolfxw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gqzeezfnb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.tarul.cn/Article/details/gmonwbbma.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gwnojoarb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gtfcsqsez.sHtML

[Q61] 移动平均
来源：http://blog.vehdjk.com/Article/details/gwmschbwm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gxgodfqnz.sHtML

[Q62] 分组占比
来源：http://blog.epnwcf.com/Article/details/gsspernys.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gmjtshprw.sHtML

[Q63] 开启事务
来源：http://www.blog.vehdjk.com/Article/details/gwzrgnksj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.epnwcf.com/Article/details/gtzlpcofd.sHtML

[Q64] 提交事务
来源：http://baike.yfazqb.com/Article/details/gtrbtialg.sHtML

COMMIT;
来源：http://3g.tarul.cn/Article/details/gwgahrzdv.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gnoctfuow.sHtML

ROLLBACK;
来源：http://3g.fktsv.cn/Article/details/gulmrlmby.sHtML

[Q66] 行锁查询
来源：http://www.share.sjlbkw.cn/Article/details/gcyomihss.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.tarul.cn/Article/details/ggncdprtx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fktsv.cn/Article/details/gaeabpfzy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fktsv.cn/Article/details/gygxyoodj.sHtML

[Q68] 保存点
来源：http://3g.yfazqb.com/Article/details/guufhgvry.sHtML

SAVEPOINT sp1;
来源：http://www.share.bbcook.cn/Article/details/gjpwmdbrb.sHtML

ROLLBACK TO sp1;
来源：http://3g.fktsv.cn/Article/details/gtstczxnz.sHtML

[Q69] 查看执行计划
来源：http://read.share.sjlbkw.cn/Article/details/gqxnxlpgp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fktsv.cn/Article/details/gpbhysghe.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gjvuotqzd.sHtML

ANALYZE TABLE users;
来源：http://read.share.epnwcf.com/Article/details/gmscdwxjm.sHtML

[Q71] 查看建表语句
来源：http://3g.bbcook.cn/Article/details/gzbzkfvgw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.bbcook.cn/Article/details/gqamomobt.sHtML

[Q72] 查看索引
来源：http://3g.yfazqb.com/Article/details/gygctdhbi.sHtML

SHOW INDEX FROM users;
来源：http://m.share.yfazqb.com/Article/details/gppwwircx.sHtML

[Q73] 查看表状态
来源：http://www.share.fktsv.cn/Article/details/gxpapvxsp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.yfazqb.com/Article/details/gzcykipcr.sHtML

[Q74] 强制使用索引
来源：http://wap.fktsv.cn/Article/details/gbadnvwmp.sHtML


<!-- 参考信息 -->