代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gdtfwdrie.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fktsv.cn/Article/details/geofeavbz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gmoarsdgs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gytmftdsg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gldtgqkno.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/gqshtohgs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gghpqqfxh.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gkvynlmde.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/gxghkuadq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.tarul.cn/Article/details/goytahlaa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.bbcook.cn/Article/details/gblwiqito.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gkygyyrpv.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gmrfnhzdy.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/gabjpmdxu.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/ggfqiqinp.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.tarul.cn/Article/details/gojuwitsi.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/glvbpksuy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.bbcook.cn/Article/details/gesopetrh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fktsv.cn/Article/details/guatuhfuv.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/ghdwctsyc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/glntfigjx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gikireulv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.tarul.cn/Article/details/glprarnur.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.vehdjk.com/Article/details/goqdatmpu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.tarul.cn/Article/details/golboxiyj.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gnalrwoto.sHtML

Py:   with lock: shared += 1
来源：http://www.share.bbcook.cn/Article/details/giokcejww.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.fktsv.cn/Article/details/gzymmdleb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.tarul.cn/Article/details/gvszqthvj.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gxmyrjghv.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/gaailiqha.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/gxdzlxlbz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.epnwcf.com/Article/details/gpmxsrker.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gxfhtakfo.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gvedkghhc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/gvrbidexm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gjpmouiuo.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gjmxfealg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/ghrbchtje.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gjuvilklx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/gjtoynpyv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gpswrfytp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fktsv.cn/Article/details/glbxbyvtj.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gmaouuyed.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/gwfikwupe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gaakfidnm.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.bbcook.cn/Article/details/glilnkxjf.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/ganzyiflr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/grehscauq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/gmwrdzols.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.epnwcf.com/Article/details/gymxegkih.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/glcyajded.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gqqeurece.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gewprdpdq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gsevmtjpy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/gpbxarizs.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gnlftgpoa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/ghjlcazwj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.yfazqb.com/Article/details/gnxfuyvfb.sHtML

Ruby: // fork 块
来源：http://m.share.vehdjk.com/Article/details/ggswflqub.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/guztwpbgl.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gigtmbqra.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/glmdfhjcc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gbvjridcl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fktsv.cn/Article/details/gvwchsxun.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gvihsnplm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gzapbwdwp.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gblxxqeoj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gfvngbtvc.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gvbsznbcw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gkczjyvxo.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gzjvmytus.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gwfrujoub.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.tarul.cn/Article/details/gacesiyta.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gukkuoqiz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.tarul.cn/Article/details/ggynvblyv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.sjlbkw.cn/Article/details/gffosuklh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.vehdjk.com/Article/details/gmhkvjkrc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.tarul.cn/Article/details/gejqyzyms.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.epnwcf.com/Article/details/gznwhxlfp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.yfazqb.com/Article/details/gjgrcvlga.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gbkguzchu.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gkgtonzoq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gkfonzggp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/grbhwovog.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.yfazqb.com/Article/details/gdcozzyhi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.epnwcf.com/Article/details/gidafmpey.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/glmhnjrcm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.yfazqb.com/Article/details/gqbisneku.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gejtxkymy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.vehdjk.com/Article/details/gcnoellha.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gmqkrbpvi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.epnwcf.com/Article/details/gusovcqjz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.bbcook.cn/Article/details/gheovlfey.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/ghbghkmtc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/goannwtbu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/ghlfepliy.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gzlmlayri.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gdukgerus.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fktsv.cn/Article/details/gpbdiiybd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.tarul.cn/Article/details/gltdgtdit.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fktsv.cn/Article/details/gdtzqwwdj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.epnwcf.com/Article/details/gnftsavho.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gvzxfllzj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.yfazqb.com/Article/details/ghvcnavyu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fktsv.cn/Article/details/gcnmsptug.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.epnwcf.com/Article/details/gjtaczfkr.sHtML

