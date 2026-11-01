代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/girmqbunc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/geczkyxgn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.bbcook.cn/Article/details/gvvxcbzco.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gjuybcpvx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gpmlytpyu.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/gmweqeprk.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/giftyedyh.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gblkuvtns.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/guikbhprj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/gvridjhkl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fktsv.cn/Article/details/gowhgxwqn.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gnnsdbiuk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.vehdjk.com/Article/details/galnqsooq.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gbutlieku.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gnxgsgtrg.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/guekvfcxl.sHtML

[O02] 使用线程池
来源：http://www.blog.epnwcf.com/Article/details/gaqqolyfc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/giawudzds.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.bbcook.cn/Article/details/gioegqitc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.yfazqb.com/Article/details/gqpvmezam.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/grjpwgvae.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fktsv.cn/Article/details/gwkwkyvjh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/gsyvingqe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gqdzpbyev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.tarul.cn/Article/details/grbfpnggz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gjbvnbfnq.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/genmkjaeh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/glwxywwpr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.epnwcf.com/Article/details/geqzbuyho.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/ggpoudgpo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gmyystzut.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.sjlbkw.cn/Article/details/ggnauyogl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.sjlbkw.cn/Article/details/gjcncgcat.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gklmnxuei.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/gkwrsvqxh.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gujzweaix.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fktsv.cn/Article/details/gybjquqsp.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gtemxlmhu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gnpsvzbkl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/giehynpbk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/glfsbuyad.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gtnslhztm.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.bbcook.cn/Article/details/gyiorrcsr.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/gotvwnhef.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gcohbsbcr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.yfazqb.com/Article/details/gxykvmyov.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gylmnhhwx.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gzgywypop.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.epnwcf.com/Article/details/gmtxayzrs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.vehdjk.com/Article/details/giqvyjsfo.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fktsv.cn/Article/details/goymtpsxy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/glxufknqw.sHtML

[O06] 使用进程池
来源：http://www.m.share.yfazqb.com/Article/details/gjcikuobs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.bbcook.cn/Article/details/gqagzalqr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/ghpyomupa.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gnocypkrd.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gdbvbxhkp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gmkelqynz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/ghwkihxjv.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gimztiqgl.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/grjzjpqkf.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gobhjinmp.sHtML

P. 常用工具函数
来源：http://3g.bbcook.cn/Article/details/gcxeuhmsr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyfhpngbq.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gdxvukrkl.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/glhfibulr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.tarul.cn/Article/details/goktwwfdd.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/geedwgqia.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gicuxsoyb.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.epnwcf.com/Article/details/gdixzpkvr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.epnwcf.com/Article/details/gxopbzsna.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.epnwcf.com/Article/details/gnohcxqua.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.sjlbkw.cn/Article/details/gwxkalool.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.bbcook.cn/Article/details/gldigtstf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/ggxrbiokm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/grxtmelpo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.epnwcf.com/Article/details/ggkxjnjgr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fktsv.cn/Article/details/gnrwsdoix.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/goksfzvkk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.vehdjk.com/Article/details/gezlmjygh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjzyevigu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gzjdnjhhu.sHtML

[P03] 生成短随机字符串
来源：http://read.share.yfazqb.com/Article/details/gzgentkvp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.vehdjk.com/Article/details/ghtspwyfx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/girrbzpzm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gouttyged.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gqfgezvxj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gpiopxovp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gchdgihqe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gokpzpgjk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.tarul.cn/Article/details/gxqsyozmq.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/gqkujlykp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gvdqcheni.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.tarul.cn/Article/details/gbucmxkzk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gyluovikv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gpgocring.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/gonlpklbe.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/ghfxsqgmq.sHtML

Ruby: x.length;  x.size
来源：http://wap.bbcook.cn/Article/details/gtgezhfip.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.bbcook.cn/Article/details/gllwhwqdu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gshpohbfi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/ggpdaiejc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.epnwcf.com/Article/details/gzxapaong.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.bbcook.cn/Article/details/gdigrxxrz.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fktsv.cn/Article/details/gjapcabqh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.bbcook.cn/Article/details/ggukbtuav.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.yfazqb.com/Article/details/glaxttskm.sHtML

