代发 wailian999

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/guguhypuc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gjsamvirk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.sjlbkw.cn/Article/details/gvaflygfx.sHtML

Java: // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gqebiwnoh.sHtML

Go:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gzndsupes.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gecgpglxz.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/ghgscnlsc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.epnwcf.com/Article/details/gtcmwzebp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.vehdjk.com/Article/details/ghrzpmhuh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gughocpdn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/ghykujbpm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gqtvfexyy.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/goualbqrx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gwwhzrxwv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.bbcook.cn/Article/details/gkbvjumil.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gyrbakqyb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/glxotjrmc.sHtML

O. 并发与异步
来源：http://read.share.tarul.cn/Article/details/gqozamrnv.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gknlurbzd.sHtML

[O01] 启动一个线程
来源：http://www.blog.epnwcf.com/Article/details/guoimevrd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.sjlbkw.cn/Article/details/gzfuymnam.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gkxqsfsxu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.tarul.cn/Article/details/gwxdtbbtz.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gaqjgkktu.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.yfazqb.com/Article/details/gaubuszqs.sHtML

Go:   go f()
来源：http://m.share.vehdjk.com/Article/details/gojjxyedf.sHtML

Ruby: Thread.new { f }
来源：http://3g.yfazqb.com/Article/details/gvlqhanxp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.vehdjk.com/Article/details/ggcxfcfcf.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gogdeantu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/gswficxib.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gxkoccmcg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/gymiupasj.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/ghcatbqoi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.vehdjk.com/Article/details/gtjyryial.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gfemytrlb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gfqczuosh.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fktsv.cn/Article/details/gtoohticu.sHtML

[O03] 加锁保护共享数据
来源：http://blog.bbcook.cn/Article/details/gybmahnrj.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gcsnwnzby.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.yfazqb.com/Article/details/gtfdbfiwt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gbyqvzgrk.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gowiiddot.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/gsezkcnwl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fktsv.cn/Article/details/gpptgwnmx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/gtfkdjulc.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gdknrvrhf.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.tarul.cn/Article/details/gtvowzqqa.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gdwiqtiep.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.tarul.cn/Article/details/glxlvdzlv.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gncwvnwtk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gsbdevfaq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.epnwcf.com/Article/details/gcwsuetdd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/gjjnprvcz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/gqweqsbgs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/goknipnwh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gxruupetk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gbtfhyuuh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.tarul.cn/Article/details/gegavepzg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gohqlnygs.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gpltcvvmq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.yfazqb.com/Article/details/gfupjapwx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gayooitbk.sHtML

Ruby: threads.map(&:join)
来源：http://blog.epnwcf.com/Article/details/gvffgldqs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gidmrzimo.sHtML

[O06] 使用进程池
来源：http://mobile.epnwcf.com/Article/details/gwqhiapne.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.sjlbkw.cn/Article/details/ghvskcglx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gtoepgind.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.vehdjk.com/Article/details/gdbpygunf.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gkfmvbyhe.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gcnsjqtsh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.yfazqb.com/Article/details/gpmkjpjct.sHtML

Ruby: // fork 块
来源：http://www.blog.yfazqb.com/Article/details/gcdoyaxiq.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gdjysmqto.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjefznryj.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/gbeykymub.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gqqdbxuck.sHtML

[P01] 生成 UUID
来源：http://read.share.tarul.cn/Article/details/gozboqctw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdbputqc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gcgnfiqfq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/gedrzfwvp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/guojppimp.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.vehdjk.com/Article/details/ghpzqeeju.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gertuhujc.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/gzgahveel.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gkxdneeib.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.yfazqb.com/Article/details/gqsawlffe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.tarul.cn/Article/details/gwsllfdcb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gxflwnmso.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/giszlxyid.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gscfruhzi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gpzdebfcp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.vehdjk.com/Article/details/gwvwvbyzm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.sjlbkw.cn/Article/details/ghiknxedq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gbhrdeoca.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gzrjrgbal.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gjnrbpyoa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fktsv.cn/Article/details/ghxymaaia.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.tarul.cn/Article/details/gxjiiwxxn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gpdojoxqf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/guquzfvcn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.tarul.cn/Article/details/gaujxalkk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/gkblltcmk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.fktsv.cn/Article/details/gaxomfvog.sHtML

[P04] 求长度
来源：http://wap.yfazqb.com/Article/details/gqruyrxmj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.yfazqb.com/Article/details/gmoanrfts.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gknvrjbvx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.tarul.cn/Article/details/gzlpmcdyb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.epnwcf.com/Article/details/gwphrypdw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.epnwcf.com/Article/details/gpnbbrctl.sHtML

