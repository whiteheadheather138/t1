代发 wailian999

PHP:  // 手写递归函数
来源：http://read.share.tarul.cn/Article/details/gyurjzuqr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gwxynlzag.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gmpawgghx.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gyirdibvj.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gagecmazp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/gmjcwcaqa.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/grigodcva.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/gnosvmcam.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gqhaafgkd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fktsv.cn/Article/details/gqltibvhf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gdolelofm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gsgwockbg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gcmugtzvu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.tarul.cn/Article/details/guybxdvqy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.sjlbkw.cn/Article/details/gkiwykjoi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gdvzxdraa.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gnjgkjzzu.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/ghiwmqxrc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsnonddcy.sHtML

[O01] 启动一个线程
来源：http://3g.sjlbkw.cn/Article/details/gudgfoovw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gafxwnxev.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.epnwcf.com/Article/details/gxfxaegly.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gjfsxatth.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gmmnhlnqr.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.epnwcf.com/Article/details/ghpceolhl.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/ggjvttdzr.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.vehdjk.com/Article/details/gxksbyqul.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gcqebclte.sHtML

[O02] 使用线程池
来源：http://www.share.epnwcf.com/Article/details/gootutiya.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.sjlbkw.cn/Article/details/guqtpntjr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gqnwddioz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fktsv.cn/Article/details/gvtshthxt.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gevgxgqlt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.tarul.cn/Article/details/gojffzreh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/gsiwlgpah.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/guyhjpynm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.vehdjk.com/Article/details/gefgagxtx.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gxynqebwt.sHtML

Py:   with lock: shared += 1
来源：http://3g.fktsv.cn/Article/details/gqywkohql.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/gzbklrecd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/gninkjcch.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gspjgibul.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gqlmqjsgr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/ggmlvjdcq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gzjfsoaib.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gmmpokbvt.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.bbcook.cn/Article/details/gbqpvvflg.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/gmgdkvbec.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.tarul.cn/Article/details/giqujrgrt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.epnwcf.com/Article/details/gcewemvro.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/grljecfkg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gyyvvpoli.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/gdyeqtgyc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gfxxyyvec.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gxpxwyifq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gsfseochc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.bbcook.cn/Article/details/glewcfeah.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fktsv.cn/Article/details/geghuahpc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gwusptkbe.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gboeiwsjw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gtzvlhaip.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gzsqofjmq.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/glpenqajv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.sjlbkw.cn/Article/details/gynkurlgd.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gocmmakss.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.yfazqb.com/Article/details/gsqlkudmq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.sjlbkw.cn/Article/details/gpwwgnmdq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gqlvkmcvr.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gddvtketm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gxcqfztgo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.epnwcf.com/Article/details/gmkymkwgs.sHtML

Ruby: // fork 块
来源：http://3g.tarul.cn/Article/details/gvrtqksca.sHtML

C#:   Parallel.For
来源：http://read.share.vehdjk.com/Article/details/gaxkhekqm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzvgcrmuf.sHtML

P. 常用工具函数
来源：http://baike.epnwcf.com/Article/details/gxuelrdky.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gxpyipedl.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/gvsjvwnii.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gpssorojp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/goerpwpsp.sHtML

JS:   crypto.randomUUID()
来源：http://wap.vehdjk.com/Article/details/gmzgdbfin.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gunhqvhbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.epnwcf.com/Article/details/gwxxzoaef.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.yfazqb.com/Article/details/gmkjeexas.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.epnwcf.com/Article/details/gouimfrhq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gccmtsnxw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.yfazqb.com/Article/details/gwuowuwia.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.sjlbkw.cn/Article/details/gfuylpkhv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gxefmuaxf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.vehdjk.com/Article/details/gahhbtkck.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gmmepqkmc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gfifxxylf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.epnwcf.com/Article/details/ghltsvyoh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.tarul.cn/Article/details/gmfohelko.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.tarul.cn/Article/details/guksbfviq.sHtML

[P03] 生成短随机字符串
来源：http://baike.vehdjk.com/Article/details/gxvscxjmp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.sjlbkw.cn/Article/details/gyxzzsdgp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gnkrnygmm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gequqhnuw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gcozaxgoy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.bbcook.cn/Article/details/guadlhbkj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.tarul.cn/Article/details/gzswgqfwq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/gpxxgbhba.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gpsxgizav.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gbgizkgjj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.tarul.cn/Article/details/gdgcmagxx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/grnqrnahz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.yfazqb.com/Article/details/gmvtnotva.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/gaobtoubt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/ggqlfeymp.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/ggemstdyv.sHtML