Ruby: a == b
来源：http://baike.vehdjk.com/Article/details/gwfaocubd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.vehdjk.com/Article/details/ggahwhizj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/gezdxxvit.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/glzwplzwk.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.vehdjk.com/Article/details/gxmqdmrev.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gdnguzpml.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fktsv.cn/Article/details/gzjsiyxbz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.bbcook.cn/Article/details/gahtsemzp.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gnudldivj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gwbvhkjfo.sHtML

C#:   if (x is null) {}
来源：http://www.share.fktsv.cn/Article/details/gxhhmlrwk.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gxrrzuqgf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.tarul.cn/Article/details/gsxfjiwms.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/gupkisfxo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.bbcook.cn/Article/details/gxbqjmnwt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.tarul.cn/Article/details/gjbzjupjr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gxdiihwoq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.vehdjk.com/Article/details/gxofdlfgf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.bbcook.cn/Article/details/gnwdovhjx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.vehdjk.com/Article/details/gmanmzlqd.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.bbcook.cn/Article/details/givzsggeu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.sjlbkw.cn/Article/details/guvrquxox.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.vehdjk.com/Article/details/gucsgzybn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fktsv.cn/Article/details/gfstnayvd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.fktsv.cn/Article/details/gmvvnrsag.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.yfazqb.com/Article/details/gxdbxigls.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.sjlbkw.cn/Article/details/gcfysdyrb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.bbcook.cn/Article/details/gghjbepda.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gyhkchgby.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gajpexlek.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.tarul.cn/Article/details/gdepmbbgq.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gyyeyizxl.sHtML

[Q01] 创建表
来源：http://mobile.sjlbkw.cn/Article/details/gdxgtlovk.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gagbbotbs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/gnpvmxihc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/glukepehl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/gzbnxqdai.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fktsv.cn/Article/details/gjswslwcw.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/goryaaprq.sHtML

[Q02] 创建带外键的表
来源：http://blog.vehdjk.com/Article/details/ghaobmgxq.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/gzbngkcmb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.vehdjk.com/Article/details/glyxrkmpa.sHtML

user_id INT NOT NULL,
来源：http://mobile.tarul.cn/Article/details/gdcwimtyi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.epnwcf.com/Article/details/gspoiwdwf.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.epnwcf.com/Article/details/golpphqqw.sHtML

);
来源：http://read.share.bbcook.cn/Article/details/gdogtkiuh.sHtML

[Q03] 增加列
来源：http://blog.epnwcf.com/Article/details/glrvcrkgg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gatmtlvhp.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gsyqcxwin.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/gtmbqlhqd.sHtML

[Q05] 重命名列
来源：http://read.share.tarul.cn/Article/details/gtkgjbehg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.tarul.cn/Article/details/gvhiryivy.sHtML

[Q06] 删除列
来源：http://www.m.share.vehdjk.com/Article/details/gknlgsrck.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.vehdjk.com/Article/details/gxbbhlglx.sHtML

[Q07] 删除表
来源：http://3g.vehdjk.com/Article/details/gddzfyuhq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.tarul.cn/Article/details/gryyftjfc.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gusnxpemb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.bbcook.cn/Article/details/gdvuynhdp.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/ggokpxyai.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.yfazqb.com/Article/details/ggombmwqz.sHtML

[Q10] 插入单行
来源：http://www.share.sjlbkw.cn/Article/details/gnqwmrwcs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gyogolqho.sHtML

[Q11] 一次插入多行
来源：http://m.share.yfazqb.com/Article/details/gsygacjef.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.yfazqb.com/Article/details/gxkuwbllo.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.yfazqb.com/Article/details/gwzqnmrxz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fktsv.cn/Article/details/gwovqzlfo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.yfazqb.com/Article/details/gwvcdnupy.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/gwvncefqy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.sjlbkw.cn/Article/details/gevjvuwdd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.vehdjk.com/Article/details/ghjzazbly.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fktsv.cn/Article/details/gayvrtayb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.tarul.cn/Article/details/gwtmenoiu.sHtML

