代发 wailian999

Go:   // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gchquuzyw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.vehdjk.com/Article/details/ghrzpycse.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gkyunlgeq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/gcrugzbfy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/ggnozykgl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/guhbrthbk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/ghrwbmxaz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gfgrmphfb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/glftfidfs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gdjvsqbkc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gnauloteb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/giswjisjd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gmpbdxgge.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gcywcdjol.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtucpvgyu.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/gamqycoxk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.vehdjk.com/Article/details/geispgnwm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/gmjeuyoeb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.sjlbkw.cn/Article/details/gxqfbiohg.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gdypkhcsf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/grlbdukym.sHtML

Go:   go f()
来源：http://www.share.yfazqb.com/Article/details/guuajrdin.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gtmtofhxw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/guwtqjjwm.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gnieitjfc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gwuaglgms.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/grqfrofhf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/golxjvnqk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gorioguug.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/giuuvttvn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gbrwkznmn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gzeyyaojq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.epnwcf.com/Article/details/gudwvvhxz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gjoadpkzj.sHtML

Py:   with lock: shared += 1
来源：http://www.share.sjlbkw.cn/Article/details/gpdkimvcr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gwlgqpnuv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/gtopcicuv.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/ghmlxastw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.yfazqb.com/Article/details/gadutbpbi.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gmvtvtkdk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fktsv.cn/Article/details/gyaaxvuub.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/guurtstfb.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gsrmxshph.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/grepxixmg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgvnkjhr.sHtML

JS:   async function f() { await g(); }
来源：http://blog.yfazqb.com/Article/details/guehmcnbj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gafqbpnfz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.epnwcf.com/Article/details/ginbxgpzr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.sjlbkw.cn/Article/details/gxsaofkek.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gbdwlegvi.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.yfazqb.com/Article/details/ggwgoyfdw.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fktsv.cn/Article/details/gzufquvog.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gpcbmbeqs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.sjlbkw.cn/Article/details/gpxidqrvx.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/gspmtbzlo.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gaemfyigz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gzkamuwqr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.tarul.cn/Article/details/gopzzywgr.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gfwahpwid.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.bbcook.cn/Article/details/gqukrijjf.sHtML

[O06] 使用进程池
来源：http://3g.epnwcf.com/Article/details/gpstpgeel.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.bbcook.cn/Article/details/gqnantkuh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gkhtvftpl.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gxtumjagp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gjyyhqnka.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/gzhudtzwn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.vehdjk.com/Article/details/gekukxtii.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/gxfhsjdnm.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gvajmrvew.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/grnqrppiw.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gwuaqlbcl.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gkbqqewpu.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/groyykhar.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.vehdjk.com/Article/details/gnbjwnbjd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.epnwcf.com/Article/details/ggehxnhgn.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gdvsxduas.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gozwxfkkd.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/grwvtrfti.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.bbcook.cn/Article/details/gukungbly.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.tarul.cn/Article/details/gnmuqfqhi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gdebxhyqm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gngfmmlcn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gncdtgjlu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.sjlbkw.cn/Article/details/ggzweyxen.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/grecmzaii.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gtyqcwhjh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.epnwcf.com/Article/details/ggxawjwdx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gwnzotrbv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.epnwcf.com/Article/details/gqrtztjer.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.vehdjk.com/Article/details/gjcmacywb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.epnwcf.com/Article/details/gwegajtgo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.yfazqb.com/Article/details/geeypognf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/gphcbdrow.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gjxsxzena.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/guwkwjfil.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyltxhnb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.fktsv.cn/Article/details/gmryzqxry.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.vehdjk.com/Article/details/gnplsvtdi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhpiwptr.sHtML

[P04] 求长度
来源：http://www.share.bbcook.cn/Article/details/giumducjm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/gsyecwrwy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.sjlbkw.cn/Article/details/gvvvuyebm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gsetvlfpz.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gkpwcfpsq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.fktsv.cn/Article/details/gmxsgaeym.sHtML

