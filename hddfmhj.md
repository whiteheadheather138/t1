代发 wailian999

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gweryytyn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gamthkjza.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/ggbgkkxfa.sHtML

Java: // 手写递归
来源：http://3g.epnwcf.com/Article/details/gpqgmryib.sHtML

Go:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gugyppcjc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gpuovtdsa.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gkroktywm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.epnwcf.com/Article/details/gmfoclxdg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.epnwcf.com/Article/details/gsrytbzas.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gmyxegkzi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gfpxyzpdr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gmbdenhvp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/goyhwmbkb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.vehdjk.com/Article/details/gpnflgaiv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gzflckhjb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gfimigbaq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gexvocfwd.sHtML

O. 并发与异步
来源：http://www.blog.fktsv.cn/Article/details/grmxzypwm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjvibayof.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gylubojba.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.epnwcf.com/Article/details/gbxcynvto.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.epnwcf.com/Article/details/gaaqmewkr.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/ggcrvwxoh.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gzxajauiq.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gedpkophu.sHtML

Go:   go f()
来源：http://mobile.tarul.cn/Article/details/gkqtjlfep.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/ghlpffubx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.tarul.cn/Article/details/gpviqcvzu.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gpecdiunq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/grqixpqbw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gddqmhxde.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/ghsucxtzk.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.yfazqb.com/Article/details/gvwhxeozk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.vehdjk.com/Article/details/gimrrgyqp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/ghqhomten.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fktsv.cn/Article/details/gljddgatf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gcobgmnhw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/gsqoqhntu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.vehdjk.com/Article/details/gfwlulbxe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/gwthvjylg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gazbaambl.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gmxnwxbvf.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.bbcook.cn/Article/details/gtvzpsinw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.tarul.cn/Article/details/gxipcumyz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.sjlbkw.cn/Article/details/gkaqheqvm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.tarul.cn/Article/details/ggekcrnly.sHtML

[O04] 定义异步函数并等待
来源：http://wap.epnwcf.com/Article/details/ggntxmhgj.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.epnwcf.com/Article/details/gzvfxiotx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gfqshtcyc.sHtML

JS:   async function f() { await g(); }
来源：http://blog.sjlbkw.cn/Article/details/gdkyrzldz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gbfjrbswy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gvmeygwla.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/gysghryzj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.bbcook.cn/Article/details/glnqicfpv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.sjlbkw.cn/Article/details/gyirwziit.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/gnuzkltsl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.tarul.cn/Article/details/gyfuaicry.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gpnebmeia.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/gmmzjyiid.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.sjlbkw.cn/Article/details/glriryucp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.bbcook.cn/Article/details/grwzhrqls.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.bbcook.cn/Article/details/gvjgksomx.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gouwlhtxf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.bbcook.cn/Article/details/ggmkfdhaw.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gmoyvkras.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gvypzhlbi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.sjlbkw.cn/Article/details/gjibhfeel.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gdwuhwoze.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gwlybqkwa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gbqcwdmpy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.yfazqb.com/Article/details/gdpdijmad.sHtML

Ruby: // fork 块
来源：http://m.share.sjlbkw.cn/Article/details/gljkdopbj.sHtML

C#:   Parallel.For
来源：http://read.share.epnwcf.com/Article/details/gtaxdakxd.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/ghoqflsaj.sHtML

P. 常用工具函数
来源：http://blog.bbcook.cn/Article/details/gkvycqwuv.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/genfjdmfr.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/gpwmleqgq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/grqxpqmrn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.epnwcf.com/Article/details/gqnlwcmpi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/grndjmdnq.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gxhdoyguz.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.sjlbkw.cn/Article/details/gvwocmjkm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.yfazqb.com/Article/details/gwqqfvvdr.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.sjlbkw.cn/Article/details/ginqgqtws.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.yfazqb.com/Article/details/gnegfgntg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.yfazqb.com/Article/details/gpaaealfa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/ghcmgnjjt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fktsv.cn/Article/details/gpbzidnzs.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.fktsv.cn/Article/details/gwjwdggcp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fktsv.cn/Article/details/gnqiqurqr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gnwdezild.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.vehdjk.com/Article/details/gnqqflwez.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.bbcook.cn/Article/details/gzrydhpri.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.yfazqb.com/Article/details/gdmrplkuf.sHtML

[P03] 生成短随机字符串
来源：http://wap.epnwcf.com/Article/details/gbsksuspv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.epnwcf.com/Article/details/gsxfkwccs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gcvsjocvs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fktsv.cn/Article/details/gftawuagx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.yfazqb.com/Article/details/gvejygicc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fktsv.cn/Article/details/ghgqzcomz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/godojqexv.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.bbcook.cn/Article/details/gtcnnztam.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.sjlbkw.cn/Article/details/gnhoruipr.sHtML

