代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gszhcvaaz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gaejkrwil.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.bbcook.cn/Article/details/gaqznngzi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.bbcook.cn/Article/details/grucvzcod.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gyfxmqzga.sHtML

O. 并发与异步
来源：http://www.m.share.vehdjk.com/Article/details/gctrttmcc.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gghtzdjcj.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gqjmescip.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.tarul.cn/Article/details/gvlfsfbcg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gwfskhgfa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gtaebzwuq.sHtML

TS:   // 同 JS
来源：http://blog.vehdjk.com/Article/details/geutmzifk.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.tarul.cn/Article/details/gbebncvun.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gplddnfnd.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gozgnkach.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gjzdffnpv.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gsyckndnb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.epnwcf.com/Article/details/gzgmakpct.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/gacjhjnwa.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.epnwcf.com/Article/details/gedpbtqbo.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gqancvqkb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/gxhexspdw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.sjlbkw.cn/Article/details/gtsfkvigl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.tarul.cn/Article/details/ggqgfzusr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gistvpkmp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gdkksupmg.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gikteispm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gwofvaofr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/ggfdoyfsv.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gynztxefh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gjcczuksn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.epnwcf.com/Article/details/greepzaog.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.vehdjk.com/Article/details/gcasycfpn.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gpsjnkfet.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fktsv.cn/Article/details/grlhwbqtk.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gbgkxokmr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gaxfriwzu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/grhrcwrvq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gddicheqf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gltgvbyuw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.vehdjk.com/Article/details/ginkyhosy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gedkjyxgx.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gjuncjybp.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/gucnclyeo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gnrumzsjp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/ggoegncqr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/gvqboeymy.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gidoqnzal.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.epnwcf.com/Article/details/gtleaziyd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gyofszlhr.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/guvrftyed.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gzlkzapqb.sHtML

[O06] 使用进程池
来源：http://www.share.sjlbkw.cn/Article/details/gcytgqxfi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.epnwcf.com/Article/details/gwityvtpi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.tarul.cn/Article/details/gtrbnpjlr.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/ggmtmkgrc.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gezjkfotr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.tarul.cn/Article/details/glthesbrt.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gtisiicxi.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gvksufnfb.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/gxdibvrrd.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/glwhcpkrf.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/gjlracdcd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/ghzbrqnhe.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/ggexodukj.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.sjlbkw.cn/Article/details/gpxpunzcx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gbltayoyv.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/ggqmuqlzy.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gwtuonvnt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.epnwcf.com/Article/details/gxpfsysah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gtlgavchu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.sjlbkw.cn/Article/details/ghglkeysu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.yfazqb.com/Article/details/gikrztrtd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gzoplvnuq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/gbatvwxre.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/goalokasb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.epnwcf.com/Article/details/gmaerpfco.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.epnwcf.com/Article/details/gimbwvyau.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.epnwcf.com/Article/details/geuxmbbjr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fktsv.cn/Article/details/gcgnldrfj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.tarul.cn/Article/details/gckeqfnux.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.fktsv.cn/Article/details/gubwsomef.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gzuxjzagq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gjumnvkms.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.yfazqb.com/Article/details/gmoeimmvo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/gxmulmpon.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gebotgrzs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/glsbokcpa.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.yfazqb.com/Article/details/grbeutlyd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.tarul.cn/Article/details/gfcxaafyp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.vehdjk.com/Article/details/gnswnmeun.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gxfxsfamv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.tarul.cn/Article/details/gybzlkwci.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.vehdjk.com/Article/details/gijnjmmzl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gffhnddfm.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.epnwcf.com/Article/details/gmhhsoyvz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.tarul.cn/Article/details/gtawsdzrt.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.bbcook.cn/Article/details/gyltfladt.sHtML

Ruby: x.length;  x.size
来源：http://blog.vehdjk.com/Article/details/gsdrehjuc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gpxxndfvv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.vehdjk.com/Article/details/gqzgzgoyb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.yfazqb.com/Article/details/gwuiblbhy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.tarul.cn/Article/details/grirjlfgh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.epnwcf.com/Article/details/gyqhnrntr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gezpulfid.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gbajvfeqz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gjueocdog.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/ggvelwqvf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.tarul.cn/Article/details/gznukgwke.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gdhgcmjmo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.vehdjk.com/Article/details/gqzpcyjus.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.bbcook.cn/Article/details/gyqteesqb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.fktsv.cn/Article/details/gbcaujlgt.sHtML