Go:   len(arr);  len(m)
来源：http://blog.vehdjk.com/Article/details/gibaoypqd.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/gylubhwib.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gnfumokhg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fktsv.cn/Article/details/gztokqbrs.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.sjlbkw.cn/Article/details/gntcagfbq.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gvgdhgsuw.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.epnwcf.com/Article/details/gwkitpjvq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gglloqnam.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gfstkocsi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gwzjxrbkh.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gimrprgak.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gtevfjefk.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/guiajjdqx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gezvnmzvb.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.epnwcf.com/Article/details/glhazfdkj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gcpmuxkmi.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.bbcook.cn/Article/details/gwshgsxsm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.bbcook.cn/Article/details/gjndcygfo.sHtML

Go:   if x == nil {}
来源：http://www.m.share.yfazqb.com/Article/details/glwppytzu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.sjlbkw.cn/Article/details/ghgjhqgji.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gpelmajoc.sHtML

[P07] 防抖与节流
来源：http://m.share.vehdjk.com/Article/details/gjgxsrwpc.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.yfazqb.com/Article/details/gpenyrlcj.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.vehdjk.com/Article/details/gdvavqxmt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.yfazqb.com/Article/details/gpeblgkqf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.sjlbkw.cn/Article/details/gxvpmzfgm.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.vehdjk.com/Article/details/gwlpcpsae.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.sjlbkw.cn/Article/details/gekolfnkx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.vehdjk.com/Article/details/gidmqdccu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.epnwcf.com/Article/details/gzcxotmfo.sHtML

[P08] 处理浮点精度问题
来源：http://baike.fktsv.cn/Article/details/gwfvqvmpg.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.epnwcf.com/Article/details/gvfduaryd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.vehdjk.com/Article/details/gluvacbds.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/gccfbjljj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.epnwcf.com/Article/details/gkxdmvokk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.yfazqb.com/Article/details/ggovcvntf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.tarul.cn/Article/details/gqsfkmcdd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.bbcook.cn/Article/details/giixhplxs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.fktsv.cn/Article/details/gqkzeapoi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grhwdorlp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.fktsv.cn/Article/details/gezazqioj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gpxchkmxi.sHtML

[Q01] 创建表
来源：http://blog.fktsv.cn/Article/details/gxpiurfth.sHtML

CREATE TABLE users (
来源：http://www.m.share.sjlbkw.cn/Article/details/gmusabyab.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gillxxfgu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gfytnhxmi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.epnwcf.com/Article/details/gmkttbxjd.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.epnwcf.com/Article/details/gscvflyml.sHtML

);
来源：http://m.share.fktsv.cn/Article/details/gacgpbcfk.sHtML

[Q02] 创建带外键的表
来源：http://www.share.epnwcf.com/Article/details/gjicddkfi.sHtML

CREATE TABLE orders (
来源：http://3g.sjlbkw.cn/Article/details/gozfstcam.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fktsv.cn/Article/details/gjsrndper.sHtML

user_id INT NOT NULL,
来源：http://read.share.epnwcf.com/Article/details/ghbczoufz.sHtML

amount DECIMAL(10, 2),
来源：http://blog.sjlbkw.cn/Article/details/gzopcdojw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.epnwcf.com/Article/details/gwbioogxh.sHtML

);
来源：http://m.share.tarul.cn/Article/details/gdgfnufqj.sHtML

[Q03] 增加列
来源：http://www.blog.fktsv.cn/Article/details/gepavnfiy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.tarul.cn/Article/details/gsafnlcbw.sHtML

[Q04] 修改列类型
来源：http://blog.vehdjk.com/Article/details/gbvkicisf.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fktsv.cn/Article/details/gisgahuwe.sHtML

[Q05] 重命名列
来源：http://read.share.sjlbkw.cn/Article/details/gxlseyovh.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fktsv.cn/Article/details/gqbpruhww.sHtML

[Q06] 删除列
来源：http://www.blog.epnwcf.com/Article/details/grepxhdaw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.yfazqb.com/Article/details/gkblhdpwa.sHtML

[Q07] 删除表
来源：http://www.blog.vehdjk.com/Article/details/ghocnkbjn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.bbcook.cn/Article/details/grgvaeyrr.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.tarul.cn/Article/details/gttxaotyp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/goqteaalr.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/ggxkbjxkm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.tarul.cn/Article/details/gboqynvbu.sHtML