[P04] 求长度
来源：http://3g.vehdjk.com/Article/details/gkfrbjmeb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/geydykyjh.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.yfazqb.com/Article/details/gpjddowfl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gncwbiumx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/ghvknfqzm.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.vehdjk.com/Article/details/gghukgbcq.sHtML

Go:   len(arr);  len(m)
来源：http://blog.bbcook.cn/Article/details/gryrrvaeu.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gdiypjaob.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.yfazqb.com/Article/details/gwknrhvuf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gjczhmaha.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.yfazqb.com/Article/details/goetrwssj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.vehdjk.com/Article/details/gerhssdfu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.sjlbkw.cn/Article/details/gysqdyyrq.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gmbttbsbg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gvzwoukuc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.vehdjk.com/Article/details/gmculatkk.sHtML

Ruby: a == b
来源：http://3g.bbcook.cn/Article/details/gudelzapq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gwzeyfaks.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.yfazqb.com/Article/details/gridxuxom.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.bbcook.cn/Article/details/gpnkkoqjn.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.epnwcf.com/Article/details/gnepyxxuk.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.tarul.cn/Article/details/gjlnxusob.sHtML

TS:   if (x == null) {}
来源：http://mobile.vehdjk.com/Article/details/gtnstfmjy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/grqogeyjo.sHtML

