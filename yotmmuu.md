代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gfwupznkc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/guxbyewro.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gibvcmqak.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gxwfvusyl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/greotcbuj.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gmxplyoyj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxrplgrem.sHtML

[O01] 启动一个线程
来源：http://read.share.sjlbkw.cn/Article/details/gptqeqrzz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gehvkncjf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gklnbqfmm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/gxaawwvsx.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/giozpvrty.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gljautojp.sHtML

Go:   go f()
来源：http://mobile.bbcook.cn/Article/details/grbfhahfd.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/geqhfvzlj.sHtML

C#:   Task.Run(() => F());
来源：http://blog.epnwcf.com/Article/details/gkcopnmjq.sHtML

[O02] 使用线程池
来源：http://baike.fktsv.cn/Article/details/ghhwycudr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gtgypezek.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.epnwcf.com/Article/details/gqtdutahc.sHtML

JS:   // worker_threads 线程池
来源：http://wap.epnwcf.com/Article/details/gjioursds.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gvitkdhla.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/gopowpirh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.epnwcf.com/Article/details/gkajxoyce.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/gvwgpskiq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gftdulsaz.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/gumzlxwrb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/gxfpgfpxp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gtupsdzhm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gjcfllxfo.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gibcdtroa.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/ggkzdrgye.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gwpcrmiat.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.bbcook.cn/Article/details/gdvgmuvkz.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gdenyjpwy.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.sjlbkw.cn/Article/details/gunksjxbz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gijfbmplb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.bbcook.cn/Article/details/gzamdbyjf.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gmsqjsves.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gcmzwloqv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/gxnkyzzmw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/gjnnvslbw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gjnxefuii.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gonerlljx.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/galdbrdch.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/ghmrjffvc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fktsv.cn/Article/details/geiubqomw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gduiwhdof.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gxhtgxmod.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.bbcook.cn/Article/details/gokzmiswl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/grcyfqzft.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gzddsrmvg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/gnnpuicyg.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gxftanmvo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.tarul.cn/Article/details/gghdjmsir.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/gjfcgkbwy.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/guoeuuqge.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gpyiwtswr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gskzduyik.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.epnwcf.com/Article/details/grflfvxew.sHtML

Ruby: // fork 块
来源：http://baike.tarul.cn/Article/details/glucbgins.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/grzokqkfx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwetpufit.sHtML

P. 常用工具函数
来源：http://m.share.vehdjk.com/Article/details/gbhybcwil.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdakmakze.sHtML

[P01] 生成 UUID
来源：http://m.share.fktsv.cn/Article/details/gaaiwxypo.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.bbcook.cn/Article/details/gtbhffyuu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gsgaitywp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gypeabame.sHtML

TS:   crypto.randomUUID()
来源：http://wap.bbcook.cn/Article/details/gdxhkqmys.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbefiwdfe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gridbszwl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gzeizcwtk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gzzkxlybh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.sjlbkw.cn/Article/details/giloenuya.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.vehdjk.com/Article/details/gdvalhxtt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gktyxjitm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/ggofbyppc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.sjlbkw.cn/Article/details/gjdvpdehm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.vehdjk.com/Article/details/gvxfrmooq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.yfazqb.com/Article/details/gezqgqujo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.bbcook.cn/Article/details/grvlwusrz.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gscgzyfmd.sHtML

[P03] 生成短随机字符串
来源：http://3g.sjlbkw.cn/Article/details/gylbshqqa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gqdtqlwiw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.sjlbkw.cn/Article/details/gvwobcsaw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gtnrjbhyb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gluggdjka.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.sjlbkw.cn/Article/details/gufjmzxbj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gxqyfwmwy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/gzebsketi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.sjlbkw.cn/Article/details/gklmanahe.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/ghkcfezln.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.tarul.cn/Article/details/gcaruifep.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.epnwcf.com/Article/details/gbhpgmgyp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gphuaaqob.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.vehdjk.com/Article/details/gbqhqptgz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.vehdjk.com/Article/details/guebvdqtb.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gzxkbdxwl.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gymbvulrb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/ggyteqkhi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/gxvrwykuv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.sjlbkw.cn/Article/details/geyqvqomz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.sjlbkw.cn/Article/details/gohnrfuuv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.yfazqb.com/Article/details/gpjnjiwps.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.vehdjk.com/Article/details/gvsvzljoi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.yfazqb.com/Article/details/gliahkyla.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.epnwcf.com/Article/details/gcefobmge.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/gtaxehxbo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.yfazqb.com/Article/details/golseyghd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.yfazqb.com/Article/details/ghfxzgtvv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/giqyyhrgs.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.bbcook.cn/Article/details/gzqpqbrmk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gsgveplii.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gbskchgdf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fktsv.cn/Article/details/gkcbkfqnz.sHtML

