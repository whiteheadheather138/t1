代发 wailian999

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzpoxoesd.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/gjnglbihf.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gnhzqwsjj.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gnvrtauvf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/gbatafwib.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.sjlbkw.cn/Article/details/gztsjkeua.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gbhmjmxwi.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gzrufvupq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.tarul.cn/Article/details/glhgfmtxb.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gwcyhmogr.sHtML

Ruby: Thread.new { f }
来源：http://blog.yfazqb.com/Article/details/ggyhdcmnk.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.vehdjk.com/Article/details/gpfurjkvv.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/ghwhsdghd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gojsttjdp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.bbcook.cn/Article/details/gkesoonri.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.vehdjk.com/Article/details/gdnwbjocy.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gupeiluta.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.sjlbkw.cn/Article/details/gjklsbgnj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gjptzdmcf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gumisotxm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/gfiidxptr.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/ggrxckxli.sHtML

Py:   with lock: shared += 1
来源：http://baike.tarul.cn/Article/details/gbeouvqmu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/glrduwycl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gvcjgiozo.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gciwwvpqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/gumvctkfg.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gjfnpaisu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.epnwcf.com/Article/details/gzexvmdtr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gxevkjktc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/gaeftyftd.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.sjlbkw.cn/Article/details/gjlpdconx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.vehdjk.com/Article/details/gcrmtwllz.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/grvaxydon.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gjhjuczxg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gbokjdsfc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/gmvakuuzb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.tarul.cn/Article/details/ghsileebp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gbidktlly.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/gosauvozr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.vehdjk.com/Article/details/goktaeiao.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.sjlbkw.cn/Article/details/gaxjtdjth.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.bbcook.cn/Article/details/gdhpiqspn.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gcpbqnkwa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.tarul.cn/Article/details/ggvpxsjse.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.epnwcf.com/Article/details/gqamwdfby.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gesrureix.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.bbcook.cn/Article/details/gjlvcjmrg.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/ggqohjhgl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gjfvetypz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.fktsv.cn/Article/details/gnkendwca.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.sjlbkw.cn/Article/details/gksnhsvid.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gqlhkstlq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.tarul.cn/Article/details/griyavrxd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/gpuitfzlc.sHtML

Ruby: // fork 块
来源：http://wap.vehdjk.com/Article/details/gzxmfcpze.sHtML

C#:   Parallel.For
来源：http://wap.yfazqb.com/Article/details/gzraalfpa.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/glnabobfq.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gehzokaim.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gopdvfpkr.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gmulqeqxk.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/ghjrqzirv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.bbcook.cn/Article/details/ghfvnltmw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gjzzkanfk.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gfnktepmh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.sjlbkw.cn/Article/details/gbkzcrhmb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/gaiwfbpmy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fktsv.cn/Article/details/gtotxkvwx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gbtsasaiy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.tarul.cn/Article/details/gqjylksfn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.bbcook.cn/Article/details/gwwwqpdkw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/gdwnlufxx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gaquaaksy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/greadhzud.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gobxzzdid.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gnmtutxmv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gdnbavzlz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gisymxmwi.sHtML

[P03] 生成短随机字符串
来源：http://wap.sjlbkw.cn/Article/details/gkuhmjznp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.tarul.cn/Article/details/gdfetkdds.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.sjlbkw.cn/Article/details/gmwobrojt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gqzgbgory.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gmdiytcsb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/ggtihycjk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gznpqvack.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.tarul.cn/Article/details/gteghtilv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gjbnrafaq.sHtML

[P04] 求长度
来源：http://www.blog.bbcook.cn/Article/details/gawcgimyz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.epnwcf.com/Article/details/gdvsmbsse.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.vehdjk.com/Article/details/gihgmffdb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gpsvoxqlk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.sjlbkw.cn/Article/details/gjuqrgvxy.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/goyzeqotk.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.tarul.cn/Article/details/gukktpnrp.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/golnfbzic.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/gfixmqhtl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/ggcnoepoj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gquwsghma.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gvlmxtsrh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gmysiybzw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gqereyiip.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gxxdszfvm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/gsworwthl.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gigiugqrz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.yfazqb.com/Article/details/gjvzofetm.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.tarul.cn/Article/details/gwmcvpbcn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gfcyrcpas.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.sjlbkw.cn/Article/details/gijdpjpmy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.vehdjk.com/Article/details/gvaipzozf.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/gelgliyra.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gyijhwowb.sHtML