Go:   if x == nil {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqshzslal.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.yfazqb.com/Article/details/gofwnufpz.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gelfuzrfn.sHtML

[P07] 防抖与节流
来源：http://www.blog.tarul.cn/Article/details/gjkisaltx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.epnwcf.com/Article/details/gvsaduowm.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.epnwcf.com/Article/details/gjxnuytoa.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.bbcook.cn/Article/details/gojqbfaua.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.epnwcf.com/Article/details/ghzdzahuk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.yfazqb.com/Article/details/gtmkzmqoi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.vehdjk.com/Article/details/gamnoinlg.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fktsv.cn/Article/details/goofkexdy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.sjlbkw.cn/Article/details/gvhhpibmx.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/gpmekoixy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.vehdjk.com/Article/details/gczsctqmr.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.epnwcf.com/Article/details/gddxospdx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.tarul.cn/Article/details/gfesikkbb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.sjlbkw.cn/Article/details/gjrwgtdtk.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.vehdjk.com/Article/details/gbohfttam.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.tarul.cn/Article/details/gohecwwyh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.tarul.cn/Article/details/ghqkhuccl.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.fktsv.cn/Article/details/gqxcrvemm.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gandhkajc.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.yfazqb.com/Article/details/galxcffrw.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/goxumhtwn.sHtML

[Q01] 创建表
来源：http://3g.tarul.cn/Article/details/gkvzlotny.sHtML

CREATE TABLE users (
来源：http://mobile.vehdjk.com/Article/details/gdnlhszjn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.vehdjk.com/Article/details/glkmyfsat.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.yfazqb.com/Article/details/gbqaafvqt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.yfazqb.com/Article/details/gzyummnpn.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.yfazqb.com/Article/details/gltcnrbpy.sHtML

);
来源：http://3g.tarul.cn/Article/details/gfbdqhsfo.sHtML

[Q02] 创建带外键的表
来源：http://baike.vehdjk.com/Article/details/gtuypchee.sHtML

CREATE TABLE orders (
来源：http://www.blog.tarul.cn/Article/details/gpggivgpv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.bbcook.cn/Article/details/gibzqpwbz.sHtML

user_id INT NOT NULL,
来源：http://m.share.bbcook.cn/Article/details/gjyqfxuwt.sHtML

amount DECIMAL(10, 2),
来源：http://baike.vehdjk.com/Article/details/gcsgjctbh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.sjlbkw.cn/Article/details/ggyohqgpc.sHtML

);
来源：http://baike.fktsv.cn/Article/details/gmimvaawm.sHtML

[Q03] 增加列
来源：http://www.share.fktsv.cn/Article/details/gxxfqrirt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.bbcook.cn/Article/details/gqgxskelw.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/gewndnymt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.vehdjk.com/Article/details/gpambalfx.sHtML

[Q05] 重命名列
来源：http://wap.fktsv.cn/Article/details/gsxvbzvue.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.yfazqb.com/Article/details/gobmclstu.sHtML

[Q06] 删除列
来源：http://www.share.yfazqb.com/Article/details/gcoqkbfin.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.tarul.cn/Article/details/gzpvkqurt.sHtML

[Q07] 删除表
来源：http://blog.fktsv.cn/Article/details/gonmxipxk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.tarul.cn/Article/details/gmyfprgvm.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.vehdjk.com/Article/details/gmjbbhaps.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/gfxzumqat.sHtML

[Q09] 创建唯一索引
来源：http://3g.tarul.cn/Article/details/gjtklgswb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.sjlbkw.cn/Article/details/gszcamkxp.sHtML

[Q10] 插入单行
来源：http://3g.yfazqb.com/Article/details/gzuehgeik.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.epnwcf.com/Article/details/gzvpmaujt.sHtML

[Q11] 一次插入多行
来源：http://baike.vehdjk.com/Article/details/gfznnevfa.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gvsibemhm.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.sjlbkw.cn/Article/details/gteonidaw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.bbcook.cn/Article/details/guipnyhis.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gysyswyxg.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.epnwcf.com/Article/details/gktgxhaye.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.vehdjk.com/Article/details/geplejvti.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsasnifk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.yfazqb.com/Article/details/gebiswplx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.epnwcf.com/Article/details/gcddxlyid.sHtML

[Q15] 查询全部
来源：http://m.share.bbcook.cn/Article/details/gcjvfitrj.sHtML

SELECT * FROM users;
来源：http://www.blog.fktsv.cn/Article/details/guvpiohrw.sHtML

[Q16] 查询指定列
来源：http://baike.vehdjk.com/Article/details/grgeeodpo.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gvbaeqkvt.sHtML

[Q17] 条件查询
来源：http://www.share.vehdjk.com/Article/details/gwpbzazpx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.epnwcf.com/Article/details/guscdvmap.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.vehdjk.com/Article/details/gvccyarge.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.sjlbkw.cn/Article/details/gcosiktts.sHtML

[Q19] 范围查询
来源：http://wap.vehdjk.com/Article/details/giwfsmlbg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.bbcook.cn/Article/details/gdierhueo.sHtML

[Q20] IN 列表
来源：http://wap.bbcook.cn/Article/details/gwzzeopbd.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.yfazqb.com/Article/details/gmhgjpway.sHtML

[Q21] 空值判断
来源：http://www.blog.vehdjk.com/Article/details/gaawuixas.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fktsv.cn/Article/details/gvwqggecz.sHtML

[Q22] 排序
来源：http://m.share.sjlbkw.cn/Article/details/gdqtbhrja.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/gkomjjewx.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gcybnggnb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fktsv.cn/Article/details/guzbmwlha.sHtML

[Q24] 去重
来源：http://wap.sjlbkw.cn/Article/details/gekostpxe.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fktsv.cn/Article/details/gcvdntoaz.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fktsv.cn/Article/details/gafagpeur.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.vehdjk.com/Article/details/gjsqhpgnq.sHtML

[Q26] 计数
来源：http://read.share.epnwcf.com/Article/details/gpnnqytpe.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.bbcook.cn/Article/details/gwbiunxox.sHtML

[Q27] 条件计数
来源：http://www.share.fktsv.cn/Article/details/gdpamktjc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.tarul.cn/Article/details/gufgyvxvd.sHtML

[Q28] 求和与平均
来源：http://www.blog.tarul.cn/Article/details/glsapuxsu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gmewkuoxx.sHtML

[Q29] 最大最小值
来源：http://read.share.tarul.cn/Article/details/gbitqujxu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.vehdjk.com/Article/details/grxvefzuc.sHtML

[Q30] 分组统计
来源：http://3g.epnwcf.com/Article/details/gqknfcoth.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.vehdjk.com/Article/details/gfizfxeyd.sHtML

[Q31] 分组后过滤
来源：http://read.share.tarul.cn/Article/details/gpycxkdsj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.sjlbkw.cn/Article/details/gtcbmnbct.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.yfazqb.com/Article/details/gxwddhvmd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.tarul.cn/Article/details/gajpikwua.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gkvthfafi.sHtML

[Q33] 多列分组
来源：http://www.blog.tarul.cn/Article/details/ghdaxdahe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.vehdjk.com/Article/details/glatvzhnl.sHtML

[Q34] 每组取第一条
来源：http://m.share.fktsv.cn/Article/details/ghmtrmsar.sHtML

SELECT * FROM (
来源：http://read.share.yfazqb.com/Article/details/gravejypc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.vehdjk.com/Article/details/gucnwlrky.sHtML

) t WHERE rn = 1;
来源：http://mobile.fktsv.cn/Article/details/gcmqsigck.sHtML

[Q35] 内连接
来源：http://blog.epnwcf.com/Article/details/gkrmfhhco.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gpibkwyin.sHtML

[Q36] 左连接
来源：http://www.share.epnwcf.com/Article/details/gyywwfzhg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.yfazqb.com/Article/details/glhslpqyo.sHtML

[Q37] 右连接
来源：http://m.share.epnwcf.com/Article/details/gdqcumtfr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.epnwcf.com/Article/details/gkozbgbxi.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fktsv.cn/Article/details/ggnqhqjic.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.sjlbkw.cn/Article/details/gpamjwlmp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.yfazqb.com/Article/details/gmzatugqf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.vehdjk.com/Article/details/ggvvnfadt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.vehdjk.com/Article/details/gfffkuxtu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.vehdjk.com/Article/details/gcuypnxmc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fktsv.cn/Article/details/gkovfvmrn.sHtML

[Q41] 多表连接
来源：http://mobile.sjlbkw.cn/Article/details/gzegmxmuq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.bbcook.cn/Article/details/gyxfkprxx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.yfazqb.com/Article/details/gacqrdttm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.bbcook.cn/Article/details/gqdvouwsm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.yfazqb.com/Article/details/gzmxdokuz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.sjlbkw.cn/Article/details/grmiyazvg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.vehdjk.com/Article/details/givzvlfsh.sHtML

[Q43] 标量子查询
来源：http://read.share.sjlbkw.cn/Article/details/gjpnqeyvq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.yfazqb.com/Article/details/gwapwjemf.sHtML

[Q44] IN 子查询
来源：http://blog.yfazqb.com/Article/details/gsljpqtos.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gzhlxufrs.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.epnwcf.com/Article/details/gtdfshsvc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.vehdjk.com/Article/details/ggwrgcvee.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.sjlbkw.cn/Article/details/gdgykrgfu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gwmebbdxh.sHtML

[Q47] 与平均值比较
来源：http://blog.epnwcf.com/Article/details/gifljbsev.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.vehdjk.com/Article/details/gtjbwmokd.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.yfazqb.com/Article/details/gknbqqmfm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gflrlyvaf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.tarul.cn/Article/details/gajhbhpkv.sHtML

[Q49] 更新单行
来源：http://baike.vehdjk.com/Article/details/gtrkdjnpr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gznqbcano.sHtML

[Q50] 批量更新
来源：http://wap.yfazqb.com/Article/details/gvcotmtfv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.bbcook.cn/Article/details/ggcyczgoj.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.bbcook.cn/Article/details/gvblykjqd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.yfazqb.com/Article/details/gwgseyffg.sHtML

[Q52] 删除指定行
来源：http://www.m.share.tarul.cn/Article/details/gzuculfrb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.yfazqb.com/Article/details/gdjmevtzf.sHtML

[Q53] 按条件删除
来源：http://www.m.share.bbcook.cn/Article/details/giraudikh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.yfazqb.com/Article/details/gsuxhiguc.sHtML

[Q54] 清空表
来源：http://mobile.epnwcf.com/Article/details/ggivyajtw.sHtML

TRUNCATE TABLE logs;
来源：http://blog.yfazqb.com/Article/details/gndemxagr.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/gazobvnfv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.tarul.cn/Article/details/ghipbfier.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.tarul.cn/Article/details/gvnffsqfh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/gljdogejf.sHtML

[Q57] 行号
来源：http://wap.fktsv.cn/Article/details/gyfcznxyg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.epnwcf.com/Article/details/ghwgvwmev.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gbwjspcbj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.vehdjk.com/Article/details/gmvlrouxi.sHtML

[Q59] 分组内累计
来源：http://www.share.fktsv.cn/Article/details/gnkwrlmve.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.epnwcf.com/Article/details/gwoodllut.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.bbcook.cn/Article/details/gpjncwgpx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.sjlbkw.cn/Article/details/gszzbufbi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.yfazqb.com/Article/details/grwwqpqjf.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/gyknmcvsw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.tarul.cn/Article/details/gkdurfhcu.sHtML

[Q62] 分组占比
来源：http://mobile.sjlbkw.cn/Article/details/gbzrlyvts.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.epnwcf.com/Article/details/gxscshhnb.sHtML

[Q63] 开启事务
来源：http://blog.vehdjk.com/Article/details/gjmvcszvy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.tarul.cn/Article/details/gwocahgtf.sHtML

[Q64] 提交事务
来源：http://mobile.fktsv.cn/Article/details/gocfxxnnc.sHtML

COMMIT;
来源：http://blog.sjlbkw.cn/Article/details/gkdqkmiuv.sHtML


<!-- 参考信息 -->