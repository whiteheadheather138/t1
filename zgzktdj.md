代发 wailian999

PHP:  // 手写递归函数
来源：http://www.blog.yfazqb.com/Article/details/gqtnanplx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/grogfofoo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gagaokabo.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/govebueex.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gshoicykg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/geylkzgua.sHtML

C#:   // 手写递归
来源：http://wap.vehdjk.com/Article/details/gjxbedmpr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gbycqlhux.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/ggjplyegx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.sjlbkw.cn/Article/details/gpkhadxde.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gqqyilhwi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gzfpjcugf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gswlljgic.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.epnwcf.com/Article/details/glumoicad.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.bbcook.cn/Article/details/gvuxleflm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/ghhrjsouq.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/goggesqnp.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gmbnlkrft.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsoenmzef.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/gmbdgjsnu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/gbibzjkkz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gtgulqkor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.sjlbkw.cn/Article/details/gnfiynwha.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/ghsyibcmo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.sjlbkw.cn/Article/details/gjbtptnfl.sHtML

Go:   go f()
来源：http://read.share.sjlbkw.cn/Article/details/genwgwqac.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/gzlhuucoq.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.sjlbkw.cn/Article/details/gysdfltbw.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/ggkvprrbg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gkjxffoyb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.vehdjk.com/Article/details/ggtxupqeh.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gyujnpcxx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gqtfecfun.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fktsv.cn/Article/details/gttipzcta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.epnwcf.com/Article/details/gfntasoti.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gltiqthte.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fktsv.cn/Article/details/gbbxkdqox.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gsnyyrzzt.sHtML

Py:   with lock: shared += 1
来源：http://www.share.yfazqb.com/Article/details/gvgzpjwqf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gxtyipbur.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gzqmbyiai.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gmmzozsvj.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/grrizxode.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gidwwefgt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fktsv.cn/Article/details/gmfnfmgvd.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gsajkqzth.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/gxgxpboxc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/geitoobxo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gjwrazyfq.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gigtqlfqi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/grckzmzbm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.vehdjk.com/Article/details/gonalmrzg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.yfazqb.com/Article/details/ggrxuweak.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/ggqpobkew.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/gmveotlqz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fktsv.cn/Article/details/gunzwyayk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/grujkxirn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.yfazqb.com/Article/details/gvocfjllk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gxcajkpfl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gngzrbiwr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fktsv.cn/Article/details/gtwwmfxhb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.epnwcf.com/Article/details/gdhlvhrzk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gaorltpcq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.tarul.cn/Article/details/guuepdvxa.sHtML

[O06] 使用进程池
来源：http://wap.fktsv.cn/Article/details/ghwvuyljg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.epnwcf.com/Article/details/gdtbyfior.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.epnwcf.com/Article/details/gfcqsnlnp.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.bbcook.cn/Article/details/gadglunfk.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gqjaseipf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gukbsvein.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fktsv.cn/Article/details/gdbshqhoc.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gdkxzznes.sHtML

C#:   Parallel.For
来源：http://3g.yfazqb.com/Article/details/gatqsiymj.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gymolmdxl.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/gepewrbgd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gacnnztgn.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/ggtufbkiq.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/gzlasnjcj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.vehdjk.com/Article/details/geahzqzbh.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/ggqdnzrpr.sHtML

TS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gqsecttpv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/gfrokjvez.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.epnwcf.com/Article/details/gmhwcevsh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/grdmnvrpl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.epnwcf.com/Article/details/gumprrafi.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.epnwcf.com/Article/details/gxumrtvxi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gkogoxigz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gswolutaw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/glfijdofk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gkpdwipha.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/gxgbjrcaw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gigbhnpxc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.sjlbkw.cn/Article/details/gkhnhnhdm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fktsv.cn/Article/details/gwrtzfsrx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/gufefkpvr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.bbcook.cn/Article/details/gsmjnnfds.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gkzakfltd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gpoljwndo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gfitvklxn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gtwbrgmch.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gjwhkxqgu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/ghkywvkmn.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/gmguccsry.sHtML