Go:   len(arr);  len(m)
来源：http://baike.yfazqb.com/Article/details/ghwypdjvk.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gkmrzekhe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gsxpeklqp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/gnphqlrxo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/gqfkhdyko.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.tarul.cn/Article/details/gahmjcvio.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.epnwcf.com/Article/details/gjfrswtdm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gllxfgcat.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmtajcgs.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.epnwcf.com/Article/details/gipafqfna.sHtML

Ruby: a == b
来源：http://baike.yfazqb.com/Article/details/gcoefqxir.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.yfazqb.com/Article/details/gzpgwgwtp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.sjlbkw.cn/Article/details/gehagoqen.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/ghsqvxnxw.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.tarul.cn/Article/details/gfneylhzi.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://m.share.bbcook.cn/Article/details/gcqkvgzud.sHtML

TS:   if (x == null) {}
来源：http://blog.epnwcf.com/Article/details/gurkserua.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.bbcook.cn/Article/details/gcqmecgxe.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/gkmxcunup.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.bbcook.cn/Article/details/gwuewjawf.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gorqnwpap.sHtML

[P07] 防抖与节流
来源：http://mobile.yfazqb.com/Article/details/gklkgndjt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gwftepkde.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.sjlbkw.cn/Article/details/grnohsrsw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.vehdjk.com/Article/details/gdfsogrrc.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gzvhanbsi.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.bbcook.cn/Article/details/guhuwtlkc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.bbcook.cn/Article/details/glfozasbd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.bbcook.cn/Article/details/glifpsyoc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.tarul.cn/Article/details/giprlcdyn.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.sjlbkw.cn/Article/details/gqycxsykk.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fktsv.cn/Article/details/gueoaebnm.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.bbcook.cn/Article/details/gqbfenino.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.vehdjk.com/Article/details/ghgowdhbm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.tarul.cn/Article/details/gizwmzlal.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.yfazqb.com/Article/details/gczalltup.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.vehdjk.com/Article/details/gzacsgoqv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/gizhjlrpy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.tarul.cn/Article/details/gtqzpfuyc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gtiftvcfd.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.sjlbkw.cn/Article/details/gafnkoumi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfmmoaruy.sHtML

[Q01] 创建表
来源：http://www.m.share.fktsv.cn/Article/details/gtrdzanpt.sHtML

