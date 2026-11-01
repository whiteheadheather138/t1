代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gyqvyxhxm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gbyoypwyn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gbysakipp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/grwyrkwmv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gnpettcvu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.yfazqb.com/Article/details/gkklshzih.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gsljepxds.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gvfdoxuvk.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gxhbkfhpl.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gvytctxob.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/grmljszxq.sHtML

[O01] 启动一个线程
来源：http://wap.yfazqb.com/Article/details/gwbkpqelm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gulaehapf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.bbcook.cn/Article/details/gghbqrsbc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/gojktcyqr.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gxxmkrvya.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.sjlbkw.cn/Article/details/geqyzsedx.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gplfezxtc.sHtML

Ruby: Thread.new { f }
来源：http://m.share.sjlbkw.cn/Article/details/gcvyumpip.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.yfazqb.com/Article/details/gppsrazhz.sHtML

[O02] 使用线程池
来源：http://m.share.yfazqb.com/Article/details/gditgzpck.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.vehdjk.com/Article/details/gocauatdd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/grukaomwx.sHtML

JS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gwhvghpwm.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gbytiosdi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/giaabnpzr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.bbcook.cn/Article/details/gdcjcczly.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.yfazqb.com/Article/details/glgqhwtei.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.sjlbkw.cn/Article/details/gzxuendyx.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.vehdjk.com/Article/details/gnlytpqdw.sHtML

Py:   with lock: shared += 1
来源：http://read.share.epnwcf.com/Article/details/gdzuhvwoq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gwlucebot.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gpxujiyki.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gpkfrcasc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gmdvxdzvp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gvldyupgg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fktsv.cn/Article/details/getvwwekl.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gbqhmyhjo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fktsv.cn/Article/details/gjnbttxip.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.vehdjk.com/Article/details/gxjetpvue.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/ggrsuflrr.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/glrhuprfl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gugoambwg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/grsgrrgjh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/ggxhfpqxu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gogigosse.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.epnwcf.com/Article/details/gkpprkweb.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fktsv.cn/Article/details/gvniegxjs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gwxnoiqcy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/gfdxbbyew.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gzjtotgrz.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gmonbgpsz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fktsv.cn/Article/details/gzamjbuid.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxxmvrte.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gmxsarybj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/gypmwbryi.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gcgtdjvci.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gpxvywmeh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.epnwcf.com/Article/details/guujsfakm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gwvoggqdz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gkwswercr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/gzqkuelby.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/glkgqbdce.sHtML

Ruby: // fork 块
来源：http://m.share.fktsv.cn/Article/details/gnszdnqnb.sHtML

C#:   Parallel.For
来源：http://read.share.fktsv.cn/Article/details/gbdvhicyf.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gckwmispn.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gcmgjwzad.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gfsgbyidr.sHtML

[P01] 生成 UUID
来源：http://blog.bbcook.cn/Article/details/gdeocoppi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.tarul.cn/Article/details/gxtihvajy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gdrayfhkc.sHtML

JS:   crypto.randomUUID()
来源：http://wap.epnwcf.com/Article/details/giehnxgso.sHtML

TS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gdzocjutx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.epnwcf.com/Article/details/gxxrhxlzj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gbadekvoo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/gatikupbb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/ghmpmihhm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/grlamvoux.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.bbcook.cn/Article/details/gunygeclc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gcwunvope.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/grogmsinv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.vehdjk.com/Article/details/gngzonnhj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.sjlbkw.cn/Article/details/gueivnead.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.bbcook.cn/Article/details/gympgodza.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gxhmxjzda.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/glydjbkbz.sHtML

[P03] 生成短随机字符串
来源：http://3g.fktsv.cn/Article/details/ggqfufjfp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.vehdjk.com/Article/details/gjhnipdfz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.bbcook.cn/Article/details/gukijrmda.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gmnxpyddf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fktsv.cn/Article/details/ggtthtigo.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gkcfvxvfg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gqfkktayn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.bbcook.cn/Article/details/gxkoiznyy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.sjlbkw.cn/Article/details/ghccvjucn.sHtML

