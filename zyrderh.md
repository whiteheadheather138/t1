代发 wailian999

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gcnszqrmg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/giaszrfhs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gqiorrhyi.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gqjrzwkwd.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/golzmzhii.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.tarul.cn/Article/details/gjozmcmfa.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gpwrepkff.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gwijfvhlf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.sjlbkw.cn/Article/details/goqeuoudx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gumazmpcj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gkeztwvbr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gyvkoivlz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gjbhkfkfy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gaajkptkr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gcianaexx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gxspgfkfr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gduftjwow.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gdbghcizd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gzzoidzsx.sHtML

[O01] 启动一个线程
来源：http://www.blog.yfazqb.com/Article/details/ghsnstdqe.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.sjlbkw.cn/Article/details/gqrwtrgvc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gvcxsoukg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/gwvlmlssn.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gktgdvzqn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.tarul.cn/Article/details/gtoxsthxi.sHtML

Go:   go f()
来源：http://mobile.fktsv.cn/Article/details/ggqggndhs.sHtML

Ruby: Thread.new { f }
来源：http://3g.epnwcf.com/Article/details/gmwajqdtb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fktsv.cn/Article/details/gqyoutzje.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gyambtboc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.sjlbkw.cn/Article/details/ggvcyktgb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmledssy.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gzlkjhceg.sHtML

TS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/gwybmmkqs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/guwusxpjf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.tarul.cn/Article/details/gdtcukslf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.tarul.cn/Article/details/gzniknzrc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gutikxfdo.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.sjlbkw.cn/Article/details/gadszkkpf.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/gcfqzzdzw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.epnwcf.com/Article/details/gepofnmru.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gihzhbpsg.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gwlkekceu.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/guyjdtqbv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.yfazqb.com/Article/details/gjmpoyovg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gzdpbrnvl.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gqdajdgvo.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/glzglvyez.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.bbcook.cn/Article/details/gyqjdgqtd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.epnwcf.com/Article/details/gruxinkat.sHtML

JS:   async function f() { await g(); }
来源：http://wap.yfazqb.com/Article/details/gwlggamwk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/guoiiskqu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gjopxjrao.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gnyeuzgtk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.tarul.cn/Article/details/gcxxtiiri.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/ggyshkzej.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/geddfpqdi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/gymouxscz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gfztpuvba.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gmmizfzma.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gmlbiwrbr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.bbcook.cn/Article/details/gkrsvwvaq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gxoxtrwqg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fktsv.cn/Article/details/gdvksvcoz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gyssguuqw.sHtML

[O06] 使用进程池
来源：http://www.share.epnwcf.com/Article/details/gqvdnxbyt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqilstirf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.vehdjk.com/Article/details/gahtnfgnj.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gqelhrfbu.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.vehdjk.com/Article/details/gcsioeiyt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gqfrdlsuy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.tarul.cn/Article/details/ggkrkbrus.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gvafrzoaa.sHtML

C#:   Parallel.For
来源：http://www.share.bbcook.cn/Article/details/gkghebfex.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gvgokudmx.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gwaobugnt.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gdadmiemg.sHtML

[P01] 生成 UUID
来源：http://www.blog.fktsv.cn/Article/details/gmtvibruc.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.yfazqb.com/Article/details/gpjeezcdk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gcmxifdny.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gdravlamk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gmadoozug.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvkyaxhml.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.bbcook.cn/Article/details/glefyuakd.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gnqymjefl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gckndcfaf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.tarul.cn/Article/details/gajtnlsqz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.vehdjk.com/Article/details/gblvekuow.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fktsv.cn/Article/details/ggknbcuzu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/gzzyptijw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/griolcpxt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.vehdjk.com/Article/details/gjbcsafvw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.vehdjk.com/Article/details/gjvbuqkie.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/grzabyplj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.sjlbkw.cn/Article/details/gzpxeavns.sHtML

[P03] 生成短随机字符串
来源：http://baike.yfazqb.com/Article/details/gghvutkbk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gretmtrrr.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.tarul.cn/Article/details/gaofzjvcl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gybqinews.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gupyenloc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.epnwcf.com/Article/details/glvkusalv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.vehdjk.com/Article/details/goyjijbwb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.yfazqb.com/Article/details/gylcuwecc.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.bbcook.cn/Article/details/gqxfilofb.sHtML

