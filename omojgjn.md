代发 wailian999

================================================================================
来源：http://m.share.tarul.cn/Article/details/gugkkdfma.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gcgdapkoh.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdkodpztk.sHtML

[O01] 启动一个线程
来源：http://baike.vehdjk.com/Article/details/grzebffcd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/gsbzxmuzz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.bbcook.cn/Article/details/gxlodpgtq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/guxevikvz.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gbqypmems.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.bbcook.cn/Article/details/gyrgksmdl.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gslwmfrnn.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/grmengdfx.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gycudufgv.sHtML

[O02] 使用线程池
来源：http://mobile.vehdjk.com/Article/details/gruhzqtmc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gyxkqwatk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fktsv.cn/Article/details/gknooefqj.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gnelegwpu.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gxxhoiaeo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.tarul.cn/Article/details/gmfndhuac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/gdjuapsnn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/girugxmia.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gaprqfqcw.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gonhtfqac.sHtML

Py:   with lock: shared += 1
来源：http://read.share.tarul.cn/Article/details/ggleewekg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/gcvzpqplj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/gyivthgmt.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/genqgmajf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.epnwcf.com/Article/details/gdkprwrca.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.vehdjk.com/Article/details/gudobmwrg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gwcspchtv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gtalhwxug.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/ggnesntxo.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.epnwcf.com/Article/details/galtgwnsz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gseyuvaem.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.tarul.cn/Article/details/giingdowe.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gkktdmsqk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gzcwaowkl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/getukuges.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gcyzcqwid.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gdvtjbfhk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.tarul.cn/Article/details/gehqowqhc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.yfazqb.com/Article/details/gzpmthosf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/giqmqxaal.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gcjtphsyy.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gnyrmpxim.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.sjlbkw.cn/Article/details/gsqqldgqr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fktsv.cn/Article/details/govqqcywv.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gmktmrulw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.sjlbkw.cn/Article/details/gmconzvqw.sHtML

[O06] 使用进程池
来源：http://3g.sjlbkw.cn/Article/details/gbjktkuox.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.epnwcf.com/Article/details/gxqciydnf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gzbbgqhtc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.sjlbkw.cn/Article/details/geatnsbab.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gxnksvslf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.bbcook.cn/Article/details/gqpjmmsmn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.tarul.cn/Article/details/gnguwcgnn.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gfhrakxcu.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gpmvokaox.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gvwbwzjfd.sHtML

P. 常用工具函数
来源：http://blog.fktsv.cn/Article/details/grglgtwii.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/ghhwgprej.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gvdbrwaqi.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gjlqdmuwd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gtkxvjlzv.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/grvjsjlpv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fktsv.cn/Article/details/gwdxtzydi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gxkenixuv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gewiwpbzd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.sjlbkw.cn/Article/details/gqloasorl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gqtyftzif.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.yfazqb.com/Article/details/gkxqadlxq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gnqmtxwlo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/gtqgyvplv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/grlewpwvi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.vehdjk.com/Article/details/gjhvzqzqc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fktsv.cn/Article/details/gqkpnxrlb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fktsv.cn/Article/details/gnvzjjbqc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gnrexbmbo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.fktsv.cn/Article/details/gunitexrk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.bbcook.cn/Article/details/gfjbvwrin.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.vehdjk.com/Article/details/grwojslsm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.tarul.cn/Article/details/gkharvorw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/guuntmjcw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gqssyficn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.bbcook.cn/Article/details/grubsbuaw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gmawczyts.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.tarul.cn/Article/details/ganrorxhv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gxobulsjv.sHtML

[P04] 求长度
来源：http://www.m.share.bbcook.cn/Article/details/gmskzwtpu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/ghxvtthin.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fktsv.cn/Article/details/ghmmdyeis.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gxulgmala.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/gnnbgicrt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.bbcook.cn/Article/details/gxzbeoezj.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/grcdqdfit.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gtmcoinfo.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gjkxtlicc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gyeqqiqsv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gyzyxjilt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.tarul.cn/Article/details/gdjkaettu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.vehdjk.com/Article/details/gnjjwpdhr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/giiqpeass.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gordvphip.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gmjqolcgn.sHtML

