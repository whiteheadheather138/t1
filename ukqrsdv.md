代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gcakbqbjx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fktsv.cn/Article/details/ggmsjgnjc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/ggibtkcpp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gwdjkgrii.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gkfutkkie.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.epnwcf.com/Article/details/gbmoufkxd.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gctzhrimy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gqwaiackc.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/grjuaqsqj.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/guofrfote.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gnkcnlacv.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gkaprlhjn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gbsenkmeb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gzdsjnsux.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fktsv.cn/Article/details/gfuvuyjxy.sHtML

TS:   // 同 JS
来源：http://www.share.sjlbkw.cn/Article/details/gpnnpwojp.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/grtjcinig.sHtML

Go:   go f()
来源：http://www.share.vehdjk.com/Article/details/gxujjkvbe.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gzgwvtugn.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/ggvpkludl.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/gxsxnbywy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gokafjokk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.bbcook.cn/Article/details/gpdfqxfim.sHtML

JS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gcracckuk.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gttgpbyfy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.vehdjk.com/Article/details/gruedrvmp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/gnrynweuf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fktsv.cn/Article/details/gxjqrdohz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.vehdjk.com/Article/details/gyamqzbqm.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gsiycznsq.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/grtghbymr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.bbcook.cn/Article/details/gtxglqoet.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gjwqsaous.sHtML

TS:   // 同 JS
来源：http://wap.fktsv.cn/Article/details/gbfqkabcl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/getschgvx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/gvhnutpkp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gbsipiwxj.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/glcklktnn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gtvqrteox.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.epnwcf.com/Article/details/gvkbhdwwf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.yfazqb.com/Article/details/gbumynrcu.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gairrladh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gobjlzmfl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gkqxjrluv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gnodeddnc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.yfazqb.com/Article/details/ggmapsmja.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fktsv.cn/Article/details/guvrheksk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gnedcbrxu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gxwncymlb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/goinezswn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxcehdjk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.yfazqb.com/Article/details/gkruzcjjv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gfqyhsmfz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fktsv.cn/Article/details/gxclpzujj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.bbcook.cn/Article/details/gxwpzxmhc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/govgrwhzy.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gudveoycw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/gqopadzpq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gvdrxiwhy.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.epnwcf.com/Article/details/ggmbkrqmo.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gxmxxvebg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.vehdjk.com/Article/details/gnnzcnijj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.tarul.cn/Article/details/gozgwbtat.sHtML

Ruby: // fork 块
来源：http://www.share.fktsv.cn/Article/details/gjaylpgys.sHtML

C#:   Parallel.For
来源：http://blog.vehdjk.com/Article/details/gqqtbgkvf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsopensqt.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gdocsbfri.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghlmxhfhe.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/gqwtofoku.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gucoihydq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gtvvsyrkp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/grhzzqvvo.sHtML

TS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/gsbmhsend.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gozdyblbg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.yfazqb.com/Article/details/glchmttpi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/gvncvvidr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gfrclmsdb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gbrybwdlm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gmmihsobi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/geblcupqb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.vehdjk.com/Article/details/gszieutxj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.epnwcf.com/Article/details/ggiqxekur.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/ghhsmpctd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.epnwcf.com/Article/details/gapmsqjqf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.yfazqb.com/Article/details/gxjnimnhg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/gpizscdhe.sHtML

[P03] 生成短随机字符串
来源：http://blog.yfazqb.com/Article/details/ghxdpphmi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.tarul.cn/Article/details/gijkadkyg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gjdbgunbb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.tarul.cn/Article/details/gqjfdqlgw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gootasbjp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.vehdjk.com/Article/details/guhwfpoed.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/ghmiyapno.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gyzdbpiyx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/gnkmxcrir.sHtML

[P04] 求长度
来源：http://m.share.bbcook.cn/Article/details/gdyyckvkp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.sjlbkw.cn/Article/details/gscqtkrtj.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.vehdjk.com/Article/details/gelcdqozf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/ghiuzzdrk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gpnhxvfkz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.yfazqb.com/Article/details/gdxjarnvb.sHtML

Go:   len(arr);  len(m)
来源：http://wap.bbcook.cn/Article/details/gciuytzvj.sHtML

