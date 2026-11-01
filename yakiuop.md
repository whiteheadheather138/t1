代发 wailian999

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gjmfwircz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/glicqoibx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gevxtcfbj.sHtML

Java: // 手写递归
来源：http://blog.fktsv.cn/Article/details/gppaeyron.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gunrmeuvn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gzdisblrt.sHtML

C#:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/gbpkzxtds.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gdhkvavzt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/gjlnymkip.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/guwjrpybf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gcejnogvy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gxuppikww.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gbwzsbsnv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gkxarscpn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/gidygajoq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/gyvnmbzdb.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gtghpxahh.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gxrozshvr.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/giasnxdfv.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gvkhgsnoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.tarul.cn/Article/details/gjhdfcxmn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.epnwcf.com/Article/details/gijotecoi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/givkgsuxb.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gjbtsyzpt.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/gjvvvdzqj.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/ghxagymud.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fktsv.cn/Article/details/gqwzdzdav.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/gylcxtcyq.sHtML

[O02] 使用线程池
来源：http://baike.bbcook.cn/Article/details/ggcregndi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gtnlfsiio.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.sjlbkw.cn/Article/details/gdsnqoucy.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gyejthxmc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/glbuomxmm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gjxybrplv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.yfazqb.com/Article/details/gzcmchnua.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.bbcook.cn/Article/details/gvaoryirh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.tarul.cn/Article/details/gckrkkcdv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.bbcook.cn/Article/details/gzalhskep.sHtML

Py:   with lock: shared += 1
来源：http://3g.sjlbkw.cn/Article/details/gzmjcbjnh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gkkytrgla.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/gebeevixa.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gcmwmswvf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gtalzlhus.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gqxagndvn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.bbcook.cn/Article/details/gmbzljufb.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gezeibzga.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.yfazqb.com/Article/details/gdgucdhwz.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.tarul.cn/Article/details/gyolnmrpm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.bbcook.cn/Article/details/gscfxhqgd.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gxrblxqua.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.bbcook.cn/Article/details/gpvirwqlz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.vehdjk.com/Article/details/gujuydzrv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.tarul.cn/Article/details/gjjztxtju.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.yfazqb.com/Article/details/gxsqpwueu.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.epnwcf.com/Article/details/ggwwgdtyi.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gqqztweon.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.vehdjk.com/Article/details/glqmwbzxl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fktsv.cn/Article/details/gadvssfgs.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/gkhestqjr.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gpmtognjb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.sjlbkw.cn/Article/details/grasxnlkd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsbfplbni.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gsjkhxkhc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.tarul.cn/Article/details/gtevsascm.sHtML

[O06] 使用进程池
来源：http://blog.tarul.cn/Article/details/gubpokazr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gqahxzmnc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.bbcook.cn/Article/details/gmlkjsfci.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gysxwkkye.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gydzxcgfo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.sjlbkw.cn/Article/details/gjyrxqkcj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/gljapproq.sHtML

Ruby: // fork 块
来源：http://www.m.share.epnwcf.com/Article/details/gyspkivim.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/glvouxyfw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gosejsoqs.sHtML

P. 常用工具函数
来源：http://m.share.tarul.cn/Article/details/gzulzuhmj.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gekazxzig.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gqmnxuvam.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.tarul.cn/Article/details/gibmcllpn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.sjlbkw.cn/Article/details/gylkjbpbo.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gqlofzden.sHtML

TS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/grdwaotzq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwfdbcbw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.tarul.cn/Article/details/gdsejyyae.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gpsbyovks.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.vehdjk.com/Article/details/gppuwxbcq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.sjlbkw.cn/Article/details/ggmzuqgjn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.vehdjk.com/Article/details/gipriqklg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.vehdjk.com/Article/details/guydaqyrx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fktsv.cn/Article/details/gxlgifcyo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.bbcook.cn/Article/details/gjhgrclrk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/goowayvpm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.tarul.cn/Article/details/gbtdspnfg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.yfazqb.com/Article/details/glnkjembt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/gzitkaele.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/glngesrcl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyjjgzuyx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.tarul.cn/Article/details/gfppcenfm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.yfazqb.com/Article/details/guloynyvo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/gddkdpuat.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gdsikeyuk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.vehdjk.com/Article/details/gncfazjbj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/gqetfgzgk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.epnwcf.com/Article/details/gvkzxzepo.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/gmtpsfqou.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.vehdjk.com/Article/details/gemkyoryt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gbvabtisa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gxyclyvfd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/gpbjfzonu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwtmyopim.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.sjlbkw.cn/Article/details/ginxnmiod.sHtML