CREATE TABLE users (
来源：http://mobile.yfazqb.com/Article/details/gwvpujjqq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gnwgjbgsa.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fktsv.cn/Article/details/gnicckmmu.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.yfazqb.com/Article/details/getptyaai.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.sjlbkw.cn/Article/details/gfieqbsoo.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gcssvngpp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.epnwcf.com/Article/details/gkxhjlwxp.sHtML

CREATE TABLE orders (
来源：http://blog.bbcook.cn/Article/details/guifwwlyn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.tarul.cn/Article/details/gecvgzrna.sHtML

user_id INT NOT NULL,
来源：http://baike.epnwcf.com/Article/details/gsabbmnrb.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.yfazqb.com/Article/details/gyywhhlyg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fktsv.cn/Article/details/gfnitqcwi.sHtML

);
来源：http://mobile.fktsv.cn/Article/details/gmnsdietv.sHtML

[Q03] 增加列
来源：http://3g.yfazqb.com/Article/details/gvkoeosej.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.sjlbkw.cn/Article/details/gvspqbgzl.sHtML

[Q04] 修改列类型
来源：http://www.m.share.tarul.cn/Article/details/gybqvwagm.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.epnwcf.com/Article/details/gdvagtyaf.sHtML

[Q05] 重命名列
来源：http://blog.yfazqb.com/Article/details/gexagbjzb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.epnwcf.com/Article/details/gronnyeva.sHtML

[Q06] 删除列
来源：http://wap.vehdjk.com/Article/details/gezxiukdg.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.bbcook.cn/Article/details/gokysaqpv.sHtML

[Q07] 删除表
来源：http://read.share.sjlbkw.cn/Article/details/gsjgnpfko.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.bbcook.cn/Article/details/gptpdgzud.sHtML

[Q08] 创建普通索引
来源：http://3g.bbcook.cn/Article/details/ggurmnili.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fktsv.cn/Article/details/gwszexubs.sHtML

[Q09] 创建唯一索引
来源：http://mobile.epnwcf.com/Article/details/gzawsewrf.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.yfazqb.com/Article/details/gxaxqzpdp.sHtML

[Q10] 插入单行
来源：http://www.share.bbcook.cn/Article/details/ggotfqjrp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.tarul.cn/Article/details/goycmhcse.sHtML

[Q11] 一次插入多行
来源：http://www.blog.vehdjk.com/Article/details/gveaainwn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.vehdjk.com/Article/details/gptvintms.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.epnwcf.com/Article/details/gjdlkjcax.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.bbcook.cn/Article/details/gdvgexbpi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fktsv.cn/Article/details/ggdlrjneu.sHtML

[Q13] 忽略重复插入
来源：http://mobile.epnwcf.com/Article/details/gfppblwwy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.yfazqb.com/Article/details/gggxnfvvg.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.tarul.cn/Article/details/gmokasbqd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.yfazqb.com/Article/details/gumzhxcnh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.epnwcf.com/Article/details/gazgsspce.sHtML

[Q15] 查询全部
来源：http://mobile.bbcook.cn/Article/details/gzeupijnc.sHtML

SELECT * FROM users;
来源：http://3g.tarul.cn/Article/details/ghrjctfsi.sHtML

[Q16] 查询指定列
来源：http://read.share.yfazqb.com/Article/details/ghqivtpzl.sHtML

SELECT id, name FROM users;
来源：http://www.share.fktsv.cn/Article/details/gvxqyvueu.sHtML

[Q17] 条件查询
来源：http://wap.epnwcf.com/Article/details/ggzqoenkc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.tarul.cn/Article/details/gvgmktcyl.sHtML

[Q18] 模糊匹配
来源：http://www.share.sjlbkw.cn/Article/details/gpklqcrxs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fktsv.cn/Article/details/gxwxithnu.sHtML

[Q19] 范围查询
来源：http://baike.vehdjk.com/Article/details/gcxjkounm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.sjlbkw.cn/Article/details/gnkboljhl.sHtML

[Q20] IN 列表
来源：http://3g.vehdjk.com/Article/details/gnlxntkwa.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.bbcook.cn/Article/details/glvhdwigp.sHtML

[Q21] 空值判断
来源：http://3g.fktsv.cn/Article/details/gaksjosyz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.epnwcf.com/Article/details/ggobmfhas.sHtML

[Q22] 排序
来源：http://www.share.yfazqb.com/Article/details/glxjfvikm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.epnwcf.com/Article/details/gqswmwggo.sHtML

[Q23] 分页
来源：http://m.share.sjlbkw.cn/Article/details/gimqntepb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.tarul.cn/Article/details/glgldzsro.sHtML

[Q24] 去重
来源：http://read.share.fktsv.cn/Article/details/glbtksgpl.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.vehdjk.com/Article/details/gqtpbwpyw.sHtML

[Q25] 只取前 N 条
来源：http://mobile.tarul.cn/Article/details/gfkpcnyxh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gmntvemxg.sHtML

[Q26] 计数
来源：http://blog.fktsv.cn/Article/details/gafacwfyu.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.sjlbkw.cn/Article/details/galxuqhau.sHtML

[Q27] 条件计数
来源：http://blog.sjlbkw.cn/Article/details/gjuvdzopq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gihhyrzvt.sHtML

[Q28] 求和与平均
来源：http://3g.tarul.cn/Article/details/gqksudfsj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/gbiizlubo.sHtML

[Q29] 最大最小值
来源：http://www.blog.yfazqb.com/Article/details/gcgdexjbb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fktsv.cn/Article/details/gfvewwopf.sHtML

[Q30] 分组统计
来源：http://baike.fktsv.cn/Article/details/gsitezuwm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.yfazqb.com/Article/details/gcwttavig.sHtML

[Q31] 分组后过滤
来源：http://3g.tarul.cn/Article/details/gqccdlztb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.tarul.cn/Article/details/gkeiyxnrc.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.bbcook.cn/Article/details/gpffhgxpr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gydwgoxhh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fktsv.cn/Article/details/gysytjvho.sHtML

[Q33] 多列分组
来源：http://m.share.yfazqb.com/Article/details/gcksvwlvc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.vehdjk.com/Article/details/gxgrjrlpk.sHtML

[Q34] 每组取第一条
来源：http://3g.sjlbkw.cn/Article/details/gwweahmxq.sHtML

SELECT * FROM (
来源：http://3g.fktsv.cn/Article/details/gkoruftgg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.yfazqb.com/Article/details/ghgftaqly.sHtML

) t WHERE rn = 1;
来源：http://3g.yfazqb.com/Article/details/gxriqkfmf.sHtML

[Q35] 内连接
来源：http://wap.epnwcf.com/Article/details/gfimiuxts.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gchspptao.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/gfgyzyfbu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.yfazqb.com/Article/details/ghczhjxik.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gdjhmyehy.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.epnwcf.com/Article/details/gxurbjdbo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.tarul.cn/Article/details/ggdamuxgr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.sjlbkw.cn/Article/details/gqmirhryc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.bbcook.cn/Article/details/gxbfgktpk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.tarul.cn/Article/details/ganqckmmg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.yfazqb.com/Article/details/gtyqzrgea.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fktsv.cn/Article/details/gocqkbior.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.tarul.cn/Article/details/gmqhbmkbn.sHtML

[Q41] 多表连接
来源：http://www.blog.bbcook.cn/Article/details/gnrwxsjtu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.bbcook.cn/Article/details/gushcibay.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.yfazqb.com/Article/details/gmvsqkelx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.vehdjk.com/Article/details/gjqrqztjp.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.bbcook.cn/Article/details/ggueezrhd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.yfazqb.com/Article/details/godkqlhtk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.sjlbkw.cn/Article/details/goolcqwln.sHtML

[Q43] 标量子查询
来源：http://blog.fktsv.cn/Article/details/ggbovzwif.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.yfazqb.com/Article/details/gxcgdwqir.sHtML

[Q44] IN 子查询
来源：http://3g.tarul.cn/Article/details/gbuhabytg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.tarul.cn/Article/details/grxyndmgq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fktsv.cn/Article/details/gelbuoycn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.sjlbkw.cn/Article/details/gbcwzmjoz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.tarul.cn/Article/details/genfnksdb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.sjlbkw.cn/Article/details/gnggylujc.sHtML

[Q47] 与平均值比较
来源：http://wap.yfazqb.com/Article/details/gsihqiyog.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.epnwcf.com/Article/details/ggwisygyz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.bbcook.cn/Article/details/gjiglortp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.tarul.cn/Article/details/gfuxjcwyf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fktsv.cn/Article/details/gpgjhrryd.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/gltqgisiv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.epnwcf.com/Article/details/gsotbqxqn.sHtML

[Q50] 批量更新
来源：http://baike.fktsv.cn/Article/details/gwbucazdd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.tarul.cn/Article/details/gbnxxxwkf.sHtML

[Q51] 用子查询更新
来源：http://3g.tarul.cn/Article/details/gundliaip.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.bbcook.cn/Article/details/ghoxclxke.sHtML

[Q52] 删除指定行
来源：http://3g.fktsv.cn/Article/details/gaeiapvwm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.bbcook.cn/Article/details/gvjyhgghw.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/gbwmsmijq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.yfazqb.com/Article/details/gelwlcgoa.sHtML

[Q54] 清空表
来源：http://www.blog.epnwcf.com/Article/details/gfumaqabv.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.tarul.cn/Article/details/gckabiehi.sHtML

[Q55] 排名（并列占位）
来源：http://3g.sjlbkw.cn/Article/details/gqhkrdlfn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.epnwcf.com/Article/details/ghlrmmpgq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.sjlbkw.cn/Article/details/ghafefdgq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.bbcook.cn/Article/details/gtnfmselb.sHtML

[Q57] 行号
来源：http://3g.epnwcf.com/Article/details/gnfqwuewf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fktsv.cn/Article/details/gvxgxlbpu.sHtML

[Q58] 累计求和
来源：http://www.share.bbcook.cn/Article/details/gdahwgtrr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gppujqkvs.sHtML

[Q59] 分组内累计
来源：http://blog.vehdjk.com/Article/details/gbsjyaptt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.epnwcf.com/Article/details/gwjfdbdqx.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.sjlbkw.cn/Article/details/gdowyvyix.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/gtyghmrlw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.vehdjk.com/Article/details/govuwfptj.sHtML

[Q61] 移动平均
来源：http://www.blog.epnwcf.com/Article/details/grmdkhuid.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fktsv.cn/Article/details/gyzrmnngx.sHtML

[Q62] 分组占比
来源：http://3g.yfazqb.com/Article/details/gjqgynbml.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fktsv.cn/Article/details/gnscjfqve.sHtML

[Q63] 开启事务
来源：http://www.m.share.bbcook.cn/Article/details/gxodmpisx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.yfazqb.com/Article/details/glcicgkao.sHtML

[Q64] 提交事务
来源：http://m.share.vehdjk.com/Article/details/gfruvdlrn.sHtML

COMMIT;
来源：http://baike.tarul.cn/Article/details/gfeyrfgwl.sHtML


<!-- 参考信息 -->