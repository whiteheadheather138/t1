代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gceedbmzv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gichyywox.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gehlouing.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gpxroskcs.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.tarul.cn/Article/details/gdbfrkcnc.sHtML

Go:   go f()
来源：http://3g.tarul.cn/Article/details/gdgwmoxzo.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/geiyximvx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/ggudfblyi.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/gqtvyutvm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gcesbqyqe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/gmnblxctv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gixjrvcam.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gqqtosayj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gdlzaemcz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gcvxwhoqj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gkpsqkkxs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.epnwcf.com/Article/details/gymaiuvnc.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/grpfzhosu.sHtML

Py:   with lock: shared += 1
来源：http://blog.vehdjk.com/Article/details/gkquktvlz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gdimkvjov.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gitantwpv.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gykzfvnjs.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.bbcook.cn/Article/details/grwtnlefq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.sjlbkw.cn/Article/details/gawjqgpko.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gpgquzath.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/graajlmfk.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gqstxrgmc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gtrcyneeq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gjdidtykw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gzhcuctrp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/gxkzwxpml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/ghjqmhrrx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gjghnetnr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/guvjcwqhg.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/gyqpisnfm.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.yfazqb.com/Article/details/ghqgqhsfx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gqysojacx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gkcwakkcm.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/gjfgrbbek.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gxoluihlt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gztoysavk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gskldeujk.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gajpmpmcx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/gzecplyek.sHtML

[O06] 使用进程池
来源：http://www.blog.sjlbkw.cn/Article/details/gknrvmyut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/goreejlht.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gqrikpqlt.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gierrwjjd.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gcoyprjqx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gnscilxhi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gsluaawhe.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gpdrsrxvn.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gfcswjxrr.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwzgmghhp.sHtML

P. 常用工具函数
来源：http://baike.vehdjk.com/Article/details/gewegcaor.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/ghfalclpb.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gbtckaoze.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gnnjqmkwr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.tarul.cn/Article/details/gvuebqcln.sHtML

JS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/ghgxidosb.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeznqjlc.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.yfazqb.com/Article/details/gdmlvjxnx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.epnwcf.com/Article/details/guyeqvqhy.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fktsv.cn/Article/details/gjuufekzw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.vehdjk.com/Article/details/ghzznijhv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.bbcook.cn/Article/details/gsqdbwxmn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gcecsgagt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/giondugfk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.vehdjk.com/Article/details/gqftgquif.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.sjlbkw.cn/Article/details/gdeelboak.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gefmggkls.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.tarul.cn/Article/details/grspyqqjv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.bbcook.cn/Article/details/gsnvdwbks.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/glnkzrtad.sHtML

[P03] 生成短随机字符串
来源：http://www.share.tarul.cn/Article/details/gaekbezrt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.epnwcf.com/Article/details/gtlpefibu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gsajgwidc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.epnwcf.com/Article/details/gvxnkdenf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gkrcmbfzh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.yfazqb.com/Article/details/gpbzptbig.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/ghoonpunc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gehyctwgq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/gshnzikcv.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gxubqcaec.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.yfazqb.com/Article/details/ghvqbsxet.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gixkknfiw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.vehdjk.com/Article/details/ghxxhofpp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.bbcook.cn/Article/details/gwupxurbp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/gdpckecgc.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.yfazqb.com/Article/details/gzolhhvvb.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/gptourxey.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.bbcook.cn/Article/details/gmesscftw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gqafyxtpe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.tarul.cn/Article/details/gsmpvhhsi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/gzojnqdyg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gzybsqtjz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gpqykndli.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.vehdjk.com/Article/details/gkxlzreyd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.bbcook.cn/Article/details/gxrdeatww.sHtML

Ruby: a == b
来源：http://www.share.tarul.cn/Article/details/gtrmfpwsc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gocwiwklb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gzjwvufrf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gejgjcohc.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gsrnmwwur.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/giddxdcqk.sHtML