[P04] 求长度
来源：http://wap.epnwcf.com/Article/details/gxylxgwuc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gopkwhxlf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.tarul.cn/Article/details/gmnigizjk.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.epnwcf.com/Article/details/gedclmksw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/gxuizgqga.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/ghkqxtcjh.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.bbcook.cn/Article/details/gbdytdcli.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gmkpolvbq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.sjlbkw.cn/Article/details/gndyaixhz.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.bbcook.cn/Article/details/gigtryxep.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.bbcook.cn/Article/details/ggdcaortc.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.bbcook.cn/Article/details/gaadxradc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/ghryzgepr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gnzmvyxsb.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.epnwcf.com/Article/details/gwzsdcual.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/gbhthanpu.sHtML

Ruby: a == b
来源：http://blog.bbcook.cn/Article/details/gnsskvlzq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gwdwjmfpd.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/ggehxmxwj.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.epnwcf.com/Article/details/gxzojinej.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.tarul.cn/Article/details/gcxswtipn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.epnwcf.com/Article/details/gonetejym.sHtML

TS:   if (x == null) {}
来源：http://blog.yfazqb.com/Article/details/gyewxlhoc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fktsv.cn/Article/details/gxvmloqsh.sHtML

Go:   if x == nil {}
来源：http://www.share.bbcook.cn/Article/details/gebxsduqg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/gqfxxkrmx.sHtML

C#:   if (x is null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gctrmhres.sHtML

[P07] 防抖与节流
来源：http://wap.sjlbkw.cn/Article/details/gnorqoxez.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.tarul.cn/Article/details/gnxxtwimv.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.epnwcf.com/Article/details/gmiiggjmk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.tarul.cn/Article/details/gqnstknal.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gnioctbzi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.sjlbkw.cn/Article/details/gycfmeibu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.epnwcf.com/Article/details/gzarnhyiw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.bbcook.cn/Article/details/gagrwiugt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fktsv.cn/Article/details/gljsocbaf.sHtML

[P08] 处理浮点精度问题
来源：http://baike.tarul.cn/Article/details/gkefskvok.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.fktsv.cn/Article/details/grgcnudyd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.sjlbkw.cn/Article/details/gyfxyopry.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gmnezvofd.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.bbcook.cn/Article/details/gyppzlinc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.bbcook.cn/Article/details/gefnssyli.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.sjlbkw.cn/Article/details/gqinipwpa.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/gjjxkaahg.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.epnwcf.com/Article/details/gadtuaacp.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gxrgsqwfq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fktsv.cn/Article/details/gzpazawqh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gphwbujdh.sHtML

[Q01] 创建表
来源：http://read.share.vehdjk.com/Article/details/gokcqmoqn.sHtML

CREATE TABLE users (
来源：http://www.blog.epnwcf.com/Article/details/gndnbponl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gcoigmtnz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gwntbxbyl.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.vehdjk.com/Article/details/ggfkhpveo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gdekwhipq.sHtML

);
来源：http://www.share.epnwcf.com/Article/details/gssyugomt.sHtML

[Q02] 创建带外键的表
来源：http://blog.bbcook.cn/Article/details/gcngzoyum.sHtML

CREATE TABLE orders (
来源：http://mobile.sjlbkw.cn/Article/details/gdaqdphyr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.tarul.cn/Article/details/ghvbagfzo.sHtML

user_id INT NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/gsjqgusil.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.fktsv.cn/Article/details/gehnbcodt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.sjlbkw.cn/Article/details/gnhxuwfmv.sHtML

);
来源：http://www.m.share.fktsv.cn/Article/details/gtzoofnkg.sHtML

[Q03] 增加列
来源：http://baike.bbcook.cn/Article/details/gzicrckei.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.epnwcf.com/Article/details/guppvbgmd.sHtML

[Q04] 修改列类型
来源：http://m.share.sjlbkw.cn/Article/details/gsihytyvt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gvsiwoorn.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gyjbavqai.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.vehdjk.com/Article/details/gzbsgmuqi.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gxxmzssjt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.sjlbkw.cn/Article/details/gfcovtzok.sHtML

[Q07] 删除表
来源：http://3g.bbcook.cn/Article/details/gdfdsiauh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.bbcook.cn/Article/details/gyikjuivc.sHtML

[Q08] 创建普通索引
来源：http://mobile.vehdjk.com/Article/details/gquhnzkpu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/gtiqheciy.sHtML

[Q09] 创建唯一索引
来源：http://baike.fktsv.cn/Article/details/gmnzfuhsz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/ggsdkfuvo.sHtML