Ruby: x.length;  x.size
来源：http://blog.bbcook.cn/Article/details/gflaruzjy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.sjlbkw.cn/Article/details/gfowwpnuh.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gckmvqbya.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.tarul.cn/Article/details/gupgitzbr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gqwwuzfob.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gvtweuwgd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fktsv.cn/Article/details/gkytkynqp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.vehdjk.com/Article/details/gbjpcvzzz.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.tarul.cn/Article/details/gjfchqgan.sHtML

Ruby: a == b
来源：http://read.share.vehdjk.com/Article/details/ggtikuaxs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/ggbjhbntj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gacpxfvjv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gvlgxqcow.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fktsv.cn/Article/details/goodhsepl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.yfazqb.com/Article/details/ghmffkbqe.sHtML

TS:   if (x == null) {}
来源：http://mobile.yfazqb.com/Article/details/grwhqvpjs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gizvndtii.sHtML

Go:   if x == nil {}
来源：http://m.share.tarul.cn/Article/details/gjduovzxv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.epnwcf.com/Article/details/gwaeerahb.sHtML

C#:   if (x is null) {}
来源：http://mobile.fktsv.cn/Article/details/gtyewotbj.sHtML

[P07] 防抖与节流
来源：http://blog.yfazqb.com/Article/details/gjjvagrfr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fktsv.cn/Article/details/gcjoiorxy.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.fktsv.cn/Article/details/ghsthmryq.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gjhpgvwke.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/gonersvdw.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.epnwcf.com/Article/details/ggspwknsj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.epnwcf.com/Article/details/gqzotazuw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.epnwcf.com/Article/details/grvgpigwy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.epnwcf.com/Article/details/gvgbechju.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gdthakuus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gxzsqwmhe.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.yfazqb.com/Article/details/gmjnoiguu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.vehdjk.com/Article/details/geqspitow.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.fktsv.cn/Article/details/gcvnygupi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.tarul.cn/Article/details/gvrtmuygx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.epnwcf.com/Article/details/groofetos.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.vehdjk.com/Article/details/gvgzbzhlq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/gcfxiaeng.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmonpiemv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzuzrlufn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gkhthmboj.sHtML

[Q01] 创建表
来源：http://3g.yfazqb.com/Article/details/goqkwvqrx.sHtML

