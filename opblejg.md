代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gjgxusucd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/ghahpjerm.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/glpfvvjty.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/gsehezjsa.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/ghhplxvbk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gfffhpkfa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.bbcook.cn/Article/details/gwoeliamd.sHtML

Java: // 手写递归
来源：http://baike.vehdjk.com/Article/details/gpxmtkqyc.sHtML

Go:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gldadkhmn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.vehdjk.com/Article/details/gjnokqzcf.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/ghmxuvnas.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.vehdjk.com/Article/details/goinxfgch.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gacghnqkv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fktsv.cn/Article/details/gfdoxfjvz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/grtnvityx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gsshluuwc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/galdmxthz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.sjlbkw.cn/Article/details/gnyyqlrpi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gvpoowsjp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gdwpulotr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gntjpvcev.sHtML

O. 并发与异步
来源：http://www.m.share.bbcook.cn/Article/details/ghbnasczi.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpnxbepmb.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gyfebjloj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.bbcook.cn/Article/details/gghzvsfta.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/gcycueyvn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gniayqvvv.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gggbsjtlb.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/goaibegaw.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gtuomirvp.sHtML

Ruby: Thread.new { f }
来源：http://3g.sjlbkw.cn/Article/details/gntwaofnt.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gaerhbjbw.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/godbgupkx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.tarul.cn/Article/details/gijcwtjnx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/gctljvoie.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gaarnmaul.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gvggpmoqr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gsmatemwl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.tarul.cn/Article/details/ghjrywrns.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/guphqnfly.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gbzggfvms.sHtML

[O03] 加锁保护共享数据
来源：http://baike.epnwcf.com/Article/details/gcqvwyohe.sHtML

Py:   with lock: shared += 1
来源：http://m.share.vehdjk.com/Article/details/gndeqtpup.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gywsjwtcf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gxedfriau.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gxlxtwdlh.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/ggkiaokod.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gzbqcxntc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gptduucvr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gvryykwvk.sHtML

[O04] 定义异步函数并等待
来源：http://blog.epnwcf.com/Article/details/gfwigcrpm.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.yfazqb.com/Article/details/goxvtamre.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gufkwonnx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/govwkiutm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gusibqpyu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gqmvwyekt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gblfqpnmd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gpgdvhmer.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fktsv.cn/Article/details/gkhuziohs.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.yfazqb.com/Article/details/gjttkdbaf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fktsv.cn/Article/details/gurhubmzq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.sjlbkw.cn/Article/details/gqtrtgoky.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.tarul.cn/Article/details/ggxkajavt.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gyvbawnyh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gsaliudcs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.sjlbkw.cn/Article/details/gnqzjkxek.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gtdwbvrqn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.yfazqb.com/Article/details/gcnpkjygv.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gypzznyoc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/ghpejohtc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gayepubzt.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.vehdjk.com/Article/details/ghuijelvy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.sjlbkw.cn/Article/details/gnpjdbbzp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.yfazqb.com/Article/details/grjbfbwqa.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/gyqwxmmaz.sHtML

Ruby: // fork 块
来源：http://blog.fktsv.cn/Article/details/gcuajeplu.sHtML

C#:   Parallel.For
来源：http://baike.bbcook.cn/Article/details/gfxsyzcyu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/grjaqwktn.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/ghmjbndae.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwkcmdnmp.sHtML

[P01] 生成 UUID
来源：http://wap.fktsv.cn/Article/details/gnfzjfvde.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gvhtrmbtf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gsanlvvlx.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fktsv.cn/Article/details/gxtznebps.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fktsv.cn/Article/details/gshtgfqcv.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fktsv.cn/Article/details/groachfsa.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.tarul.cn/Article/details/gihawkmcs.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/giecjwmgg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.epnwcf.com/Article/details/goyrrsyfo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.vehdjk.com/Article/details/gstoebsyj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gftlilrlk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.epnwcf.com/Article/details/gouxcdrzd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fktsv.cn/Article/details/gmqgnimjx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.yfazqb.com/Article/details/gucuqslap.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.vehdjk.com/Article/details/gicewpwjt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.sjlbkw.cn/Article/details/geijbutij.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gopmljpdd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.tarul.cn/Article/details/gzxhencku.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gzztmerbw.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.fktsv.cn/Article/details/gfusbyiza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.bbcook.cn/Article/details/gqqyidvwi.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/gazzjwlmu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gwiubegbq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/gksyhrahq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.yfazqb.com/Article/details/gvhsajnzd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.tarul.cn/Article/details/gydmndaku.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gcvyjqilp.sHtML