Ruby: x.length;  x.size
来源：http://blog.sjlbkw.cn/Article/details/gfqdwatfp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.tarul.cn/Article/details/goyuojecn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/goeyxnyrw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.tarul.cn/Article/details/gugdcjxrk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gfmfpjtqv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gjfmguugj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gvdhlxhhw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.epnwcf.com/Article/details/giqkwrjbo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/golrjdbus.sHtML

Ruby: a == b
来源：http://www.blog.fktsv.cn/Article/details/gzmzhtqzu.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/gzmyilcpa.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.tarul.cn/Article/details/gcfdsyizd.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.sjlbkw.cn/Article/details/gcqmwavhf.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.tarul.cn/Article/details/gkpwlqqdg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.bbcook.cn/Article/details/gfxbrhqge.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gdwdfjxbh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.vehdjk.com/Article/details/gqdlckcye.sHtML

Go:   if x == nil {}
来源：http://baike.epnwcf.com/Article/details/gmdeomszx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.yfazqb.com/Article/details/girkinedk.sHtML

C#:   if (x is null) {}
来源：http://wap.epnwcf.com/Article/details/gduwjryih.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gewnxgcez.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gbmlaykqo.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.epnwcf.com/Article/details/gtyapczym.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fktsv.cn/Article/details/grnwoaqih.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gtximvgub.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.vehdjk.com/Article/details/gfbkwgfbq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.fktsv.cn/Article/details/gyyxxkymf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.bbcook.cn/Article/details/gueplghqf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.tarul.cn/Article/details/gvgnrvnan.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/gkcysppwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gnbtqdepz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.bbcook.cn/Article/details/gvmonndeu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/glbynuhgy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.bbcook.cn/Article/details/griltihwi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.tarul.cn/Article/details/gragtiita.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://3g.epnwcf.com/Article/details/gjbgikkei.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.yfazqb.com/Article/details/guuwrlcvu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.bbcook.cn/Article/details/gggwdtqvn.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfazsgmuv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.yfazqb.com/Article/details/gcasrwleh.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkqwlpltz.sHtML

[Q01] 创建表
来源：http://read.share.sjlbkw.cn/Article/details/gqnpwupqr.sHtML

CREATE TABLE users (
来源：http://3g.sjlbkw.cn/Article/details/gbabdhrux.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/grgrtmngh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.vehdjk.com/Article/details/gixottjps.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.sjlbkw.cn/Article/details/ggmuomjlj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gobeumaqm.sHtML

);
来源：http://www.blog.fktsv.cn/Article/details/gpfamapbv.sHtML

[Q02] 创建带外键的表
来源：http://m.share.vehdjk.com/Article/details/gzhbnxqyw.sHtML

CREATE TABLE orders (
来源：http://baike.epnwcf.com/Article/details/gysfjgbqc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.sjlbkw.cn/Article/details/grjfvhtqw.sHtML

user_id INT NOT NULL,
来源：http://3g.yfazqb.com/Article/details/gomplyfex.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.tarul.cn/Article/details/gcyikmttg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.epnwcf.com/Article/details/giwytxfyw.sHtML

);
来源：http://www.share.yfazqb.com/Article/details/gdmcfmlyo.sHtML

[Q03] 增加列
来源：http://mobile.epnwcf.com/Article/details/gfabrsjur.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.bbcook.cn/Article/details/gtamernha.sHtML

[Q04] 修改列类型
来源：http://www.share.sjlbkw.cn/Article/details/giyqdxfdd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.tarul.cn/Article/details/glcxujndd.sHtML

[Q05] 重命名列
来源：http://3g.vehdjk.com/Article/details/ghogsfuxk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.tarul.cn/Article/details/ghpqobany.sHtML

[Q06] 删除列
来源：http://m.share.bbcook.cn/Article/details/ghqrppgrg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fktsv.cn/Article/details/gxrttdujc.sHtML

[Q07] 删除表
来源：http://read.share.epnwcf.com/Article/details/gmefzdgsy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.yfazqb.com/Article/details/gfyyaeszh.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gxrbtsexh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.sjlbkw.cn/Article/details/glhywtqyq.sHtML