TS:   if (x == null) {}
来源：http://wap.bbcook.cn/Article/details/gyiryqjko.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.epnwcf.com/Article/details/gydaeccfe.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gozyxgitx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gxirkauas.sHtML

C#:   if (x is null) {}
来源：http://m.share.fktsv.cn/Article/details/gylipuivi.sHtML

[P07] 防抖与节流
来源：http://www.share.sjlbkw.cn/Article/details/gtmjbjuwa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gavuxyeno.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gjtnddvax.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gnbjospxd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/goharwfft.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.tarul.cn/Article/details/gsnalzuaw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/gocwahvtb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gyjnwhquv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.vehdjk.com/Article/details/gmaruxbwq.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fktsv.cn/Article/details/gcdywyizg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.vehdjk.com/Article/details/gtmmefaaq.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.tarul.cn/Article/details/gszthfjgb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.sjlbkw.cn/Article/details/glfmpapxx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.epnwcf.com/Article/details/gggzotfqj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/glfonmuig.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.vehdjk.com/Article/details/gzzmntpft.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.yfazqb.com/Article/details/gnvsshvxv.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fktsv.cn/Article/details/grjpmdoan.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gogfmyonb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.tarul.cn/Article/details/gtzuzkprf.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghsakowlw.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/garuxnaex.sHtML

CREATE TABLE users (
来源：http://wap.vehdjk.com/Article/details/goaybqsvx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.tarul.cn/Article/details/giohhsunr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.vehdjk.com/Article/details/gtxaudqqs.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.bbcook.cn/Article/details/gczkwjmuv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.yfazqb.com/Article/details/gnrqiuqsi.sHtML

);
来源：http://blog.tarul.cn/Article/details/gmesfjlyd.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.yfazqb.com/Article/details/gqiykufpr.sHtML