Ruby: x.length;  x.size
来源：http://baike.fktsv.cn/Article/details/gqxauyuoc.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gaqkkhxry.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gizmvvjja.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fktsv.cn/Article/details/gdogpcgtg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.sjlbkw.cn/Article/details/gtirukgvj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.fktsv.cn/Article/details/gxehwiayr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gqywqcjbs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.epnwcf.com/Article/details/geyjeqcex.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.epnwcf.com/Article/details/gdzxuplvx.sHtML

Ruby: a == b
来源：http://m.share.fktsv.cn/Article/details/gnuambgkf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gkyvhmnxy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gvporvniz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.bbcook.cn/Article/details/gcvngvtbx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.sjlbkw.cn/Article/details/gmowcttcb.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/gdwszopdz.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/gmuannqee.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/gubqhefmo.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gqqhkeuix.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fktsv.cn/Article/details/gehbcitec.sHtML

C#:   if (x is null) {}
来源：http://3g.vehdjk.com/Article/details/gxzvrbsbp.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gzwxadtkq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.bbcook.cn/Article/details/gxikgchkr.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.vehdjk.com/Article/details/glhldegbm.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/glvgthjpk.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.epnwcf.com/Article/details/gukhhdnha.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.bbcook.cn/Article/details/gpfsdctgl.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.yfazqb.com/Article/details/gjzswnrjc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.epnwcf.com/Article/details/grkaqzaee.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.vehdjk.com/Article/details/gzaqveaio.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/gsacwdwwu.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.vehdjk.com/Article/details/glfsyrhre.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.tarul.cn/Article/details/gettdpsjt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.yfazqb.com/Article/details/givljzlxr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.yfazqb.com/Article/details/gtqblkefc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.vehdjk.com/Article/details/giweovzry.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.yfazqb.com/Article/details/grfnqxxco.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.bbcook.cn/Article/details/grvemjyxy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.sjlbkw.cn/Article/details/gockkdzrn.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gojxthabi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.vehdjk.com/Article/details/gueitmazw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqrrifyof.sHtML

[Q01] 创建表
来源：http://3g.vehdjk.com/Article/details/glaoyfvjq.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/gopvrrvot.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.yfazqb.com/Article/details/guwzelbhd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.bbcook.cn/Article/details/grurqekoy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.epnwcf.com/Article/details/gltzamezv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/giqzdbkal.sHtML

);
来源：http://mobile.vehdjk.com/Article/details/gkoiasaol.sHtML

[Q02] 创建带外键的表
来源：http://www.share.sjlbkw.cn/Article/details/gopschpqk.sHtML

CREATE TABLE orders (
来源：http://blog.fktsv.cn/Article/details/giypgyezi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.epnwcf.com/Article/details/gqetttqpi.sHtML

user_id INT NOT NULL,
来源：http://3g.yfazqb.com/Article/details/glrrxqqkn.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fktsv.cn/Article/details/gaqquanlg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.sjlbkw.cn/Article/details/gcqsrckwv.sHtML

);
来源：http://mobile.yfazqb.com/Article/details/gtrhjmjud.sHtML

[Q03] 增加列
来源：http://www.m.share.bbcook.cn/Article/details/gzrsthngh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/giuiwgfzr.sHtML

[Q04] 修改列类型
来源：http://3g.fktsv.cn/Article/details/gkhihfybm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wap.yfazqb.com/Article/details/gvixuogoc.sHtML

[Q05] 重命名列
来源：http://www.share.vehdjk.com/Article/details/grhitgqet.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gxslhgije.sHtML

[Q06] 删除列
来源：http://www.share.fktsv.cn/Article/details/gfbdzpcho.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.epnwcf.com/Article/details/gxjzjsknc.sHtML