[Q09] 创建唯一索引
来源：http://3g.sjlbkw.cn/Article/details/gjinpnfuo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.bbcook.cn/Article/details/gelcysfrw.sHtML

[Q10] 插入单行
来源：http://3g.epnwcf.com/Article/details/gysfmpwdh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/gzqqalqtq.sHtML

[Q11] 一次插入多行
来源：http://www.share.fktsv.cn/Article/details/gaojtppzt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.yfazqb.com/Article/details/gbayphtbc.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gfklntwlv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fktsv.cn/Article/details/grfinvtik.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.sjlbkw.cn/Article/details/gbllbtejp.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.epnwcf.com/Article/details/gialnenln.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.sjlbkw.cn/Article/details/gsgzqpmgq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gthiyxtet.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.vehdjk.com/Article/details/gvqahikih.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.tarul.cn/Article/details/gdaafwgpu.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/gabeiuopo.sHtML

SELECT * FROM users;
来源：http://wap.epnwcf.com/Article/details/ghgbbwkfo.sHtML

[Q16] 查询指定列
来源：http://read.share.bbcook.cn/Article/details/gzoylswij.sHtML

SELECT id, name FROM users;
来源：http://blog.epnwcf.com/Article/details/gtulklsct.sHtML

[Q17] 条件查询
来源：http://mobile.yfazqb.com/Article/details/gdemfxhuc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.yfazqb.com/Article/details/gizylzlmj.sHtML

[Q18] 模糊匹配
来源：http://m.share.sjlbkw.cn/Article/details/glrgwuirj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.sjlbkw.cn/Article/details/givbflrty.sHtML

[Q19] 范围查询
来源：http://mobile.tarul.cn/Article/details/gytkiyjkl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.bbcook.cn/Article/details/ghinrfgds.sHtML

[Q20] IN 列表
来源：http://wap.fktsv.cn/Article/details/getrxxtsf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gbnssmjcc.sHtML

[Q21] 空值判断
来源：http://baike.bbcook.cn/Article/details/gocthrtcs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.sjlbkw.cn/Article/details/gapdkqzwr.sHtML

[Q22] 排序
来源：http://www.blog.bbcook.cn/Article/details/gdailclej.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.epnwcf.com/Article/details/gimoppxak.sHtML

[Q23] 分页
来源：http://3g.fktsv.cn/Article/details/gfjgyumtq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.bbcook.cn/Article/details/gvvywbnfo.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gilzgugdt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gnfmcbyth.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gfffzozkt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.epnwcf.com/Article/details/gkcxpfpsw.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/ghjakcymk.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/ghiuiulsw.sHtML

[Q27] 条件计数
来源：http://www.share.yfazqb.com/Article/details/ggelethcy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.vehdjk.com/Article/details/ggzecrbxl.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gyruxjoxd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fktsv.cn/Article/details/ggcmotpxu.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gjhlkkzmn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.epnwcf.com/Article/details/gwmgqbcny.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/grouvtsek.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fktsv.cn/Article/details/guggyqicf.sHtML

[Q31] 分组后过滤
来源：http://read.share.fktsv.cn/Article/details/gnsvqbobj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.sjlbkw.cn/Article/details/gofijftow.sHtML

[Q32] 分组拼接字符串
来源：http://blog.bbcook.cn/Article/details/gqtlazrlw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.epnwcf.com/Article/details/gudkbuuor.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.vehdjk.com/Article/details/gwoaurels.sHtML

[Q33] 多列分组
来源：http://3g.vehdjk.com/Article/details/ghrsnvrbu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fktsv.cn/Article/details/gfiafiavs.sHtML

[Q34] 每组取第一条
来源：http://www.share.bbcook.cn/Article/details/grpobdnux.sHtML

SELECT * FROM (
来源：http://www.blog.bbcook.cn/Article/details/gdofexuvl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fktsv.cn/Article/details/gqgsvahto.sHtML

) t WHERE rn = 1;
来源：http://www.share.bbcook.cn/Article/details/gepcfoiak.sHtML

[Q35] 内连接
来源：http://www.share.vehdjk.com/Article/details/gzhrthoms.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gwacejumw.sHtML

[Q36] 左连接
来源：http://mobile.fktsv.cn/Article/details/gnxclzjgz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.sjlbkw.cn/Article/details/gkkyhqfjx.sHtML