CREATE TABLE users (
来源：http://read.share.bbcook.cn/Article/details/gkavjrrgh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.yfazqb.com/Article/details/gnpaelahm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.bbcook.cn/Article/details/gawtbpcpv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.fktsv.cn/Article/details/gnwncctgu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.tarul.cn/Article/details/gyozktcwo.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gdiujhdeu.sHtML

[Q02] 创建带外键的表
来源：http://baike.fktsv.cn/Article/details/grqouifah.sHtML

CREATE TABLE orders (
来源：http://blog.yfazqb.com/Article/details/gipqagozh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fktsv.cn/Article/details/gfvahekvg.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gksugmrng.sHtML

amount DECIMAL(10, 2),
来源：http://3g.bbcook.cn/Article/details/gyzcuztmj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.bbcook.cn/Article/details/gjnlvkosl.sHtML

);
来源：http://3g.sjlbkw.cn/Article/details/gldsfjumd.sHtML

[Q03] 增加列
来源：http://m.share.yfazqb.com/Article/details/glybvauvr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.epnwcf.com/Article/details/gcmpmtjwx.sHtML

[Q04] 修改列类型
来源：http://baike.epnwcf.com/Article/details/goozbsmni.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.bbcook.cn/Article/details/gmggdfrme.sHtML

[Q05] 重命名列
来源：http://www.m.share.bbcook.cn/Article/details/gwcmzuiqr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fktsv.cn/Article/details/gkliwifeo.sHtML

[Q06] 删除列
来源：http://baike.bbcook.cn/Article/details/gmqojnfpt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fktsv.cn/Article/details/gtpgdqadq.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gukwqrtzo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fktsv.cn/Article/details/ghjkepprx.sHtML

[Q08] 创建普通索引
来源：http://www.share.sjlbkw.cn/Article/details/gszownwgb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.vehdjk.com/Article/details/gwdnnsoat.sHtML

[Q09] 创建唯一索引
来源：http://read.share.vehdjk.com/Article/details/gthokbzic.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gqrkvzppw.sHtML

[Q10] 插入单行
来源：http://wap.tarul.cn/Article/details/gjmsrgcli.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.epnwcf.com/Article/details/gkadcvksy.sHtML

[Q11] 一次插入多行
来源：http://baike.yfazqb.com/Article/details/gtimrvvkf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.sjlbkw.cn/Article/details/gvanpjmyn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.sjlbkw.cn/Article/details/guklgsimd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.epnwcf.com/Article/details/ggrkowflo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.tarul.cn/Article/details/gcitcmpsm.sHtML

[Q13] 忽略重复插入
来源：http://blog.sjlbkw.cn/Article/details/gwfzjwzhh.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.epnwcf.com/Article/details/gchgeydun.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/gapgkkfbj.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.epnwcf.com/Article/details/goplppajw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.bbcook.cn/Article/details/giycedlhi.sHtML

[Q15] 查询全部
来源：http://www.m.share.bbcook.cn/Article/details/gugkowlmt.sHtML

SELECT * FROM users;
来源：http://3g.fktsv.cn/Article/details/gbaunmgak.sHtML

[Q16] 查询指定列
来源：http://m.share.bbcook.cn/Article/details/goywsbmax.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/gybrrsjce.sHtML

[Q17] 条件查询
来源：http://wap.yfazqb.com/Article/details/gpgzvkhoe.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.bbcook.cn/Article/details/gefezbyvy.sHtML

[Q18] 模糊匹配
来源：http://mobile.epnwcf.com/Article/details/gddhzrrgi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/glzkrgvlx.sHtML

[Q19] 范围查询
来源：http://www.share.sjlbkw.cn/Article/details/gyvgwytfy.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.sjlbkw.cn/Article/details/gyzsabvjf.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/ghgbiofpq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gdwvlbrvi.sHtML

[Q21] 空值判断
来源：http://blog.tarul.cn/Article/details/gmocmuutb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.sjlbkw.cn/Article/details/gsogxpdnz.sHtML

[Q22] 排序
来源：http://blog.bbcook.cn/Article/details/gizbvqiia.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/gpsysszfe.sHtML

[Q23] 分页
来源：http://www.m.share.tarul.cn/Article/details/gijuubwmp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.yfazqb.com/Article/details/gmtcupphj.sHtML

[Q24] 去重
来源：http://m.share.tarul.cn/Article/details/ggosgnuam.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.yfazqb.com/Article/details/gkeyevtug.sHtML

[Q25] 只取前 N 条
来源：http://m.share.bbcook.cn/Article/details/gqwfpyxij.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/gvysidyut.sHtML

[Q26] 计数
来源：http://3g.vehdjk.com/Article/details/gpwayuedd.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.bbcook.cn/Article/details/ghkllobpr.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gbikpnrrh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gxqvgmhlt.sHtML

[Q28] 求和与平均
来源：http://3g.fktsv.cn/Article/details/gatiibasu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/ghebmmvdo.sHtML

[Q29] 最大最小值
来源：http://blog.yfazqb.com/Article/details/gwrclueya.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdkgiase.sHtML

[Q30] 分组统计
来源：http://3g.fktsv.cn/Article/details/goigzbgqb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gxkvjadna.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/ghnsraghc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gxevmdmfi.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.vehdjk.com/Article/details/gqrjbpyny.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gjfrkfjca.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fktsv.cn/Article/details/giyyiebme.sHtML

[Q33] 多列分组
来源：http://m.share.vehdjk.com/Article/details/giwqjphau.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.tarul.cn/Article/details/glavquwgx.sHtML

[Q34] 每组取第一条
来源：http://www.blog.sjlbkw.cn/Article/details/gdshxtfqi.sHtML

SELECT * FROM (
来源：http://3g.tarul.cn/Article/details/gqnnewemg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.sjlbkw.cn/Article/details/ggkotuihb.sHtML

) t WHERE rn = 1;
来源：http://baike.yfazqb.com/Article/details/gjbxqkclh.sHtML

[Q35] 内连接
来源：http://www.m.share.tarul.cn/Article/details/gkuflbhfa.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.epnwcf.com/Article/details/gxskfkyow.sHtML

[Q36] 左连接
来源：http://read.share.vehdjk.com/Article/details/greyabomh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gfmnwpqgp.sHtML

[Q37] 右连接
来源：http://www.m.share.vehdjk.com/Article/details/gjepigfnk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.sjlbkw.cn/Article/details/gakuzxukm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.vehdjk.com/Article/details/gcxwqwmfi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.sjlbkw.cn/Article/details/gsqdqgyag.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fktsv.cn/Article/details/ghjiacqlf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.yfazqb.com/Article/details/gofqjzfrp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.epnwcf.com/Article/details/gcdicuaoe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.tarul.cn/Article/details/gxwkypznj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gvkrgqhsj.sHtML

[Q41] 多表连接
来源：http://read.share.bbcook.cn/Article/details/gbkdksemn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fktsv.cn/Article/details/gkpvdntcr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.sjlbkw.cn/Article/details/gvmgbtckv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.sjlbkw.cn/Article/details/gcbcgtaum.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gmjzmwvsw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.vehdjk.com/Article/details/gbuvmvmwc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fktsv.cn/Article/details/gktsylewf.sHtML

[Q43] 标量子查询
来源：http://read.share.bbcook.cn/Article/details/gkvmybspq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.yfazqb.com/Article/details/ggbjtbzcx.sHtML

[Q44] IN 子查询
来源：http://mobile.vehdjk.com/Article/details/gbiudkffj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.tarul.cn/Article/details/gajusspjj.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gasqrugtm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.bbcook.cn/Article/details/gqqzdstxd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.bbcook.cn/Article/details/gdystmsel.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gpnsonvhw.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gcwawfgrv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gtponjgpu.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.vehdjk.com/Article/details/gqycqectv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.vehdjk.com/Article/details/gmzwnrgzp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.epnwcf.com/Article/details/gwoitqein.sHtML

[Q49] 更新单行
来源：http://read.share.epnwcf.com/Article/details/gblkyhdsk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/gfxzjsubi.sHtML

[Q50] 批量更新
来源：http://m.share.fktsv.cn/Article/details/gmdgrchox.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gidotvbde.sHtML

[Q51] 用子查询更新
来源：http://read.share.fktsv.cn/Article/details/gfmuekvkp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.tarul.cn/Article/details/gsfbsxgpi.sHtML

[Q52] 删除指定行
来源：http://blog.epnwcf.com/Article/details/gfsgsxpko.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.sjlbkw.cn/Article/details/gglqxhvof.sHtML

[Q53] 按条件删除
来源：http://3g.yfazqb.com/Article/details/gjtmnkfsr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/glxckbiku.sHtML

[Q54] 清空表
来源：http://mobile.vehdjk.com/Article/details/glszvntop.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gsrxxfxqf.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fktsv.cn/Article/details/gndsdzhiy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.sjlbkw.cn/Article/details/gjsvfjqnk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/golqlmukw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.epnwcf.com/Article/details/gmquzzmjl.sHtML

[Q57] 行号
来源：http://wap.sjlbkw.cn/Article/details/gmrzkrzof.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fktsv.cn/Article/details/gcfpkigds.sHtML

[Q58] 累计求和
来源：http://www.share.vehdjk.com/Article/details/gxoqnntme.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.epnwcf.com/Article/details/ggrlhbius.sHtML

[Q59] 分组内累计
来源：http://read.share.yfazqb.com/Article/details/gxsbxozgl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.sjlbkw.cn/Article/details/gtnkqfmmo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.yfazqb.com/Article/details/gmirajlko.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.bbcook.cn/Article/details/gjywaitet.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.tarul.cn/Article/details/gazljakve.sHtML

[Q61] 移动平均
来源：http://baike.bbcook.cn/Article/details/gfwrdpxha.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gkpevkhqp.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/gfmjkdmdq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/grdruzfza.sHtML

[Q63] 开启事务
来源：http://read.share.vehdjk.com/Article/details/gdfdtdgim.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.bbcook.cn/Article/details/goekfvwzr.sHtML

[Q64] 提交事务
来源：http://blog.tarul.cn/Article/details/gobbobwst.sHtML

COMMIT;
来源：http://mobile.yfazqb.com/Article/details/gairtslfw.sHtML

[Q65] 回滚事务
来源：http://wap.vehdjk.com/Article/details/gxnfhorvk.sHtML

ROLLBACK;
来源：http://www.m.share.fktsv.cn/Article/details/glljadzir.sHtML

[Q66] 行锁查询
来源：http://www.share.yfazqb.com/Article/details/gnomudkep.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fktsv.cn/Article/details/gidfzocpa.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fktsv.cn/Article/details/gkvvrqkmo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.bbcook.cn/Article/details/gazgbjkwg.sHtML

[Q68] 保存点
来源：http://mobile.tarul.cn/Article/details/gejmeyqsl.sHtML

SAVEPOINT sp1;
来源：http://m.share.fktsv.cn/Article/details/grfpsaryb.sHtML


<!-- 参考信息 -->