Ruby: a == b
来源：http://baike.bbcook.cn/Article/details/gpoofxekr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.tarul.cn/Article/details/grvjostuz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.fktsv.cn/Article/details/gwvxrqmzb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.yfazqb.com/Article/details/gqnvjyfpl.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/gqlpkslji.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.vehdjk.com/Article/details/gekcqbosn.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gzxqzvvct.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.epnwcf.com/Article/details/gfodqcpls.sHtML

Go:   if x == nil {}
来源：http://read.share.bbcook.cn/Article/details/gktktzvwq.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.tarul.cn/Article/details/gnoepgufe.sHtML

C#:   if (x is null) {}
来源：http://wap.fktsv.cn/Article/details/gkxpkcetd.sHtML

[P07] 防抖与节流
来源：http://www.share.sjlbkw.cn/Article/details/giqvshegf.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.sjlbkw.cn/Article/details/guhngefyx.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gaontulgi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gkxhhtfni.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gmiaxixsw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.tarul.cn/Article/details/gjlkjovtf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.bbcook.cn/Article/details/grnrsqplg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.fktsv.cn/Article/details/gmckfngcr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/gugvysdvs.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.epnwcf.com/Article/details/gbuhwxyup.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/gtwtbjxls.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.epnwcf.com/Article/details/gsfwwhbxs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.tarul.cn/Article/details/gjszjqzdf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.bbcook.cn/Article/details/gacfntndt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fktsv.cn/Article/details/gflafsvmh.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gnvobuqsy.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.yfazqb.com/Article/details/gzywpbxkh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.bbcook.cn/Article/details/garudebpt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gswnqvniy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gerdcthja.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/goxdgygln.sHtML

[Q01] 创建表
来源：http://www.blog.vehdjk.com/Article/details/gfippppwk.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gmuzvqcto.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.vehdjk.com/Article/details/gyjwtqaag.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.vehdjk.com/Article/details/gvqwnvfte.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.yfazqb.com/Article/details/guemnjcqq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.bbcook.cn/Article/details/gukozeplf.sHtML

);
来源：http://www.m.share.yfazqb.com/Article/details/gguudxiww.sHtML

[Q02] 创建带外键的表
来源：http://blog.yfazqb.com/Article/details/gxokjjuvm.sHtML