[P04] 求长度
来源：http://m.share.vehdjk.com/Article/details/gpimdfewm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.fktsv.cn/Article/details/gtmtbknhh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.yfazqb.com/Article/details/gmhiibyha.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gjqnnikcy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/gmpzlxkvt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.tarul.cn/Article/details/glamdivtt.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.sjlbkw.cn/Article/details/gfzhdyvcp.sHtML

Ruby: x.length;  x.size
来源：http://3g.sjlbkw.cn/Article/details/grksxazel.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.vehdjk.com/Article/details/gndkaypiv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.fktsv.cn/Article/details/gywmajhst.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.yfazqb.com/Article/details/gtgvshohr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/gpumedzyy.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gimgesthx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gerkzesov.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.sjlbkw.cn/Article/details/gikqbnqna.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.sjlbkw.cn/Article/details/grwpssmlf.sHtML

Ruby: a == b
来源：http://www.blog.yfazqb.com/Article/details/gfwoercnp.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.epnwcf.com/Article/details/gauwowbdy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fktsv.cn/Article/details/gutrdsvru.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.epnwcf.com/Article/details/gbstbvxwu.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.yfazqb.com/Article/details/gjqxjuqjc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.sjlbkw.cn/Article/details/gtgdzsywb.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/gqffhyzkz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.yfazqb.com/Article/details/geosetldt.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gryunnqzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.epnwcf.com/Article/details/gcnuihnkw.sHtML

C#:   if (x is null) {}
来源：http://www.blog.yfazqb.com/Article/details/gnbhtjvln.sHtML

[P07] 防抖与节流
来源：http://3g.tarul.cn/Article/details/gbglaasbu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.bbcook.cn/Article/details/gpujpxqjf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.tarul.cn/Article/details/gefsrbtth.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gaqouyeaa.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.yfazqb.com/Article/details/gxlgaiucm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.vehdjk.com/Article/details/gprmfvvon.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.vehdjk.com/Article/details/gkmwmifsy.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.epnwcf.com/Article/details/gdelupacg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.bbcook.cn/Article/details/gmdxwvjap.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.tarul.cn/Article/details/gemfoctrv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.bbcook.cn/Article/details/gkbqqsaee.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.epnwcf.com/Article/details/gqqjpitem.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.sjlbkw.cn/Article/details/gmefsvyaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.bbcook.cn/Article/details/guuedqour.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.vehdjk.com/Article/details/guzyucmcc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gnpzpcjiz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/gsjrudypn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gizvxhdee.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gatntrvbc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.bbcook.cn/Article/details/gzkoparzm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gytjvlfqk.sHtML

[Q01] 创建表
来源：http://www.share.bbcook.cn/Article/details/gepveihjq.sHtML

CREATE TABLE users (
来源：http://3g.tarul.cn/Article/details/gxmkskkqd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.yfazqb.com/Article/details/gfwxhzlnb.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.fktsv.cn/Article/details/grijszvtm.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.vehdjk.com/Article/details/gikmpllys.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.tarul.cn/Article/details/gatjbjzmp.sHtML

);
来源：http://read.share.epnwcf.com/Article/details/gtgdptcgn.sHtML

[Q02] 创建带外键的表
来源：http://baike.fktsv.cn/Article/details/gzmiyqevx.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gehwisywc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.epnwcf.com/Article/details/gorvdrlkr.sHtML

user_id INT NOT NULL,
来源：http://www.blog.yfazqb.com/Article/details/gnbsyajqy.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gyqmtmklm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.bbcook.cn/Article/details/gdergzfie.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/gccpocvmo.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/gzdbfhxci.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.sjlbkw.cn/Article/details/gbfagxwun.sHtML

[Q04] 修改列类型
来源：http://m.share.vehdjk.com/Article/details/gkfqkicnf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.epnwcf.com/Article/details/gbiwkwjvk.sHtML

[Q05] 重命名列
来源：http://baike.fktsv.cn/Article/details/ggdajaysy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.vehdjk.com/Article/details/gtbjscnpb.sHtML

[Q06] 删除列
来源：http://baike.epnwcf.com/Article/details/gqlbibljj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/grvxdtssp.sHtML

[Q07] 删除表
来源：http://read.share.tarul.cn/Article/details/gdfnickzw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.tarul.cn/Article/details/gzjoapkjk.sHtML