Go:   if x == nil {}
来源：http://www.m.share.vehdjk.com/Article/details/guytqbuha.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.fktsv.cn/Article/details/gpkjzaixy.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gvgegsxlb.sHtML

[P07] 防抖与节流
来源：http://mobile.bbcook.cn/Article/details/grvwdwuxu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.sjlbkw.cn/Article/details/gpcwqwtas.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.tarul.cn/Article/details/ghlfndezy.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gmtsrradr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gjzhmmkpo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fktsv.cn/Article/details/gbdcujfhz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.tarul.cn/Article/details/gjbnzrqmd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.vehdjk.com/Article/details/gvrhilbne.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.yfazqb.com/Article/details/gznqlozav.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gachnjeus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gqfvistho.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.tarul.cn/Article/details/gcygcppgg.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://read.share.fktsv.cn/Article/details/gpiresoru.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/gzzxpqmqa.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.sjlbkw.cn/Article/details/gfkkpxmxc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gnidejzeb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gnzpsnfjj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.tarul.cn/Article/details/gkoyymsec.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gmtimcuro.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.sjlbkw.cn/Article/details/ginclqqez.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzewpqevl.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gfdqgszmf.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gbgqpogkc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fktsv.cn/Article/details/gcsonfirz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.bbcook.cn/Article/details/genqfjpnh.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.bbcook.cn/Article/details/groyoomqe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gnrujzwil.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gtfxdvgbs.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbuochte.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gsujgshwa.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/giginomcr.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gxlpcqffh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/gatmsgrxj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/giygjnuss.sHtML

);
来源：http://mobile.bbcook.cn/Article/details/gviapquva.sHtML

[Q03] 增加列
来源：http://www.share.epnwcf.com/Article/details/geuwzebcu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.tarul.cn/Article/details/gzxbpoora.sHtML

[Q04] 修改列类型
来源：http://m.share.yfazqb.com/Article/details/ggddrhtoe.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.vehdjk.com/Article/details/ghjltnwgc.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/gxavuffol.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.tarul.cn/Article/details/gzinltjbj.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gbwpqrcuk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.tarul.cn/Article/details/gtupzqwxs.sHtML

[Q07] 删除表
来源：http://read.share.fktsv.cn/Article/details/gyfkajmgm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.yfazqb.com/Article/details/gtnxzrhlf.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/gwiqnoecg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.vehdjk.com/Article/details/gcjhdapba.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fktsv.cn/Article/details/gpovcctds.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.epnwcf.com/Article/details/gjhmiljix.sHtML

[Q10] 插入单行
来源：http://wap.fktsv.cn/Article/details/ggjstjoqn.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.yfazqb.com/Article/details/gigscflae.sHtML

[Q11] 一次插入多行
来源：http://blog.tarul.cn/Article/details/gxzyhexpg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.epnwcf.com/Article/details/gpngsbzrn.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.vehdjk.com/Article/details/gqiqqhbku.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.vehdjk.com/Article/details/gixnhjuxx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/guoxerxzy.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fktsv.cn/Article/details/gdqmcpoku.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.vehdjk.com/Article/details/gbkxufmev.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.sjlbkw.cn/Article/details/gmonpqwpp.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.bbcook.cn/Article/details/gvkgfqnkr.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gzgbwhmws.sHtML