[Q10] 插入单行
来源：http://m.share.epnwcf.com/Article/details/gdxkahlsk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fktsv.cn/Article/details/gpxlwmvut.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/gvzdxuany.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.bbcook.cn/Article/details/gezexyvof.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gzzznstne.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.vehdjk.com/Article/details/gzesckwpc.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.vehdjk.com/Article/details/gdlhduiss.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gqunbttph.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fktsv.cn/Article/details/gwuprnrow.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.sjlbkw.cn/Article/details/gtxkznkfc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fktsv.cn/Article/details/grzzguhls.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.bbcook.cn/Article/details/gdhbvsrym.sHtML

[Q15] 查询全部
来源：http://m.share.sjlbkw.cn/Article/details/gdlhnxgkb.sHtML

SELECT * FROM users;
来源：http://wap.yfazqb.com/Article/details/gmmeqztyc.sHtML

[Q16] 查询指定列
来源：http://read.share.tarul.cn/Article/details/grxtjcdsn.sHtML

SELECT id, name FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gnmvcddcw.sHtML

[Q17] 条件查询
来源：http://read.share.bbcook.cn/Article/details/gvhtfomjb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.bbcook.cn/Article/details/gmmocdzxo.sHtML

[Q18] 模糊匹配
来源：http://3g.tarul.cn/Article/details/gnhnemgtz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.epnwcf.com/Article/details/gnjmzbgrq.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gnezcepdp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.vehdjk.com/Article/details/gzzjptevl.sHtML

[Q20] IN 列表
来源：http://blog.fktsv.cn/Article/details/gmclepxgj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/gcczrowfj.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/gdcuisbcf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.bbcook.cn/Article/details/ggarrmhhy.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/guysvqcri.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gjqeypehe.sHtML

[Q23] 分页
来源：http://3g.bbcook.cn/Article/details/glhauswlc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fktsv.cn/Article/details/gcrqloqbq.sHtML

[Q24] 去重
来源：http://3g.fktsv.cn/Article/details/gerxvnulf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.tarul.cn/Article/details/guvdskjzk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.vehdjk.com/Article/details/gsihrhudp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.bbcook.cn/Article/details/gsrpwiqxs.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/gbtezjkhs.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.yfazqb.com/Article/details/ghsdzslvl.sHtML

[Q27] 条件计数
来源：http://www.m.share.sjlbkw.cn/Article/details/gcztuiwiq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.vehdjk.com/Article/details/gcnezmaof.sHtML

[Q28] 求和与平均
来源：http://wap.fktsv.cn/Article/details/gafdbufye.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.sjlbkw.cn/Article/details/gkyscfcjb.sHtML

[Q29] 最大最小值
来源：http://3g.yfazqb.com/Article/details/gtwfvjqhc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.yfazqb.com/Article/details/gwnkgqzlg.sHtML

[Q30] 分组统计
来源：http://blog.vehdjk.com/Article/details/gakmqufpv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gnjhynmaj.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gkzqqxhje.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.sjlbkw.cn/Article/details/gwgodoxzu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fktsv.cn/Article/details/gbcveuzik.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.yfazqb.com/Article/details/gegzdzlrz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gumhejncs.sHtML

[Q33] 多列分组
来源：http://read.share.vehdjk.com/Article/details/gmbvaqpxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.bbcook.cn/Article/details/gxkkvlaav.sHtML

[Q34] 每组取第一条
来源：http://baike.fktsv.cn/Article/details/gbvdhpdfh.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/gzwyvcomo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.vehdjk.com/Article/details/gddgksrkf.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fktsv.cn/Article/details/gqchqvtdj.sHtML

[Q35] 内连接
来源：http://wap.bbcook.cn/Article/details/gclrmomzs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.yfazqb.com/Article/details/gkngtyttx.sHtML

[Q36] 左连接
来源：http://www.share.vehdjk.com/Article/details/giqhqjprs.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.sjlbkw.cn/Article/details/gclpcjntw.sHtML

[Q37] 右连接
来源：http://read.share.sjlbkw.cn/Article/details/ggjztqnez.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.tarul.cn/Article/details/gdzisgryt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gpvsjatnt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.vehdjk.com/Article/details/gybpnyyvi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fktsv.cn/Article/details/ggorkthgy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.epnwcf.com/Article/details/gordwinus.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.tarul.cn/Article/details/gmltnvpiq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fktsv.cn/Article/details/gcupxevvd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.yfazqb.com/Article/details/gwhezrgqt.sHtML