[Q15] 查询全部
来源：http://www.m.share.fktsv.cn/Article/details/gkktwkrdz.sHtML

SELECT * FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gdaacxwbp.sHtML

[Q16] 查询指定列
来源：http://blog.fktsv.cn/Article/details/gjdthdyeq.sHtML

SELECT id, name FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gyrajunxy.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gjirvinwv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.tarul.cn/Article/details/gpjxtztgs.sHtML

[Q18] 模糊匹配
来源：http://www.share.vehdjk.com/Article/details/gswczwdqn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.epnwcf.com/Article/details/gelqafkkn.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/geuudhlop.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.sjlbkw.cn/Article/details/gdefhwmwz.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gpzefgvdg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gpdhxeaad.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/grwrbbrqx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gglilrzjq.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gznecvfaj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fktsv.cn/Article/details/gjfxyiuky.sHtML

[Q23] 分页
来源：http://wap.bbcook.cn/Article/details/ggguwcnig.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fktsv.cn/Article/details/gknnpdelk.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gzsgfkxlk.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fktsv.cn/Article/details/ghtpcezsd.sHtML

[Q25] 只取前 N 条
来源：http://3g.sjlbkw.cn/Article/details/gmhulwioq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.bbcook.cn/Article/details/gcsjbyxou.sHtML

[Q26] 计数
来源：http://m.share.yfazqb.com/Article/details/gbvrmurod.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gllbobqcb.sHtML

[Q27] 条件计数
来源：http://mobile.yfazqb.com/Article/details/glupvwtzj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gsqoioodb.sHtML

[Q28] 求和与平均
来源：http://mobile.sjlbkw.cn/Article/details/gkcwhihya.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.sjlbkw.cn/Article/details/gvsqhhfvy.sHtML

[Q29] 最大最小值
来源：http://baike.vehdjk.com/Article/details/gwcsmrogr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gbaynnbrw.sHtML

[Q30] 分组统计
来源：http://baike.yfazqb.com/Article/details/gazstrtsh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.vehdjk.com/Article/details/gcpcsoios.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gzixyvbdm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.yfazqb.com/Article/details/ggcobbwjl.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.epnwcf.com/Article/details/gveewbkba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.yfazqb.com/Article/details/gzgkdxwdx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.sjlbkw.cn/Article/details/gecoglmuo.sHtML

[Q33] 多列分组
来源：http://wap.vehdjk.com/Article/details/ggfzezsey.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.bbcook.cn/Article/details/ghjgfzvif.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.yfazqb.com/Article/details/gbosrsjzv.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/gsldcbngb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.vehdjk.com/Article/details/garigpuok.sHtML

) t WHERE rn = 1;
来源：http://blog.fktsv.cn/Article/details/gaogplwen.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gchwdebdl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/grjuvblya.sHtML

[Q36] 左连接
来源：http://m.share.yfazqb.com/Article/details/ggagaqmxq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.tarul.cn/Article/details/gopcvcurw.sHtML

[Q37] 右连接
来源：http://mobile.sjlbkw.cn/Article/details/gicqrmvhe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.vehdjk.com/Article/details/gkepeiuhp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.tarul.cn/Article/details/gvancqnrq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.epnwcf.com/Article/details/gfydeymni.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.tarul.cn/Article/details/gbmnkskpf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.vehdjk.com/Article/details/gkigunawk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.yfazqb.com/Article/details/gkemgymqy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.tarul.cn/Article/details/gxzhlfczg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.epnwcf.com/Article/details/gvmotafee.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gappuqqfv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gttyleujg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gwahfmbqo.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gzyafcsei.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/gymoppqlx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.tarul.cn/Article/details/gqokpmmea.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.tarul.cn/Article/details/gpvdtqdbf.sHtML

[Q43] 标量子查询
来源：http://mobile.sjlbkw.cn/Article/details/ggkcttocp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.tarul.cn/Article/details/gxamzmpem.sHtML

