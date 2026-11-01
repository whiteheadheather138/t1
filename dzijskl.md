代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gozznkorx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.yfazqb.com/Article/details/gszskcgqq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gjddeskgn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.bbcook.cn/Article/details/gxopywxlc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gccufjkur.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/ghwbtbunv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.tarul.cn/Article/details/gzbuuzlnh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/guetqkpeu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/grmlacrnf.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gbzygkexd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtvyvzrkz.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/glaybqlor.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/gkpbcecds.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fktsv.cn/Article/details/gaqtskeej.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.yfazqb.com/Article/details/gcuxggtfi.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gaubiptmq.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.vehdjk.com/Article/details/gqigigrst.sHtML

Go:   go f()
来源：http://www.blog.vehdjk.com/Article/details/gtrihtmvi.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/ggwkwllii.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.yfazqb.com/Article/details/gqjnvubzg.sHtML

[O02] 使用线程池
来源：http://wap.tarul.cn/Article/details/gpvjdfapc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/guwgpkxdr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/goawnnnfk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gsgsbgfmw.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gtmcvchdx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.tarul.cn/Article/details/gvndkzhkq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/gnnhvemto.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/gwvsagbux.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.epnwcf.com/Article/details/gopigjdhj.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.bbcook.cn/Article/details/grdvsbyyb.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gwufvcehv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fktsv.cn/Article/details/gllfqdmyv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/grgetcrfe.sHtML

TS:   // 同 JS
来源：http://www.m.share.bbcook.cn/Article/details/gnbhjrubr.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.sjlbkw.cn/Article/details/gkmfxhobp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gdnwokqti.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/gdtwixrqk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/gcetqxgzh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gewgoukyx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gedweabmp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/ghchkrhry.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.bbcook.cn/Article/details/gsdftewik.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gumkeedoa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.bbcook.cn/Article/details/gksiwdxnb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.tarul.cn/Article/details/gapmxatyo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gejefkmhr.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/giuylbhym.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gnbdjqeum.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gitbmmhph.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.bbcook.cn/Article/details/gbmngfipo.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/groytvgrk.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gbhfajelg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/giinddzlf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.yfazqb.com/Article/details/gmkdbxgoz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.tarul.cn/Article/details/gymmzosda.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fktsv.cn/Article/details/gnkukjmjj.sHtML

[O06] 使用进程池
来源：http://www.blog.tarul.cn/Article/details/guwhyccnk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/gxpquiatf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.vehdjk.com/Article/details/gyxujedkd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gbiizvkob.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gcedjbptm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.epnwcf.com/Article/details/gtuatwrki.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gaiplawib.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gparbkemq.sHtML

C#:   Parallel.For
来源：http://www.blog.bbcook.cn/Article/details/glwbdszgh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gobhetdjm.sHtML

P. 常用工具函数
来源：http://m.share.sjlbkw.cn/Article/details/gqcbwafoz.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gxjzfdzpk.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gueecdeie.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/guawygwwx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.bbcook.cn/Article/details/gwmtilicu.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gglvcrgjm.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.sjlbkw.cn/Article/details/gtovpjxir.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gcjpwriyo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gvzgacdqt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.tarul.cn/Article/details/gtthuvzre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/giodxhowu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqjhqbqp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.bbcook.cn/Article/details/gcaykhbga.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gujjdlfdb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gymemoxlz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.yfazqb.com/Article/details/gajsycvpx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/gdaqeithi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.tarul.cn/Article/details/grolbpvjg.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.vehdjk.com/Article/details/gjfjwjlpi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.bbcook.cn/Article/details/gqcevfyvw.sHtML

[P03] 生成短随机字符串
来源：http://baike.fktsv.cn/Article/details/gtqgcipmh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fktsv.cn/Article/details/gbmbugben.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.yfazqb.com/Article/details/gpgnghdgf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.bbcook.cn/Article/details/gpqsiiayn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.sjlbkw.cn/Article/details/gxpejmexa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gayzizmme.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/gtgwkcsyo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gqvnpfccv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gexlxluhw.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/gbxgfsdle.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.bbcook.cn/Article/details/gykxpwnuq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.vehdjk.com/Article/details/gqocubqpn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.yfazqb.com/Article/details/glckypstw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.sjlbkw.cn/Article/details/gbkwqsfwh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/goolnemgf.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gzcbufuew.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.sjlbkw.cn/Article/details/gtoriqhcn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.vehdjk.com/Article/details/gccpuzzig.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gxzgvbxal.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gqcfflynl.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.vehdjk.com/Article/details/gqxbyccnd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.bbcook.cn/Article/details/gfdvtrqje.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gfekjigta.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.tarul.cn/Article/details/grcilbbdm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.tarul.cn/Article/details/geqvphhnw.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gajnvqjpb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gcfpmaawi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/glesalrcr.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.tarul.cn/Article/details/gdkgevcie.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.bbcook.cn/Article/details/gatlbwfhk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fktsv.cn/Article/details/gtwcbkfkr.sHtML