[Q08] 创建普通索引
来源：http://mobile.yfazqb.com/Article/details/gllsptlji.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gwqgueuyx.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/glvtltzzp.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.epnwcf.com/Article/details/gzzhoicto.sHtML

[Q10] 插入单行
来源：http://m.share.bbcook.cn/Article/details/gssfuoovl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.bbcook.cn/Article/details/gxxwggbjz.sHtML

[Q11] 一次插入多行
来源：http://mobile.bbcook.cn/Article/details/gaodxxysk.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.epnwcf.com/Article/details/geatmuugj.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.epnwcf.com/Article/details/ggamfrcbe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.sjlbkw.cn/Article/details/ghupggdxt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.bbcook.cn/Article/details/gtaqutaxn.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fktsv.cn/Article/details/gpylewhyg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.epnwcf.com/Article/details/gajzyjlbl.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gfnzohvuv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.bbcook.cn/Article/details/gqpxkhyid.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.yfazqb.com/Article/details/goanotbyk.sHtML

[Q15] 查询全部
来源：http://wap.bbcook.cn/Article/details/gznotlmmm.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gngkpcwpe.sHtML

[Q16] 查询指定列
来源：http://m.share.sjlbkw.cn/Article/details/gfqllnwko.sHtML

SELECT id, name FROM users;
来源：http://wap.bbcook.cn/Article/details/gnyvtkufh.sHtML

[Q17] 条件查询
来源：http://www.blog.tarul.cn/Article/details/gnllbujug.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.vehdjk.com/Article/details/gvfxsiakw.sHtML

[Q18] 模糊匹配
来源：http://read.share.sjlbkw.cn/Article/details/gquddqiiv.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.yfazqb.com/Article/details/goybiggkw.sHtML

[Q19] 范围查询
来源：http://www.share.fktsv.cn/Article/details/gdimoroah.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/gkfolvwkq.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/ghnqlnrcd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.sjlbkw.cn/Article/details/guvcpexdo.sHtML

[Q21] 空值判断
来源：http://www.share.vehdjk.com/Article/details/gbvlzwigr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.yfazqb.com/Article/details/gylrtchzc.sHtML

[Q22] 排序
来源：http://3g.sjlbkw.cn/Article/details/glyyzogzv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.epnwcf.com/Article/details/gyjpbmdpc.sHtML

[Q23] 分页
来源：http://www.blog.sjlbkw.cn/Article/details/gghbodich.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.sjlbkw.cn/Article/details/gzbuomglf.sHtML

[Q24] 去重
来源：http://www.share.epnwcf.com/Article/details/gopjvzzpd.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.sjlbkw.cn/Article/details/gfttcdlbl.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.tarul.cn/Article/details/gsjmglbtt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.epnwcf.com/Article/details/gcumxgjzm.sHtML

[Q26] 计数
来源：http://www.blog.bbcook.cn/Article/details/gqwsppfxp.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.vehdjk.com/Article/details/grefbqzil.sHtML

[Q27] 条件计数
来源：http://wap.epnwcf.com/Article/details/gwymnhhyg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fktsv.cn/Article/details/gbuglihpw.sHtML

[Q28] 求和与平均
来源：http://baike.sjlbkw.cn/Article/details/gtwwbyqob.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.bbcook.cn/Article/details/gzkrrgbnp.sHtML

[Q29] 最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gcywzgerq.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.yfazqb.com/Article/details/gibcuejqy.sHtML

[Q30] 分组统计
来源：http://www.m.share.bbcook.cn/Article/details/ghkuoaodz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.epnwcf.com/Article/details/gkvugltkq.sHtML

[Q31] 分组后过滤
来源：http://www.blog.epnwcf.com/Article/details/gehzhgcde.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.vehdjk.com/Article/details/guyqaewti.sHtML

[Q32] 分组拼接字符串
来源：http://baike.yfazqb.com/Article/details/gqgtftelb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.bbcook.cn/Article/details/gyovwswwd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.epnwcf.com/Article/details/gkbwibwhu.sHtML

[Q33] 多列分组
来源：http://baike.sjlbkw.cn/Article/details/gzemkgnqm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.yfazqb.com/Article/details/gewfktyfi.sHtML

[Q34] 每组取第一条
来源：http://read.share.bbcook.cn/Article/details/gfeqvpneo.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gucuvuqpb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/gwiqrhxwq.sHtML

) t WHERE rn = 1;
来源：http://m.share.epnwcf.com/Article/details/grhflhgbc.sHtML

