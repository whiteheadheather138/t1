代发 wailian999

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gteoscczi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.yfazqb.com/Article/details/grfcsclpk.sHtML

C#:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gwigdmlqg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gzwtcpxnb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/gpgmsqxjd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fktsv.cn/Article/details/gkyfgrbpw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gzwkykwzq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gbnkndeut.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gpdlnyofv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gpwanjadm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.vehdjk.com/Article/details/gjuyjabmb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gbfatclpq.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gxrvbfsbz.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gebiipolg.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/goulqefjn.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/gcvmsnano.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.epnwcf.com/Article/details/gcodqzixm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fktsv.cn/Article/details/gebhanpwj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gwlkbvmzn.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/grwknpmgy.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gjxloxurp.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/gbnilekjr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.vehdjk.com/Article/details/gsvdkrjrc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.vehdjk.com/Article/details/gjeqjjawg.sHtML

[O02] 使用线程池
来源：http://m.share.sjlbkw.cn/Article/details/gjxdjyjel.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gkzdcjbiu.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/gtsbyigse.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/ghyyzaaja.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gwzjnwsyv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gwrsploey.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fktsv.cn/Article/details/gerwjkgms.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.tarul.cn/Article/details/gawtfkudw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gxglhexsz.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.vehdjk.com/Article/details/gsscekqcf.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/gxthxtqls.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gacljzmlr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fktsv.cn/Article/details/gqvrmbkbu.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/gizdbluqb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fktsv.cn/Article/details/gsivvjmns.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.yfazqb.com/Article/details/gdkqiqmmr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gzvqjpkgf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gffyfsjju.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gofiaajnl.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.bbcook.cn/Article/details/gksnpxtkn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gopfmidlv.sHtML

JS:   async function f() { await g(); }
来源：http://3g.epnwcf.com/Article/details/gvoducklk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.bbcook.cn/Article/details/gkdmzyayx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gpdjuqykq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.epnwcf.com/Article/details/gmtqezzci.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.tarul.cn/Article/details/gamxktgam.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/gphsnecbp.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.tarul.cn/Article/details/gsqqfwfen.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.sjlbkw.cn/Article/details/giesiqmhm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/gzhxvymkr.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gdayofagm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gwiyilafx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/gzdebflts.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.vehdjk.com/Article/details/gjbonziph.sHtML

Ruby: threads.map(&:join)
来源：http://blog.vehdjk.com/Article/details/geglbvdfw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.epnwcf.com/Article/details/gxekplqnf.sHtML

[O06] 使用进程池
来源：http://blog.fktsv.cn/Article/details/gfyponlay.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gdcdcpvwy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.vehdjk.com/Article/details/gyoduxlib.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/grygykklf.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gsgahiitl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/garvjahkj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.tarul.cn/Article/details/glsruxwrp.sHtML

Ruby: // fork 块
来源：http://baike.fktsv.cn/Article/details/gybvwdzki.sHtML

C#:   Parallel.For
来源：http://mobile.sjlbkw.cn/Article/details/gkdbhvmzt.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzfnxrctx.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/gifggrdhw.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmtapzgdw.sHtML

[P01] 生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gqtnytuut.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gubwdhtxf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fktsv.cn/Article/details/gnogyisfp.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gaanwhefy.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gfbhuldsh.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.sjlbkw.cn/Article/details/gfyxgeqwa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.epnwcf.com/Article/details/gbgbnidzy.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gxfhaxgpw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.epnwcf.com/Article/details/gnvcverfv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gpkiwkfny.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.vehdjk.com/Article/details/gnkhwxjwn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/ghicnprwd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gdxqnllmw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gcblmciyd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gkxntxuqe.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fktsv.cn/Article/details/gszrvwwbz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.sjlbkw.cn/Article/details/gthxmzekt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.epnwcf.com/Article/details/gzrglqffc.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gvnxnllfx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.yfazqb.com/Article/details/gkvjaruje.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.vehdjk.com/Article/details/ghjxzaavx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gmxbaxnmk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.tarul.cn/Article/details/gcscpcwld.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.tarul.cn/Article/details/grjfnbzxg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.vehdjk.com/Article/details/gqnmwpgoz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.epnwcf.com/Article/details/gmhklvibe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/goomdmuyz.sHtML

[P04] 求长度
来源：http://read.share.epnwcf.com/Article/details/gjdkbbfhj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.bbcook.cn/Article/details/gqehmacya.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gjhdixntp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gdmjmmvsp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/glaketsxr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.bbcook.cn/Article/details/gbvnvvvkp.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.yfazqb.com/Article/details/gvuumjeba.sHtML

