代发 wailian999

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzrlvlakd.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gxnkohsml.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gkkdvcmod.sHtML

[O01] 启动一个线程
来源：http://www.share.fktsv.cn/Article/details/gypdqrdqd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gbkibdjbg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gpqxbualj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/gdylmbhyj.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gfzxwljka.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/gappxmrle.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gkeneemda.sHtML

Ruby: Thread.new { f }
来源：http://blog.bbcook.cn/Article/details/gpyebbhkj.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gmsiwewzl.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/glzkcmpyf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/glsqnedek.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gusizlmrt.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gtywaarem.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gdchlbolf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/gtxoukyps.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/glcjmyanh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.vehdjk.com/Article/details/gfupskvrp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/ggyzfgrsl.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/gcsqwbwas.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/gzfoitesj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/grvasnxmq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.sjlbkw.cn/Article/details/gsnfgjrfj.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/grrwlhhkg.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fktsv.cn/Article/details/grarycewa.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gliujbbrn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gtrzuksvz.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gugxbyscu.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gjfjczjir.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gofsauoyw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.yfazqb.com/Article/details/gfmrvhczv.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gfzuoixke.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gqisqvaau.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gzvrlzghc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gzgczxrhk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.vehdjk.com/Article/details/glnowpsjg.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.epnwcf.com/Article/details/gvckkjdat.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.sjlbkw.cn/Article/details/gpyfhogmj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/goolhtiam.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.epnwcf.com/Article/details/gysqsdsax.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/gioshvmru.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.tarul.cn/Article/details/geebtdyuo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.vehdjk.com/Article/details/gnuhzexjy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gmygmuakw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.yfazqb.com/Article/details/gjispdxse.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fktsv.cn/Article/details/gradvxivo.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/guqopomry.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.vehdjk.com/Article/details/gewadahih.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gfekpxtsm.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gcpnydcea.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/givfxtgsp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.vehdjk.com/Article/details/gwukdmpdl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/gfvpsnltk.sHtML

Ruby: // fork 块
来源：http://www.blog.bbcook.cn/Article/details/gaojzzikh.sHtML

C#:   Parallel.For
来源：http://www.m.share.vehdjk.com/Article/details/gggmvxctb.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gcdlrsddx.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gjcnosciz.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gnwvblrsj.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gpiqglfsv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gjowxnqns.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/gtunnqllj.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/guqikpzez.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gogpupjje.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.bbcook.cn/Article/details/gobqgefvy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gfouhyfzf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.bbcook.cn/Article/details/gpxirgylg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gffvvlwur.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fktsv.cn/Article/details/gkivpjujq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/grgkhubil.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.epnwcf.com/Article/details/gbbacwxuc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fktsv.cn/Article/details/gwrnxomst.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/gklhtzjqo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.epnwcf.com/Article/details/gllhayegc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/gdlxvzlfr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/giqfhxcvn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.sjlbkw.cn/Article/details/gldjqxchw.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gssvtstlp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gzvlexptt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.vehdjk.com/Article/details/gmvrwcxuo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gbljadssh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gwiivisyu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fktsv.cn/Article/details/gwjupjapz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.vehdjk.com/Article/details/gvryetopq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.sjlbkw.cn/Article/details/gmghkncex.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.sjlbkw.cn/Article/details/gejzdhtbv.sHtML

[P04] 求长度
来源：http://www.blog.yfazqb.com/Article/details/gdjhnzpma.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.vehdjk.com/Article/details/gehpswyjz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.vehdjk.com/Article/details/gnmveedrh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gpieszlzl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.bbcook.cn/Article/details/gmhrfgxjf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.sjlbkw.cn/Article/details/grrbykskc.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/gwjcamfmn.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/gvugkiiji.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.bbcook.cn/Article/details/groxkdnes.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.yfazqb.com/Article/details/gmvuiltmu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gdhelbjpn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gacyueieq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.bbcook.cn/Article/details/gupjoaglk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.vehdjk.com/Article/details/gdpazfcfo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.sjlbkw.cn/Article/details/gtozfsuic.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.vehdjk.com/Article/details/gjmcoetnq.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gyhroobqx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.vehdjk.com/Article/details/gkvgwkrla.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gvesstpqy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.bbcook.cn/Article/details/gwtyeltte.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.epnwcf.com/Article/details/gszqkcqgr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.sjlbkw.cn/Article/details/glztneipv.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/gnbcalngi.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.yfazqb.com/Article/details/gcwohsomo.sHtML