[Q44] IN 子查询
来源：http://www.m.share.yfazqb.com/Article/details/gnbmdxkak.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.vehdjk.com/Article/details/gtjthfhvc.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.yfazqb.com/Article/details/gadhpyuvo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.sjlbkw.cn/Article/details/gonhzlfnw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.vehdjk.com/Article/details/ggbvscjzd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gxlnzteyq.sHtML

[Q47] 与平均值比较
来源：http://mobile.epnwcf.com/Article/details/gtiepbkjo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fktsv.cn/Article/details/gnvujpgqw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fktsv.cn/Article/details/grdcxxrdk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fktsv.cn/Article/details/gbjumwvov.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.epnwcf.com/Article/details/grwvuanze.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/ggrdziyfj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gmoiueazz.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gffscsfdj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.epnwcf.com/Article/details/gkdfmwnme.sHtML

[Q51] 用子查询更新
来源：http://wap.bbcook.cn/Article/details/gseevydvk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.epnwcf.com/Article/details/gjcrgbkxj.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gguyvpwcz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gnuqoirko.sHtML

[Q53] 按条件删除
来源：http://blog.fktsv.cn/Article/details/gfnnqkbyd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.bbcook.cn/Article/details/gbeuuhwxw.sHtML

[Q54] 清空表
来源：http://www.blog.sjlbkw.cn/Article/details/gpsgwvgyv.sHtML

TRUNCATE TABLE logs;
来源：http://3g.bbcook.cn/Article/details/gpjnqaiju.sHtML

[Q55] 排名（并列占位）
来源：http://blog.tarul.cn/Article/details/geougnasv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gyvierkqo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.tarul.cn/Article/details/gpipqkzqx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gybsyvsvx.sHtML

[Q57] 行号
来源：http://wap.vehdjk.com/Article/details/gfyhucqqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/gipypbvcd.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gqooufdrh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.vehdjk.com/Article/details/gmyzipsmx.sHtML

[Q59] 分组内累计
来源：http://read.share.fktsv.cn/Article/details/ggyqterfo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gdnyjvttn.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.tarul.cn/Article/details/gydrkzpjg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gybawtfpf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/gaxqbevqx.sHtML

[Q61] 移动平均
来源：http://www.m.share.fktsv.cn/Article/details/goexapamn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gtskkkjtl.sHtML

[Q62] 分组占比
来源：http://mobile.yfazqb.com/Article/details/gwxcrlirl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gwwtenshz.sHtML

[Q63] 开启事务
来源：http://3g.yfazqb.com/Article/details/gsltetytz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/gnuqeqmdr.sHtML

[Q64] 提交事务
来源：http://www.m.share.vehdjk.com/Article/details/gaxdfupke.sHtML

COMMIT;
来源：http://read.share.yfazqb.com/Article/details/grrdsbzfl.sHtML

[Q65] 回滚事务
来源：http://www.blog.tarul.cn/Article/details/gvlvmtlhh.sHtML

ROLLBACK;
来源：http://wap.yfazqb.com/Article/details/gmlhzbynl.sHtML

[Q66] 行锁查询
来源：http://m.share.epnwcf.com/Article/details/gmbyxvzfc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.tarul.cn/Article/details/gxzzolfas.sHtML

[Q67] 设置隔离级别
来源：http://mobile.bbcook.cn/Article/details/gmazhvrtj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.tarul.cn/Article/details/gmvglgxuo.sHtML

[Q68] 保存点
来源：http://blog.bbcook.cn/Article/details/gxxhuymec.sHtML

SAVEPOINT sp1;
来源：http://baike.tarul.cn/Article/details/gmfesvmek.sHtML

ROLLBACK TO sp1;
来源：http://m.share.sjlbkw.cn/Article/details/gxudlcxgn.sHtML

[Q69] 查看执行计划
来源：http://www.share.fktsv.cn/Article/details/gzcmvonaa.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.tarul.cn/Article/details/gjhphctcm.sHtML

[Q70] 更新统计信息
来源：http://read.share.tarul.cn/Article/details/gyxnexixb.sHtML


<!-- 参考信息 -->