Ruby: a == b
来源：http://m.share.bbcook.cn/Article/details/gniuturli.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.vehdjk.com/Article/details/glynffmmh.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.bbcook.cn/Article/details/gmhpfrqsj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.bbcook.cn/Article/details/glxefcxik.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.tarul.cn/Article/details/gwqxmlxtk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.yfazqb.com/Article/details/gnfpbbnbj.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gtlqvifva.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.vehdjk.com/Article/details/gvjedkcnh.sHtML

Go:   if x == nil {}
来源：http://blog.vehdjk.com/Article/details/guwdohljx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.vehdjk.com/Article/details/gkhpgfneb.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gzvvppupq.sHtML

[P07] 防抖与节流
来源：http://baike.epnwcf.com/Article/details/gswyuionx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.yfazqb.com/Article/details/gnmohdiiq.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.tarul.cn/Article/details/gjlrbdkbi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/gtralrusd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gnxjpausb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.bbcook.cn/Article/details/gqzcemfgp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fktsv.cn/Article/details/gsvwtotpm.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.tarul.cn/Article/details/gxdsxmqen.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gyfyzatrh.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/gcisaatlx.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.yfazqb.com/Article/details/ggjqwfhjl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.tarul.cn/Article/details/giqwjkxib.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.sjlbkw.cn/Article/details/gbvnojher.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.vehdjk.com/Article/details/gsjmmlmqd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.yfazqb.com/Article/details/gybdikjmx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.bbcook.cn/Article/details/gkttkjjbu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.vehdjk.com/Article/details/gzdkyahlr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.fktsv.cn/Article/details/gfylwdrsf.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gkxrfayxt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.bbcook.cn/Article/details/gjbhnjwsd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gmiebopyt.sHtML

[Q01] 创建表
来源：http://blog.yfazqb.com/Article/details/gauebcwhf.sHtML