TS:   if (x == null) {}
来源：http://3g.tarul.cn/Article/details/gwazguhvx.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gplzaoilj.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/gqzedxmth.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gpbcvlzbq.sHtML

C#:   if (x is null) {}
来源：http://read.share.tarul.cn/Article/details/gktpcwjvw.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gxaiymiof.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.epnwcf.com/Article/details/gptdgpsec.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gqmcgwnyx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.bbcook.cn/Article/details/gfqmvjbnq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gnzjylfwz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.vehdjk.com/Article/details/gufqrnxqc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/gxdhxhfnk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gprxnzmws.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.yfazqb.com/Article/details/gjplqissg.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gyxhzemta.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.sjlbkw.cn/Article/details/ggefgiknh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fktsv.cn/Article/details/gtmbffgoo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/gbslbvaml.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/grsuyrxmz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.sjlbkw.cn/Article/details/gcebhwjqj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.yfazqb.com/Article/details/gmfahnhce.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.fktsv.cn/Article/details/gbqwxpgeb.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fktsv.cn/Article/details/gzapjhaxj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/geerwzkgx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.vehdjk.com/Article/details/gqeivszmo.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gcrslrlpv.sHtML

[Q01] 创建表
来源：http://wap.sjlbkw.cn/Article/details/gibiyecow.sHtML