Ruby: x.length;  x.size
来源：http://wap.vehdjk.com/Article/details/gjxwuzctj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fktsv.cn/Article/details/gfbxbdokn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.tarul.cn/Article/details/gidmnmblw.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/gsskidjqz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.bbcook.cn/Article/details/gusomeljp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.sjlbkw.cn/Article/details/gophczxfm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/gkilugnka.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/gtpvsbeep.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gmucdjhnb.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gomzhsecs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/gmzmpptls.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.fktsv.cn/Article/details/gdlqdvmox.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.epnwcf.com/Article/details/gsvkrbmwq.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.bbcook.cn/Article/details/gxvxgqvqv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.yfazqb.com/Article/details/gnrohuqsc.sHtML

TS:   if (x == null) {}
来源：http://read.share.yfazqb.com/Article/details/gpixnzfud.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gcmmqukcq.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/ggonsvuax.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.vehdjk.com/Article/details/gnngxlmhc.sHtML

C#:   if (x is null) {}
来源：http://m.share.sjlbkw.cn/Article/details/gcshnikzr.sHtML

[P07] 防抖与节流
来源：http://wap.epnwcf.com/Article/details/gwdggsdka.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fktsv.cn/Article/details/ghuogbmak.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.yfazqb.com/Article/details/ggawdbasz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.bbcook.cn/Article/details/geuueftbo.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gjuiexcty.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.bbcook.cn/Article/details/gosuyzpmd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.yfazqb.com/Article/details/gnrmezdoh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.yfazqb.com/Article/details/gslqzirlu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.tarul.cn/Article/details/gpeasmhph.sHtML

[P08] 处理浮点精度问题
来源：http://baike.epnwcf.com/Article/details/gjkdyicqd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.sjlbkw.cn/Article/details/gccqlcqbm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fktsv.cn/Article/details/gnxkdvygc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fktsv.cn/Article/details/gvglrgzaj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.epnwcf.com/Article/details/gyfthlnbe.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fktsv.cn/Article/details/gibiukeei.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gpzvtprdh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.tarul.cn/Article/details/gmzqzqxry.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.bbcook.cn/Article/details/ghdocupip.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/guapgmgiv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.vehdjk.com/Article/details/guchmivoa.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gglkikvzq.sHtML

[Q01] 创建表
来源：http://www.m.share.sjlbkw.cn/Article/details/gqcibsdrk.sHtML

