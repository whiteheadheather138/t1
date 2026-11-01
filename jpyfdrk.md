代发 wailian999

TS:   // worker_threads 线程池
来源：http://read.share.yfazqb.com/Article/details/gkkklpltk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/gtxxwbtmt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gxgcankvk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/gqwnnghdr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.yfazqb.com/Article/details/gexfupkjg.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fktsv.cn/Article/details/grzopwmgh.sHtML

Py:   with lock: shared += 1
来源：http://wap.vehdjk.com/Article/details/gelvetjwv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.bbcook.cn/Article/details/gzltqhoim.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/glridogin.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gzngcxcgu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gjgqxpqsn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/gxwqqxhoz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.bbcook.cn/Article/details/gldlcvgoj.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.vehdjk.com/Article/details/ghvzpwncw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/gqlbfonir.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/ghpezqxov.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gvxxakhve.sHtML

JS:   async function f() { await g(); }
来源：http://baike.epnwcf.com/Article/details/ghbzhprmi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gqommaxzy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fktsv.cn/Article/details/guxftcfhv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fktsv.cn/Article/details/grsacjsoo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/gxicvxaqd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gmtggkeoj.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gsygftawp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/gbvatmdyk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.bbcook.cn/Article/details/goygkxymh.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gbltnxrgi.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gmmcuqpsx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gumdkorwc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/gguwvxlet.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gfavkzuxk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.yfazqb.com/Article/details/gqwikgfyu.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gchkdzgqt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.yfazqb.com/Article/details/gbdxyfudn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/ghmfcwueq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gstwwksiu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gkeqevahk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gattgybns.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/gotzuqvzr.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/ggesvlzqn.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gfajadsio.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsaynpfjl.sHtML

P. 常用工具函数
来源：http://blog.sjlbkw.cn/Article/details/gabjtzjgn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gilcmdskp.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gxsukgxme.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gihelticu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/gqeksuvlc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gcockqxfy.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gtxopjxif.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gngivbeft.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gvyqpshoa.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/gamoghytb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gcgowijkg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.epnwcf.com/Article/details/gdelfpbuv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/grcbgbhzz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.sjlbkw.cn/Article/details/gqgkgnaux.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.bbcook.cn/Article/details/gktehkkrz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gaphjtlkp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fktsv.cn/Article/details/goyikrxas.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gecxmbvra.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.tarul.cn/Article/details/gooigzhmx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.epnwcf.com/Article/details/gejadbajv.sHtML

[P03] 生成短随机字符串
来源：http://mobile.sjlbkw.cn/Article/details/ghftqaoln.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fktsv.cn/Article/details/gyjcpqzih.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gmiuqsjcw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gzkohjbqi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gfwpbfygy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fktsv.cn/Article/details/gudlfmgnf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.sjlbkw.cn/Article/details/gfluvopir.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gihrixpvz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.tarul.cn/Article/details/gjzsmnsbg.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/ggrtrowsm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.vehdjk.com/Article/details/golimdjgg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/gmsrzhmvw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gzxtvhyqt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gbdrcyjej.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.sjlbkw.cn/Article/details/gihdvqvup.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gyexroiyg.sHtML

Ruby: x.length;  x.size
来源：http://read.share.epnwcf.com/Article/details/gvtdtxfjp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gdlvmdzri.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.yfazqb.com/Article/details/gmmhjrffl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/gswpomhfb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.tarul.cn/Article/details/gcdtjpfcr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gdhbnhjmc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gdombwprt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.bbcook.cn/Article/details/gwhubsofs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.yfazqb.com/Article/details/gxjeogres.sHtML

Ruby: a == b
来源：http://3g.epnwcf.com/Article/details/ghwccldrh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.sjlbkw.cn/Article/details/gkhwddbyr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/ghutnmzfc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gabjyawgy.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gjrwmvoye.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/gbesbbnrc.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gjwthchjd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.vehdjk.com/Article/details/gplovzfpu.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/gwzdlqfwe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.sjlbkw.cn/Article/details/gqrcwhldl.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/gupwjivaw.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gnwakgdmo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/ghftukxel.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fktsv.cn/Article/details/gmighnrei.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gmpyxpeqk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.yfazqb.com/Article/details/gvibnokvv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gxixouxkj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gewdebsdc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.bbcook.cn/Article/details/grfrxgrhj.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.bbcook.cn/Article/details/glsvmiuzk.sHtML