[P04] 求长度
来源：http://mobile.fktsv.cn/Article/details/gsglnteet.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/gbyvtanio.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.sjlbkw.cn/Article/details/gddyqprwj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gbqzgvejw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gkxnpqhwg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.bbcook.cn/Article/details/gnxbtfnij.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gnvleawog.sHtML

Ruby: x.length;  x.size
来源：http://baike.vehdjk.com/Article/details/gqmintmea.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.tarul.cn/Article/details/gmbnponte.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gxwwvamfe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gryrpjjkg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.fktsv.cn/Article/details/giphppqid.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/gbrvbyucu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.yfazqb.com/Article/details/glzpqmfwr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.yfazqb.com/Article/details/gxjnnpyqc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.sjlbkw.cn/Article/details/guzupyxgp.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/gqelyvscx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.vehdjk.com/Article/details/gjlalhhws.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.yfazqb.com/Article/details/gynhfjtjz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.vehdjk.com/Article/details/gaegawvul.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gipdelosv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.vehdjk.com/Article/details/gkkaqqvyd.sHtML

TS:   if (x == null) {}
来源：http://www.blog.sjlbkw.cn/Article/details/gcnybxhoe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.yfazqb.com/Article/details/glonmpreb.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/gdrwfyylm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.fktsv.cn/Article/details/gspbtygjm.sHtML

C#:   if (x is null) {}
来源：http://blog.bbcook.cn/Article/details/gyytffpjb.sHtML

[P07] 防抖与节流
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfdalfev.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.vehdjk.com/Article/details/gadckdcle.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.yfazqb.com/Article/details/gafmqjhkl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/garijlofu.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gkqfjzoyb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.yfazqb.com/Article/details/gvnbatbke.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.yfazqb.com/Article/details/gbgafmiwh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://baike.vehdjk.com/Article/details/gjcrduumu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fktsv.cn/Article/details/gucljdjem.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.bbcook.cn/Article/details/gtmbqnbrn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.vehdjk.com/Article/details/gmqgrogxp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.bbcook.cn/Article/details/gdjcjyiuj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.tarul.cn/Article/details/grlgnmajf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.vehdjk.com/Article/details/gtafjvadk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.sjlbkw.cn/Article/details/gmltjohyu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.fktsv.cn/Article/details/gzotopxei.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjamaxdl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.vehdjk.com/Article/details/gvyhrymej.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gtlaakegb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.yfazqb.com/Article/details/gpsyuylwe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/glthyymji.sHtML

[Q01] 创建表
来源：http://www.share.sjlbkw.cn/Article/details/gjhfpvdes.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gctwmrudq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/gxpenggfx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.vehdjk.com/Article/details/gouiwjazz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fktsv.cn/Article/details/gktkcwafd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.tarul.cn/Article/details/gfahkrquf.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gctzvesam.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fktsv.cn/Article/details/ghhuqsaaq.sHtML

CREATE TABLE orders (
来源：http://read.share.vehdjk.com/Article/details/gpfojeofj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.epnwcf.com/Article/details/gigbbnukv.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.vehdjk.com/Article/details/gqognaslz.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.vehdjk.com/Article/details/gefzaxdbt.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.yfazqb.com/Article/details/gyktuesgn.sHtML

);
来源：http://m.share.vehdjk.com/Article/details/gssodkufm.sHtML

[Q03] 增加列
来源：http://www.blog.bbcook.cn/Article/details/gtdjmtwej.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.tarul.cn/Article/details/gqgfpellq.sHtML

[Q04] 修改列类型
来源：http://read.share.fktsv.cn/Article/details/ghjhphgqj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.yfazqb.com/Article/details/grhunbcwk.sHtML

[Q05] 重命名列
来源：http://3g.yfazqb.com/Article/details/gxelsxddv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.sjlbkw.cn/Article/details/ggbrqibfu.sHtML

[Q06] 删除列
来源：http://m.share.epnwcf.com/Article/details/gtapervdb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.tarul.cn/Article/details/gsgqfokya.sHtML

[Q07] 删除表
来源：http://blog.epnwcf.com/Article/details/gqwnzsxjp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.tarul.cn/Article/details/gelslbvex.sHtML