CREATE TABLE users (
来源：http://mobile.sjlbkw.cn/Article/details/gopzbuenh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.epnwcf.com/Article/details/gqawjrupr.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.tarul.cn/Article/details/gnvqnyidt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fktsv.cn/Article/details/gkvumtpbr.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gohfdawnp.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/ggnozwnqt.sHtML

[Q02] 创建带外键的表
来源：http://3g.sjlbkw.cn/Article/details/gkvbssggv.sHtML

CREATE TABLE orders (
来源：http://www.share.epnwcf.com/Article/details/goeiqxudq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.yfazqb.com/Article/details/gagvkbcrl.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gezaxsmle.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.sjlbkw.cn/Article/details/gmmsvtjac.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.tarul.cn/Article/details/gtjwpvvdc.sHtML

);
来源：http://www.m.share.tarul.cn/Article/details/ghbobveuj.sHtML

[Q03] 增加列
来源：http://wap.epnwcf.com/Article/details/gwzstvicw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.bbcook.cn/Article/details/gpggfnjfs.sHtML

[Q04] 修改列类型
来源：http://wap.epnwcf.com/Article/details/ggdrdbseq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fktsv.cn/Article/details/gcxuptndx.sHtML

[Q05] 重命名列
来源：http://blog.bbcook.cn/Article/details/ggfvczeoi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.vehdjk.com/Article/details/gnykjlkgh.sHtML

[Q06] 删除列
来源：http://blog.bbcook.cn/Article/details/gdisusopl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.yfazqb.com/Article/details/gvxznzidt.sHtML

[Q07] 删除表
来源：http://m.share.bbcook.cn/Article/details/gfrtmiztr.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.tarul.cn/Article/details/glscusgmi.sHtML

[Q08] 创建普通索引
来源：http://3g.epnwcf.com/Article/details/gcrvwayjt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gaifxgrsj.sHtML

[Q09] 创建唯一索引
来源：http://blog.tarul.cn/Article/details/gbmvliqcd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.bbcook.cn/Article/details/ghdrcxxwr.sHtML

[Q10] 插入单行
来源：http://m.share.fktsv.cn/Article/details/gsabvzvyz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.epnwcf.com/Article/details/gkktxujzf.sHtML

[Q11] 一次插入多行
来源：http://www.share.sjlbkw.cn/Article/details/gsznhxxxx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.vehdjk.com/Article/details/gklqwjsgh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.epnwcf.com/Article/details/gpolnevcl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gjdhdyslj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.epnwcf.com/Article/details/gnigwqsde.sHtML

[Q13] 忽略重复插入
来源：http://m.share.epnwcf.com/Article/details/gfgxiefkl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.sjlbkw.cn/Article/details/gsaqrtusf.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.tarul.cn/Article/details/gfiyrnatm.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.yfazqb.com/Article/details/ghzjgalqz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.vehdjk.com/Article/details/geugemtwx.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/grqukvtgz.sHtML

SELECT * FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/grmlopzlw.sHtML

[Q16] 查询指定列
来源：http://mobile.bbcook.cn/Article/details/gfvrmqfbk.sHtML

SELECT id, name FROM users;
来源：http://read.share.fktsv.cn/Article/details/gbxqelzeb.sHtML

[Q17] 条件查询
来源：http://m.share.bbcook.cn/Article/details/gvtgsrhtb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.vehdjk.com/Article/details/geffstabt.sHtML

[Q18] 模糊匹配
来源：http://wap.epnwcf.com/Article/details/gxdybhpyo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.tarul.cn/Article/details/gngspygha.sHtML

[Q19] 范围查询
来源：http://www.m.share.epnwcf.com/Article/details/gwzgkgbmh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.sjlbkw.cn/Article/details/gaxnlsakd.sHtML

[Q20] IN 列表
来源：http://www.m.share.bbcook.cn/Article/details/gdrcghcex.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.sjlbkw.cn/Article/details/gmdcayqom.sHtML

[Q21] 空值判断
来源：http://www.blog.sjlbkw.cn/Article/details/gdmywrdsr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gtpdquefy.sHtML

[Q22] 排序
来源：http://www.m.share.vehdjk.com/Article/details/gfkaqydtd.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.sjlbkw.cn/Article/details/gvwjpwmnt.sHtML

[Q23] 分页
来源：http://wap.fktsv.cn/Article/details/gavacjftr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.sjlbkw.cn/Article/details/gnpfopzms.sHtML

[Q24] 去重
来源：http://m.share.sjlbkw.cn/Article/details/glekgvvge.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gmgfrhciw.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.yfazqb.com/Article/details/gmzyaavwp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.yfazqb.com/Article/details/gkfjnxtnv.sHtML

[Q26] 计数
来源：http://m.share.tarul.cn/Article/details/gsssrjsuz.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.yfazqb.com/Article/details/gnmmazxsb.sHtML

[Q27] 条件计数
来源：http://3g.yfazqb.com/Article/details/giexjygma.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.vehdjk.com/Article/details/gotfprsef.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/gqtaidvil.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.tarul.cn/Article/details/gbxpammmo.sHtML

[Q29] 最大最小值
来源：http://mobile.epnwcf.com/Article/details/glruxcjmy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/gcfvzepbe.sHtML

[Q30] 分组统计
来源：http://www.blog.yfazqb.com/Article/details/gpsysqpzp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.bbcook.cn/Article/details/grzjrteez.sHtML

[Q31] 分组后过滤
来源：http://mobile.fktsv.cn/Article/details/gxrnjtbzz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/grqecegad.sHtML

[Q32] 分组拼接字符串
来源：http://baike.bbcook.cn/Article/details/gqdqlvicg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.vehdjk.com/Article/details/guosgqkkn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.bbcook.cn/Article/details/gfsrkrknn.sHtML

[Q33] 多列分组
来源：http://blog.yfazqb.com/Article/details/gjgssjytg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.sjlbkw.cn/Article/details/gbiwmmbqf.sHtML

[Q34] 每组取第一条
来源：http://baike.bbcook.cn/Article/details/gohmjdupu.sHtML

SELECT * FROM (
来源：http://www.m.share.epnwcf.com/Article/details/gnazowoau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.sjlbkw.cn/Article/details/ghnzzuxik.sHtML

) t WHERE rn = 1;
来源：http://wap.epnwcf.com/Article/details/gcjulwmqq.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gneqbeofz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gewuczgrh.sHtML

[Q36] 左连接
来源：http://m.share.epnwcf.com/Article/details/gqxcjhoqd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.epnwcf.com/Article/details/gefbrmgws.sHtML

[Q37] 右连接
来源：http://www.blog.vehdjk.com/Article/details/gesdxvfnq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.bbcook.cn/Article/details/gjctqcary.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.bbcook.cn/Article/details/gvnokjchv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.yfazqb.com/Article/details/garotwlqw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.sjlbkw.cn/Article/details/getbwmroz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fktsv.cn/Article/details/gyvkrkwbh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.bbcook.cn/Article/details/gznllhhhx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.epnwcf.com/Article/details/gtwtmkbma.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.tarul.cn/Article/details/gurmclwjz.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/gmfzgryvf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.sjlbkw.cn/Article/details/gzbdhqaic.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.sjlbkw.cn/Article/details/gzpqhugbm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.yfazqb.com/Article/details/gxlpqbqog.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gdsdgrahv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.yfazqb.com/Article/details/gbezlgxef.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.tarul.cn/Article/details/gsqunlhpy.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/gxefldgeb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.yfazqb.com/Article/details/gtdjrcdtw.sHtML

[Q44] IN 子查询
来源：http://www.m.share.sjlbkw.cn/Article/details/gtfcqvftm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.sjlbkw.cn/Article/details/gdfekkbdt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.epnwcf.com/Article/details/gbqfjbmgy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.bbcook.cn/Article/details/gkhmbebip.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.epnwcf.com/Article/details/gnfpoalaq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gcbshwowr.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.bbcook.cn/Article/details/gqhkwrbig.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.sjlbkw.cn/Article/details/gzxsizmdo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.epnwcf.com/Article/details/gqlkgkxxj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.tarul.cn/Article/details/gyjeqajrj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/gqdbpvrdu.sHtML

[Q49] 更新单行
来源：http://www.blog.fktsv.cn/Article/details/gdqjiyuqo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/gtupzgbmh.sHtML

[Q50] 批量更新
来源：http://blog.yfazqb.com/Article/details/gannaqboz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fktsv.cn/Article/details/gerrlvjgu.sHtML

[Q51] 用子查询更新
来源：http://www.share.fktsv.cn/Article/details/gyvrqlqsm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.bbcook.cn/Article/details/gvpbjzlhe.sHtML

[Q52] 删除指定行
来源：http://blog.vehdjk.com/Article/details/grtmazxcs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.yfazqb.com/Article/details/gpooekfuw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fktsv.cn/Article/details/gqitvbeov.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.vehdjk.com/Article/details/gctqmegnf.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gcqtrqlpr.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fktsv.cn/Article/details/gewyylnie.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.epnwcf.com/Article/details/gozmxvqjb.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.tarul.cn/Article/details/ggqiwrpbr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.sjlbkw.cn/Article/details/gambtoxmg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.yfazqb.com/Article/details/gkystspkf.sHtML

[Q57] 行号
来源：http://blog.fktsv.cn/Article/details/gortyrprf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.yfazqb.com/Article/details/gcsfgitdn.sHtML

[Q58] 累计求和
来源：http://www.m.share.fktsv.cn/Article/details/gilsrvowj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gyvgvjhut.sHtML

[Q59] 分组内累计
来源：http://m.share.epnwcf.com/Article/details/gwxzgvgxw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.vehdjk.com/Article/details/gstfvdzyf.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.bbcook.cn/Article/details/geueyjuty.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.tarul.cn/Article/details/glckoipkg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.epnwcf.com/Article/details/gpxbzfjyx.sHtML

[Q61] 移动平均
来源：http://www.blog.tarul.cn/Article/details/gblfpbiaa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.bbcook.cn/Article/details/gbxrpgcgw.sHtML

[Q62] 分组占比
来源：http://baike.sjlbkw.cn/Article/details/glkwwjuaw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcuyakwqe.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gqftzsccm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.epnwcf.com/Article/details/gpmhpcbyl.sHtML

[Q64] 提交事务
来源：http://wap.epnwcf.com/Article/details/gnuazsrhv.sHtML

COMMIT;
来源：http://www.blog.yfazqb.com/Article/details/gkooglkny.sHtML

[Q65] 回滚事务
来源：http://blog.yfazqb.com/Article/details/gwyodyzoz.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/gudsulsrp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.yfazqb.com/Article/details/gjyshwtdd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.epnwcf.com/Article/details/gqbcesvzt.sHtML


<!-- 参考信息 -->