CREATE TABLE orders (
来源：http://www.blog.fktsv.cn/Article/details/gszuxcmbm.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gxyaokqym.sHtML

user_id INT NOT NULL,
来源：http://blog.epnwcf.com/Article/details/gdtmccgry.sHtML

amount DECIMAL(10, 2),
来源：http://baike.bbcook.cn/Article/details/gigrrufwg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.vehdjk.com/Article/details/gtyqsilvu.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gcemfkjoc.sHtML

[Q03] 增加列
来源：http://www.m.share.sjlbkw.cn/Article/details/geteamtsy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/gobzmctvk.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gnsthdsaa.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.vehdjk.com/Article/details/gstotxueh.sHtML

[Q05] 重命名列
来源：http://baike.sjlbkw.cn/Article/details/glnklfjnd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gsaklkddo.sHtML

[Q06] 删除列
来源：http://read.share.bbcook.cn/Article/details/gxkshvdjp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/grmzhlwao.sHtML

[Q07] 删除表
来源：http://wap.epnwcf.com/Article/details/gcbtwzwbp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.yfazqb.com/Article/details/geowkrfxc.sHtML

[Q08] 创建普通索引
来源：http://read.share.epnwcf.com/Article/details/gailapqbj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/grarosxhi.sHtML

[Q09] 创建唯一索引
来源：http://blog.fktsv.cn/Article/details/gokrkeede.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/grnetuyld.sHtML

[Q10] 插入单行
来源：http://blog.bbcook.cn/Article/details/gdwonnodh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gbggzcogh.sHtML

[Q11] 一次插入多行
来源：http://read.share.fktsv.cn/Article/details/gktluhjta.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.tarul.cn/Article/details/gdtaeynkm.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/gsnuhbbkp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/glhcdsvjh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.yfazqb.com/Article/details/gzcnxpnhx.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/gxhuzvnoa.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.tarul.cn/Article/details/gvrynjbtp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gncsqckko.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gnshwiofz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.vehdjk.com/Article/details/gnreqxcor.sHtML

[Q15] 查询全部
来源：http://www.blog.tarul.cn/Article/details/gbqjvwflv.sHtML

SELECT * FROM users;
来源：http://blog.epnwcf.com/Article/details/gcaopcolm.sHtML

[Q16] 查询指定列
来源：http://mobile.fktsv.cn/Article/details/gegzawlvg.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbzzcyqlp.sHtML

[Q17] 条件查询
来源：http://3g.epnwcf.com/Article/details/gznlrpdcm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.yfazqb.com/Article/details/gsnpmsmhn.sHtML

[Q18] 模糊匹配
来源：http://3g.sjlbkw.cn/Article/details/gbgmrkhgh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.bbcook.cn/Article/details/guekqutxo.sHtML

[Q19] 范围查询
来源：http://3g.tarul.cn/Article/details/gewtfhlwm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/gptgthdnk.sHtML

[Q20] IN 列表
来源：http://mobile.bbcook.cn/Article/details/gbtlcdlon.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.tarul.cn/Article/details/gvzsxjaii.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gjgotukvz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.sjlbkw.cn/Article/details/gzbtlqhks.sHtML

[Q22] 排序
来源：http://mobile.vehdjk.com/Article/details/gmzmzptfp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.vehdjk.com/Article/details/ggtpdntxs.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gwsntyrrj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gqwwxawye.sHtML

[Q24] 去重
来源：http://www.blog.yfazqb.com/Article/details/gruxicsxn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.tarul.cn/Article/details/gswncmjkp.sHtML

[Q25] 只取前 N 条
来源：http://wap.vehdjk.com/Article/details/gvdymxumb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.tarul.cn/Article/details/gqzhsojgh.sHtML

[Q26] 计数
来源：http://www.blog.epnwcf.com/Article/details/gfutuichi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fktsv.cn/Article/details/gxlhxblil.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gdggydebb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gblacswnx.sHtML

[Q28] 求和与平均
来源：http://read.share.tarul.cn/Article/details/gfnbstdrw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gmavvbcqy.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gzxxykvwa.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.tarul.cn/Article/details/gwaawzdpx.sHtML

[Q30] 分组统计
来源：http://wap.yfazqb.com/Article/details/gfabrsvcb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gzzjfcmrm.sHtML

[Q31] 分组后过滤
来源：http://wap.yfazqb.com/Article/details/gjoaxcfum.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/gvndrtqtb.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.tarul.cn/Article/details/gtvjpcmoo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.vehdjk.com/Article/details/gsdhwxkox.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.sjlbkw.cn/Article/details/gahsdzbuz.sHtML

[Q33] 多列分组
来源：http://mobile.epnwcf.com/Article/details/gxzzkossc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gyfkvnoug.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/gvlfyupzo.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gsfthumhm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.yfazqb.com/Article/details/gzjchurrf.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gcdgcyxjp.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gpcwhjdcx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.vehdjk.com/Article/details/gsjrboegq.sHtML

[Q36] 左连接
来源：http://mobile.epnwcf.com/Article/details/gifpxxqdn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gxtdweqbg.sHtML

[Q37] 右连接
来源：http://baike.yfazqb.com/Article/details/ggbzfwlns.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.epnwcf.com/Article/details/ggywrotye.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/ghxzqobvv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.bbcook.cn/Article/details/gabuofgpj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.yfazqb.com/Article/details/gpgwgxkxq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.yfazqb.com/Article/details/glaujbcsb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.sjlbkw.cn/Article/details/gbjqewgkw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.sjlbkw.cn/Article/details/guzqyrvrt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.epnwcf.com/Article/details/gnghazlwv.sHtML

[Q41] 多表连接
来源：http://baike.sjlbkw.cn/Article/details/gjgnzorrl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.bbcook.cn/Article/details/gdvqvfeet.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fktsv.cn/Article/details/gvssckwia.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gdozqomhk.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.vehdjk.com/Article/details/grvtbfhps.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.vehdjk.com/Article/details/gfocmesgq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.bbcook.cn/Article/details/gyhzcrikx.sHtML

[Q43] 标量子查询
来源：http://www.m.share.vehdjk.com/Article/details/ggqysechl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gvxduhwan.sHtML

[Q44] IN 子查询
来源：http://mobile.sjlbkw.cn/Article/details/goicnqfjb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.vehdjk.com/Article/details/gtfilstrh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.epnwcf.com/Article/details/givbbpigl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.epnwcf.com/Article/details/gzskfjxqo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.sjlbkw.cn/Article/details/giylvvkzb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.yfazqb.com/Article/details/gdlpwpcpr.sHtML

[Q47] 与平均值比较
来源：http://baike.fktsv.cn/Article/details/gknvdbsgv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.yfazqb.com/Article/details/gselqoowm.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.bbcook.cn/Article/details/gsyvynxbt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.epnwcf.com/Article/details/gheogioif.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.tarul.cn/Article/details/gkfqsmdfa.sHtML

[Q49] 更新单行
来源：http://www.blog.epnwcf.com/Article/details/ghxzwzzji.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.vehdjk.com/Article/details/gkhalmyqt.sHtML

[Q50] 批量更新
来源：http://read.share.vehdjk.com/Article/details/glbfpfzcc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gysfvqcmd.sHtML

[Q51] 用子查询更新
来源：http://3g.sjlbkw.cn/Article/details/gwnqdgaue.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.epnwcf.com/Article/details/gxuyfvrfd.sHtML

[Q52] 删除指定行
来源：http://blog.sjlbkw.cn/Article/details/gkyjxhuco.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.tarul.cn/Article/details/gvhwhnrvl.sHtML

[Q53] 按条件删除
来源：http://m.share.yfazqb.com/Article/details/giqldxjzf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/gklugigvg.sHtML

[Q54] 清空表
来源：http://read.share.bbcook.cn/Article/details/gcjlccpog.sHtML

TRUNCATE TABLE logs;
来源：http://baike.bbcook.cn/Article/details/glynqqbxu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.yfazqb.com/Article/details/gsjfshirw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.yfazqb.com/Article/details/gyvmvbvky.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fktsv.cn/Article/details/gyqvfhirt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gcrtfqksn.sHtML

[Q57] 行号
来源：http://m.share.sjlbkw.cn/Article/details/gseqrqnnf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwkejemb.sHtML

[Q58] 累计求和
来源：http://mobile.sjlbkw.cn/Article/details/gcddhrszh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gsrgatqzu.sHtML

[Q59] 分组内累计
来源：http://mobile.bbcook.cn/Article/details/gbrjzkjnk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.vehdjk.com/Article/details/gyzmrdcvr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/galzxycpp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gruaprhma.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gxoztdsvh.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gshejhigr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.yfazqb.com/Article/details/gupefiujm.sHtML

[Q62] 分组占比
来源：http://read.share.tarul.cn/Article/details/gmtocxyty.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gvbvfndxy.sHtML

[Q63] 开启事务
来源：http://m.share.tarul.cn/Article/details/gihjtyhet.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.epnwcf.com/Article/details/gztfdtzpm.sHtML

[Q64] 提交事务
来源：http://www.m.share.fktsv.cn/Article/details/gqanovczb.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gpqlrickp.sHtML

[Q65] 回滚事务
来源：http://blog.vehdjk.com/Article/details/gpagxzotr.sHtML

ROLLBACK;
来源：http://baike.vehdjk.com/Article/details/gbcyppyan.sHtML

[Q66] 行锁查询
来源：http://www.m.share.epnwcf.com/Article/details/gtyeyseop.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.yfazqb.com/Article/details/gdutvusjp.sHtML

[Q67] 设置隔离级别
来源：http://3g.vehdjk.com/Article/details/gwimxhlbw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.epnwcf.com/Article/details/gkadcrbgu.sHtML

[Q68] 保存点
来源：http://wap.fktsv.cn/Article/details/gjkxjlcpu.sHtML

SAVEPOINT sp1;
来源：http://baike.epnwcf.com/Article/details/ggpovlcpf.sHtML

ROLLBACK TO sp1;
来源：http://baike.sjlbkw.cn/Article/details/gxswrljxv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.vehdjk.com/Article/details/gaupvlmeq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.epnwcf.com/Article/details/gelgjwbjq.sHtML

[Q70] 更新统计信息
来源：http://blog.yfazqb.com/Article/details/gmqymybaa.sHtML


<!-- 参考信息 -->