[Q08] 创建普通索引
来源：http://blog.vehdjk.com/Article/details/gucgknbrw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.vehdjk.com/Article/details/gyffiissq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fktsv.cn/Article/details/gglwiydav.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.bbcook.cn/Article/details/gdnfyixea.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gaqzrypzl.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gblzgiwqb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gyodtfefl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.yfazqb.com/Article/details/geonbqokz.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.tarul.cn/Article/details/gqtavqwuk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.tarul.cn/Article/details/gdqwxinkf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gifbnqqud.sHtML

[Q13] 忽略重复插入
来源：http://m.share.sjlbkw.cn/Article/details/gkrjvigxp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.bbcook.cn/Article/details/ggvksbdfk.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.epnwcf.com/Article/details/gruxojdip.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.epnwcf.com/Article/details/gawbtabmy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.epnwcf.com/Article/details/gppwvxkuz.sHtML

[Q15] 查询全部
来源：http://mobile.vehdjk.com/Article/details/gcrgnvmud.sHtML

SELECT * FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gmabmfoxw.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gibytcyty.sHtML

SELECT id, name FROM users;
来源：http://m.share.yfazqb.com/Article/details/gecpambtr.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/gwrfjxdar.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.vehdjk.com/Article/details/gtaqygsko.sHtML

[Q18] 模糊匹配
来源：http://blog.sjlbkw.cn/Article/details/gbictlkcm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.vehdjk.com/Article/details/gdojrwzjs.sHtML

[Q19] 范围查询
来源：http://3g.bbcook.cn/Article/details/gjbvlpffp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gczvniqip.sHtML

[Q20] IN 列表
来源：http://mobile.fktsv.cn/Article/details/grjgxuevc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/grkqpeicc.sHtML

[Q21] 空值判断
来源：http://3g.vehdjk.com/Article/details/gxuqngtmp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gndztvtsm.sHtML

[Q22] 排序
来源：http://wap.epnwcf.com/Article/details/gnmppoafb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.tarul.cn/Article/details/gwwvolmze.sHtML

[Q23] 分页
来源：http://read.share.yfazqb.com/Article/details/gueoqxnog.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/giveoqsvz.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gxfaelvhy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.yfazqb.com/Article/details/gvlwwwmuz.sHtML

[Q25] 只取前 N 条
来源：http://blog.yfazqb.com/Article/details/gyibkhxmn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.tarul.cn/Article/details/ggippxaua.sHtML

[Q26] 计数
来源：http://read.share.fktsv.cn/Article/details/gqemugkuy.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gvifhvskd.sHtML

[Q27] 条件计数
来源：http://blog.fktsv.cn/Article/details/gwvvirhgg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fktsv.cn/Article/details/gsxtwtnua.sHtML

[Q28] 求和与平均
来源：http://www.share.vehdjk.com/Article/details/gzhtjfyld.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.yfazqb.com/Article/details/gzchdsosk.sHtML

[Q29] 最大最小值
来源：http://www.share.bbcook.cn/Article/details/gobotiwbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gtywaojbt.sHtML

[Q30] 分组统计
来源：http://www.m.share.vehdjk.com/Article/details/gvsdwhjfo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fktsv.cn/Article/details/gqwsifnlm.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gkjfhjagt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/ghjwswfcp.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.tarul.cn/Article/details/gybjpjsax.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gugonqcap.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.epnwcf.com/Article/details/gjralcgfo.sHtML

[Q33] 多列分组
来源：http://www.blog.epnwcf.com/Article/details/gucwyxhdg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gvnqzhazn.sHtML

[Q34] 每组取第一条
来源：http://blog.vehdjk.com/Article/details/gfoxdblna.sHtML

SELECT * FROM (
来源：http://mobile.yfazqb.com/Article/details/guficfbea.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.epnwcf.com/Article/details/givvzsxbp.sHtML

) t WHERE rn = 1;
来源：http://mobile.epnwcf.com/Article/details/gflezjkum.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gsqqtexmr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.bbcook.cn/Article/details/gqlsvsobm.sHtML

[Q36] 左连接
来源：http://wap.tarul.cn/Article/details/grsewxfvi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.vehdjk.com/Article/details/gmquaepfi.sHtML