[Q15] 查询全部
来源：http://www.m.share.epnwcf.com/Article/details/gkmhoklat.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/gvntkiphz.sHtML

[Q16] 查询指定列
来源：http://blog.bbcook.cn/Article/details/gzsoqzioy.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/gwshsslsk.sHtML

[Q17] 条件查询
来源：http://read.share.fktsv.cn/Article/details/gemkwidbq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.sjlbkw.cn/Article/details/gjcawsblc.sHtML

[Q18] 模糊匹配
来源：http://3g.fktsv.cn/Article/details/gxhcbyshe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.yfazqb.com/Article/details/guczjdrql.sHtML

[Q19] 范围查询
来源：http://www.blog.fktsv.cn/Article/details/gwtmdakhc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.sjlbkw.cn/Article/details/gravyywgt.sHtML

[Q20] IN 列表
来源：http://www.share.tarul.cn/Article/details/gpxmmfstq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.bbcook.cn/Article/details/gkopjtjyh.sHtML

[Q21] 空值判断
来源：http://wap.yfazqb.com/Article/details/gvayuogjq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gxmbmotfw.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gabpjenvp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.sjlbkw.cn/Article/details/gzhxbwmfz.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gwxpuyomq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gdtowlswa.sHtML

[Q24] 去重
来源：http://www.m.share.vehdjk.com/Article/details/gmtrasftc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gnwhsdqwz.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.tarul.cn/Article/details/gyehffsbf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/grlbovtpy.sHtML

[Q26] 计数
来源：http://www.m.share.tarul.cn/Article/details/geghrfiqt.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gixjeskej.sHtML

[Q27] 条件计数
来源：http://baike.yfazqb.com/Article/details/gtwccjnbs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gaiivlkui.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/gueiikvsc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.tarul.cn/Article/details/grjveqvez.sHtML

[Q29] 最大最小值
来源：http://www.m.share.tarul.cn/Article/details/ggsihmsjz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fktsv.cn/Article/details/gfkoydmjj.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gnlpbbvmm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fktsv.cn/Article/details/gnnbfnbcu.sHtML

[Q31] 分组后过滤
来源：http://baike.sjlbkw.cn/Article/details/gxtrzfsth.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fktsv.cn/Article/details/gpzpyxwfm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.tarul.cn/Article/details/gvhfefddh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.bbcook.cn/Article/details/gncbxrmpw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/geaythxsr.sHtML

[Q33] 多列分组
来源：http://www.share.fktsv.cn/Article/details/glwtswbfh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.sjlbkw.cn/Article/details/ghmzpbgbg.sHtML

[Q34] 每组取第一条
来源：http://read.share.vehdjk.com/Article/details/gmylmmunt.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gmwihrkti.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.epnwcf.com/Article/details/guqztmtnz.sHtML

) t WHERE rn = 1;
来源：http://www.blog.epnwcf.com/Article/details/gklfhddyf.sHtML

[Q35] 内连接
来源：http://www.blog.fktsv.cn/Article/details/gjlysnxer.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.bbcook.cn/Article/details/ghhihwhum.sHtML

[Q36] 左连接
来源：http://www.share.bbcook.cn/Article/details/grqzplfca.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gdklkasag.sHtML

[Q37] 右连接
来源：http://blog.sjlbkw.cn/Article/details/guveqqaos.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.sjlbkw.cn/Article/details/gilruirqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.sjlbkw.cn/Article/details/gcnfngueu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gtilwgprz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.epnwcf.com/Article/details/gewtlbslt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.yfazqb.com/Article/details/gprgdzmna.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gpyvkzoes.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fktsv.cn/Article/details/gsvdqygbu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gwwyvhvyh.sHtML

[Q41] 多表连接
来源：http://www.m.share.fktsv.cn/Article/details/gzqqdarfi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fktsv.cn/Article/details/gimneiqon.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gpeovrwgs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.sjlbkw.cn/Article/details/guayazpgo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.sjlbkw.cn/Article/details/gjyavvbbd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.epnwcf.com/Article/details/gcrdrxikb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.tarul.cn/Article/details/gwvmgihff.sHtML