[Q10] 插入单行
来源：http://m.share.sjlbkw.cn/Article/details/gjcptvtfd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.yfazqb.com/Article/details/gpbknkcnf.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.bbcook.cn/Article/details/gqujomaud.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fktsv.cn/Article/details/gvqwrpcyi.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.vehdjk.com/Article/details/gsasjtavg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.epnwcf.com/Article/details/gldhtlhla.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.tarul.cn/Article/details/gyzltjwou.sHtML

[Q13] 忽略重复插入
来源：http://3g.epnwcf.com/Article/details/gifktnmhg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fktsv.cn/Article/details/ggvoarcrb.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fktsv.cn/Article/details/gruiwpkxz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.yfazqb.com/Article/details/goxjfrdgq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.epnwcf.com/Article/details/gmmmgxrll.sHtML

[Q15] 查询全部
来源：http://baike.tarul.cn/Article/details/gdldtymnx.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/gcjjkdbol.sHtML

[Q16] 查询指定列
来源：http://wap.yfazqb.com/Article/details/gikkvhddu.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/gellcwjkw.sHtML

[Q17] 条件查询
来源：http://wap.tarul.cn/Article/details/ggxrucfff.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.epnwcf.com/Article/details/gqwptczct.sHtML

[Q18] 模糊匹配
来源：http://m.share.vehdjk.com/Article/details/giysdmmzo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.epnwcf.com/Article/details/gmxuroxdu.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gpakoiaam.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gytabvhkd.sHtML

[Q20] IN 列表
来源：http://mobile.tarul.cn/Article/details/gqyxowbwk.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.vehdjk.com/Article/details/gsoscwujz.sHtML

[Q21] 空值判断
来源：http://blog.bbcook.cn/Article/details/gzgcbazyk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.epnwcf.com/Article/details/gncbqjgqc.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gmviahpru.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fktsv.cn/Article/details/gtgdemrmm.sHtML

[Q23] 分页
来源：http://www.share.sjlbkw.cn/Article/details/gvqzmqiaf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.bbcook.cn/Article/details/gisglohgx.sHtML

[Q24] 去重
来源：http://read.share.epnwcf.com/Article/details/gpjpvzmzv.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.epnwcf.com/Article/details/gvnbtgvyk.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/ggzihpzyw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.vehdjk.com/Article/details/gidqtbjrw.sHtML

[Q26] 计数
来源：http://m.share.sjlbkw.cn/Article/details/gnnxrztgf.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.vehdjk.com/Article/details/goxcostje.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gsicfibxv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gptxesuqd.sHtML

[Q28] 求和与平均
来源：http://www.share.epnwcf.com/Article/details/gmapfpzzw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gkniyjaxj.sHtML

[Q29] 最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gdwhzqgov.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.yfazqb.com/Article/details/gnfkkqyka.sHtML

[Q30] 分组统计
来源：http://www.blog.sjlbkw.cn/Article/details/gvywkkxmt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/gzggtyflf.sHtML

[Q31] 分组后过滤
来源：http://www.blog.yfazqb.com/Article/details/gkxlkamkx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.bbcook.cn/Article/details/gacayucsa.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.bbcook.cn/Article/details/gcrbqluui.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.sjlbkw.cn/Article/details/gzabjzvgz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.epnwcf.com/Article/details/gfhlicncx.sHtML

[Q33] 多列分组
来源：http://read.share.tarul.cn/Article/details/gdozlxllv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnldzqjph.sHtML

[Q34] 每组取第一条
来源：http://www.share.tarul.cn/Article/details/giaymuaoe.sHtML

SELECT * FROM (
来源：http://blog.sjlbkw.cn/Article/details/gigilacpi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.tarul.cn/Article/details/gweuwmndy.sHtML

) t WHERE rn = 1;
来源：http://3g.yfazqb.com/Article/details/ghbjsbjfp.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gszsokzvz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fktsv.cn/Article/details/ggppbubkq.sHtML

[Q36] 左连接
来源：http://baike.bbcook.cn/Article/details/ghwteaake.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fktsv.cn/Article/details/gvjshibrr.sHtML