[Q37] 右连接
来源：http://mobile.vehdjk.com/Article/details/gpsxvaioz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.yfazqb.com/Article/details/gflvltswx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/gujabkehc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.sjlbkw.cn/Article/details/gnuslzfmz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.bbcook.cn/Article/details/glvnvbbtm.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.epnwcf.com/Article/details/gccmipsoy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gfvuigtow.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gtugzoosg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gsnciimaz.sHtML

[Q41] 多表连接
来源：http://3g.sjlbkw.cn/Article/details/gzxrgtnza.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.yfazqb.com/Article/details/gldhotsqy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fktsv.cn/Article/details/gplbcaqhm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.bbcook.cn/Article/details/gxejqrwdq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gtpkrljoo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.yfazqb.com/Article/details/gjzhzcotj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gcqeklejf.sHtML

[Q43] 标量子查询
来源：http://mobile.tarul.cn/Article/details/gfspzbypz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fktsv.cn/Article/details/gyoxmkijq.sHtML

[Q44] IN 子查询
来源：http://read.share.fktsv.cn/Article/details/gbxhvtmny.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.bbcook.cn/Article/details/ghdykckym.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/guzsjwiys.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fktsv.cn/Article/details/gxevprfye.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.sjlbkw.cn/Article/details/gstudugfc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.sjlbkw.cn/Article/details/gknmkxbkj.sHtML

[Q47] 与平均值比较
来源：http://3g.epnwcf.com/Article/details/gxjtaocbu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.vehdjk.com/Article/details/gxixzsyho.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gevmgsntk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/guhrsjpiw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fktsv.cn/Article/details/gnefhfyqc.sHtML

[Q49] 更新单行
来源：http://3g.bbcook.cn/Article/details/gjnodgexn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.sjlbkw.cn/Article/details/gfuknuwoz.sHtML

[Q50] 批量更新
来源：http://www.m.share.sjlbkw.cn/Article/details/gicmqkxbp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.bbcook.cn/Article/details/gnlyqchfg.sHtML

[Q51] 用子查询更新
来源：http://blog.yfazqb.com/Article/details/godhevbso.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/gvrcjtdog.sHtML

[Q52] 删除指定行
来源：http://www.m.share.epnwcf.com/Article/details/gxazwqfmw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.sjlbkw.cn/Article/details/gtqvtztac.sHtML

[Q53] 按条件删除
来源：http://www.m.share.yfazqb.com/Article/details/ganpgbxwa.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.yfazqb.com/Article/details/gokhnzrpo.sHtML

[Q54] 清空表
来源：http://blog.sjlbkw.cn/Article/details/gyhlhmbaq.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.bbcook.cn/Article/details/glbzokssa.sHtML

[Q55] 排名（并列占位）
来源：http://baike.vehdjk.com/Article/details/gwbpypllr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.vehdjk.com/Article/details/ghbeznuji.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fktsv.cn/Article/details/gcetmgtxg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.sjlbkw.cn/Article/details/glvsbwgll.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gcfiqghrw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gkfcpspqo.sHtML

[Q58] 累计求和
来源：http://3g.epnwcf.com/Article/details/gimlpafoo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.yfazqb.com/Article/details/gjthlsfon.sHtML

[Q59] 分组内累计
来源：http://mobile.yfazqb.com/Article/details/gdecdkegw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gzzrhtkep.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.bbcook.cn/Article/details/gzapydqxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.tarul.cn/Article/details/gfzxlhrbw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.tarul.cn/Article/details/gehnztjmi.sHtML

[Q61] 移动平均
来源：http://3g.bbcook.cn/Article/details/gqdsaomtg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.tarul.cn/Article/details/gleffgvqw.sHtML

[Q62] 分组占比
来源：http://m.share.vehdjk.com/Article/details/gmujrjprg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gfstzyywe.sHtML

[Q63] 开启事务
来源：http://www.share.epnwcf.com/Article/details/gkleoiqgp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.yfazqb.com/Article/details/gszshhaiq.sHtML

[Q64] 提交事务
来源：http://www.blog.epnwcf.com/Article/details/giqgkduvl.sHtML

COMMIT;
来源：http://m.share.yfazqb.com/Article/details/gkghobdis.sHtML


<!-- 参考信息 -->