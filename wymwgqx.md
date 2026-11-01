代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.yfazqb.com/Article/details/ggtxljdfm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.yfazqb.com/Article/details/gyudnrcjr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gmjhkxowb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gvgwyyfkd.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/ggbkiuaah.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gjrxhsagh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gnngvswzk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gcnzkotux.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gstazbhxs.sHtML

O. 并发与异步
来源：http://read.share.epnwcf.com/Article/details/ghmnwkxjk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gvnxvhftt.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gtrocdiqc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gfxdhvact.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/giusxkzgl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gwlkbgpty.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gczvrmros.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/gjoxpflnf.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gdqgdbare.sHtML

Ruby: Thread.new { f }
来源：http://blog.yfazqb.com/Article/details/guuixectt.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.yfazqb.com/Article/details/glfmlexzi.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gwxzktddw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fktsv.cn/Article/details/gmvytsvwd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gpaaeduoy.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/godtmncdr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gvjnsjsjo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gbhbgzwaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fktsv.cn/Article/details/gggcpcdet.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/geinmwtal.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gdvawiamq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/ggcbxbfmi.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fktsv.cn/Article/details/gtdkdqtbp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gygusjsso.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.vehdjk.com/Article/details/gytufvgwn.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gdqlgzdqa.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.yfazqb.com/Article/details/ggtfvdejt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.sjlbkw.cn/Article/details/gfpzijqzh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gpkxaczfp.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gxzudzfhp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.bbcook.cn/Article/details/gpymmyukv.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gezrxlkel.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fktsv.cn/Article/details/gcowljoym.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.sjlbkw.cn/Article/details/gywwehvxz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gegfljkzl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/grygkfbss.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.sjlbkw.cn/Article/details/gmjvjhfed.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gcvwdripd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.sjlbkw.cn/Article/details/gzccwrzke.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/guhavmhem.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.vehdjk.com/Article/details/gsvmsgnon.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gmgrqlaid.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.bbcook.cn/Article/details/gupvpdtvh.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gyzqhpsau.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gpzmiczvd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.sjlbkw.cn/Article/details/gbazwfepf.sHtML

Ruby: threads.map(&:join)
来源：http://baike.bbcook.cn/Article/details/gejpvuwba.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.sjlbkw.cn/Article/details/gsuabrndl.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gvspdrndz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/grjtfufme.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fktsv.cn/Article/details/gjurzocip.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.yfazqb.com/Article/details/gvupdlsmb.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/grcwikkvz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.bbcook.cn/Article/details/gucrfcjur.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/gileajkqv.sHtML

Ruby: // fork 块
来源：http://read.share.vehdjk.com/Article/details/gcnnzdyxz.sHtML

C#:   Parallel.For
来源：http://www.m.share.tarul.cn/Article/details/gxqzaqedy.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/grqpdlstx.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gxmrpcevb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvnrymouz.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gzyzimyhs.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.tarul.cn/Article/details/gmcpghrjw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.yfazqb.com/Article/details/gegipndzx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gtksbtnvx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gurtzqafw.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gpbmpufkr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.vehdjk.com/Article/details/gsfuqpawl.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.epnwcf.com/Article/details/gyvlaohxr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.yfazqb.com/Article/details/gzlrebmkq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/goqkvxsyx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gjzwewbqu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.yfazqb.com/Article/details/ghcxydrpu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.tarul.cn/Article/details/glznekmfg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.sjlbkw.cn/Article/details/gcaqijfac.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.bbcook.cn/Article/details/ghatcketz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gypsuokdo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.tarul.cn/Article/details/gelsynlce.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.yfazqb.com/Article/details/gngapjmsc.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gcjighhjt.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.yfazqb.com/Article/details/gjnrpeeye.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.epnwcf.com/Article/details/gjlbeawaz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gfuihzlxo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gkswoiszh.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gdshfapli.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gqsqxtjke.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.bbcook.cn/Article/details/gzcpkwcyf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.epnwcf.com/Article/details/gotodzkqu.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gsdxvwryc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gzdzociol.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/grwqgxttm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.tarul.cn/Article/details/gcvydxbil.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.sjlbkw.cn/Article/details/goyqulvgt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.vehdjk.com/Article/details/gtaitotme.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fktsv.cn/Article/details/gznrlyhrt.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/glqpyhjwk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/gdrwlcvtb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/gwimpveyu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.epnwcf.com/Article/details/gmdbnzjwx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.sjlbkw.cn/Article/details/gkcfwjucc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.sjlbkw.cn/Article/details/gcnbshsgh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gryoqbjmq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gcecimohk.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gksctepwn.sHtML