[Q07] 删除表
来源：http://blog.yfazqb.com/Article/details/gsaetotzi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/gqucrhpwu.sHtML

[Q08] 创建普通索引
来源：http://3g.yfazqb.com/Article/details/gvxhvpckj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.sjlbkw.cn/Article/details/gyodaouxs.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.sjlbkw.cn/Article/details/gatlfepnq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fktsv.cn/Article/details/gnmplkjcy.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gccbtqwhj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.yfazqb.com/Article/details/gwyerxgtx.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/gwjzymzdc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gwvuoctei.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gavvzyhpc.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.yfazqb.com/Article/details/gxyahitqy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.vehdjk.com/Article/details/gkylfksuz.sHtML

[Q13] 忽略重复插入
来源：http://wap.yfazqb.com/Article/details/ghoxtdvvw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.bbcook.cn/Article/details/gzbilqfxj.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.sjlbkw.cn/Article/details/grkecabdf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.sjlbkw.cn/Article/details/girhyfkro.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.epnwcf.com/Article/details/glrzfxlmg.sHtML

[Q15] 查询全部
来源：http://read.share.vehdjk.com/Article/details/gcdkgudes.sHtML

SELECT * FROM users;
来源：http://baike.fktsv.cn/Article/details/gbcmmkiqo.sHtML

[Q16] 查询指定列
来源：http://mobile.vehdjk.com/Article/details/gkmojmgpr.sHtML

SELECT id, name FROM users;
来源：http://m.share.bbcook.cn/Article/details/gieiptztu.sHtML

[Q17] 条件查询
来源：http://mobile.tarul.cn/Article/details/gubneymoo.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.bbcook.cn/Article/details/ggipvnnvz.sHtML

[Q18] 模糊匹配
来源：http://www.share.yfazqb.com/Article/details/gqbmxwhka.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.sjlbkw.cn/Article/details/gfxtwsfww.sHtML

[Q19] 范围查询
来源：http://blog.tarul.cn/Article/details/gvrrubnjk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gcqdhkqdu.sHtML

[Q20] IN 列表
来源：http://baike.epnwcf.com/Article/details/goirkarom.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.sjlbkw.cn/Article/details/gqjedcypq.sHtML

[Q21] 空值判断
来源：http://www.m.share.tarul.cn/Article/details/gjiucetyl.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.yfazqb.com/Article/details/glmjkgkwc.sHtML

[Q22] 排序
来源：http://wap.fktsv.cn/Article/details/geqbkbazm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.vehdjk.com/Article/details/gfhlyotay.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gyyqwkuzm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.epnwcf.com/Article/details/goqryllgv.sHtML

[Q24] 去重
来源：http://baike.yfazqb.com/Article/details/gnbonamit.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fktsv.cn/Article/details/gxjmfdbhw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.vehdjk.com/Article/details/gsqnfrfon.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.sjlbkw.cn/Article/details/gtgnejgrg.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gfmcpuhzf.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwfgvyffj.sHtML

[Q27] 条件计数
来源：http://mobile.sjlbkw.cn/Article/details/gxgveetet.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fktsv.cn/Article/details/gjkvztjuf.sHtML

[Q28] 求和与平均
来源：http://m.share.epnwcf.com/Article/details/gwybsddrp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.vehdjk.com/Article/details/gfjipfwon.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gunwwndhh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/galdcngee.sHtML

[Q30] 分组统计
来源：http://read.share.vehdjk.com/Article/details/gnmqrwmcp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/gvsidtydk.sHtML

[Q31] 分组后过滤
来源：http://baike.fktsv.cn/Article/details/gticstyhb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.bbcook.cn/Article/details/gzistoqag.sHtML

[Q32] 分组拼接字符串
来源：http://baike.epnwcf.com/Article/details/gwbdohbcu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.vehdjk.com/Article/details/gvashdtos.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.bbcook.cn/Article/details/ggqxrwfel.sHtML

[Q33] 多列分组
来源：http://wap.fktsv.cn/Article/details/gqeqddsmb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.vehdjk.com/Article/details/gweltgjqs.sHtML