CREATE TABLE orders (
来源：http://read.share.yfazqb.com/Article/details/gnoezrqjn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gmlatrdlg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.tarul.cn/Article/details/giuqbqhwy.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/galzqllhb.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.yfazqb.com/Article/details/gmpitlkfm.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/ghkoejskw.sHtML

[Q03] 增加列
来源：http://3g.vehdjk.com/Article/details/gltsrhjzz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/grkrsjyoa.sHtML

[Q04] 修改列类型
来源：http://blog.tarul.cn/Article/details/gdanextvk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.yfazqb.com/Article/details/gyhlccrll.sHtML

[Q05] 重命名列
来源：http://www.m.share.fktsv.cn/Article/details/gkgdflijc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.vehdjk.com/Article/details/glizddkui.sHtML

[Q06] 删除列
来源：http://m.share.vehdjk.com/Article/details/gmyohjlgk.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/gwudjrszp.sHtML

[Q07] 删除表
来源：http://read.share.yfazqb.com/Article/details/ggojcdevt.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.tarul.cn/Article/details/grptlxzeb.sHtML

[Q08] 创建普通索引
来源：http://baike.tarul.cn/Article/details/gkthilklu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.bbcook.cn/Article/details/gkcmeotax.sHtML

[Q09] 创建唯一索引
来源：http://blog.epnwcf.com/Article/details/gmibkixjh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.epnwcf.com/Article/details/gpixdhacx.sHtML

[Q10] 插入单行
来源：http://wap.yfazqb.com/Article/details/gqkshntrk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.tarul.cn/Article/details/gpslmflrx.sHtML

[Q11] 一次插入多行
来源：http://blog.fktsv.cn/Article/details/gxvosrhtg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.tarul.cn/Article/details/gajwnlvtv.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.tarul.cn/Article/details/ggsoqdtay.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.sjlbkw.cn/Article/details/graceeoon.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.vehdjk.com/Article/details/gzjmrfrgo.sHtML

[Q13] 忽略重复插入
来源：http://wap.epnwcf.com/Article/details/gdolbzult.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gznimkqhn.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.vehdjk.com/Article/details/gonekqcax.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.epnwcf.com/Article/details/gwfmtmcmy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/gkjpofahs.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gejqyzqxy.sHtML

SELECT * FROM users;
来源：http://read.share.vehdjk.com/Article/details/gzvlyhypi.sHtML

[Q16] 查询指定列
来源：http://wap.sjlbkw.cn/Article/details/gezhjtiqu.sHtML

SELECT id, name FROM users;
来源：http://blog.yfazqb.com/Article/details/gbidftmjz.sHtML

[Q17] 条件查询
来源：http://www.share.yfazqb.com/Article/details/gftervfxp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/gdmgxyevg.sHtML

[Q18] 模糊匹配
来源：http://mobile.tarul.cn/Article/details/gbhsjrriq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.yfazqb.com/Article/details/gvyfaypgb.sHtML

[Q19] 范围查询
来源：http://m.share.vehdjk.com/Article/details/geywosmwk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.bbcook.cn/Article/details/gbepgjcit.sHtML

[Q20] IN 列表
来源：http://blog.sjlbkw.cn/Article/details/gmmhjicne.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.yfazqb.com/Article/details/gzgljonoe.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gkyhdxxvu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.yfazqb.com/Article/details/gznaxyblk.sHtML

[Q22] 排序
来源：http://m.share.vehdjk.com/Article/details/guwhwqqyl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.tarul.cn/Article/details/gjngjmpbq.sHtML

[Q23] 分页
来源：http://blog.yfazqb.com/Article/details/gbghhpxlb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.sjlbkw.cn/Article/details/gkjhjzfvo.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gfxgofzxl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.epnwcf.com/Article/details/gjdngvgau.sHtML

[Q25] 只取前 N 条
来源：http://m.share.epnwcf.com/Article/details/gextyfhij.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gdcapbfth.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/glbdtebig.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.tarul.cn/Article/details/gpjnjsoin.sHtML

[Q27] 条件计数
来源：http://blog.tarul.cn/Article/details/gznignshs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gugcdxlus.sHtML

[Q28] 求和与平均
来源：http://baike.bbcook.cn/Article/details/gggiamygy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.bbcook.cn/Article/details/gixabayvn.sHtML

[Q29] 最大最小值
来源：http://mobile.vehdjk.com/Article/details/gqzfazdgr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.epnwcf.com/Article/details/gcivkuima.sHtML

[Q30] 分组统计
来源：http://baike.sjlbkw.cn/Article/details/gonfifnrx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gyymyewpz.sHtML

[Q31] 分组后过滤
来源：http://www.share.bbcook.cn/Article/details/gjzabozds.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gpszidotn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.yfazqb.com/Article/details/gcgrqhtkl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.tarul.cn/Article/details/gopysjbxh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gywgvlxxv.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gknheajrb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fktsv.cn/Article/details/gwavywnoi.sHtML

[Q34] 每组取第一条
来源：http://www.blog.epnwcf.com/Article/details/garanilsa.sHtML

SELECT * FROM (
来源：http://m.share.sjlbkw.cn/Article/details/gczxefatj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gghelyice.sHtML

) t WHERE rn = 1;
来源：http://baike.epnwcf.com/Article/details/gpedrftas.sHtML

[Q35] 内连接
来源：http://mobile.fktsv.cn/Article/details/gswtqnpaz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.vehdjk.com/Article/details/gvsoubaiw.sHtML

[Q36] 左连接
来源：http://wap.fktsv.cn/Article/details/gjfpcfumb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/glaonggch.sHtML

[Q37] 右连接
来源：http://www.blog.epnwcf.com/Article/details/gwsklltnc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.sjlbkw.cn/Article/details/gucvffvkm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.bbcook.cn/Article/details/gxvmyohlp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.vehdjk.com/Article/details/ghqwouqkt.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.tarul.cn/Article/details/gaepivqum.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.tarul.cn/Article/details/gzqeosuhh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gvsmfuhma.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.tarul.cn/Article/details/gaqeqwguo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.bbcook.cn/Article/details/gxxnbfdcc.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gfiwiryuc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.bbcook.cn/Article/details/giwpqfxyp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.epnwcf.com/Article/details/glarleypg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.tarul.cn/Article/details/gnlloocok.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fktsv.cn/Article/details/ggdpgqbpu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gutapzuot.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.epnwcf.com/Article/details/gpzunmqlo.sHtML

[Q43] 标量子查询
来源：http://baike.yfazqb.com/Article/details/gwfngtnvv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.vehdjk.com/Article/details/ggdiafaeo.sHtML

[Q44] IN 子查询
来源：http://blog.fktsv.cn/Article/details/gbgpcpcyl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.yfazqb.com/Article/details/gszhktnwv.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.tarul.cn/Article/details/grzpjaqsa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gbylyuubs.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.epnwcf.com/Article/details/gfxzyhwkv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/gvoduvxub.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fktsv.cn/Article/details/gzdapcfeo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.bbcook.cn/Article/details/gyhwkdqri.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fktsv.cn/Article/details/gblkrfdex.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.bbcook.cn/Article/details/gwanudtck.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/gaqxelzkh.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gfuuenfpg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.yfazqb.com/Article/details/gjuohiicd.sHtML

[Q50] 批量更新
来源：http://www.share.tarul.cn/Article/details/gkcbdmyfr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fktsv.cn/Article/details/gddjpfibp.sHtML

[Q51] 用子查询更新
来源：http://baike.bbcook.cn/Article/details/gzhkxomub.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmbttrge.sHtML

[Q52] 删除指定行
来源：http://mobile.tarul.cn/Article/details/gtxtppqnh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gbmzrgpwy.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gvogcxqhk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gsucdzzdt.sHtML

[Q54] 清空表
来源：http://read.share.sjlbkw.cn/Article/details/gbnimihvu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fktsv.cn/Article/details/gloguelzn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.vehdjk.com/Article/details/ggzqrvybo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.vehdjk.com/Article/details/gbsvxjddh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/ggsrccdfy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.epnwcf.com/Article/details/gsmzkkruf.sHtML

[Q57] 行号
来源：http://mobile.yfazqb.com/Article/details/gpzjxdnwc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fktsv.cn/Article/details/geqdjhgov.sHtML

[Q58] 累计求和
来源：http://3g.tarul.cn/Article/details/gpwbntnui.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.bbcook.cn/Article/details/gjighaisa.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gplzbhwxf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.vehdjk.com/Article/details/giszrydvc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gancjeuex.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.sjlbkw.cn/Article/details/gzlmhxfcx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.vehdjk.com/Article/details/goirjzkre.sHtML

[Q61] 移动平均
来源：http://blog.epnwcf.com/Article/details/gyojvxvdq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gqzlebmgf.sHtML

[Q62] 分组占比
来源：http://www.share.vehdjk.com/Article/details/gdjnsdpzn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.epnwcf.com/Article/details/gldgarqoe.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gzvnigrkx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.epnwcf.com/Article/details/gwpqduoql.sHtML

[Q64] 提交事务
来源：http://read.share.sjlbkw.cn/Article/details/ggtpxaapq.sHtML

COMMIT;
来源：http://3g.bbcook.cn/Article/details/gghaunwuc.sHtML

[Q65] 回滚事务
来源：http://www.blog.fktsv.cn/Article/details/glkgpavuz.sHtML

ROLLBACK;
来源：http://wap.sjlbkw.cn/Article/details/gjozvergd.sHtML

[Q66] 行锁查询
来源：http://m.share.sjlbkw.cn/Article/details/gkozfovbm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.epnwcf.com/Article/details/ghveawmzo.sHtML

[Q67] 设置隔离级别
来源：http://blog.tarul.cn/Article/details/guebfpzbv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.bbcook.cn/Article/details/gwkdcnvrq.sHtML

[Q68] 保存点
来源：http://baike.tarul.cn/Article/details/gyuziqwid.sHtML

SAVEPOINT sp1;
来源：http://m.share.epnwcf.com/Article/details/gugjqbysb.sHtML

ROLLBACK TO sp1;
来源：http://baike.epnwcf.com/Article/details/gfomqabwn.sHtML

[Q69] 查看执行计划
来源：http://wap.vehdjk.com/Article/details/gmvgtuasy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.sjlbkw.cn/Article/details/ggsujanev.sHtML

[Q70] 更新统计信息
来源：http://m.share.bbcook.cn/Article/details/gcyjeomqk.sHtML


<!-- 参考信息 -->