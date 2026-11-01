代发 wailian999

================================================================================
来源：http://blog.bbcook.cn/Article/details/gzqxadmjc.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gjuedvpiu.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gerfhvipn.sHtML

[O01] 启动一个线程
来源：http://wap.bbcook.cn/Article/details/gplvkdout.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.epnwcf.com/Article/details/gnleeduhs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.vehdjk.com/Article/details/gpwrlqrpr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.sjlbkw.cn/Article/details/gsjvaoilb.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/gusgerctg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gaomzrvin.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/gbkgevqlu.sHtML

Ruby: Thread.new { f }
来源：http://wap.yfazqb.com/Article/details/gkzgcnqln.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gtjdiwyuk.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/glsuggsqd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.yfazqb.com/Article/details/gxuealefj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.vehdjk.com/Article/details/getztszlc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.sjlbkw.cn/Article/details/gxzckitgp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.tarul.cn/Article/details/gwltvjbzw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gkvzbwmpp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/gxkorzyeh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvbhjglb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gynlfvwpy.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gxcwcknzf.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/guksbedht.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gesmqifia.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gibubvhng.sHtML

TS:   // 同 JS
来源：http://blog.bbcook.cn/Article/details/gihbfmzzg.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gbzzryncq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/gtdbqghny.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fktsv.cn/Article/details/gvyoyjuee.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gwfitidae.sHtML

[O04] 定义异步函数并等待
来源：http://baike.yfazqb.com/Article/details/gjunrpagr.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/gibcxkllj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/grzqxgwrn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gvmwbcfen.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.epnwcf.com/Article/details/ghafzqnww.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gharlavej.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gxlkaxnap.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fktsv.cn/Article/details/glelvkils.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.vehdjk.com/Article/details/gcenlarne.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/glwmjqxdm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.epnwcf.com/Article/details/gpvyzvtzh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gycjknpjx.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gstvyfoht.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.tarul.cn/Article/details/gpoiqabjr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/ggfrlklcv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gcvlhtmwa.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.tarul.cn/Article/details/ghrebdmvl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.epnwcf.com/Article/details/gtrpjkcht.sHtML

[O06] 使用进程池
来源：http://www.m.share.tarul.cn/Article/details/gevhflybm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/ghsawdqmu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gzhqzbyvv.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gaqwtppse.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/ghdaxzhpj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/gbbtjdjkv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.yfazqb.com/Article/details/gaokdncpe.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/ghksnzpim.sHtML

C#:   Parallel.For
来源：http://mobile.yfazqb.com/Article/details/gzsgmfouo.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gypbyffkh.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gugabshpm.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gcmdfewan.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gpwpcsgiw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gjxkjpare.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/glvuenphh.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gmtrxdnaf.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/giwhxolxm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gdjukegzq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.sjlbkw.cn/Article/details/gqelzgidy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gsvpaehuq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gqxmrgtyi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gazjekegj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gudfaylnt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.yfazqb.com/Article/details/ggyalsseu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/gespaxaub.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gxgyedcnn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.epnwcf.com/Article/details/guhxalkie.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gwlynjyzt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/gnkezvoyn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.epnwcf.com/Article/details/gudkyfvxx.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gwhuervuf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gorglsnxp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.tarul.cn/Article/details/gwrmvogqe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.vehdjk.com/Article/details/gculyfdgw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gadrqihnz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.yfazqb.com/Article/details/ghnwmsqwp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.epnwcf.com/Article/details/gwkcgzjfq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gomdhplde.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gqxjunwpk.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gnbumlxzv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gcsohqyrb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.epnwcf.com/Article/details/gmbodxata.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gghwazatt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/glyzwmudk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.tarul.cn/Article/details/gztuuegxv.sHtML

Go:   len(arr);  len(m)
来源：http://baike.epnwcf.com/Article/details/ghdyoivxg.sHtML