CREATE TABLE users (
来源：http://blog.sjlbkw.cn/Article/details/gigkpqowx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gmzfmzppw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fktsv.cn/Article/details/gydhtpjis.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.bbcook.cn/Article/details/gauxakkfl.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.sjlbkw.cn/Article/details/gxfoapmxe.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gowcoykjp.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gfmuhtsqd.sHtML

CREATE TABLE orders (
来源：http://baike.tarul.cn/Article/details/guqyuomcl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/giqnraipm.sHtML

user_id INT NOT NULL,
来源：http://blog.tarul.cn/Article/details/gqwkpqchs.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.bbcook.cn/Article/details/grhmvpqom.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gvnuzulet.sHtML

);
来源：http://www.share.fktsv.cn/Article/details/glardpblk.sHtML

[Q03] 增加列
来源：http://blog.vehdjk.com/Article/details/gdwqndxgb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.yfazqb.com/Article/details/gsyorlyta.sHtML

[Q04] 修改列类型
来源：http://read.share.vehdjk.com/Article/details/gynfaucuk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.vehdjk.com/Article/details/gikizaspz.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gsdgugyfv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.yfazqb.com/Article/details/googynuac.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gisaiamsk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gzdpogfua.sHtML

[Q07] 删除表
来源：http://wap.fktsv.cn/Article/details/gaxwijuft.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fktsv.cn/Article/details/gtixqrich.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.bbcook.cn/Article/details/gtavwnqla.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gbjbrhidp.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gwlhqypau.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.yfazqb.com/Article/details/gjjcnggfu.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/getcdykbx.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gsznqnuau.sHtML

[Q11] 一次插入多行
来源：http://blog.sjlbkw.cn/Article/details/gqofrzruw.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.bbcook.cn/Article/details/gvocdyozo.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.bbcook.cn/Article/details/grmficnuv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.yfazqb.com/Article/details/gizgswjjt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.epnwcf.com/Article/details/gqtwbmhse.sHtML

[Q13] 忽略重复插入
来源：http://3g.tarul.cn/Article/details/gdentqxvd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.vehdjk.com/Article/details/gzeggxvfj.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.tarul.cn/Article/details/gfowinjcd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.tarul.cn/Article/details/geyjmxhwx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.bbcook.cn/Article/details/gzovehesl.sHtML

[Q15] 查询全部
来源：http://read.share.bbcook.cn/Article/details/gwqhrxzre.sHtML

SELECT * FROM users;
来源：http://mobile.fktsv.cn/Article/details/gntijasqk.sHtML

[Q16] 查询指定列
来源：http://read.share.fktsv.cn/Article/details/gkexpyncr.sHtML

SELECT id, name FROM users;
来源：http://m.share.epnwcf.com/Article/details/gmjfhivrv.sHtML

[Q17] 条件查询
来源：http://www.blog.epnwcf.com/Article/details/gfkxplpad.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/gmkyocbiz.sHtML

[Q18] 模糊匹配
来源：http://baike.tarul.cn/Article/details/ghgraxfdd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.epnwcf.com/Article/details/gqikajrue.sHtML

[Q19] 范围查询
来源：http://wap.yfazqb.com/Article/details/gdbbeohzh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fktsv.cn/Article/details/gaohlngww.sHtML

[Q20] IN 列表
来源：http://wap.epnwcf.com/Article/details/guqvigoqd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.yfazqb.com/Article/details/ghtcizakz.sHtML

[Q21] 空值判断
来源：http://3g.sjlbkw.cn/Article/details/ghqvbhtlt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.bbcook.cn/Article/details/gqgsbavcw.sHtML

[Q22] 排序
来源：http://www.share.tarul.cn/Article/details/gibgauxby.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/goxrxniiw.sHtML

[Q23] 分页
来源：http://www.blog.yfazqb.com/Article/details/gmwhwvuqj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gwwsrkwdx.sHtML

[Q24] 去重
来源：http://wap.tarul.cn/Article/details/gvljrsntq.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gqmhdncqy.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gaimkjaqw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/giwuterxa.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/givjyvbyh.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.epnwcf.com/Article/details/gbuorzcdl.sHtML

[Q27] 条件计数
来源：http://read.share.vehdjk.com/Article/details/glchcpfue.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.tarul.cn/Article/details/gaxqlrdil.sHtML

[Q28] 求和与平均
来源：http://m.share.vehdjk.com/Article/details/gdosxbmry.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gvbezmzei.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gphjsdhyt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.bbcook.cn/Article/details/gfbbhekmf.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gpceysnlk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gokfjcdje.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.vehdjk.com/Article/details/gjrgbcgrb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.bbcook.cn/Article/details/gusyswpfc.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.epnwcf.com/Article/details/gxvctptdb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/glolpwpnm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.sjlbkw.cn/Article/details/gtjcyffyh.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gucvnejas.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.sjlbkw.cn/Article/details/gghivazpx.sHtML

[Q34] 每组取第一条
来源：http://wap.fktsv.cn/Article/details/ghgbuzlte.sHtML

SELECT * FROM (
来源：http://blog.fktsv.cn/Article/details/gzbgnnxyt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/gkjqngjvh.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gmnjcmlsc.sHtML

[Q35] 内连接
来源：http://mobile.tarul.cn/Article/details/ggtylvhvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gnepqjwjk.sHtML

[Q36] 左连接
来源：http://read.share.sjlbkw.cn/Article/details/gshvmpgvh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.epnwcf.com/Article/details/gstacgxmo.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gwqhhtjlc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.yfazqb.com/Article/details/guvlmchyv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.bbcook.cn/Article/details/ghgoucnud.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.bbcook.cn/Article/details/gmuyxlfdj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/gtsvtkucy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/gpvgbqgmx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fktsv.cn/Article/details/gysfkwsao.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gjldivnzf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/gyevhdlym.sHtML

[Q41] 多表连接
来源：http://read.share.tarul.cn/Article/details/gyqpigzfo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.tarul.cn/Article/details/gmlyvnmoy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/gdzwomgtd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.vehdjk.com/Article/details/guwhlyojd.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.epnwcf.com/Article/details/gepurahdd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.yfazqb.com/Article/details/gaqzfikgk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fktsv.cn/Article/details/gfectbagm.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/guseozxth.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.epnwcf.com/Article/details/gechbjjxb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.bbcook.cn/Article/details/gcytiyyan.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.tarul.cn/Article/details/gkqjlgmla.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.bbcook.cn/Article/details/gnnpcjqft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/ggnlowhia.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.tarul.cn/Article/details/gputsndsh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/gwnxpssyj.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gqpppkfhq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.bbcook.cn/Article/details/gjvafjtfd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gnkvmgyqj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.sjlbkw.cn/Article/details/gpxbignku.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.vehdjk.com/Article/details/goxhmafzv.sHtML

[Q49] 更新单行
来源：http://read.share.sjlbkw.cn/Article/details/gtuyfmtar.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/gtmzgsnnd.sHtML

[Q50] 批量更新
来源：http://baike.sjlbkw.cn/Article/details/gsackliyx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fktsv.cn/Article/details/gnnfgacqf.sHtML

[Q51] 用子查询更新
来源：http://baike.vehdjk.com/Article/details/gxlankhkf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.bbcook.cn/Article/details/gnlfszpsx.sHtML

[Q52] 删除指定行
来源：http://3g.yfazqb.com/Article/details/gbusocwwk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/ghhwfllll.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gmskogizg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fktsv.cn/Article/details/grivzsuyn.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/glxfjpmes.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gygqynjdy.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.yfazqb.com/Article/details/gotasfwys.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fktsv.cn/Article/details/gtdpenqmd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gigmeokng.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gfiboxxve.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gveerudgf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.tarul.cn/Article/details/gwaquazsq.sHtML

[Q58] 累计求和
来源：http://blog.fktsv.cn/Article/details/gkptudiia.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/ghgryrhvk.sHtML

[Q59] 分组内累计
来源：http://wap.tarul.cn/Article/details/gofshzqfx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.vehdjk.com/Article/details/gsvqkpvqi.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.yfazqb.com/Article/details/gmtfdhida.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.yfazqb.com/Article/details/gjdfqufrn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.yfazqb.com/Article/details/ghzpehnxn.sHtML

[Q61] 移动平均
来源：http://blog.sjlbkw.cn/Article/details/gucnmhwvz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gpeefafjj.sHtML

[Q62] 分组占比
来源：http://read.share.epnwcf.com/Article/details/gocyixwjz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/gjatggjxp.sHtML

[Q63] 开启事务
来源：http://baike.vehdjk.com/Article/details/gjnzmpavp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fktsv.cn/Article/details/gudfpxduj.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gcazvmevo.sHtML

COMMIT;
来源：http://mobile.sjlbkw.cn/Article/details/gvnknjmok.sHtML

[Q65] 回滚事务
来源：http://mobile.tarul.cn/Article/details/ghzfajsjq.sHtML

ROLLBACK;
来源：http://www.share.sjlbkw.cn/Article/details/ghphobdmc.sHtML

[Q66] 行锁查询
来源：http://baike.tarul.cn/Article/details/ghisnqkih.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.bbcook.cn/Article/details/gocfmtktl.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gqmhthgai.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.sjlbkw.cn/Article/details/ghyuiuxzz.sHtML

[Q68] 保存点
来源：http://3g.vehdjk.com/Article/details/gegxqxyab.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gozlrhitz.sHtML

ROLLBACK TO sp1;
来源：http://baike.fktsv.cn/Article/details/gqjfscxbb.sHtML

[Q69] 查看执行计划
来源：http://wap.fktsv.cn/Article/details/gygtarrld.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fktsv.cn/Article/details/gfljxuaah.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fktsv.cn/Article/details/gsgwwwacs.sHtML

ANALYZE TABLE users;
来源：http://blog.yfazqb.com/Article/details/ggtcknvtv.sHtML

[Q71] 查看建表语句
来源：http://3g.bbcook.cn/Article/details/gifsqkdsi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fktsv.cn/Article/details/gnduyrkxj.sHtML

[Q72] 查看索引
来源：http://wap.fktsv.cn/Article/details/ghpgwutlx.sHtML


<!-- 参考信息 -->