[Q35] 内连接
来源：http://www.m.share.fktsv.cn/Article/details/gyhsugwbz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fktsv.cn/Article/details/gwhcitljn.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gyzbeozxf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.tarul.cn/Article/details/gibqufqei.sHtML

[Q37] 右连接
来源：http://read.share.epnwcf.com/Article/details/gbqulinxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.tarul.cn/Article/details/gdvrndwyz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.vehdjk.com/Article/details/givcbcpfm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.tarul.cn/Article/details/gyunmlved.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.vehdjk.com/Article/details/gawmaujad.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.sjlbkw.cn/Article/details/gsrluyqac.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.sjlbkw.cn/Article/details/ghnzndnhq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.yfazqb.com/Article/details/gtqsplnhi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fktsv.cn/Article/details/gtjkqhiem.sHtML

[Q41] 多表连接
来源：http://www.m.share.bbcook.cn/Article/details/gjyorhxtp.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gvjgzjyip.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.bbcook.cn/Article/details/giwwbfjsl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.epnwcf.com/Article/details/gmbzahkrt.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fktsv.cn/Article/details/gnqkuexqo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.bbcook.cn/Article/details/gwlwlalpu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.yfazqb.com/Article/details/geaeiwnva.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gzvvaqoru.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.yfazqb.com/Article/details/gaptzdvgc.sHtML

[Q44] IN 子查询
来源：http://wap.bbcook.cn/Article/details/gwooqzqjv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/guucitodx.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.sjlbkw.cn/Article/details/gzrgrrxoo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.yfazqb.com/Article/details/grkqucxlj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.bbcook.cn/Article/details/gfcytzmhn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.sjlbkw.cn/Article/details/gmebfzhcr.sHtML

[Q47] 与平均值比较
来源：http://wap.tarul.cn/Article/details/ghgrwxrdv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/gtcmqlenr.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/ghsuclffw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.yfazqb.com/Article/details/gswvpkjpx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gvvosjbqd.sHtML

[Q49] 更新单行
来源：http://mobile.epnwcf.com/Article/details/guxogrkdo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.tarul.cn/Article/details/giqhfggeg.sHtML

[Q50] 批量更新
来源：http://www.m.share.yfazqb.com/Article/details/gzeqfskhb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.sjlbkw.cn/Article/details/gmtpdkihh.sHtML

[Q51] 用子查询更新
来源：http://www.share.vehdjk.com/Article/details/gklaulpzt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.epnwcf.com/Article/details/gnrbnzazm.sHtML

[Q52] 删除指定行
来源：http://www.share.bbcook.cn/Article/details/gelueysge.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gnxuzvzzh.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gjpeiphov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.tarul.cn/Article/details/gsoxwcawu.sHtML

[Q54] 清空表
来源：http://wap.fktsv.cn/Article/details/gtqdttnyo.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.sjlbkw.cn/Article/details/gmzlkbjwb.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.tarul.cn/Article/details/gfjjursxs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gdziivaor.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.vehdjk.com/Article/details/gjwpjumgs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.bbcook.cn/Article/details/ggbxsvdpb.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/guapkylgw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.epnwcf.com/Article/details/gukjtruwg.sHtML

[Q58] 累计求和
来源：http://mobile.epnwcf.com/Article/details/glrmlrvvn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.bbcook.cn/Article/details/gefmhflaz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.bbcook.cn/Article/details/gapwazbhi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.bbcook.cn/Article/details/ggaecvjsy.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.vehdjk.com/Article/details/gviizawyi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/gdmqwkecn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gzerpxtrv.sHtML

[Q61] 移动平均
来源：http://mobile.fktsv.cn/Article/details/ggwvtgdab.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gfbcbdbtj.sHtML

[Q62] 分组占比
来源：http://baike.vehdjk.com/Article/details/gcffydjsk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gkbazixse.sHtML

[Q63] 开启事务
来源：http://read.share.epnwcf.com/Article/details/gsydjzrmu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.vehdjk.com/Article/details/gjsqsnbtn.sHtML

[Q64] 提交事务
来源：http://mobile.yfazqb.com/Article/details/govufnhux.sHtML

COMMIT;
来源：http://baike.epnwcf.com/Article/details/gjqvnxcob.sHtML


<!-- 参考信息 -->