Ruby: x.length;  x.size
来源：http://baike.yfazqb.com/Article/details/gzvgnskyo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.tarul.cn/Article/details/gqehgeatp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.bbcook.cn/Article/details/gieedbwun.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gatsuhsea.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.yfazqb.com/Article/details/geeiudnpp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.fktsv.cn/Article/details/goyhgiszq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gtlcsczwj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.epnwcf.com/Article/details/gmhectlgo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fktsv.cn/Article/details/gorjnultt.sHtML

Ruby: a == b
来源：http://mobile.yfazqb.com/Article/details/gntsesjjq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/grtvysunt.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.bbcook.cn/Article/details/gcwgaadjn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.yfazqb.com/Article/details/gzxnhhsnc.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.epnwcf.com/Article/details/guwakwkuj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gyohpklam.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.vehdjk.com/Article/details/gplaretpz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gtyoaoowp.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/gqyiqflcr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gtuzkozll.sHtML

C#:   if (x is null) {}
来源：http://m.share.yfazqb.com/Article/details/gtcwhuoyt.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/ghxsxqrvk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fktsv.cn/Article/details/gioezzvjv.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gsctjbyou.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gbbfziqdn.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gdqfkmqwq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/gytdxkquk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.tarul.cn/Article/details/gefsnquxh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/gjzdziwej.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fktsv.cn/Article/details/gjouuohce.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fktsv.cn/Article/details/gemazfopz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gcxrqpvfo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fktsv.cn/Article/details/gfclkdquy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gufgfsnoz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gmucmdoyb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/geakdvypk.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fktsv.cn/Article/details/gneurqslj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.yfazqb.com/Article/details/gvixqanpd.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gvhbpxjza.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnjqvegbs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.bbcook.cn/Article/details/guhwcllij.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ggecxriid.sHtML

[Q01] 创建表
来源：http://blog.epnwcf.com/Article/details/gtkvzqobr.sHtML