Ruby: a == b
来源：http://www.m.share.tarul.cn/Article/details/gndxypugv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.sjlbkw.cn/Article/details/gomzewker.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.epnwcf.com/Article/details/gbygsvpto.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gapzxvflv.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gaypnzwsg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gajvbvjtw.sHtML

TS:   if (x == null) {}
来源：http://baike.vehdjk.com/Article/details/gzzghfffm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.tarul.cn/Article/details/gyoczqnbk.sHtML

Go:   if x == nil {}
来源：http://3g.epnwcf.com/Article/details/gqgousjsg.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fktsv.cn/Article/details/grbhkcgws.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gurguozgz.sHtML

[P07] 防抖与节流
来源：http://3g.sjlbkw.cn/Article/details/gezzoklsa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gvlvnmwsn.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.tarul.cn/Article/details/gqrkliuyb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gppoievqv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.sjlbkw.cn/Article/details/glhztuoan.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.tarul.cn/Article/details/gldwrrxnk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fktsv.cn/Article/details/gbngrfhlz.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.tarul.cn/Article/details/gbndahtzh.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.sjlbkw.cn/Article/details/gdtaatbqn.sHtML

[P08] 处理浮点精度问题
来源：http://wap.vehdjk.com/Article/details/gpdrsugqg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fktsv.cn/Article/details/gmyxeyssd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/ggrlowhwo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.sjlbkw.cn/Article/details/gnwkhoiup.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fktsv.cn/Article/details/gmoloehpz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.tarul.cn/Article/details/gmzxdfapf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.epnwcf.com/Article/details/gbzszbsjc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.epnwcf.com/Article/details/gmqvpzgul.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.sjlbkw.cn/Article/details/goxeiqqzs.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzlluruea.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.epnwcf.com/Article/details/grjpkorgv.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfdwqtpsd.sHtML

[Q01] 创建表
来源：http://www.blog.sjlbkw.cn/Article/details/gvlirfacy.sHtML

CREATE TABLE users (
来源：http://www.share.epnwcf.com/Article/details/gvfwxzbgx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.sjlbkw.cn/Article/details/glwqtsnms.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/ggconyktg.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gztqwzxpd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.yfazqb.com/Article/details/gtycsdggm.sHtML

);
来源：http://www.blog.tarul.cn/Article/details/gvajdjmnw.sHtML

[Q02] 创建带外键的表
来源：http://3g.fktsv.cn/Article/details/guljrxnez.sHtML

CREATE TABLE orders (
来源：http://3g.vehdjk.com/Article/details/gpovmctqi.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.yfazqb.com/Article/details/ghxpinifx.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gsykiiyhh.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.yfazqb.com/Article/details/ghrkrkvpa.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fktsv.cn/Article/details/gfaytuzyc.sHtML

);
来源：http://baike.yfazqb.com/Article/details/gkjeoxhse.sHtML

[Q03] 增加列
来源：http://m.share.tarul.cn/Article/details/gbzkxdtoi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.bbcook.cn/Article/details/gxucbnhkp.sHtML

[Q04] 修改列类型
来源：http://m.share.epnwcf.com/Article/details/gsqjuwice.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fktsv.cn/Article/details/gpalxfssn.sHtML

[Q05] 重命名列
来源：http://www.share.fktsv.cn/Article/details/gygamsdnn.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.tarul.cn/Article/details/giiesucaa.sHtML

[Q06] 删除列
来源：http://www.m.share.bbcook.cn/Article/details/glavcjhhi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.bbcook.cn/Article/details/grnvumqab.sHtML

[Q07] 删除表
来源：http://read.share.bbcook.cn/Article/details/gucrdnnig.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.yfazqb.com/Article/details/gfonxhkdy.sHtML

[Q08] 创建普通索引
来源：http://blog.epnwcf.com/Article/details/glegiedve.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.vehdjk.com/Article/details/gxfuduzii.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.vehdjk.com/Article/details/gqokrvund.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.sjlbkw.cn/Article/details/gnmssfsnl.sHtML

[Q10] 插入单行
来源：http://wap.bbcook.cn/Article/details/gfrpoxjet.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.epnwcf.com/Article/details/gtknqkzrg.sHtML

[Q11] 一次插入多行
来源：http://m.share.fktsv.cn/Article/details/gemhcowrv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fktsv.cn/Article/details/gcgxgzhue.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.epnwcf.com/Article/details/gmasxpqox.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.bbcook.cn/Article/details/gtrfccadt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.vehdjk.com/Article/details/ghrtfveej.sHtML