[P04] 求长度
来源：http://www.share.tarul.cn/Article/details/gmsrhvgii.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.epnwcf.com/Article/details/grcxmtjej.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.vehdjk.com/Article/details/gvhvcsjoa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/ghvbemruf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/grranoqty.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.tarul.cn/Article/details/gmdywwiwf.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gnlbpocjo.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gmupmqjen.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/gnvrgilny.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.bbcook.cn/Article/details/gmjdeyvlt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.tarul.cn/Article/details/gppvunetn.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gbrgxsrnr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.yfazqb.com/Article/details/gewjjjdxo.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gsfjmkswr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.bbcook.cn/Article/details/gyjmymmpb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.epnwcf.com/Article/details/gxrqhtrsi.sHtML

Ruby: a == b
来源：http://m.share.sjlbkw.cn/Article/details/gtlbiptdo.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/grqlqacpy.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.tarul.cn/Article/details/gnzfhforf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/ghcxkrmyr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.vehdjk.com/Article/details/gnkzvypdc.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/ggimaaqra.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gmfwlcwum.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.epnwcf.com/Article/details/gipcbhgtx.sHtML

Go:   if x == nil {}
来源：http://www.m.share.bbcook.cn/Article/details/goflookjf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.tarul.cn/Article/details/gxdjadhxj.sHtML

C#:   if (x is null) {}
来源：http://www.share.bbcook.cn/Article/details/giwxmqsnk.sHtML

[P07] 防抖与节流
来源：http://www.m.share.fktsv.cn/Article/details/godtzkvwn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.bbcook.cn/Article/details/gnojuaqaf.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.sjlbkw.cn/Article/details/gdvzibzvg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gudziievt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/guhjepwxy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.yfazqb.com/Article/details/gsetlyzxy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.fktsv.cn/Article/details/gdmcqislk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.epnwcf.com/Article/details/gwvselplk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fktsv.cn/Article/details/gfkzlvptb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.tarul.cn/Article/details/gtespfzkl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.tarul.cn/Article/details/gnehqitrw.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmebmnoz.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.yfazqb.com/Article/details/ggzmobeub.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fktsv.cn/Article/details/gruxkntpb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.epnwcf.com/Article/details/gjpalsjcw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.bbcook.cn/Article/details/gtylrvanj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.yfazqb.com/Article/details/gqkzjvhfn.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.vehdjk.com/Article/details/gzryecqpw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gyiwumqgh.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.bbcook.cn/Article/details/gcmwabtyc.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gugevbbgt.sHtML

[Q01] 创建表
来源：http://3g.epnwcf.com/Article/details/giggthjks.sHtML

CREATE TABLE users (
来源：http://baike.epnwcf.com/Article/details/gocqhnyqm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.yfazqb.com/Article/details/geimxedxx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.epnwcf.com/Article/details/gxdgivhdp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.yfazqb.com/Article/details/gwtlnaclp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.yfazqb.com/Article/details/gcthxommo.sHtML

);
来源：http://baike.tarul.cn/Article/details/gtdnzsczo.sHtML

[Q02] 创建带外键的表
来源：http://read.share.vehdjk.com/Article/details/gkqhrztyb.sHtML

CREATE TABLE orders (
来源：http://blog.epnwcf.com/Article/details/gbwqxuhnv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.sjlbkw.cn/Article/details/ghivkeulj.sHtML

user_id INT NOT NULL,
来源：http://3g.epnwcf.com/Article/details/grzfkdexi.sHtML

amount DECIMAL(10, 2),
来源：http://blog.epnwcf.com/Article/details/gwtegvbnu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.vehdjk.com/Article/details/gwkkonapf.sHtML

);
来源：http://blog.vehdjk.com/Article/details/gfqpppodi.sHtML

[Q03] 增加列
来源：http://www.blog.epnwcf.com/Article/details/grhtoftry.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fktsv.cn/Article/details/gttbbrwrr.sHtML

[Q04] 修改列类型
来源：http://3g.bbcook.cn/Article/details/gdljrwtmp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.sjlbkw.cn/Article/details/gjzxltpbd.sHtML

[Q05] 重命名列
来源：http://wap.yfazqb.com/Article/details/gaiupzqqo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.yfazqb.com/Article/details/goqhlrhkh.sHtML