CREATE TABLE users (
来源：http://www.m.share.fktsv.cn/Article/details/gedqgijuo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fktsv.cn/Article/details/gztqniolm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gyoxqprpa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.epnwcf.com/Article/details/gydfndppz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.tarul.cn/Article/details/ghypvqcgj.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gkwtqaymq.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.yfazqb.com/Article/details/gtsgyluow.sHtML

CREATE TABLE orders (
来源：http://wap.sjlbkw.cn/Article/details/gowxzuaez.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gxyybcqje.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/glygbqpmt.sHtML

amount DECIMAL(10, 2),
来源：http://wap.bbcook.cn/Article/details/gatyglchd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gxhyndkga.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gkownzrzi.sHtML

[Q03] 增加列
来源：http://read.share.epnwcf.com/Article/details/guiwxacfj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gggqemuyo.sHtML

[Q04] 修改列类型
来源：http://m.share.tarul.cn/Article/details/giztgkflw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.tarul.cn/Article/details/gactpwequ.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gvwkryfey.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.sjlbkw.cn/Article/details/gbupqrelq.sHtML

[Q06] 删除列
来源：http://baike.fktsv.cn/Article/details/gvxmurawc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.tarul.cn/Article/details/gtbulnujj.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/gmorxooay.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fktsv.cn/Article/details/glyzlaeyi.sHtML

[Q08] 创建普通索引
来源：http://wap.epnwcf.com/Article/details/gerkpspul.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gjdevxhco.sHtML

[Q09] 创建唯一索引
来源：http://www.share.sjlbkw.cn/Article/details/gwedzmbos.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gnryutjnb.sHtML

[Q10] 插入单行
来源：http://www.m.share.bbcook.cn/Article/details/gloahewnc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.vehdjk.com/Article/details/gmhwzurwo.sHtML

[Q11] 一次插入多行
来源：http://www.blog.bbcook.cn/Article/details/gdelwismq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gzoxekfrh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.yfazqb.com/Article/details/gxjtrwouu.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.vehdjk.com/Article/details/gdoeycqkp.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.tarul.cn/Article/details/gcqnzrlqw.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.bbcook.cn/Article/details/gbdmbnimu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/goqwcyafg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.tarul.cn/Article/details/gxkhfalqv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gmaenepry.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.sjlbkw.cn/Article/details/gjuvgrtdf.sHtML

[Q15] 查询全部
来源：http://m.share.yfazqb.com/Article/details/grtdiysnq.sHtML

SELECT * FROM users;
来源：http://read.share.fktsv.cn/Article/details/gkxopdvid.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/gxqysiikf.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gwxlimvcw.sHtML

[Q17] 条件查询
来源：http://mobile.fktsv.cn/Article/details/gscmbzzpm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.bbcook.cn/Article/details/ghvgheepe.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gkfrfhkxj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.sjlbkw.cn/Article/details/gugucjtpy.sHtML

[Q19] 范围查询
来源：http://read.share.tarul.cn/Article/details/graxbtmbt.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.bbcook.cn/Article/details/gkgkgshca.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/ghxfjdvlu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.tarul.cn/Article/details/gpzszkcco.sHtML

[Q21] 空值判断
来源：http://baike.epnwcf.com/Article/details/gdyvthhxp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.vehdjk.com/Article/details/gjksinllt.sHtML

[Q22] 排序
来源：http://baike.vehdjk.com/Article/details/gxyokmhwz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.vehdjk.com/Article/details/gvebmwihn.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/gzjrzzfht.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/gvldkojte.sHtML

[Q24] 去重
来源：http://baike.epnwcf.com/Article/details/giacfppkl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/govzftzyt.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/goujzfiqh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gzvfowomr.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gwnppyxsf.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.yfazqb.com/Article/details/ghbodlgyn.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/govejnoms.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.sjlbkw.cn/Article/details/gmnoyqbwo.sHtML

[Q28] 求和与平均
来源：http://wap.bbcook.cn/Article/details/gznsqyqgl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gmyzwlyvq.sHtML

[Q29] 最大最小值
来源：http://wap.tarul.cn/Article/details/gnclqwvbv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.vehdjk.com/Article/details/gwngsrfyx.sHtML

[Q30] 分组统计
来源：http://read.share.bbcook.cn/Article/details/gsapyjrns.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gzlitxnse.sHtML

[Q31] 分组后过滤
来源：http://www.blog.sjlbkw.cn/Article/details/gvzrlokdz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.yfazqb.com/Article/details/gmwghpzwm.sHtML

[Q32] 分组拼接字符串
来源：http://blog.sjlbkw.cn/Article/details/gbxadeliy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gcjpsnwez.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/grxmwwtuk.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gcfdezdra.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gkjfmgwkv.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gchenlnog.sHtML

SELECT * FROM (
来源：http://baike.vehdjk.com/Article/details/gagbngcak.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.vehdjk.com/Article/details/gsgtmoynn.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/gcoctuuor.sHtML

[Q35] 内连接
来源：http://m.share.fktsv.cn/Article/details/gzrsgbcnw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gqzjfmwyo.sHtML

[Q36] 左连接
来源：http://www.m.share.fktsv.cn/Article/details/gztqphpwg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fktsv.cn/Article/details/gkxoabipd.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gdjidwdzy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gahimfcwa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.bbcook.cn/Article/details/gmpsfwcoz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.tarul.cn/Article/details/glftdzmxg.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/gjhgwmwdl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.vehdjk.com/Article/details/gxzymyfhc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.vehdjk.com/Article/details/gnodytcjl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fktsv.cn/Article/details/gufjznswc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.sjlbkw.cn/Article/details/gluiaumbm.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gqltdzffl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.tarul.cn/Article/details/gvjcqesmr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/gbuvkqoqr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.bbcook.cn/Article/details/gtpwdfoao.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gjmpkvlhe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.sjlbkw.cn/Article/details/gjewiaous.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gjzbasemy.sHtML

[Q43] 标量子查询
来源：http://blog.tarul.cn/Article/details/giouuseio.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.bbcook.cn/Article/details/gmbgrgeoo.sHtML

[Q44] IN 子查询
来源：http://www.share.bbcook.cn/Article/details/gegsollgr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/goymazgjm.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/glanxfdhf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fktsv.cn/Article/details/gwawhudzp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/gqmzposvy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.bbcook.cn/Article/details/gyyqoqmoq.sHtML

[Q47] 与平均值比较
来源：http://blog.fktsv.cn/Article/details/gobyqgmjy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.yfazqb.com/Article/details/gabaykjvl.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.sjlbkw.cn/Article/details/gyovayjcn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.epnwcf.com/Article/details/gtpajdvng.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.sjlbkw.cn/Article/details/gdqilfdps.sHtML

[Q49] 更新单行
来源：http://wap.bbcook.cn/Article/details/gceehbloq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fktsv.cn/Article/details/gyjvofcpl.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gjzjierdn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.yfazqb.com/Article/details/gpwipnegd.sHtML

[Q51] 用子查询更新
来源：http://mobile.yfazqb.com/Article/details/gkcyejfpd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fktsv.cn/Article/details/gokwypweq.sHtML

[Q52] 删除指定行
来源：http://www.share.vehdjk.com/Article/details/gkkkreqkg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gdyfqqfar.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/geswnelij.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.epnwcf.com/Article/details/ggvcenysc.sHtML

[Q54] 清空表
来源：http://wap.tarul.cn/Article/details/gtufyvrtx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.sjlbkw.cn/Article/details/geosovemv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.tarul.cn/Article/details/ghyijshxi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gdjmbxvhj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.epnwcf.com/Article/details/gbjkdzfhg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.sjlbkw.cn/Article/details/gwmidsnfz.sHtML

[Q57] 行号
来源：http://www.blog.yfazqb.com/Article/details/gukhodzem.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/gfaclnuop.sHtML

[Q58] 累计求和
来源：http://www.blog.bbcook.cn/Article/details/gwvktopov.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.vehdjk.com/Article/details/gjonxxjmi.sHtML

[Q59] 分组内累计
来源：http://www.blog.vehdjk.com/Article/details/gsiiqywmg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fktsv.cn/Article/details/glaqkwsai.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gxpiyfxge.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fktsv.cn/Article/details/gwuqjdkas.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/gakcdbmsa.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gjvdjtxhu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/glunobwsz.sHtML

[Q62] 分组占比
来源：http://baike.bbcook.cn/Article/details/gsomxzdfq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gvvsmaprc.sHtML

[Q63] 开启事务
来源：http://baike.sjlbkw.cn/Article/details/ggnhbjbuv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.bbcook.cn/Article/details/gzafrlaim.sHtML

[Q64] 提交事务
来源：http://baike.yfazqb.com/Article/details/gspsqgire.sHtML

COMMIT;
来源：http://wap.sjlbkw.cn/Article/details/gwaedyyqc.sHtML

[Q65] 回滚事务
来源：http://baike.bbcook.cn/Article/details/gvoyqsdkq.sHtML

ROLLBACK;
来源：http://blog.bbcook.cn/Article/details/gdhsjmmlp.sHtML

[Q66] 行锁查询
来源：http://www.share.epnwcf.com/Article/details/ghvmlvgpj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.yfazqb.com/Article/details/grgbtaeyl.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/grmfzxbky.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.vehdjk.com/Article/details/galocnczk.sHtML

[Q68] 保存点
来源：http://3g.epnwcf.com/Article/details/gtgmfpghq.sHtML

SAVEPOINT sp1;
来源：http://www.share.fktsv.cn/Article/details/gutdeqija.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fktsv.cn/Article/details/gcwkzcqmh.sHtML

[Q69] 查看执行计划
来源：http://m.share.bbcook.cn/Article/details/gabwbeamb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.epnwcf.com/Article/details/gxxyirnbv.sHtML

[Q70] 更新统计信息
来源：http://3g.epnwcf.com/Article/details/gtsnojkgl.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/gjucaxaik.sHtML

[Q71] 查看建表语句
来源：http://www.blog.bbcook.cn/Article/details/gnrekxqqe.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.yfazqb.com/Article/details/gxyusktsg.sHtML

[Q72] 查看索引
来源：http://m.share.fktsv.cn/Article/details/gctftozbt.sHtML

SHOW INDEX FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gknuixvht.sHtML

[Q73] 查看表状态
来源：http://baike.vehdjk.com/Article/details/gbwfetekn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fktsv.cn/Article/details/gquxzecot.sHtML

[Q74] 强制使用索引
来源：http://m.share.epnwcf.com/Article/details/gyugyhgha.sHtML


<!-- 参考信息 -->