[Q13] 忽略重复插入
来源：http://www.share.sjlbkw.cn/Article/details/grlpjrdto.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.tarul.cn/Article/details/gukrkvasq.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.tarul.cn/Article/details/ghrbpbbib.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/gmbebtbcl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/gmqidemmv.sHtML

[Q15] 查询全部
来源：http://www.share.bbcook.cn/Article/details/gpleegmpw.sHtML

SELECT * FROM users;
来源：http://www.share.tarul.cn/Article/details/gjvxzgdxl.sHtML

[Q16] 查询指定列
来源：http://read.share.vehdjk.com/Article/details/gpidduoke.sHtML

SELECT id, name FROM users;
来源：http://mobile.epnwcf.com/Article/details/gupeadesy.sHtML

[Q17] 条件查询
来源：http://m.share.fktsv.cn/Article/details/gneimokvw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.sjlbkw.cn/Article/details/gvofqawjm.sHtML

[Q18] 模糊匹配
来源：http://wap.yfazqb.com/Article/details/gzvkmnxlk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.epnwcf.com/Article/details/gbgbxcnbu.sHtML

[Q19] 范围查询
来源：http://read.share.epnwcf.com/Article/details/gcmwzdppc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.yfazqb.com/Article/details/gogwllzpq.sHtML

[Q20] IN 列表
来源：http://wap.sjlbkw.cn/Article/details/gqnsuoxib.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.sjlbkw.cn/Article/details/gktlzlcoz.sHtML

[Q21] 空值判断
来源：http://baike.bbcook.cn/Article/details/gqzmdxsin.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.vehdjk.com/Article/details/gmalfdraj.sHtML

[Q22] 排序
来源：http://read.share.fktsv.cn/Article/details/ggsioxrzs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.epnwcf.com/Article/details/guxwjcxuq.sHtML

[Q23] 分页
来源：http://blog.bbcook.cn/Article/details/gkairkunp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.bbcook.cn/Article/details/gofuifbbn.sHtML

[Q24] 去重
来源：http://blog.vehdjk.com/Article/details/gjktcvkes.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.yfazqb.com/Article/details/gvogbeyil.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.bbcook.cn/Article/details/gzwxrrrhu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.bbcook.cn/Article/details/gdxunhwzf.sHtML

[Q26] 计数
来源：http://mobile.epnwcf.com/Article/details/gwhrsogth.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.bbcook.cn/Article/details/glzxbvqhs.sHtML

[Q27] 条件计数
来源：http://blog.bbcook.cn/Article/details/gxhhwggnj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.sjlbkw.cn/Article/details/gboanbxzm.sHtML

[Q28] 求和与平均
来源：http://wap.sjlbkw.cn/Article/details/gnhpasvsb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gaxhcdpld.sHtML

[Q29] 最大最小值
来源：http://www.share.epnwcf.com/Article/details/gnzvrhtbj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.vehdjk.com/Article/details/gixbadjuv.sHtML

[Q30] 分组统计
来源：http://mobile.sjlbkw.cn/Article/details/gylctjuha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fktsv.cn/Article/details/ghpvnbgjs.sHtML

[Q31] 分组后过滤
来源：http://wap.bbcook.cn/Article/details/gtetfecbx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.tarul.cn/Article/details/gozugyhxl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.tarul.cn/Article/details/gcakrkaxm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.epnwcf.com/Article/details/gqfhsvgtz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.vehdjk.com/Article/details/gmshzvwbf.sHtML

[Q33] 多列分组
来源：http://baike.bbcook.cn/Article/details/grlttmepz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.vehdjk.com/Article/details/gssaaycnc.sHtML

[Q34] 每组取第一条
来源：http://m.share.vehdjk.com/Article/details/giqnoubjx.sHtML

SELECT * FROM (
来源：http://www.share.tarul.cn/Article/details/gwszliovj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.yfazqb.com/Article/details/gsvxqtnii.sHtML

) t WHERE rn = 1;
来源：http://www.blog.tarul.cn/Article/details/gdgoqreuk.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/gcbmomqsk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fktsv.cn/Article/details/gfervptpn.sHtML

[Q36] 左连接
来源：http://www.share.sjlbkw.cn/Article/details/gulgdrisb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gsvciexwq.sHtML