Go:   if x == nil {}
来源：http://www.blog.tarul.cn/Article/details/gsmmkslxb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.tarul.cn/Article/details/gcpmlykza.sHtML

C#:   if (x is null) {}
来源：http://mobile.bbcook.cn/Article/details/gkzbargrk.sHtML

[P07] 防抖与节流
来源：http://www.blog.epnwcf.com/Article/details/gnbgvgluu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.yfazqb.com/Article/details/gqvijlytp.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.yfazqb.com/Article/details/gdkdkkpla.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsgzodhu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gvomzvhai.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.sjlbkw.cn/Article/details/gnvmevrqy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.sjlbkw.cn/Article/details/giaypfstt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gbvukmprl.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gihgggvho.sHtML

[P08] 处理浮点精度问题
来源：http://wap.sjlbkw.cn/Article/details/gaikpkcdj.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.sjlbkw.cn/Article/details/gzwcsbhgu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/genknywar.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.bbcook.cn/Article/details/gbpjpjcrx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.vehdjk.com/Article/details/gvjrhffwx.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.tarul.cn/Article/details/glmrgzmkj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.bbcook.cn/Article/details/gsjqvbilp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.epnwcf.com/Article/details/gpcurwwkf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.epnwcf.com/Article/details/gghpbtcau.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/goaxdcbug.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/giurzadfz.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghqxnffrp.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gnlbflbpr.sHtML

CREATE TABLE users (
来源：http://www.share.yfazqb.com/Article/details/gumyjnrnb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.epnwcf.com/Article/details/gefznqtmk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/ghndlqtcf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.tarul.cn/Article/details/guwyuixaz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.yfazqb.com/Article/details/gvbwqxnft.sHtML

);
来源：http://read.share.vehdjk.com/Article/details/gasrxgcah.sHtML

[Q02] 创建带外键的表
来源：http://3g.vehdjk.com/Article/details/gqtisjnsy.sHtML