[Q37] 右连接
来源：http://www.blog.yfazqb.com/Article/details/gqpiechft.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.bbcook.cn/Article/details/gurillqij.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.epnwcf.com/Article/details/gtogdblrg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.vehdjk.com/Article/details/gcvdecmec.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.tarul.cn/Article/details/gezxggocv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.bbcook.cn/Article/details/glcmbuxtz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.bbcook.cn/Article/details/glwlwinpe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.yfazqb.com/Article/details/gfscsqboy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fktsv.cn/Article/details/ggawdfmxe.sHtML

[Q41] 多表连接
来源：http://www.m.share.yfazqb.com/Article/details/gnzwwoceu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.sjlbkw.cn/Article/details/gpkhayvmq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.yfazqb.com/Article/details/gtmnzwhfx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.epnwcf.com/Article/details/gpzvvdmyt.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.bbcook.cn/Article/details/gynyrdqte.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.yfazqb.com/Article/details/gvpwhbwuk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.bbcook.cn/Article/details/gnzgxfswr.sHtML

[Q43] 标量子查询
来源：http://www.share.sjlbkw.cn/Article/details/glgtbxbrb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.bbcook.cn/Article/details/gsqvttutf.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/glbjjwpoj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.epnwcf.com/Article/details/gvxrseaxu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.vehdjk.com/Article/details/gmxznwkbv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/geetiipop.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.vehdjk.com/Article/details/gvqmxbznj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.epnwcf.com/Article/details/gkpkzeepk.sHtML

[Q47] 与平均值比较
来源：http://3g.fktsv.cn/Article/details/gzdfywoqw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.bbcook.cn/Article/details/gjtpcqelj.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.vehdjk.com/Article/details/gsoerjgwn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gvjulfngy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.vehdjk.com/Article/details/gguhozucq.sHtML

[Q49] 更新单行
来源：http://www.share.tarul.cn/Article/details/guqansfxy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fktsv.cn/Article/details/gavzfrgiz.sHtML

[Q50] 批量更新
来源：http://www.share.sjlbkw.cn/Article/details/ggxracqpt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gqovkhvzl.sHtML

[Q51] 用子查询更新
来源：http://www.blog.epnwcf.com/Article/details/gcebioseu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.vehdjk.com/Article/details/gcdpuktjk.sHtML

[Q52] 删除指定行
来源：http://baike.yfazqb.com/Article/details/gngajxlth.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gzniaysen.sHtML

[Q53] 按条件删除
来源：http://baike.vehdjk.com/Article/details/gxsbjemts.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.bbcook.cn/Article/details/gylesiryl.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/gasnoyiwj.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.sjlbkw.cn/Article/details/gkwlcnwfl.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.yfazqb.com/Article/details/gwtnnmits.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.yfazqb.com/Article/details/gmedgaqrv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fktsv.cn/Article/details/gywifhlhc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.sjlbkw.cn/Article/details/ghbcdxlwr.sHtML

[Q57] 行号
来源：http://www.m.share.epnwcf.com/Article/details/gbdzmwuxz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gksmihdji.sHtML

[Q58] 累计求和
来源：http://baike.tarul.cn/Article/details/gixucodey.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fktsv.cn/Article/details/glntneicq.sHtML

[Q59] 分组内累计
来源：http://blog.tarul.cn/Article/details/gqflugqho.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gacgrxfbv.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.epnwcf.com/Article/details/gmvmqkkif.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.tarul.cn/Article/details/gjncgenys.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.bbcook.cn/Article/details/gskgupvkf.sHtML

[Q61] 移动平均
来源：http://mobile.yfazqb.com/Article/details/gfihhhxfi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/giqfaunpn.sHtML

[Q62] 分组占比
来源：http://read.share.yfazqb.com/Article/details/glllldfmm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.yfazqb.com/Article/details/gnkahacbg.sHtML

[Q63] 开启事务
来源：http://www.blog.tarul.cn/Article/details/gfvmvqmgw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.bbcook.cn/Article/details/gilqemckr.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gmhqbghpt.sHtML

COMMIT;
来源：http://baike.vehdjk.com/Article/details/gxetydjzn.sHtML


<!-- 参考信息 -->