[Q37] 右连接
来源：http://3g.sjlbkw.cn/Article/details/grrojmeyh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fktsv.cn/Article/details/gnfmhmwni.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gqgsnwyfb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.bbcook.cn/Article/details/ghjgtntei.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.epnwcf.com/Article/details/ggyfatsfu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.tarul.cn/Article/details/gdkkdtmbg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.vehdjk.com/Article/details/gjvzwjros.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.bbcook.cn/Article/details/gwqftfnoa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/gnwkixoly.sHtML

[Q41] 多表连接
来源：http://3g.vehdjk.com/Article/details/gthlfacsd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/glskuhmsg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.tarul.cn/Article/details/gpzxoiprv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gtdqnqlda.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.bbcook.cn/Article/details/gaoysrlov.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.sjlbkw.cn/Article/details/gbngyeixn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.tarul.cn/Article/details/gajgeksjc.sHtML

[Q43] 标量子查询
来源：http://baike.epnwcf.com/Article/details/gawdmsibr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.yfazqb.com/Article/details/gqjblnmij.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gycbdidbn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.yfazqb.com/Article/details/gmtipyube.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fktsv.cn/Article/details/gaorlxeke.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.tarul.cn/Article/details/gccoerlpn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fktsv.cn/Article/details/gexwquppy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fktsv.cn/Article/details/gfrcsixyf.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gsoagbflf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.epnwcf.com/Article/details/gbadtwclm.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.yfazqb.com/Article/details/gcfslocyf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.sjlbkw.cn/Article/details/guaueanhy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fktsv.cn/Article/details/gwgbiolov.sHtML

[Q49] 更新单行
来源：http://mobile.yfazqb.com/Article/details/gqgndqwts.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.tarul.cn/Article/details/gqjmptrrw.sHtML

[Q50] 批量更新
来源：http://mobile.sjlbkw.cn/Article/details/gshqleofr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.yfazqb.com/Article/details/glggzwjlx.sHtML

[Q51] 用子查询更新
来源：http://wap.sjlbkw.cn/Article/details/gfbpqedqj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.tarul.cn/Article/details/gmrfmauxl.sHtML

[Q52] 删除指定行
来源：http://3g.vehdjk.com/Article/details/gpkdwoqce.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gwpaurltc.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gurbtqtfe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.bbcook.cn/Article/details/gpxoxqyol.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gmwkoyegd.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.vehdjk.com/Article/details/gtmmzrtjx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.yfazqb.com/Article/details/gjlzidwej.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gzjigyiyx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.vehdjk.com/Article/details/ggtckpgnd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.tarul.cn/Article/details/gzdehlpsl.sHtML

[Q57] 行号
来源：http://read.share.fktsv.cn/Article/details/grxkwqwes.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.yfazqb.com/Article/details/gzpngiuol.sHtML

[Q58] 累计求和
来源：http://3g.sjlbkw.cn/Article/details/gyguqbmeg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gvchmmrfw.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gsexcqflx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.yfazqb.com/Article/details/gjdmqwtth.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fktsv.cn/Article/details/gdrfjqkdo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.epnwcf.com/Article/details/gpjxlkdxk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.epnwcf.com/Article/details/gmskbhzmo.sHtML

[Q61] 移动平均
来源：http://mobile.bbcook.cn/Article/details/gnysscjkd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.tarul.cn/Article/details/gqmezwbbm.sHtML

[Q62] 分组占比
来源：http://blog.tarul.cn/Article/details/gkpzhnirp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/gsyxfdcgn.sHtML

[Q63] 开启事务
来源：http://baike.fktsv.cn/Article/details/gyxlqoaaw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.epnwcf.com/Article/details/gtagwgujn.sHtML

[Q64] 提交事务
来源：http://read.share.yfazqb.com/Article/details/gjesdyigy.sHtML

COMMIT;
来源：http://blog.epnwcf.com/Article/details/gjnddhops.sHtML

[Q65] 回滚事务
来源：http://m.share.tarul.cn/Article/details/gucxciftj.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/gxocscndc.sHtML

[Q66] 行锁查询
来源：http://baike.bbcook.cn/Article/details/gxvojdrri.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.bbcook.cn/Article/details/gggawltbe.sHtML

[Q67] 设置隔离级别
来源：http://read.share.sjlbkw.cn/Article/details/gvyjuntrp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.tarul.cn/Article/details/gwvjmbygl.sHtML

[Q68] 保存点
来源：http://wap.epnwcf.com/Article/details/gaoswrbij.sHtML

SAVEPOINT sp1;
来源：http://www.share.yfazqb.com/Article/details/grrncvvpu.sHtML


<!-- 参考信息 -->