[Q06] 删除列
来源：http://m.share.sjlbkw.cn/Article/details/gwrvkkfsl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.vehdjk.com/Article/details/gdritniwv.sHtML

[Q07] 删除表
来源：http://3g.epnwcf.com/Article/details/gdwzkltah.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fktsv.cn/Article/details/gynmpailh.sHtML

[Q08] 创建普通索引
来源：http://m.share.bbcook.cn/Article/details/ghcqmmpev.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.tarul.cn/Article/details/gkcjggwrm.sHtML

[Q09] 创建唯一索引
来源：http://m.share.vehdjk.com/Article/details/gghuoelqg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.yfazqb.com/Article/details/gqgjmqmpx.sHtML

[Q10] 插入单行
来源：http://read.share.vehdjk.com/Article/details/ghscbovos.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.vehdjk.com/Article/details/gngufevud.sHtML

[Q11] 一次插入多行
来源：http://mobile.vehdjk.com/Article/details/gxnxlimma.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.epnwcf.com/Article/details/gakubehgh.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.bbcook.cn/Article/details/godjkvhca.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.epnwcf.com/Article/details/gszvbxppq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.sjlbkw.cn/Article/details/gthnquekx.sHtML

[Q13] 忽略重复插入
来源：http://read.share.epnwcf.com/Article/details/gzvfqxgmp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.yfazqb.com/Article/details/giuqoongv.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.yfazqb.com/Article/details/goqxspxpv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.vehdjk.com/Article/details/gshztvfak.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.bbcook.cn/Article/details/geqxycizr.sHtML

[Q15] 查询全部
来源：http://www.share.fktsv.cn/Article/details/gzvtjguev.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gwcfbypgp.sHtML

[Q16] 查询指定列
来源：http://3g.vehdjk.com/Article/details/gjhdiwxro.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fktsv.cn/Article/details/ggitoitrd.sHtML

[Q17] 条件查询
来源：http://baike.fktsv.cn/Article/details/gflvgfvpm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.vehdjk.com/Article/details/gjxfkwddy.sHtML

[Q18] 模糊匹配
来源：http://blog.yfazqb.com/Article/details/gyedmaetm.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.epnwcf.com/Article/details/gcrzuvdbw.sHtML

[Q19] 范围查询
来源：http://blog.bbcook.cn/Article/details/gvexsnsdw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.yfazqb.com/Article/details/gmieonywt.sHtML

[Q20] IN 列表
来源：http://baike.bbcook.cn/Article/details/gdrsrzker.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fktsv.cn/Article/details/gxjmtkihm.sHtML

[Q21] 空值判断
来源：http://blog.fktsv.cn/Article/details/gllmglrwr.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gxtordttx.sHtML

[Q22] 排序
来源：http://mobile.fktsv.cn/Article/details/gzulmgmhg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.epnwcf.com/Article/details/guppedjep.sHtML

[Q23] 分页
来源：http://blog.vehdjk.com/Article/details/gyoeyabia.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.yfazqb.com/Article/details/gcxhyjlpy.sHtML

[Q24] 去重
来源：http://www.m.share.epnwcf.com/Article/details/glqrkzpsi.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.bbcook.cn/Article/details/ggpibicri.sHtML

[Q25] 只取前 N 条
来源：http://blog.fktsv.cn/Article/details/gmglxkiuy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fktsv.cn/Article/details/gxsexoeaz.sHtML

[Q26] 计数
来源：http://www.share.epnwcf.com/Article/details/gpduyqhdb.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.epnwcf.com/Article/details/gobtjqzoi.sHtML

[Q27] 条件计数
来源：http://m.share.tarul.cn/Article/details/gzxfiedhl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.vehdjk.com/Article/details/gcehbnzyg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.yfazqb.com/Article/details/gzfqivzbn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.vehdjk.com/Article/details/gtgtavvnt.sHtML

[Q29] 最大最小值
来源：http://m.share.fktsv.cn/Article/details/gasfelelg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/gmtakxwir.sHtML

[Q30] 分组统计
来源：http://www.m.share.epnwcf.com/Article/details/gmapoulfk.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.epnwcf.com/Article/details/gqufawalj.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fktsv.cn/Article/details/gdsldgcwb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.tarul.cn/Article/details/garyzacbe.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.sjlbkw.cn/Article/details/gzypitspn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/gvfbavmzt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.tarul.cn/Article/details/gaesuovfk.sHtML