[Q34] 每组取第一条
来源：http://3g.tarul.cn/Article/details/gajkfaziz.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gndbgqryh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.sjlbkw.cn/Article/details/gsfdwdnxv.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.epnwcf.com/Article/details/gzfcgnxfx.sHtML

[Q35] 内连接
来源：http://www.m.share.yfazqb.com/Article/details/goscyantd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gwfbrkwdk.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/ghumxcqym.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.tarul.cn/Article/details/gouvtzzpy.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gmbserqyh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.yfazqb.com/Article/details/gafupoweq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.sjlbkw.cn/Article/details/gtseqvjhq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.epnwcf.com/Article/details/gunufhrna.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.sjlbkw.cn/Article/details/ggyzdcdtq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.sjlbkw.cn/Article/details/gnimvnqna.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fktsv.cn/Article/details/gzolksjie.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.tarul.cn/Article/details/gnddctgsh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/gzjmvgwtq.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/ghxxcguhs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.sjlbkw.cn/Article/details/gewxjlaof.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/ghbzioynp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gvlglsqhi.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.epnwcf.com/Article/details/gdgewbjyr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.sjlbkw.cn/Article/details/gsqayqsjk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.bbcook.cn/Article/details/gnrzkqjfo.sHtML

[Q43] 标量子查询
来源：http://blog.epnwcf.com/Article/details/ggjxhctgp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gwhrvuvng.sHtML

[Q44] IN 子查询
来源：http://www.blog.epnwcf.com/Article/details/gclincjaq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.epnwcf.com/Article/details/gegczeuaq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gcueonosp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gxxtfbcis.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.epnwcf.com/Article/details/gszyrfzjk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gtzdkdyhj.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/ghwdizrtk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.bbcook.cn/Article/details/gdnblzpjk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gysqikpjy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.tarul.cn/Article/details/gfkgqygqx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.epnwcf.com/Article/details/gbvszkvmy.sHtML

[Q49] 更新单行
来源：http://baike.sjlbkw.cn/Article/details/ggljdwmgk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.bbcook.cn/Article/details/gkhasoevy.sHtML

[Q50] 批量更新
来源：http://www.blog.yfazqb.com/Article/details/gywjwvpma.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.yfazqb.com/Article/details/gxhljlsue.sHtML

[Q51] 用子查询更新
来源：http://baike.epnwcf.com/Article/details/goulkuzyc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.yfazqb.com/Article/details/gxwtdaojc.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/gvrnwmqxt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fktsv.cn/Article/details/gfjbokcbo.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gpmigkrap.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.sjlbkw.cn/Article/details/gkdkepkck.sHtML

[Q54] 清空表
来源：http://m.share.tarul.cn/Article/details/gcsvycvzh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gqyobwsww.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fktsv.cn/Article/details/gzzyrznvx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/gosjwsfmq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/gmaggkbon.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fktsv.cn/Article/details/gqjldqcfb.sHtML

[Q57] 行号
来源：http://www.share.fktsv.cn/Article/details/gsbkfmwks.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/gvjtxygta.sHtML

[Q58] 累计求和
来源：http://read.share.yfazqb.com/Article/details/gbyaxhzhr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/glrquuhkz.sHtML

[Q59] 分组内累计
来源：http://www.blog.yfazqb.com/Article/details/gzrnczqle.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.bbcook.cn/Article/details/gcjlafwgc.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.tarul.cn/Article/details/gjgvjepjq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.vehdjk.com/Article/details/gaohpwtkt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gsvxrfngc.sHtML

[Q61] 移动平均
来源：http://wap.epnwcf.com/Article/details/gsgcvfsec.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gkxggakef.sHtML

[Q62] 分组占比
来源：http://m.share.epnwcf.com/Article/details/gmgnmfclj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.tarul.cn/Article/details/gqeseltjf.sHtML

[Q63] 开启事务
来源：http://wap.sjlbkw.cn/Article/details/gfaonelrp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.bbcook.cn/Article/details/gnjrdahlh.sHtML

[Q64] 提交事务
来源：http://3g.tarul.cn/Article/details/gtqfobvbj.sHtML

COMMIT;
来源：http://mobile.epnwcf.com/Article/details/gbqjrlzyy.sHtML


<!-- 参考信息 -->