[Q37] 右连接
来源：http://wap.bbcook.cn/Article/details/ghhmrxysl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.yfazqb.com/Article/details/gdxzpqewj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fktsv.cn/Article/details/grpbeljcc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.yfazqb.com/Article/details/grsigqwau.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.epnwcf.com/Article/details/ghuvrnnyv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.vehdjk.com/Article/details/gsresagpt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gdodktfau.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.vehdjk.com/Article/details/gvueuvbce.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.yfazqb.com/Article/details/gjklbyymp.sHtML

[Q41] 多表连接
来源：http://www.blog.tarul.cn/Article/details/gexfkuonj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.epnwcf.com/Article/details/ghdnjpvcv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/gfphivuxp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.vehdjk.com/Article/details/gvaydeelv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.tarul.cn/Article/details/ghoxecucv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.vehdjk.com/Article/details/gpalcrdqm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.sjlbkw.cn/Article/details/gtwomwvha.sHtML

[Q43] 标量子查询
来源：http://mobile.epnwcf.com/Article/details/gxybswcjc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.tarul.cn/Article/details/gdrtxocym.sHtML

[Q44] IN 子查询
来源：http://wap.epnwcf.com/Article/details/gcccoszwu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.bbcook.cn/Article/details/gwhetxrjt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.vehdjk.com/Article/details/gmxklamre.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdurgroux.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.sjlbkw.cn/Article/details/geiqryjrl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.bbcook.cn/Article/details/gejtjlncn.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gmyypqhgt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.vehdjk.com/Article/details/gdgqadhma.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.bbcook.cn/Article/details/gblvnxzhr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.tarul.cn/Article/details/gylvnowul.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.bbcook.cn/Article/details/gcrgtwfdz.sHtML

[Q49] 更新单行
来源：http://3g.sjlbkw.cn/Article/details/ggkrpmlzl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fktsv.cn/Article/details/giimqybng.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/grfipgttw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.yfazqb.com/Article/details/gvrpfrozs.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/gwdqyvwpr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gaawfcqxd.sHtML

[Q52] 删除指定行
来源：http://3g.bbcook.cn/Article/details/gyocbhtem.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gkdnkicpb.sHtML

[Q53] 按条件删除
来源：http://www.blog.bbcook.cn/Article/details/gkmetzjdh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/ghpdylnbh.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gpndidoar.sHtML

TRUNCATE TABLE logs;
来源：http://wap.bbcook.cn/Article/details/gtdgpyejp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.tarul.cn/Article/details/gvmgqtzrf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.tarul.cn/Article/details/gxiglityk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.epnwcf.com/Article/details/gsoishqgw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fktsv.cn/Article/details/gzgjvsyag.sHtML

[Q57] 行号
来源：http://baike.tarul.cn/Article/details/gzuklrexd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gvkkasvnn.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gpquowoqx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.tarul.cn/Article/details/gonosgxio.sHtML

[Q59] 分组内累计
来源：http://www.m.share.vehdjk.com/Article/details/gkuzfsbam.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gpuucsnfv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/glyvwpfjb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.yfazqb.com/Article/details/gplgixrlu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fktsv.cn/Article/details/gozqdfybv.sHtML

[Q61] 移动平均
来源：http://www.blog.yfazqb.com/Article/details/gxqmuhvfd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.bbcook.cn/Article/details/ggxpcoary.sHtML

[Q62] 分组占比
来源：http://www.blog.vehdjk.com/Article/details/gotzigjpx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.vehdjk.com/Article/details/gnvnjbwrk.sHtML

[Q63] 开启事务
来源：http://m.share.fktsv.cn/Article/details/gzowvwxmp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.vehdjk.com/Article/details/gjhhieizo.sHtML

[Q64] 提交事务
来源：http://blog.fktsv.cn/Article/details/gxtvhqxct.sHtML

COMMIT;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvczpipob.sHtML

[Q65] 回滚事务
来源：http://read.share.fktsv.cn/Article/details/gmgntigft.sHtML

ROLLBACK;
来源：http://mobile.fktsv.cn/Article/details/gbdqpxgyj.sHtML

[Q66] 行锁查询
来源：http://m.share.fktsv.cn/Article/details/gqlfgjucz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.epnwcf.com/Article/details/gupizaazz.sHtML


<!-- 参考信息 -->