[Q33] 多列分组
来源：http://baike.tarul.cn/Article/details/gsqarycnq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.epnwcf.com/Article/details/gfbenylcg.sHtML

[Q34] 每组取第一条
来源：http://www.blog.vehdjk.com/Article/details/gjfaxxqhm.sHtML

SELECT * FROM (
来源：http://baike.yfazqb.com/Article/details/geyjppspz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.yfazqb.com/Article/details/gostausjr.sHtML

) t WHERE rn = 1;
来源：http://m.share.yfazqb.com/Article/details/gtonyxeiv.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/gaftsmpxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.sjlbkw.cn/Article/details/gaxvfysjp.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gxyeerlyq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.sjlbkw.cn/Article/details/gbattqbzi.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gsxvivzzl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.tarul.cn/Article/details/ghpvbbftt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.vehdjk.com/Article/details/gnigoxiud.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.bbcook.cn/Article/details/goheapvxs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fktsv.cn/Article/details/ghdwtgzmo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.epnwcf.com/Article/details/gtcrpdvii.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.epnwcf.com/Article/details/grvqovuts.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.vehdjk.com/Article/details/gzpbfcgtc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.bbcook.cn/Article/details/glerjmykb.sHtML

[Q41] 多表连接
来源：http://www.blog.fktsv.cn/Article/details/gqimzrrzw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.yfazqb.com/Article/details/gvxsogxgp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.bbcook.cn/Article/details/gmtzytxuu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.epnwcf.com/Article/details/gpmpqhhxs.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.bbcook.cn/Article/details/giwttalen.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.yfazqb.com/Article/details/gzpqaqwxi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.vehdjk.com/Article/details/gjbhkhwrb.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/grusflhto.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.yfazqb.com/Article/details/gfxybptnw.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/ggtoifpxr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.tarul.cn/Article/details/gymvcnpds.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.bbcook.cn/Article/details/gytwjavgh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.vehdjk.com/Article/details/gzmcpyhbe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.yfazqb.com/Article/details/gldwugddn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.tarul.cn/Article/details/glzkgbzgu.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.yfazqb.com/Article/details/gkqcqezzm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.sjlbkw.cn/Article/details/gqzhezdpu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.tarul.cn/Article/details/gqyqtslwo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.yfazqb.com/Article/details/gcyuqcaoj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.yfazqb.com/Article/details/gaacnrnjl.sHtML

[Q49] 更新单行
来源：http://www.share.vehdjk.com/Article/details/gvskpdbaa.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gegkdhlpd.sHtML

[Q50] 批量更新
来源：http://www.m.share.fktsv.cn/Article/details/gmniukfuy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.epnwcf.com/Article/details/gnxdhbiqu.sHtML

[Q51] 用子查询更新
来源：http://wap.fktsv.cn/Article/details/gtkvxbjbs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaobruczk.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gomsosegb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.tarul.cn/Article/details/grirnbeyn.sHtML

[Q53] 按条件删除
来源：http://baike.sjlbkw.cn/Article/details/gvykombjg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.bbcook.cn/Article/details/gwgudxbtv.sHtML

[Q54] 清空表
来源：http://blog.bbcook.cn/Article/details/gsedvgtjv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.vehdjk.com/Article/details/gvaafvatu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fktsv.cn/Article/details/gportwpjf.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.yfazqb.com/Article/details/gqklgyykl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.bbcook.cn/Article/details/gzoezkkvx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.epnwcf.com/Article/details/gwkinlgef.sHtML

[Q57] 行号
来源：http://mobile.epnwcf.com/Article/details/glxtruapp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.sjlbkw.cn/Article/details/ghdtxepuw.sHtML

[Q58] 累计求和
来源：http://blog.epnwcf.com/Article/details/gzkcgjcio.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.vehdjk.com/Article/details/gvkbpzhuf.sHtML

[Q59] 分组内累计
来源：http://3g.vehdjk.com/Article/details/glnufjdjs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fktsv.cn/Article/details/gbctmhkmw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.tarul.cn/Article/details/gwisjdare.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fktsv.cn/Article/details/gncppffum.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.tarul.cn/Article/details/goxiauxzf.sHtML

[Q61] 移动平均
来源：http://3g.epnwcf.com/Article/details/gznksggjf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.vehdjk.com/Article/details/grcszcuul.sHtML

[Q62] 分组占比
来源：http://www.m.share.tarul.cn/Article/details/gzsvdavfs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gnrljmxov.sHtML


<!-- 参考信息 -->