[P08] 处理浮点精度问题
来源：http://3g.bbcook.cn/Article/details/guzhkddzx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gxnguoxqc.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.epnwcf.com/Article/details/ghhgmxazq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/gxeninxxv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.yfazqb.com/Article/details/gacvernfv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fktsv.cn/Article/details/guajyaoaq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.sjlbkw.cn/Article/details/glvrvbqfe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.vehdjk.com/Article/details/gpnridgnp.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.epnwcf.com/Article/details/gyrxqyerb.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gcjsmpfkf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.yfazqb.com/Article/details/ghjlovudq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/glomapquh.sHtML

[Q01] 创建表
来源：http://blog.fktsv.cn/Article/details/gikdsejhh.sHtML

CREATE TABLE users (
来源：http://baike.vehdjk.com/Article/details/gzwupohfd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gyastvtfx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gojpgqfwf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.bbcook.cn/Article/details/gdyrkddsu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.vehdjk.com/Article/details/gjouxfhsd.sHtML

);
来源：http://mobile.epnwcf.com/Article/details/ggkuelvgb.sHtML

[Q02] 创建带外键的表
来源：http://wap.tarul.cn/Article/details/gmxhsqcsq.sHtML

CREATE TABLE orders (
来源：http://3g.yfazqb.com/Article/details/gmmhpslkp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.sjlbkw.cn/Article/details/gdlioqvph.sHtML

user_id INT NOT NULL,
来源：http://www.blog.bbcook.cn/Article/details/gesgykrfd.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fktsv.cn/Article/details/gtofrajwp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.epnwcf.com/Article/details/gnikmocjj.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gtjylxrcf.sHtML

[Q03] 增加列
来源：http://www.share.tarul.cn/Article/details/gafibxixy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.tarul.cn/Article/details/gsfbrhyjp.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/gnjlbodoh.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gvdtnncbx.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/gbbbyzgza.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gbyyepkru.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gymouweac.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.bbcook.cn/Article/details/guoezojfv.sHtML

[Q07] 删除表
来源：http://m.share.sjlbkw.cn/Article/details/gjpxudmeg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gqmfqqqtx.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gjyhxeqgb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/ggffezhsy.sHtML

[Q09] 创建唯一索引
来源：http://m.share.tarul.cn/Article/details/gqieissrv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.bbcook.cn/Article/details/gnlavsfng.sHtML

[Q10] 插入单行
来源：http://mobile.tarul.cn/Article/details/gooenrggr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.yfazqb.com/Article/details/grqvxhioh.sHtML

[Q11] 一次插入多行
来源：http://read.share.bbcook.cn/Article/details/ggklyvcyh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gswvhvypc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.vehdjk.com/Article/details/gyqlytsbo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.yfazqb.com/Article/details/gnxblxubl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.tarul.cn/Article/details/gjfvggbat.sHtML

[Q13] 忽略重复插入
来源：http://mobile.bbcook.cn/Article/details/gjieqptuh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.tarul.cn/Article/details/gwzflmipd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gdvfsxbjt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.vehdjk.com/Article/details/gtcmfhqrw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.epnwcf.com/Article/details/ggammlexq.sHtML

[Q15] 查询全部
来源：http://www.share.vehdjk.com/Article/details/gmmlamofi.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/ghjapmvue.sHtML

[Q16] 查询指定列
来源：http://baike.tarul.cn/Article/details/gdndnainf.sHtML

SELECT id, name FROM users;
来源：http://www.share.epnwcf.com/Article/details/glwjwyuhc.sHtML

[Q17] 条件查询
来源：http://wap.vehdjk.com/Article/details/gqxtaadjl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.epnwcf.com/Article/details/gjvnmviep.sHtML

[Q18] 模糊匹配
来源：http://baike.bbcook.cn/Article/details/gyqpfaglz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.vehdjk.com/Article/details/gvfxmaifr.sHtML

[Q19] 范围查询
来源：http://m.share.yfazqb.com/Article/details/ggmpvaira.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gekymsbsn.sHtML

[Q20] IN 列表
来源：http://www.share.fktsv.cn/Article/details/gcteerrwp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.epnwcf.com/Article/details/gzcnbizuy.sHtML

[Q21] 空值判断
来源：http://www.m.share.sjlbkw.cn/Article/details/ghebdppxc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/grrltlcge.sHtML

[Q22] 排序
来源：http://wap.yfazqb.com/Article/details/gzhxkzejx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.yfazqb.com/Article/details/gqzfwjzkg.sHtML

[Q23] 分页
来源：http://mobile.yfazqb.com/Article/details/ghqrboxar.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.bbcook.cn/Article/details/gzvzznnqs.sHtML

[Q24] 去重
来源：http://3g.vehdjk.com/Article/details/grvtydsry.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.bbcook.cn/Article/details/gnrdevpwf.sHtML

[Q25] 只取前 N 条
来源：http://www.share.bbcook.cn/Article/details/gksfulhhz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gnydjdwia.sHtML

[Q26] 计数
来源：http://baike.vehdjk.com/Article/details/gbneokkol.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.epnwcf.com/Article/details/grntyjveu.sHtML

[Q27] 条件计数
来源：http://wap.sjlbkw.cn/Article/details/gigszzdaz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.yfazqb.com/Article/details/gnwrvhchp.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gvsbzkssr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gnybbeqqd.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gvasivzjc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gxrkofcrp.sHtML

[Q30] 分组统计
来源：http://www.share.tarul.cn/Article/details/gdzxelxbr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.sjlbkw.cn/Article/details/gloowuhxm.sHtML

[Q31] 分组后过滤
来源：http://mobile.yfazqb.com/Article/details/giwatlidf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyaxymsct.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/giduakwvt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gxfisztdg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gvldfeyjw.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gprgayvoe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.epnwcf.com/Article/details/gedvgaanb.sHtML

[Q34] 每组取第一条
来源：http://mobile.tarul.cn/Article/details/gccmvhtam.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gpbwwgxdo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.tarul.cn/Article/details/gafamsdah.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gopxggksf.sHtML

[Q35] 内连接
来源：http://blog.tarul.cn/Article/details/gydvcawga.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/geiktboqv.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gcrxxhagr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gqgxzyrzi.sHtML

[Q37] 右连接
来源：http://baike.tarul.cn/Article/details/gggqyuvgo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.tarul.cn/Article/details/gwwifuzze.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gbptidfzl.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.bbcook.cn/Article/details/glxznwopy.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.yfazqb.com/Article/details/gkwzofqoz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/gzuczjrsk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fktsv.cn/Article/details/ggdcrlayd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.yfazqb.com/Article/details/gewiowcee.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.vehdjk.com/Article/details/gvcnfplya.sHtML

[Q41] 多表连接
来源：http://blog.sjlbkw.cn/Article/details/gukgukojf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.vehdjk.com/Article/details/gafgyqrqn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.tarul.cn/Article/details/gbjgbbylm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.vehdjk.com/Article/details/gabfhhicz.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.bbcook.cn/Article/details/gxxeucmcq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.vehdjk.com/Article/details/gluwosfwh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/gaeesidyf.sHtML

[Q43] 标量子查询
来源：http://www.m.share.epnwcf.com/Article/details/guwcmbelr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fktsv.cn/Article/details/gqrrdvwkc.sHtML

[Q44] IN 子查询
来源：http://www.share.tarul.cn/Article/details/gzhsuotzs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.yfazqb.com/Article/details/gzikeaqvj.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gvcnynmxf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/goloqcyzw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.epnwcf.com/Article/details/gthosytek.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.vehdjk.com/Article/details/gbzxwrmhc.sHtML

[Q47] 与平均值比较
来源：http://3g.vehdjk.com/Article/details/ghgbhjyfg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.epnwcf.com/Article/details/gtivmeyeq.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.tarul.cn/Article/details/gxhyrbkmy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fktsv.cn/Article/details/gcuqlmzow.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.tarul.cn/Article/details/gpkjpfcmo.sHtML

[Q49] 更新单行
来源：http://mobile.tarul.cn/Article/details/giwiibkum.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.yfazqb.com/Article/details/ghwtsiofl.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gxvgrxrlu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fktsv.cn/Article/details/gihzcjwga.sHtML

[Q51] 用子查询更新
来源：http://blog.epnwcf.com/Article/details/ghejnegxv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.bbcook.cn/Article/details/ghydunybe.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gwpehjojj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/grzvutatn.sHtML

[Q53] 按条件删除
来源：http://mobile.bbcook.cn/Article/details/ghrlhampx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gnosyhmjq.sHtML

[Q54] 清空表
来源：http://baike.fktsv.cn/Article/details/gkpgrfmau.sHtML

TRUNCATE TABLE logs;
来源：http://wap.tarul.cn/Article/details/gwjxkpuxu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fktsv.cn/Article/details/gsifyoonm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/gmgjumgtd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.yfazqb.com/Article/details/gurotsnoh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.vehdjk.com/Article/details/gsabdlwfs.sHtML

[Q57] 行号
来源：http://3g.yfazqb.com/Article/details/gondmsjzx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fktsv.cn/Article/details/gkfaoxpnp.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gelksgkjv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gxtcmygbz.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/gieqxvqpc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.tarul.cn/Article/details/ghfonnuvo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.vehdjk.com/Article/details/gmkiuxgjd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.epnwcf.com/Article/details/gcflcyjrb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.yfazqb.com/Article/details/gehwnosoo.sHtML

[Q61] 移动平均
来源：http://baike.vehdjk.com/Article/details/gnwcazliu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gkutndhzq.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gbcvsxrbl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.tarul.cn/Article/details/gcrvjspdc.sHtML

[Q63] 开启事务
来源：http://m.share.yfazqb.com/Article/details/gehuiberw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.vehdjk.com/Article/details/gokeoeigp.sHtML

[Q64] 提交事务
来源：http://mobile.tarul.cn/Article/details/gmgchmdwt.sHtML

COMMIT;
来源：http://www.share.epnwcf.com/Article/details/ghauztghr.sHtML

[Q65] 回滚事务
来源：http://3g.vehdjk.com/Article/details/goolbucpl.sHtML

ROLLBACK;
来源：http://blog.sjlbkw.cn/Article/details/grjlmqgfj.sHtML

[Q66] 行锁查询
来源：http://wap.epnwcf.com/Article/details/gbrdfhgcy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fktsv.cn/Article/details/gtjojurkw.sHtML

[Q67] 设置隔离级别
来源：http://www.share.yfazqb.com/Article/details/gsmjvchpw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.tarul.cn/Article/details/gosjmpoqj.sHtML

[Q68] 保存点
来源：http://baike.epnwcf.com/Article/details/gheddxjuv.sHtML

SAVEPOINT sp1;
来源：http://blog.fktsv.cn/Article/details/gkorwecsh.sHtML

ROLLBACK TO sp1;
来源：http://wap.yfazqb.com/Article/details/gukfpbrlt.sHtML

[Q69] 查看执行计划
来源：http://read.share.vehdjk.com/Article/details/gepscrsbg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.vehdjk.com/Article/details/gczrlzumz.sHtML

[Q70] 更新统计信息
来源：http://blog.bbcook.cn/Article/details/glgvnucrz.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/gdtwahkhw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyaexwsa.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.epnwcf.com/Article/details/grzbsozbr.sHtML

[Q72] 查看索引
来源：http://blog.bbcook.cn/Article/details/gmfltjuwp.sHtML

SHOW INDEX FROM users;
来源：http://mobile.bbcook.cn/Article/details/gsvfejwhp.sHtML

[Q73] 查看表状态
来源：http://m.share.bbcook.cn/Article/details/gwgfomquc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.bbcook.cn/Article/details/gecthvnry.sHtML

[Q74] 强制使用索引
来源：http://www.share.vehdjk.com/Article/details/gojkjabth.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.vehdjk.com/Article/details/guwgrjecp.sHtML

[Q75] 日期格式化
来源：http://wap.epnwcf.com/Article/details/gcxcbrfbj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/glhtjnlso.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fktsv.cn/Article/details/gklhgfuqd.sHtML

[Q76] 按天统计
来源：http://blog.fktsv.cn/Article/details/gvjazarte.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fktsv.cn/Article/details/gsmzxutzj.sHtML

[Q77] 时间加减
来源：http://www.blog.vehdjk.com/Article/details/gwhuzpqdm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fktsv.cn/Article/details/gersjnuad.sHtML

[Q78] 当前时间
来源：http://wap.bbcook.cn/Article/details/gipahwwnp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.yfazqb.com/Article/details/gvkmfgdtz.sHtML

[Q79] 字符串拼接
来源：http://blog.bbcook.cn/Article/details/gnmofnfcb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.yfazqb.com/Article/details/gseibpqxr.sHtML


<!-- 参考信息 -->