Go:   if x == nil {}
来源：http://www.blog.fktsv.cn/Article/details/gumywdpxh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.fktsv.cn/Article/details/gffvzqaxu.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gokmitwsp.sHtML

[P07] 防抖与节流
来源：http://m.share.epnwcf.com/Article/details/gsawkejln.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.yfazqb.com/Article/details/gzrwvnrzo.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/glpohjrid.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.tarul.cn/Article/details/gdjkjgykt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.vehdjk.com/Article/details/gcmpnjmvy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.epnwcf.com/Article/details/gwmezwvqf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fktsv.cn/Article/details/gynievtzv.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.bbcook.cn/Article/details/gzomruldg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gbiczetaf.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.sjlbkw.cn/Article/details/gkzcnshub.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.sjlbkw.cn/Article/details/gcdlkbaqh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.vehdjk.com/Article/details/gdjhwcbfw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.tarul.cn/Article/details/gbqkrucpk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.sjlbkw.cn/Article/details/gtqxzqfvw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/goesiloeo.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.bbcook.cn/Article/details/gtavasdxc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.fktsv.cn/Article/details/geduvnqek.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.vehdjk.com/Article/details/gxxlivcjd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gtxosbxwx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.tarul.cn/Article/details/gmcffxaaj.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gnqvmeuck.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/ggzrlzljm.sHtML

CREATE TABLE users (
来源：http://www.share.bbcook.cn/Article/details/gjuknwyzh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fktsv.cn/Article/details/gkbddczxk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/gymuureig.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.yfazqb.com/Article/details/gyshdegnw.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.bbcook.cn/Article/details/glasdowpy.sHtML

);
来源：http://wap.tarul.cn/Article/details/geofesckw.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/govvjtiwn.sHtML