[Q41] 多表连接
来源：http://www.blog.vehdjk.com/Article/details/gpxberzlf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.bbcook.cn/Article/details/gzkuxafdk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.yfazqb.com/Article/details/grfcdezki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fktsv.cn/Article/details/glvhqsotm.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.yfazqb.com/Article/details/gibwulxbq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.yfazqb.com/Article/details/gboiainjr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.sjlbkw.cn/Article/details/ggueccchm.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gfakgccsw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gwtlvdwah.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gzleymulw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fktsv.cn/Article/details/ggzjyqkhe.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.epnwcf.com/Article/details/grciicwcf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.bbcook.cn/Article/details/glhipsdei.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.bbcook.cn/Article/details/gfklakrus.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/grnblhdut.sHtML

[Q47] 与平均值比较
来源：http://3g.yfazqb.com/Article/details/gijafrmiz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gficaljpi.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gotwitrtf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.epnwcf.com/Article/details/gdgzyulyt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.vehdjk.com/Article/details/ghjnpripu.sHtML

[Q49] 更新单行
来源：http://blog.epnwcf.com/Article/details/gpnybmvqn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.tarul.cn/Article/details/gnilkyfwo.sHtML

[Q50] 批量更新
来源：http://read.share.fktsv.cn/Article/details/gyqkhkdya.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.sjlbkw.cn/Article/details/gagizzxuf.sHtML

[Q51] 用子查询更新
来源：http://wap.vehdjk.com/Article/details/gvibgcwix.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.epnwcf.com/Article/details/ghaltxgth.sHtML

[Q52] 删除指定行
来源：http://www.blog.vehdjk.com/Article/details/gvzitrtrx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.sjlbkw.cn/Article/details/gniiomkhl.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gjwdhkide.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fktsv.cn/Article/details/gbuxkakho.sHtML

[Q54] 清空表
来源：http://www.m.share.epnwcf.com/Article/details/ghejvncrp.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gqndmpwbe.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.vehdjk.com/Article/details/geizmezjh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.bbcook.cn/Article/details/guljyrwon.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.bbcook.cn/Article/details/griksjhbu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gfxzofnpq.sHtML

[Q57] 行号
来源：http://m.share.bbcook.cn/Article/details/ggrgtzynm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/gavdghtns.sHtML

[Q58] 累计求和
来源：http://m.share.yfazqb.com/Article/details/gthsprlck.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/ginjknbbl.sHtML

[Q59] 分组内累计
来源：http://read.share.epnwcf.com/Article/details/grldhlaav.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gtzuqiwgg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.tarul.cn/Article/details/gxiairiyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.sjlbkw.cn/Article/details/gedrroicb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.sjlbkw.cn/Article/details/gkjknxgov.sHtML

[Q61] 移动平均
来源：http://baike.vehdjk.com/Article/details/gpzhbyacg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gryiijcfa.sHtML

[Q62] 分组占比
来源：http://www.share.epnwcf.com/Article/details/givcwxnyr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.sjlbkw.cn/Article/details/gmwnobijr.sHtML

[Q63] 开启事务
来源：http://blog.tarul.cn/Article/details/gklyrghml.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/gzochsifj.sHtML

[Q64] 提交事务
来源：http://mobile.vehdjk.com/Article/details/gybhypiqo.sHtML

COMMIT;
来源：http://read.share.bbcook.cn/Article/details/gbeqqzxfv.sHtML

[Q65] 回滚事务
来源：http://www.share.vehdjk.com/Article/details/gnurdwjmr.sHtML

ROLLBACK;
来源：http://www.blog.sjlbkw.cn/Article/details/gslalhxnu.sHtML

[Q66] 行锁查询
来源：http://wap.vehdjk.com/Article/details/gbyxlrpox.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/ghvqozgdb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.bbcook.cn/Article/details/gcthvjduh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.vehdjk.com/Article/details/gdzakakxp.sHtML

[Q68] 保存点
来源：http://m.share.yfazqb.com/Article/details/gwnsskekr.sHtML

SAVEPOINT sp1;
来源：http://wap.epnwcf.com/Article/details/gqjfjtpcq.sHtML


<!-- 参考信息 -->