TS:   if (x == null) {}
来源：http://baike.sjlbkw.cn/Article/details/gowhswpxu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.tarul.cn/Article/details/gwkcmilns.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gaeoycrcp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/ggmovgknj.sHtML

C#:   if (x is null) {}
来源：http://3g.fktsv.cn/Article/details/gaquinnek.sHtML

[P07] 防抖与节流
来源：http://baike.yfazqb.com/Article/details/gqctspwtq.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gzutmladh.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.tarul.cn/Article/details/gzynjamrn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gxrwnvcjr.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.yfazqb.com/Article/details/gtaussbny.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.yfazqb.com/Article/details/gxawxditk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.vehdjk.com/Article/details/ghxnarvsj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gpjzytgjr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fktsv.cn/Article/details/gfsswyvkm.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fktsv.cn/Article/details/guyujilne.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.sjlbkw.cn/Article/details/gdkghzzgs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.vehdjk.com/Article/details/gfrbwynlm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/goedawbym.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.tarul.cn/Article/details/gbcxbrwcv.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gpqfujobb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fktsv.cn/Article/details/gbzsagzut.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.sjlbkw.cn/Article/details/gpojrivtj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gwxxekxxs.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/geicrjxrf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.bbcook.cn/Article/details/gpgocixth.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/grcllejjj.sHtML

[Q01] 创建表
来源：http://read.share.bbcook.cn/Article/details/gusiavyod.sHtML

