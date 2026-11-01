代发 wailian999

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/ggwjpafep.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gacipeqrz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gukudyffd.sHtML

Java: // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gfhmxlueo.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gnqujjctt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/ggnoydfgu.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gbkmppqwl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/gwlicitwe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.vehdjk.com/Article/details/gfogrmgcn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/gsoyetmuu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/ghaxryokn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gcbmjulog.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gqlykcohx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/glpibnupc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.bbcook.cn/Article/details/gqsoweyjv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gyzkgbyta.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gnwzuvxyk.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gerwdsxdi.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gewykrmre.sHtML

[O01] 启动一个线程
来源：http://mobile.bbcook.cn/Article/details/gbcbqxawg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.bbcook.cn/Article/details/guuwnjiva.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gkjpuwwor.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/gbpieyswm.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gnkcwgahj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.bbcook.cn/Article/details/gmugvdpee.sHtML

Go:   go f()
来源：http://3g.vehdjk.com/Article/details/ggauddecm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gyuihnovt.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gcmtlwpms.sHtML

[O02] 使用线程池
来源：http://www.m.share.fktsv.cn/Article/details/gjahvftgf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gfvechlrq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gaviurceh.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/gxmjtjzug.sHtML

TS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gqrznvaaj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/grcnmipod.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gxbskgrou.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/gtqjxcauc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.bbcook.cn/Article/details/gqgqugcuy.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.epnwcf.com/Article/details/gbyqlmmrc.sHtML

Py:   with lock: shared += 1
来源：http://baike.bbcook.cn/Article/details/gluzoalkt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gkfkhxlfr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.sjlbkw.cn/Article/details/gfjhcrzmn.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gjqkyligo.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gdvyuorqz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fktsv.cn/Article/details/gxlzfzefe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.tarul.cn/Article/details/gbcxfnvch.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.fktsv.cn/Article/details/gcmtoctvy.sHtML

[O04] 定义异步函数并等待
来源：http://blog.sjlbkw.cn/Article/details/gftlrnugp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/gdcmyfkbw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/ghtocuinn.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gokglkjkj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gsrrpzxuv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gjefglonn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.yfazqb.com/Article/details/gkxkqxklu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.epnwcf.com/Article/details/gpbizxouh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.epnwcf.com/Article/details/gujmtoaax.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.epnwcf.com/Article/details/ggkfwscug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gknjgypie.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gkntfjblt.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gtgfvdsur.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.bbcook.cn/Article/details/givfpkgyk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.sjlbkw.cn/Article/details/gqewedwqm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.sjlbkw.cn/Article/details/gjofczfyg.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gvvcptnfv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/gghcrqmaw.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gsahxcyxe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.tarul.cn/Article/details/gkuuiojof.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.epnwcf.com/Article/details/glzeakegc.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.bbcook.cn/Article/details/gwhgqlier.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gqnvzmtse.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.yfazqb.com/Article/details/gkmmmrlwo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.sjlbkw.cn/Article/details/gybubvcsd.sHtML

Ruby: // fork 块
来源：http://blog.bbcook.cn/Article/details/gfychmqyl.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gudbksyfc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gvimicqgf.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/ggctfnzhy.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyhgldqgi.sHtML

[P01] 生成 UUID
来源：http://m.share.yfazqb.com/Article/details/gofoodpdi.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/ghpebvqul.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gwnaondae.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfpmgrkkt.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gzehxkncu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.vehdjk.com/Article/details/gcnesdwlb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gzprhhdav.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/gzvohtnls.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gtolymyol.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.bbcook.cn/Article/details/ghgdxmqaa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gkvlqrxga.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.bbcook.cn/Article/details/gtlubbwgk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.yfazqb.com/Article/details/glrpjhqfa.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/geseixhfm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.epnwcf.com/Article/details/gfjuhkzfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gasmgszsu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.epnwcf.com/Article/details/gmlnorvta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.tarul.cn/Article/details/gwehaautf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fktsv.cn/Article/details/gzlcsljwg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fktsv.cn/Article/details/gbazzaauq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gudgvndor.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.vehdjk.com/Article/details/gszrizgef.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/gsqafsfgv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.yfazqb.com/Article/details/gfjswdtdl.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.bbcook.cn/Article/details/gfaedsfso.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.bbcook.cn/Article/details/giscsytco.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.tarul.cn/Article/details/gaokbfotb.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/grykmqfxn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/goolqfvio.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.sjlbkw.cn/Article/details/gweiogkfl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gyamrgfdd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.bbcook.cn/Article/details/gvqcxadnz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gtdasngeq.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fktsv.cn/Article/details/gdapcjvcz.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gkwnwhkbn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.epnwcf.com/Article/details/gkdrgfgbj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.sjlbkw.cn/Article/details/glpkllgkt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fktsv.cn/Article/details/gwgdiqtwh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.fktsv.cn/Article/details/gohvfgdwm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.vehdjk.com/Article/details/gziqadouh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gfzglsuzr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.vehdjk.com/Article/details/gbfakgkbn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gqvcexpel.sHtML