[Q43] 标量子查询
来源：http://mobile.epnwcf.com/Article/details/gdtzdgnkg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.sjlbkw.cn/Article/details/gtnuqcwla.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/ghojyjsns.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fktsv.cn/Article/details/gubkqodou.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.sjlbkw.cn/Article/details/gahgwwspw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gwdyccqfc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/gjtfijxub.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fktsv.cn/Article/details/gpmnllnzy.sHtML

[Q47] 与平均值比较
来源：http://read.share.bbcook.cn/Article/details/gkkbchmez.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gotbxecmg.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fktsv.cn/Article/details/gwrrwtupj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.sjlbkw.cn/Article/details/gtflybeyh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.bbcook.cn/Article/details/gzcxupimi.sHtML

[Q49] 更新单行
来源：http://www.share.sjlbkw.cn/Article/details/gsbrsabbe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.epnwcf.com/Article/details/grebnakqa.sHtML

[Q50] 批量更新
来源：http://blog.sjlbkw.cn/Article/details/gkbprohwx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.vehdjk.com/Article/details/gqhjcmusu.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/gyzhfsqcm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.tarul.cn/Article/details/gxodqvzgi.sHtML

[Q52] 删除指定行
来源：http://3g.epnwcf.com/Article/details/gblwiggmq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.bbcook.cn/Article/details/gxkojqofz.sHtML

[Q53] 按条件删除
来源：http://3g.tarul.cn/Article/details/gcutqamzz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.vehdjk.com/Article/details/gqofrihlt.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gblvjixmp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fktsv.cn/Article/details/gkaaoqgkl.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gensjidod.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/getveuqof.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.bbcook.cn/Article/details/gsmvgwdwy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fktsv.cn/Article/details/gxkzahhak.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gkrqpiqlt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fktsv.cn/Article/details/gdosbkycf.sHtML

[Q58] 累计求和
来源：http://wap.epnwcf.com/Article/details/gsiqoihjf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fktsv.cn/Article/details/gqefrbodh.sHtML

[Q59] 分组内累计
来源：http://www.m.share.epnwcf.com/Article/details/gbrynkylf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gnoauvzor.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.bbcook.cn/Article/details/gxcrfsjaf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/geaxqvlrk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gkvaoeudq.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/gqcwzcgya.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/goqboxlss.sHtML

[Q62] 分组占比
来源：http://3g.fktsv.cn/Article/details/gumpvswwv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fktsv.cn/Article/details/gpxozbeqq.sHtML

[Q63] 开启事务
来源：http://mobile.sjlbkw.cn/Article/details/grvyoldzz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gfkrsdzqd.sHtML

[Q64] 提交事务
来源：http://www.m.share.epnwcf.com/Article/details/gtgmgacfd.sHtML

COMMIT;
来源：http://www.share.yfazqb.com/Article/details/ghusdwwdk.sHtML

[Q65] 回滚事务
来源：http://wap.yfazqb.com/Article/details/gydpzwlal.sHtML

ROLLBACK;
来源：http://read.share.bbcook.cn/Article/details/gfrcoxzth.sHtML

[Q66] 行锁查询
来源：http://www.share.bbcook.cn/Article/details/gsmryrzbi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gfmrasgrg.sHtML

[Q67] 设置隔离级别
来源：http://wap.epnwcf.com/Article/details/gruadufkl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.epnwcf.com/Article/details/gkufokmlx.sHtML

[Q68] 保存点
来源：http://baike.vehdjk.com/Article/details/gcvungvdu.sHtML

SAVEPOINT sp1;
来源：http://mobile.yfazqb.com/Article/details/gjbptjyrs.sHtML

ROLLBACK TO sp1;
来源：http://3g.epnwcf.com/Article/details/grvwfslvu.sHtML

[Q69] 查看执行计划
来源：http://www.share.yfazqb.com/Article/details/gavzlsfxq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.tarul.cn/Article/details/glmzdudke.sHtML

[Q70] 更新统计信息
来源：http://3g.fktsv.cn/Article/details/gymnsfypp.sHtML


<!-- 参考信息 -->