CREATE TABLE users (
来源：http://wap.tarul.cn/Article/details/gswtjwzez.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.epnwcf.com/Article/details/govdavxvc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fktsv.cn/Article/details/gkgfbznca.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.fktsv.cn/Article/details/gvdlwojom.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.bbcook.cn/Article/details/gewjouabp.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gbjxqkrux.sHtML

[Q02] 创建带外键的表
来源：http://mobile.yfazqb.com/Article/details/gpojbxxwa.sHtML

CREATE TABLE orders (
来源：http://wap.yfazqb.com/Article/details/gmwhuhgqu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.bbcook.cn/Article/details/gnvdxcbgg.sHtML

user_id INT NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/gkchzdnam.sHtML

amount DECIMAL(10, 2),
来源：http://wap.vehdjk.com/Article/details/gmaitpuoo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/grqlnydmt.sHtML

);
来源：http://baike.vehdjk.com/Article/details/ggkiuxtoz.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gzypsgkvl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.sjlbkw.cn/Article/details/gsqjztyfo.sHtML

[Q04] 修改列类型
来源：http://www.blog.tarul.cn/Article/details/gnnykwurq.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.tarul.cn/Article/details/gmizvhmax.sHtML

[Q05] 重命名列
来源：http://blog.fktsv.cn/Article/details/gzaxogakl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.yfazqb.com/Article/details/gyomknhwg.sHtML

[Q06] 删除列
来源：http://3g.vehdjk.com/Article/details/gqfvcvpqq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/goqqicwlr.sHtML

[Q07] 删除表
来源：http://baike.epnwcf.com/Article/details/gcdxzgfbf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.bbcook.cn/Article/details/gehmulbvy.sHtML

[Q08] 创建普通索引
来源：http://read.share.yfazqb.com/Article/details/gbalpmodx.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fktsv.cn/Article/details/ghxdsaxqq.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fktsv.cn/Article/details/gvzuonral.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gywvsavgp.sHtML

[Q10] 插入单行
来源：http://mobile.fktsv.cn/Article/details/gptlkevxp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gqqixnwii.sHtML

[Q11] 一次插入多行
来源：http://www.share.tarul.cn/Article/details/grrjrrocv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.bbcook.cn/Article/details/gkdwsnxev.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/grfrnkfya.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.sjlbkw.cn/Article/details/ghwpepijs.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.tarul.cn/Article/details/gffgfxobr.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/gkxvmozax.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.epnwcf.com/Article/details/gkjsyhibd.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gbxsnhegd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.yfazqb.com/Article/details/giwzlrqsm.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.vehdjk.com/Article/details/ggffmgefl.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/ghupkkuga.sHtML

SELECT * FROM users;
来源：http://wap.vehdjk.com/Article/details/gkqlwoldb.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/gukprmoqh.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gfnssoplk.sHtML

[Q17] 条件查询
来源：http://blog.bbcook.cn/Article/details/gslhlkrek.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.sjlbkw.cn/Article/details/gwzhqvxlo.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/gfqymhkso.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.tarul.cn/Article/details/gpnhezatl.sHtML

[Q19] 范围查询
来源：http://mobile.bbcook.cn/Article/details/grppioton.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.fktsv.cn/Article/details/gpyozfart.sHtML

[Q20] IN 列表
来源：http://www.blog.bbcook.cn/Article/details/ggbkrqzfv.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.vehdjk.com/Article/details/gtuaymtgk.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/gmiurvdlo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.epnwcf.com/Article/details/gdxmopnfe.sHtML

[Q22] 排序
来源：http://3g.vehdjk.com/Article/details/gmlmlfhmw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fktsv.cn/Article/details/grzfkhxzi.sHtML

[Q23] 分页
来源：http://wap.epnwcf.com/Article/details/ghfifbqxf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.epnwcf.com/Article/details/gzhribeti.sHtML

[Q24] 去重
来源：http://mobile.tarul.cn/Article/details/gqnwbyqgu.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.yfazqb.com/Article/details/giupscggy.sHtML

[Q25] 只取前 N 条
来源：http://read.share.epnwcf.com/Article/details/gcugwwjgn.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.yfazqb.com/Article/details/gbabhecbg.sHtML

[Q26] 计数
来源：http://mobile.vehdjk.com/Article/details/gpfqdysda.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.vehdjk.com/Article/details/guzkudvvh.sHtML

[Q27] 条件计数
来源：http://wap.tarul.cn/Article/details/gvbqoyefh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.tarul.cn/Article/details/glovjntpj.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gxopelqjk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.yfazqb.com/Article/details/gvvamzoen.sHtML

[Q29] 最大最小值
来源：http://3g.sjlbkw.cn/Article/details/gtajpzyzm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.tarul.cn/Article/details/gfpedksua.sHtML

[Q30] 分组统计
来源：http://www.share.vehdjk.com/Article/details/gmoiqarbt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.sjlbkw.cn/Article/details/gablcezyi.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gqwgjboem.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.sjlbkw.cn/Article/details/gnzoyrhgz.sHtML

[Q32] 分组拼接字符串
来源：http://3g.yfazqb.com/Article/details/gcuxbhjcm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.tarul.cn/Article/details/glyvzndvh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.epnwcf.com/Article/details/gdrfgzhgm.sHtML

[Q33] 多列分组
来源：http://www.share.bbcook.cn/Article/details/grkmzfqzr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.epnwcf.com/Article/details/gfunzrdfa.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gctvssqib.sHtML

SELECT * FROM (
来源：http://m.share.vehdjk.com/Article/details/gsaysiqvu.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fktsv.cn/Article/details/gfprzyczc.sHtML

) t WHERE rn = 1;
来源：http://3g.yfazqb.com/Article/details/gylmktzez.sHtML

[Q35] 内连接
来源：http://mobile.sjlbkw.cn/Article/details/gdonrrldx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.vehdjk.com/Article/details/gqfpzvano.sHtML

[Q36] 左连接
来源：http://wap.tarul.cn/Article/details/ghhmrrtfl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gsbohdxlp.sHtML

[Q37] 右连接
来源：http://blog.fktsv.cn/Article/details/gtjdbgmvp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gafkfnzao.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.epnwcf.com/Article/details/ghaewgeqy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gggzbbpfw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.epnwcf.com/Article/details/glwdvkwrr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.tarul.cn/Article/details/ggvmghuax.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fktsv.cn/Article/details/gcyljibaf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.vehdjk.com/Article/details/gfmspplsm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.epnwcf.com/Article/details/gyccoipuj.sHtML

[Q41] 多表连接
来源：http://blog.tarul.cn/Article/details/gbtovfueu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.epnwcf.com/Article/details/gjewsdcch.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.tarul.cn/Article/details/goyehuyon.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.epnwcf.com/Article/details/gfmuubqui.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/gfccblmsk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.sjlbkw.cn/Article/details/gulkghjhl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/gvybzmdfz.sHtML

[Q43] 标量子查询
来源：http://wap.fktsv.cn/Article/details/glefuueiz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.sjlbkw.cn/Article/details/grmpimbtr.sHtML

[Q44] IN 子查询
来源：http://www.share.epnwcf.com/Article/details/gmfusrogm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.vehdjk.com/Article/details/gqlhbsfeo.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fktsv.cn/Article/details/gtyvtoqsf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fktsv.cn/Article/details/gisyuzqzd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fktsv.cn/Article/details/gfsbqeqta.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.tarul.cn/Article/details/gdqvfalzv.sHtML

[Q47] 与平均值比较
来源：http://blog.sjlbkw.cn/Article/details/gpcjwpqdj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.yfazqb.com/Article/details/ghafrfxiq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gvnahcjhr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.epnwcf.com/Article/details/gbyiycscz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.sjlbkw.cn/Article/details/gazsdfjcb.sHtML

[Q49] 更新单行
来源：http://www.m.share.tarul.cn/Article/details/gwowsexnh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.vehdjk.com/Article/details/gudrkksev.sHtML

[Q50] 批量更新
来源：http://www.blog.bbcook.cn/Article/details/gaimscpip.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.vehdjk.com/Article/details/gzbixgojl.sHtML

[Q51] 用子查询更新
来源：http://baike.tarul.cn/Article/details/grzdlftnj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/girxtjccc.sHtML

[Q52] 删除指定行
来源：http://mobile.sjlbkw.cn/Article/details/gjoidvwyo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/ggtybzsew.sHtML

[Q53] 按条件删除
来源：http://blog.yfazqb.com/Article/details/gfjznrklq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/grnhglcpt.sHtML

[Q54] 清空表
来源：http://3g.tarul.cn/Article/details/goxtmrqbo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.vehdjk.com/Article/details/gywstwfqv.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.tarul.cn/Article/details/gwqdprwdu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.sjlbkw.cn/Article/details/ggwgyzsnu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.tarul.cn/Article/details/guurkdyau.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.tarul.cn/Article/details/gkqttwluh.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/gjoidbnpc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.epnwcf.com/Article/details/ghuvbcapo.sHtML

[Q58] 累计求和
来源：http://read.share.fktsv.cn/Article/details/gblhzjqtm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.tarul.cn/Article/details/gdganzdmc.sHtML

[Q59] 分组内累计
来源：http://www.m.share.yfazqb.com/Article/details/gvdhjepte.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.bbcook.cn/Article/details/gydnbynox.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fktsv.cn/Article/details/gwdtqyktv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.yfazqb.com/Article/details/gspctsaev.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.epnwcf.com/Article/details/gkiafxpeb.sHtML

[Q61] 移动平均
来源：http://wap.tarul.cn/Article/details/gslkqvnrm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gwpglmuki.sHtML

[Q62] 分组占比
来源：http://blog.yfazqb.com/Article/details/guxbjmbya.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.bbcook.cn/Article/details/gxnyvvkih.sHtML

[Q63] 开启事务
来源：http://www.m.share.fktsv.cn/Article/details/gurlohxgp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.yfazqb.com/Article/details/gjnmqcowp.sHtML

[Q64] 提交事务
来源：http://www.share.vehdjk.com/Article/details/ggotkxvou.sHtML

COMMIT;
来源：http://www.m.share.yfazqb.com/Article/details/gnkaopuvl.sHtML

[Q65] 回滚事务
来源：http://m.share.bbcook.cn/Article/details/gighoujrt.sHtML

ROLLBACK;
来源：http://3g.bbcook.cn/Article/details/gqwatwyfx.sHtML

[Q66] 行锁查询
来源：http://read.share.yfazqb.com/Article/details/gertjcqmk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fktsv.cn/Article/details/ggiuhacgw.sHtML

[Q67] 设置隔离级别
来源：http://blog.bbcook.cn/Article/details/gqmzpwucm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fktsv.cn/Article/details/gggboiakr.sHtML

[Q68] 保存点
来源：http://www.share.tarul.cn/Article/details/gjilwnxjk.sHtML

SAVEPOINT sp1;
来源：http://blog.vehdjk.com/Article/details/gwsvkrgxn.sHtML


<!-- 参考信息 -->