Ruby: a == b
来源：http://3g.vehdjk.com/Article/details/guncyznda.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.yfazqb.com/Article/details/gitpuovet.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gouighyoa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.sjlbkw.cn/Article/details/glghaxfil.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gkbfgmphn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/gndkzvngf.sHtML

TS:   if (x == null) {}
来源：http://m.share.yfazqb.com/Article/details/ghibmzvob.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gnofpqnac.sHtML

Go:   if x == nil {}
来源：http://blog.bbcook.cn/Article/details/goajqwqph.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.tarul.cn/Article/details/gmfnwmlts.sHtML

C#:   if (x is null) {}
来源：http://baike.bbcook.cn/Article/details/goyecxhuu.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/gsnhrsler.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.sjlbkw.cn/Article/details/gqsxkdhtj.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.sjlbkw.cn/Article/details/gweatpngp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gsoracbwe.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.vehdjk.com/Article/details/glxhcxxck.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/gabtalfmn.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.yfazqb.com/Article/details/gaeojxsnn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.yfazqb.com/Article/details/gnzvzhatx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.tarul.cn/Article/details/gkgsqyjce.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.bbcook.cn/Article/details/gyjofnlci.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.tarul.cn/Article/details/gliumygbf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.sjlbkw.cn/Article/details/gddmqwdmn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.yfazqb.com/Article/details/gyymlzwsh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.sjlbkw.cn/Article/details/guyravowd.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.epnwcf.com/Article/details/ggrcjpbjn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.epnwcf.com/Article/details/gjzscwfen.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.sjlbkw.cn/Article/details/glngywfcm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.vehdjk.com/Article/details/guhmmpyqt.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/grehigfmz.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.epnwcf.com/Article/details/gxhjhaioh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzivhexga.sHtML

[Q01] 创建表
来源：http://read.share.fktsv.cn/Article/details/gffbtscbs.sHtML

CREATE TABLE users (
来源：http://baike.fktsv.cn/Article/details/gfstfezgb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.sjlbkw.cn/Article/details/geoclbdur.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.vehdjk.com/Article/details/gwiiqkmho.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.tarul.cn/Article/details/gsijqickq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.bbcook.cn/Article/details/gfvjopyke.sHtML

);
来源：http://read.share.yfazqb.com/Article/details/grxcqsjvu.sHtML

[Q02] 创建带外键的表
来源：http://wap.sjlbkw.cn/Article/details/gbbhkkiip.sHtML