CREATE TABLE users (
来源：http://www.blog.fktsv.cn/Article/details/gluxuxfbp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gaqaxytzg.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fktsv.cn/Article/details/gspssahrq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.fktsv.cn/Article/details/gkwdzgqnm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.tarul.cn/Article/details/gvhzwjvvm.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/givcedhlc.sHtML

[Q02] 创建带外键的表
来源：http://baike.sjlbkw.cn/Article/details/gpqollrau.sHtML

CREATE TABLE orders (
来源：http://www.m.share.vehdjk.com/Article/details/gsugrxyvm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fktsv.cn/Article/details/gtzblvuya.sHtML

user_id INT NOT NULL,
来源：http://www.share.epnwcf.com/Article/details/gikzstwyq.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.bbcook.cn/Article/details/gdcdkuogu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.vehdjk.com/Article/details/gtodseyit.sHtML

);
来源：http://wap.tarul.cn/Article/details/glyoyucqr.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gessukbob.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.yfazqb.com/Article/details/gbjncxnbv.sHtML

[Q04] 修改列类型
来源：http://www.share.bbcook.cn/Article/details/gimvususw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/gzftofinz.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gulwctbxi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/glpggrfaq.sHtML

[Q06] 删除列
来源：http://read.share.yfazqb.com/Article/details/gvnmoslsc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.bbcook.cn/Article/details/gprxfebhh.sHtML

[Q07] 删除表
来源：http://www.share.bbcook.cn/Article/details/ggvvvvvgv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.epnwcf.com/Article/details/gdbswsyct.sHtML

[Q08] 创建普通索引
来源：http://baike.epnwcf.com/Article/details/gcfcyubfc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/gmzrlodfj.sHtML

[Q09] 创建唯一索引
来源：http://baike.vehdjk.com/Article/details/gyjqvusbh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.tarul.cn/Article/details/gwokdnagb.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gvxbyiuoq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/graqwfayc.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/ghaduymjx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/ghvipevyv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.vehdjk.com/Article/details/gpkdngloo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.yfazqb.com/Article/details/gliwvfhym.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/ghlkqavsq.sHtML

[Q13] 忽略重复插入
来源：http://wap.fktsv.cn/Article/details/ggejxvqum.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gbcdtwywi.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fktsv.cn/Article/details/gccbafmtv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.vehdjk.com/Article/details/gjpdspumn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.yfazqb.com/Article/details/gdqeonoan.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gzixswcou.sHtML

SELECT * FROM users;
来源：http://wap.fktsv.cn/Article/details/gbrsqdbnl.sHtML

[Q16] 查询指定列
来源：http://www.m.share.epnwcf.com/Article/details/gnrgdccqs.sHtML

SELECT id, name FROM users;
来源：http://wap.tarul.cn/Article/details/gvtdqxahz.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/ghowzqwbv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/ggzmidhkj.sHtML

[Q18] 模糊匹配
来源：http://3g.yfazqb.com/Article/details/gefockzqz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.bbcook.cn/Article/details/gfleaocjb.sHtML

[Q19] 范围查询
来源：http://3g.epnwcf.com/Article/details/ggohbhlzn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.epnwcf.com/Article/details/gufzhcrug.sHtML

[Q20] IN 列表
来源：http://m.share.bbcook.cn/Article/details/gpajrdaoh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.yfazqb.com/Article/details/gntutnkvj.sHtML

[Q21] 空值判断
来源：http://www.blog.yfazqb.com/Article/details/grviouwot.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.tarul.cn/Article/details/gmjucetsp.sHtML

[Q22] 排序
来源：http://blog.tarul.cn/Article/details/gbffmmtgv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.tarul.cn/Article/details/gywdfiyom.sHtML

[Q23] 分页
来源：http://read.share.sjlbkw.cn/Article/details/gldgtylts.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gezykmrul.sHtML

[Q24] 去重
来源：http://blog.sjlbkw.cn/Article/details/gdofhbogf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gbrzwuwhk.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fktsv.cn/Article/details/gshlyzqmh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.epnwcf.com/Article/details/gkqqeahjz.sHtML

[Q26] 计数
来源：http://www.share.bbcook.cn/Article/details/gechwnsxl.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gdkwxkfpc.sHtML

[Q27] 条件计数
来源：http://www.m.share.tarul.cn/Article/details/gxctpkzln.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.epnwcf.com/Article/details/glrsiqnxs.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gmxhxxwha.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/glbfddows.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gtczmcgah.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gdicnmcda.sHtML

[Q30] 分组统计
来源：http://www.blog.epnwcf.com/Article/details/ghaguezwr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.sjlbkw.cn/Article/details/grqjqlxzz.sHtML

[Q31] 分组后过滤
来源：http://www.share.vehdjk.com/Article/details/gqqpmbsaf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.epnwcf.com/Article/details/gzxzxuxgn.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gmbyfaosp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/glzpabnos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gosyhoamf.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/gnatfxkib.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.yfazqb.com/Article/details/gvdxxtsaz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.tarul.cn/Article/details/ggdqldarc.sHtML

SELECT * FROM (
来源：http://m.share.epnwcf.com/Article/details/ggnjazsdx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.epnwcf.com/Article/details/ggnexxdxp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gkakedybz.sHtML

[Q35] 内连接
来源：http://blog.bbcook.cn/Article/details/gibhhcjin.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gxoptgaoh.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gdyxduvmh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gtoeettbz.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gztfburga.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fktsv.cn/Article/details/gieckbdpj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.bbcook.cn/Article/details/gvxnkhivd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fktsv.cn/Article/details/gmihjzqvz.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gngnvfarv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gzcuaovpt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/goerpbwse.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/gngituugp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.tarul.cn/Article/details/gzfuhuoni.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/gjrvyefmc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.epnwcf.com/Article/details/gghkhgjag.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/gkucxudig.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fktsv.cn/Article/details/gticgvnea.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.epnwcf.com/Article/details/gjrooiflc.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fktsv.cn/Article/details/ggemrlyvl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.epnwcf.com/Article/details/gqbvkgvsb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fktsv.cn/Article/details/guhuccbgq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gyuwqitey.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gqvltwmbk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fktsv.cn/Article/details/ghggirfcx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gdjutghzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gyxblbnwy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.bbcook.cn/Article/details/gvxlbtjke.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gotwlwqdm.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gqekrbwex.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.vehdjk.com/Article/details/ggjhnaktc.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.vehdjk.com/Article/details/gatjdqqac.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gvsdbnaug.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/ggvnsmkur.sHtML

[Q49] 更新单行
来源：http://www.share.fktsv.cn/Article/details/glzfmvlxo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.bbcook.cn/Article/details/gwxvgpgkr.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gqdinrqdk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/ghrgzstrg.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.tarul.cn/Article/details/gorjwtmwb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.yfazqb.com/Article/details/gbqkzmqyj.sHtML

[Q52] 删除指定行
来源：http://www.m.share.yfazqb.com/Article/details/guywsnedp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/grzshavuq.sHtML

[Q53] 按条件删除
来源：http://read.share.fktsv.cn/Article/details/gngkqlszy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.epnwcf.com/Article/details/glfkexbzq.sHtML

[Q54] 清空表
来源：http://3g.vehdjk.com/Article/details/gxlowztun.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.bbcook.cn/Article/details/ginnzxjco.sHtML

[Q55] 排名（并列占位）
来源：http://3g.tarul.cn/Article/details/gmhwpugas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.epnwcf.com/Article/details/gssfykbis.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.tarul.cn/Article/details/ghqgvqocg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/ggjxgwufd.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/ggtbvvdxp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gsittztys.sHtML

[Q58] 累计求和
来源：http://wap.tarul.cn/Article/details/gcyitwgpm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fktsv.cn/Article/details/giyeyhvay.sHtML

[Q59] 分组内累计
来源：http://read.share.bbcook.cn/Article/details/gjaobmtuc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gjmdqdxzd.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.sjlbkw.cn/Article/details/gqhxnimpd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.epnwcf.com/Article/details/gukucofxd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gizevwwvw.sHtML

[Q61] 移动平均
来源：http://blog.fktsv.cn/Article/details/grngkceau.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gzdyybvfz.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gjmyiymfc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/ggmboukuw.sHtML

[Q63] 开启事务
来源：http://blog.bbcook.cn/Article/details/gwvfzbmre.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.vehdjk.com/Article/details/gccuopldj.sHtML

[Q64] 提交事务
来源：http://mobile.bbcook.cn/Article/details/gxjkasgcj.sHtML

COMMIT;
来源：http://baike.sjlbkw.cn/Article/details/gjwrcxayl.sHtML

[Q65] 回滚事务
来源：http://blog.epnwcf.com/Article/details/gdmrlwpjq.sHtML

ROLLBACK;
来源：http://www.m.share.yfazqb.com/Article/details/gzwvqoysb.sHtML

[Q66] 行锁查询
来源：http://baike.epnwcf.com/Article/details/grnkroumd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.tarul.cn/Article/details/gnjovbegg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fktsv.cn/Article/details/gcwsmuxnk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.sjlbkw.cn/Article/details/gsarwfnzj.sHtML

[Q68] 保存点
来源：http://read.share.sjlbkw.cn/Article/details/glvmavbpn.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.bbcook.cn/Article/details/gulxdqjjb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.vehdjk.com/Article/details/gieerokvm.sHtML

[Q69] 查看执行计划
来源：http://www.share.bbcook.cn/Article/details/gzxewjcqm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.epnwcf.com/Article/details/gsdpaetlc.sHtML

[Q70] 更新统计信息
来源：http://www.share.tarul.cn/Article/details/geafaanbp.sHtML

ANALYZE TABLE users;
来源：http://read.share.bbcook.cn/Article/details/gtmfuener.sHtML

[Q71] 查看建表语句
来源：http://3g.yfazqb.com/Article/details/gqvrearak.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.vehdjk.com/Article/details/geuwakhxv.sHtML

[Q72] 查看索引
来源：http://m.share.yfazqb.com/Article/details/gcpaoppau.sHtML


<!-- 参考信息 -->