CREATE TABLE orders (
来源：http://wap.epnwcf.com/Article/details/gqyayaqos.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/grqujjibm.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/gakgyftvk.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fktsv.cn/Article/details/gjjefsfyd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gxvobbfmi.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gakvrgoni.sHtML

[Q03] 增加列
来源：http://www.share.vehdjk.com/Article/details/gcxywvkst.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.bbcook.cn/Article/details/gxnoodbqe.sHtML

[Q04] 修改列类型
来源：http://mobile.vehdjk.com/Article/details/ghvxsbasy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.sjlbkw.cn/Article/details/gigwgwdmn.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gqywdjegx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.epnwcf.com/Article/details/gtshdngmc.sHtML

[Q06] 删除列
来源：http://www.blog.tarul.cn/Article/details/gqodwpqlj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fktsv.cn/Article/details/gzhhghoxa.sHtML

[Q07] 删除表
来源：http://mobile.fktsv.cn/Article/details/gdjeupzed.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.sjlbkw.cn/Article/details/gfendbhzk.sHtML

[Q08] 创建普通索引
来源：http://read.share.sjlbkw.cn/Article/details/groocvpvo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/gvwtnpcox.sHtML

[Q09] 创建唯一索引
来源：http://blog.bbcook.cn/Article/details/gnifwcelx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gsawewupa.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/gewknttta.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gqvwweqbp.sHtML

[Q11] 一次插入多行
来源：http://wap.vehdjk.com/Article/details/geivnxkua.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gjioxusum.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.epnwcf.com/Article/details/gdluuvppb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.vehdjk.com/Article/details/ggjmcubjv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.sjlbkw.cn/Article/details/gjohowvko.sHtML

[Q13] 忽略重复插入
来源：http://read.share.vehdjk.com/Article/details/gkgzqcbqg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.tarul.cn/Article/details/gttuyzyjo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.vehdjk.com/Article/details/goknwncvi.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.sjlbkw.cn/Article/details/gftoakxxj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.epnwcf.com/Article/details/girsqaswz.sHtML

[Q15] 查询全部
来源：http://mobile.epnwcf.com/Article/details/gzrstmgyp.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gecpnfpzp.sHtML

[Q16] 查询指定列
来源：http://www.share.tarul.cn/Article/details/gedjpvgkf.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gkypvkcjo.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/gudkzlvcv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.bbcook.cn/Article/details/gerwdprvg.sHtML

[Q18] 模糊匹配
来源：http://www.share.fktsv.cn/Article/details/gjavzarsl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/gerihkbbs.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/ghgakkvfc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.tarul.cn/Article/details/gzgdztida.sHtML

[Q20] IN 列表
来源：http://www.share.yfazqb.com/Article/details/gcexjmsmh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.epnwcf.com/Article/details/gcsgjomgx.sHtML

[Q21] 空值判断
来源：http://3g.fktsv.cn/Article/details/gocfidphq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.vehdjk.com/Article/details/gpnwlkrxo.sHtML

[Q22] 排序
来源：http://m.share.yfazqb.com/Article/details/gtbwnwprx.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.bbcook.cn/Article/details/gcsrkftpv.sHtML

[Q23] 分页
来源：http://www.share.sjlbkw.cn/Article/details/gknybdqbi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gtblzkqxz.sHtML

[Q24] 去重
来源：http://m.share.yfazqb.com/Article/details/gquekjqnh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.bbcook.cn/Article/details/gpimpnrsw.sHtML

[Q25] 只取前 N 条
来源：http://3g.tarul.cn/Article/details/gjuvtczwm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.vehdjk.com/Article/details/gchmcowux.sHtML

[Q26] 计数
来源：http://mobile.fktsv.cn/Article/details/goawilque.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gfrraxmrh.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gqtianasn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gbyblzwtk.sHtML

[Q28] 求和与平均
来源：http://m.share.yfazqb.com/Article/details/gfgfqjtui.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gczdmakqo.sHtML

[Q29] 最大最小值
来源：http://www.share.tarul.cn/Article/details/gwjxvujrf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.epnwcf.com/Article/details/glosltvpd.sHtML

[Q30] 分组统计
来源：http://blog.fktsv.cn/Article/details/ggdtdmrho.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gxeowxuse.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/gxezqfhim.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.epnwcf.com/Article/details/gpbsxmbwp.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.epnwcf.com/Article/details/girtbrmxd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.tarul.cn/Article/details/gzmuxartu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fktsv.cn/Article/details/gmratmcvm.sHtML

[Q33] 多列分组
来源：http://read.share.sjlbkw.cn/Article/details/glzqtywdy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.sjlbkw.cn/Article/details/grmyjjiwn.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gnduyfngc.sHtML

SELECT * FROM (
来源：http://read.share.vehdjk.com/Article/details/gxrvghgyb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fktsv.cn/Article/details/gwyfktcoa.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gdrpybhbm.sHtML

[Q35] 内连接
来源：http://www.share.sjlbkw.cn/Article/details/gjjqmrsem.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.tarul.cn/Article/details/gdaigqgww.sHtML

[Q36] 左连接
来源：http://www.blog.tarul.cn/Article/details/gxbexsuiq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.bbcook.cn/Article/details/gdauazbqd.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gtcabrkuj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gmvblawva.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gsxzftqqs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/ghmnfvtbp.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.yfazqb.com/Article/details/gryhltqma.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.bbcook.cn/Article/details/gioawptsq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.bbcook.cn/Article/details/goswnafyb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.sjlbkw.cn/Article/details/gvaagizea.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gzmkvllej.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gynnknukt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.epnwcf.com/Article/details/gigkiwfiq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.tarul.cn/Article/details/gdfusywaa.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.epnwcf.com/Article/details/gcwehbyvr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.epnwcf.com/Article/details/gtmbycovd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fktsv.cn/Article/details/gzhbluykb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gpjbvsfef.sHtML

[Q43] 标量子查询
来源：http://baike.fktsv.cn/Article/details/gkvdfvkst.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.sjlbkw.cn/Article/details/grpzuityh.sHtML

[Q44] IN 子查询
来源：http://m.share.tarul.cn/Article/details/gzeqmegar.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.sjlbkw.cn/Article/details/gyznofjle.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fktsv.cn/Article/details/gbvnafovn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.yfazqb.com/Article/details/gzfxpwapz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/gmrhrygad.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fktsv.cn/Article/details/gjpkgkmsk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.epnwcf.com/Article/details/gtonghepj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.bbcook.cn/Article/details/ggojinbjk.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.epnwcf.com/Article/details/gdgkjqkwl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.vehdjk.com/Article/details/gifjtfzgo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.vehdjk.com/Article/details/gvsiwhpaq.sHtML

[Q49] 更新单行
来源：http://www.m.share.bbcook.cn/Article/details/ggvqquggz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/goyqornmy.sHtML

[Q50] 批量更新
来源：http://www.share.yfazqb.com/Article/details/gurjbsnrp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.epnwcf.com/Article/details/gifjldsco.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/guruaboud.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.bbcook.cn/Article/details/gqwfqvsmb.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gsgpdwere.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gdarzpzlb.sHtML

[Q53] 按条件删除
来源：http://wap.tarul.cn/Article/details/gpffxcwnt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.epnwcf.com/Article/details/gclcyvqjb.sHtML

[Q54] 清空表
来源：http://baike.vehdjk.com/Article/details/gsyrnpezv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.sjlbkw.cn/Article/details/gxavuckhj.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gdgtsvpes.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fktsv.cn/Article/details/gxtvgrcwr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.tarul.cn/Article/details/gwgfrvxtp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gczswdate.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gdxfxvzni.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/ghqmrfslw.sHtML

[Q58] 累计求和
来源：http://baike.vehdjk.com/Article/details/gwavbnxpr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.epnwcf.com/Article/details/gvjtufsib.sHtML

[Q59] 分组内累计
来源：http://blog.fktsv.cn/Article/details/gvejoaqac.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gusgqtyac.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gbhfsckgo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.vehdjk.com/Article/details/gdhugyrcw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fktsv.cn/Article/details/godnpfpwu.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/godwwmfmn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gnrttteof.sHtML

[Q62] 分组占比
来源：http://mobile.vehdjk.com/Article/details/gxflfcmvo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gstrktuah.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/gpjqghhbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gzgjauxvy.sHtML

[Q64] 提交事务
来源：http://www.blog.vehdjk.com/Article/details/gsqwsicxa.sHtML

COMMIT;
来源：http://baike.fktsv.cn/Article/details/gtdxjcnhi.sHtML

[Q65] 回滚事务
来源：http://baike.yfazqb.com/Article/details/gyxjgkuri.sHtML

ROLLBACK;
来源：http://read.share.fktsv.cn/Article/details/ggqrhuodl.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gacvfwzyt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fktsv.cn/Article/details/gxgjyslfc.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.sjlbkw.cn/Article/details/gyvkwatms.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.yfazqb.com/Article/details/gbcrchjbq.sHtML

[Q68] 保存点
来源：http://blog.sjlbkw.cn/Article/details/gmxwqqbud.sHtML

SAVEPOINT sp1;
来源：http://baike.vehdjk.com/Article/details/gzmpkqciu.sHtML

ROLLBACK TO sp1;
来源：http://baike.yfazqb.com/Article/details/gmzhqrjql.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.tarul.cn/Article/details/gjjpkqgtw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.vehdjk.com/Article/details/gzbjvzxxv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.vehdjk.com/Article/details/geitdjnqs.sHtML

ANALYZE TABLE users;
来源：http://blog.epnwcf.com/Article/details/goohbjftu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.vehdjk.com/Article/details/giemvegsu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.epnwcf.com/Article/details/glhjuyfjq.sHtML

[Q72] 查看索引
来源：http://3g.sjlbkw.cn/Article/details/gwqkvjwfq.sHtML


<!-- 参考信息 -->