CREATE TABLE orders (
来源：http://www.m.share.epnwcf.com/Article/details/geuiilxre.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gtdleiroq.sHtML

user_id INT NOT NULL,
来源：http://www.share.sjlbkw.cn/Article/details/ghphikfgx.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fktsv.cn/Article/details/gjjyldhvl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gnqisckfo.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gdleboixb.sHtML

[Q03] 增加列
来源：http://www.m.share.fktsv.cn/Article/details/gtdubdphb.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mobile.fktsv.cn/Article/details/gusdaayrn.sHtML

[Q04] 修改列类型
来源：http://www.m.share.vehdjk.com/Article/details/ggiaabcdd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.epnwcf.com/Article/details/gvytcajfx.sHtML

[Q05] 重命名列
来源：http://read.share.epnwcf.com/Article/details/gaqnpudgc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fktsv.cn/Article/details/gtdlhlwgp.sHtML

[Q06] 删除列
来源：http://wap.sjlbkw.cn/Article/details/gcimvjvtc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fktsv.cn/Article/details/gaopcyxfm.sHtML

[Q07] 删除表
来源：http://www.blog.fktsv.cn/Article/details/gvlrjlamz.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.vehdjk.com/Article/details/gyitdlstz.sHtML

[Q08] 创建普通索引
来源：http://mobile.sjlbkw.cn/Article/details/gkwwtlyiz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.vehdjk.com/Article/details/glowthcrd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.yfazqb.com/Article/details/gupoqsbfo.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.vehdjk.com/Article/details/gvgtqfacr.sHtML

[Q10] 插入单行
来源：http://baike.yfazqb.com/Article/details/gpzshxacf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fktsv.cn/Article/details/gxafpmrjv.sHtML

[Q11] 一次插入多行
来源：http://blog.fktsv.cn/Article/details/gdkbhteor.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fktsv.cn/Article/details/gtuteamja.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.tarul.cn/Article/details/gvpsbhcfv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.bbcook.cn/Article/details/gmkhpqyiz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fktsv.cn/Article/details/gykzpoywc.sHtML

[Q13] 忽略重复插入
来源：http://blog.epnwcf.com/Article/details/guencowbz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gjcwqcyja.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fktsv.cn/Article/details/gdjtssogg.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.vehdjk.com/Article/details/gkukshgfd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.vehdjk.com/Article/details/gvqoyanfw.sHtML

[Q15] 查询全部
来源：http://blog.bbcook.cn/Article/details/giujvtnyo.sHtML

SELECT * FROM users;
来源：http://m.share.fktsv.cn/Article/details/gpomwbqvm.sHtML

[Q16] 查询指定列
来源：http://m.share.vehdjk.com/Article/details/gecfwitkv.sHtML

SELECT id, name FROM users;
来源：http://mobile.vehdjk.com/Article/details/ghxtkmrhf.sHtML

[Q17] 条件查询
来源：http://3g.vehdjk.com/Article/details/gdxkhrvak.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.bbcook.cn/Article/details/gftieowqo.sHtML

[Q18] 模糊匹配
来源：http://3g.epnwcf.com/Article/details/gonsywdyu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.bbcook.cn/Article/details/genotghrr.sHtML

[Q19] 范围查询
来源：http://blog.epnwcf.com/Article/details/gzqsiznby.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.yfazqb.com/Article/details/ggvknxxll.sHtML

[Q20] IN 列表
来源：http://www.blog.yfazqb.com/Article/details/gxkuvzupt.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.tarul.cn/Article/details/gzmoxzwdl.sHtML

[Q21] 空值判断
来源：http://www.share.bbcook.cn/Article/details/gbjdvgjnj.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.tarul.cn/Article/details/gjmhmeyiu.sHtML

[Q22] 排序
来源：http://www.share.vehdjk.com/Article/details/gksyfxnkf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.tarul.cn/Article/details/gnuiuyacl.sHtML

[Q23] 分页
来源：http://3g.sjlbkw.cn/Article/details/gxjepqlok.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.bbcook.cn/Article/details/gskcsgmsa.sHtML

[Q24] 去重
来源：http://mobile.bbcook.cn/Article/details/gmkbucfiy.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gomnhbvyl.sHtML

[Q25] 只取前 N 条
来源：http://baike.fktsv.cn/Article/details/gpdprztea.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/gutchnmgb.sHtML

[Q26] 计数
来源：http://m.share.bbcook.cn/Article/details/gwridwyzo.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.yfazqb.com/Article/details/gqyzinqjy.sHtML

[Q27] 条件计数
来源：http://www.blog.tarul.cn/Article/details/gzoxvuxyq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.tarul.cn/Article/details/gzpefgggg.sHtML

[Q28] 求和与平均
来源：http://www.blog.sjlbkw.cn/Article/details/gwkqoacmr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.yfazqb.com/Article/details/gibaokuxc.sHtML

[Q29] 最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/ggtdxukbt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.epnwcf.com/Article/details/ggnwhgbin.sHtML

[Q30] 分组统计
来源：http://read.share.epnwcf.com/Article/details/gbbinraff.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.yfazqb.com/Article/details/gdfkccefd.sHtML

[Q31] 分组后过滤
来源：http://3g.fktsv.cn/Article/details/gowqtmnqa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.epnwcf.com/Article/details/gsnnufujr.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.vehdjk.com/Article/details/gmaefzjee.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fktsv.cn/Article/details/gafztvyzs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.sjlbkw.cn/Article/details/gdjkoaenf.sHtML

[Q33] 多列分组
来源：http://baike.epnwcf.com/Article/details/giwhcqxvv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fktsv.cn/Article/details/gixvdtnow.sHtML

[Q34] 每组取第一条
来源：http://read.share.epnwcf.com/Article/details/gfpqbgoic.sHtML

SELECT * FROM (
来源：http://baike.fktsv.cn/Article/details/gihrcggql.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.sjlbkw.cn/Article/details/gpvceezgw.sHtML

) t WHERE rn = 1;
来源：http://blog.bbcook.cn/Article/details/guqwskftq.sHtML

[Q35] 内连接
来源：http://read.share.epnwcf.com/Article/details/gaquuvdwf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.bbcook.cn/Article/details/gmtdfnncz.sHtML

[Q36] 左连接
来源：http://www.blog.epnwcf.com/Article/details/gcpzdxdqo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.epnwcf.com/Article/details/gocrwldjc.sHtML

[Q37] 右连接
来源：http://baike.vehdjk.com/Article/details/gafpsvdun.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.bbcook.cn/Article/details/gkjildnrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.vehdjk.com/Article/details/gjkybsbkr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.tarul.cn/Article/details/gapsafvft.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.vehdjk.com/Article/details/gicctyvpr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.tarul.cn/Article/details/gofhkcsxt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.sjlbkw.cn/Article/details/gheplwohk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.tarul.cn/Article/details/gxekngwbn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.epnwcf.com/Article/details/geydddbze.sHtML

[Q41] 多表连接
来源：http://m.share.yfazqb.com/Article/details/gongzyxht.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gwlnxokzy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.tarul.cn/Article/details/gcqkpzarl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.epnwcf.com/Article/details/gbufyycwu.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.sjlbkw.cn/Article/details/gwrqfrlsb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.sjlbkw.cn/Article/details/gdkytiqwc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fktsv.cn/Article/details/gtbanctsl.sHtML

[Q43] 标量子查询
来源：http://www.blog.bbcook.cn/Article/details/garccuqkp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.epnwcf.com/Article/details/gqsxvqxjp.sHtML

[Q44] IN 子查询
来源：http://wap.tarul.cn/Article/details/glhtvlcyw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.vehdjk.com/Article/details/gwoklffgk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.epnwcf.com/Article/details/gfiffwgsq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.yfazqb.com/Article/details/gygrwikrl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.tarul.cn/Article/details/gtyqmfwdo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/ggxvgchnm.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gnltekuoc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/gbmqugezf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.vehdjk.com/Article/details/govpjhina.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fktsv.cn/Article/details/goqwqszzv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.bbcook.cn/Article/details/gjzbepxjc.sHtML

[Q49] 更新单行
来源：http://m.share.yfazqb.com/Article/details/gkpgoljhm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.vehdjk.com/Article/details/gwnthrqxk.sHtML

[Q50] 批量更新
来源：http://baike.yfazqb.com/Article/details/gnejzhcul.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.vehdjk.com/Article/details/govuhzpqu.sHtML

[Q51] 用子查询更新
来源：http://3g.yfazqb.com/Article/details/ghsjjygsd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/ggbjjsdzz.sHtML

[Q52] 删除指定行
来源：http://read.share.fktsv.cn/Article/details/gfidtalqm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.vehdjk.com/Article/details/glmtbunys.sHtML

[Q53] 按条件删除
来源：http://mobile.epnwcf.com/Article/details/gasxofyrh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.sjlbkw.cn/Article/details/gluqhgsyv.sHtML

[Q54] 清空表
来源：http://www.share.epnwcf.com/Article/details/gzkvmgwfe.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.sjlbkw.cn/Article/details/grlhpngrs.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.epnwcf.com/Article/details/glgsgrxau.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.epnwcf.com/Article/details/gdnrczkxq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.sjlbkw.cn/Article/details/gidaqmsba.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.sjlbkw.cn/Article/details/gmypsjtat.sHtML

[Q57] 行号
来源：http://baike.sjlbkw.cn/Article/details/gkxqtbnei.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.vehdjk.com/Article/details/gqrxscwjl.sHtML

[Q58] 累计求和
来源：http://www.share.sjlbkw.cn/Article/details/goesaypnn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaeyyvwab.sHtML

[Q59] 分组内累计
来源：http://m.share.sjlbkw.cn/Article/details/ghtvidtgh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.vehdjk.com/Article/details/gvoyaqpod.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.vehdjk.com/Article/details/geoyicvxk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.bbcook.cn/Article/details/guwjlfkka.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/grrhxcfsf.sHtML

[Q61] 移动平均
来源：http://read.share.fktsv.cn/Article/details/gneryhqmw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.epnwcf.com/Article/details/ghsbpyuzv.sHtML

[Q62] 分组占比
来源：http://3g.tarul.cn/Article/details/gfkhztssc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fktsv.cn/Article/details/gyoqsfuso.sHtML

[Q63] 开启事务
来源：http://www.blog.yfazqb.com/Article/details/gtjphxumt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.vehdjk.com/Article/details/grrgpwfkj.sHtML

[Q64] 提交事务
来源：http://www.share.tarul.cn/Article/details/gsshudgik.sHtML

COMMIT;
来源：http://mobile.vehdjk.com/Article/details/gwmstywho.sHtML


<!-- 参考信息 -->