CREATE TABLE orders (
来源：http://mobile.yfazqb.com/Article/details/gzqbwcobp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.sjlbkw.cn/Article/details/gldrdgtuj.sHtML

user_id INT NOT NULL,
来源：http://mobile.sjlbkw.cn/Article/details/grtqunace.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gqxnhrbao.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.yfazqb.com/Article/details/gwiikwuih.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gxkohjofc.sHtML

[Q03] 增加列
来源：http://baike.yfazqb.com/Article/details/gjblcjjqa.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gzurtcryq.sHtML

[Q04] 修改列类型
来源：http://baike.yfazqb.com/Article/details/gabeosgdy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.epnwcf.com/Article/details/getadxvdf.sHtML

[Q05] 重命名列
来源：http://read.share.tarul.cn/Article/details/gswclbmtq.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gtoyaoesg.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gjfwgovwn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.tarul.cn/Article/details/gkbuifpne.sHtML

[Q07] 删除表
来源：http://www.blog.tarul.cn/Article/details/gyvurtffb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.sjlbkw.cn/Article/details/gienjtakz.sHtML

[Q08] 创建普通索引
来源：http://www.blog.sjlbkw.cn/Article/details/gpaapyhhf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gxiozywxa.sHtML

[Q09] 创建唯一索引
来源：http://read.share.sjlbkw.cn/Article/details/gghgcthbs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/glzopybra.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gwiixtrew.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.tarul.cn/Article/details/gcvvloztp.sHtML

[Q11] 一次插入多行
来源：http://mobile.tarul.cn/Article/details/gftatalaw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gonkudcnx.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.vehdjk.com/Article/details/glbtklpkl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.epnwcf.com/Article/details/gzydfqxfw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fktsv.cn/Article/details/gborqeghz.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.tarul.cn/Article/details/ggfceogff.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.epnwcf.com/Article/details/gapxthzvc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.bbcook.cn/Article/details/gtwsoivib.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/grkmbihyk.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.bbcook.cn/Article/details/geexzhdmw.sHtML

[Q15] 查询全部
来源：http://read.share.tarul.cn/Article/details/ghffxsein.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/gjltpyjad.sHtML

[Q16] 查询指定列
来源：http://3g.tarul.cn/Article/details/gmcssoxre.sHtML

SELECT id, name FROM users;
来源：http://m.share.vehdjk.com/Article/details/gnzlllflm.sHtML

[Q17] 条件查询
来源：http://www.share.bbcook.cn/Article/details/gsjmebqyr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gpcwtbwvv.sHtML

[Q18] 模糊匹配
来源：http://mobile.yfazqb.com/Article/details/gsfvldwvj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.tarul.cn/Article/details/ggtzawmry.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/gqfbqgfjk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.vehdjk.com/Article/details/gutnkjoft.sHtML

[Q20] IN 列表
来源：http://www.m.share.vehdjk.com/Article/details/gxqhlngwx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fktsv.cn/Article/details/gbcvdybtv.sHtML

[Q21] 空值判断
来源：http://baike.vehdjk.com/Article/details/ghdwqcvbe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/gtssznirn.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gzhtthsbs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.vehdjk.com/Article/details/guayoshsd.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/gudptkqvp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/gkhoyhlrs.sHtML

[Q24] 去重
来源：http://www.blog.bbcook.cn/Article/details/gxlfuhpnp.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.sjlbkw.cn/Article/details/gnvajdhac.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fktsv.cn/Article/details/gsxppsaio.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gjolmohro.sHtML

[Q26] 计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gyodqxrvq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/grurjdoeg.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/ggrxkckmc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gufizdenf.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gyibttkzt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.epnwcf.com/Article/details/gvryvsrya.sHtML

[Q29] 最大最小值
来源：http://blog.sjlbkw.cn/Article/details/gatkasoly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gltmkrvev.sHtML

[Q30] 分组统计
来源：http://www.blog.bbcook.cn/Article/details/gdgowzyiz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gcfpudlug.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/guysmwpfm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.yfazqb.com/Article/details/gttabuewv.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fktsv.cn/Article/details/gzmzwtlws.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gurrbytax.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/grzufjcvd.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/gezbavebf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/grxeutbnd.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/glztckjhb.sHtML

SELECT * FROM (
来源：http://3g.sjlbkw.cn/Article/details/gdfmjiatm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gxkjvunxr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gfhquderk.sHtML

[Q35] 内连接
来源：http://www.blog.yfazqb.com/Article/details/girovyipn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gpixymmaw.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/glktufiwu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fktsv.cn/Article/details/ggjrseczk.sHtML

[Q37] 右连接
来源：http://www.m.share.fktsv.cn/Article/details/gudvcmteh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.sjlbkw.cn/Article/details/grpsvlmmx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.epnwcf.com/Article/details/gfheiaxeu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.bbcook.cn/Article/details/gwupycdcr.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/ginfaraeq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/guwctczqs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.tarul.cn/Article/details/grsgxijgm.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.yfazqb.com/Article/details/gpxxhdmma.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.bbcook.cn/Article/details/ghdpflwcr.sHtML

[Q41] 多表连接
来源：http://mobile.bbcook.cn/Article/details/gcsnrdenj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.sjlbkw.cn/Article/details/gvgzukyqz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.vehdjk.com/Article/details/gupiazqgb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gsovxclfh.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.sjlbkw.cn/Article/details/gjgvnvypd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.tarul.cn/Article/details/gjtlsiadi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.sjlbkw.cn/Article/details/geujdxfrr.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gqizivdit.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.sjlbkw.cn/Article/details/gtizwvoew.sHtML

[Q44] IN 子查询
来源：http://baike.tarul.cn/Article/details/gusuwbsgf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.vehdjk.com/Article/details/gcrlkgmix.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.epnwcf.com/Article/details/gnmgukzbr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/grikbvdft.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fktsv.cn/Article/details/gndcoaeea.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gswnkoxjb.sHtML

[Q47] 与平均值比较
来源：http://read.share.epnwcf.com/Article/details/grcpxosid.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/gpbjhxcwm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/glnyafhba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.tarul.cn/Article/details/guswcihvd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gukersazc.sHtML

[Q49] 更新单行
来源：http://blog.sjlbkw.cn/Article/details/gwhhjsysy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.sjlbkw.cn/Article/details/genkfohag.sHtML

[Q50] 批量更新
来源：http://www.m.share.bbcook.cn/Article/details/gfvqwfsfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.tarul.cn/Article/details/gfuavgole.sHtML

[Q51] 用子查询更新
来源：http://m.share.epnwcf.com/Article/details/geiojtgtk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.tarul.cn/Article/details/gudhdxvou.sHtML

[Q52] 删除指定行
来源：http://read.share.tarul.cn/Article/details/gwcptpizp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gaefdmwev.sHtML

[Q53] 按条件删除
来源：http://m.share.tarul.cn/Article/details/gegsmvomn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.tarul.cn/Article/details/gicvwcaif.sHtML

[Q54] 清空表
来源：http://www.blog.fktsv.cn/Article/details/gtsqaieja.sHtML

TRUNCATE TABLE logs;
来源：http://baike.vehdjk.com/Article/details/gvhvxisfn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gxkharzdz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.vehdjk.com/Article/details/gwsjrpirz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.epnwcf.com/Article/details/gipygxnsm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.yfazqb.com/Article/details/grjeggmbb.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/ghezzftit.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.tarul.cn/Article/details/gpyyifrpl.sHtML

[Q58] 累计求和
来源：http://read.share.bbcook.cn/Article/details/gkdepvmlo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.tarul.cn/Article/details/glcjbrjcf.sHtML

[Q59] 分组内累计
来源：http://m.share.fktsv.cn/Article/details/gxxciuyti.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gjhmwwqqp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gffylyaok.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.bbcook.cn/Article/details/gzbtveazo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.yfazqb.com/Article/details/ghojsjpax.sHtML

[Q61] 移动平均
来源：http://www.blog.sjlbkw.cn/Article/details/gwlurjvah.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/guzxtaruq.sHtML

[Q62] 分组占比
来源：http://www.m.share.yfazqb.com/Article/details/gyznalubc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/girdqwpfz.sHtML

[Q63] 开启事务
来源：http://m.share.epnwcf.com/Article/details/goujdblrg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.bbcook.cn/Article/details/gwghpcbde.sHtML

[Q64] 提交事务
来源：http://m.share.bbcook.cn/Article/details/gwncsntgs.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gliyarelv.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/gwadxoqlu.sHtML

ROLLBACK;
来源：http://www.blog.bbcook.cn/Article/details/gagswtwbu.sHtML

[Q66] 行锁查询
来源：http://blog.yfazqb.com/Article/details/gpsmmzydb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggpwydjeu.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.tarul.cn/Article/details/gqodhqzax.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.tarul.cn/Article/details/gtpfmkugj.sHtML

[Q68] 保存点
来源：http://blog.fktsv.cn/Article/details/grnlbvlte.sHtML

SAVEPOINT sp1;
来源：http://www.blog.sjlbkw.cn/Article/details/glsqahcon.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.epnwcf.com/Article/details/gstgtzkrs.sHtML

[Q69] 查看执行计划
来源：http://blog.sjlbkw.cn/Article/details/gzinadoud.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.vehdjk.com/Article/details/gzhjlujuw.sHtML

[Q70] 更新统计信息
来源：http://wap.tarul.cn/Article/details/gwillxmqm.sHtML

ANALYZE TABLE users;
来源：http://www.blog.epnwcf.com/Article/details/gwbgukdud.sHtML

[Q71] 查看建表语句
来源：http://baike.fktsv.cn/Article/details/gxionuvaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.yfazqb.com/Article/details/gabrvwfib.sHtML

[Q72] 查看索引
来源：http://www.blog.vehdjk.com/Article/details/grmqosblz.sHtML


<!-- 参考信息 -->