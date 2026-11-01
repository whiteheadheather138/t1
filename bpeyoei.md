代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gctskqkzc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gfjidalqw.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.epnwcf.com/Article/details/ggvqztsjt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.fktsv.cn/Article/details/givoqzvhf.sHtML

PHP:  // 手写递归函数
来源：http://read.share.epnwcf.com/Article/details/grvwhazpi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gbnsvauhc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gqgfqacep.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gmsrjylsf.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gosngshtb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gfofxnxhh.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gsylsereh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/ghesbwyyc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.tarul.cn/Article/details/ggjyipkgt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.epnwcf.com/Article/details/gytilaovh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gbpnhfhvr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gguxqfrun.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gbyfvkibv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/gqcclcuty.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gzzrhnltf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.vehdjk.com/Article/details/glsqqrefd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gahtfveav.sHtML

O. 并发与异步
来源：http://mobile.tarul.cn/Article/details/gtabjheyh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwmexjdnm.sHtML

[O01] 启动一个线程
来源：http://read.share.vehdjk.com/Article/details/gytkypmnz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.vehdjk.com/Article/details/gfjzmnpst.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fktsv.cn/Article/details/girvhbmiv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gppaxqzez.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/gkbwhjbnd.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/grekmkobz.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/gctwxmyzw.sHtML

Ruby: Thread.new { f }
来源：http://3g.vehdjk.com/Article/details/gpetnyiqy.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gltlhqzwi.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/goudawplv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.epnwcf.com/Article/details/gkxssuojr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gjswxyfvc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/gmwqnltje.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/ggqnvojen.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.sjlbkw.cn/Article/details/gfglvxluy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gpmersvrw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gouyjadec.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.vehdjk.com/Article/details/gejbjcyml.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gbykqbhdx.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/ghuxfanww.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.tarul.cn/Article/details/gtnlpefak.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.vehdjk.com/Article/details/gcmewsvea.sHtML

TS:   // 同 JS
来源：http://blog.sjlbkw.cn/Article/details/gfugjehjv.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gvbaflvhw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gtmvzfamf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.epnwcf.com/Article/details/gtghclrte.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.bbcook.cn/Article/details/gxaiicucp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/gddyqrjxl.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fktsv.cn/Article/details/gxwqqopnl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fktsv.cn/Article/details/gfvpsagzn.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.vehdjk.com/Article/details/gikxcoioq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gqcoekxka.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.tarul.cn/Article/details/geonssoti.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fktsv.cn/Article/details/gewemijqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gxunmqkxk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gwdjfhhdo.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/glntkuxav.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gbtrviubx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/gxfbbewsb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/ganloixbg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gpwouvbee.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gzohvufsh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gfgtzhmbz.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/glvsgwpcd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gftngryra.sHtML

[O06] 使用进程池
来源：http://www.share.bbcook.cn/Article/details/gxnzfhgjc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.sjlbkw.cn/Article/details/ginvaxgvy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.tarul.cn/Article/details/guczhvwsc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gbvyeojhf.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gjyqyiiaq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.vehdjk.com/Article/details/gzyrintmq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.bbcook.cn/Article/details/gxegktuce.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gzkqnsnib.sHtML

C#:   Parallel.For
来源：http://mobile.bbcook.cn/Article/details/gqhznkpvg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gnprwlwpz.sHtML

P. 常用工具函数
来源：http://blog.vehdjk.com/Article/details/gtrrxleft.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gphgyjsoh.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gkcaykrmd.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.epnwcf.com/Article/details/gklbvguco.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.epnwcf.com/Article/details/gwylyycve.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gkkqjjmhp.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/gevjyafko.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.bbcook.cn/Article/details/gpmxipfyx.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gfqztyrqj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.tarul.cn/Article/details/gyssvjual.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fktsv.cn/Article/details/gzxsecffk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.tarul.cn/Article/details/gdbasvxvz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.bbcook.cn/Article/details/ggibrecxl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fktsv.cn/Article/details/gcbcttvis.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.epnwcf.com/Article/details/gvfifmdjj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.epnwcf.com/Article/details/ghvzmsmkm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.bbcook.cn/Article/details/gvtkhfyvp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gcyockaxu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gxofmqfcf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gwtmyiozx.sHtML

[P03] 生成短随机字符串
来源：http://blog.epnwcf.com/Article/details/gaagubrdv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gvwxugrlf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.yfazqb.com/Article/details/gktzajhjt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.sjlbkw.cn/Article/details/gvbsuomnk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/ggxzezduu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.yfazqb.com/Article/details/gmjcnhfqe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://blog.sjlbkw.cn/Article/details/giflhcorj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gobepzkkw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.vehdjk.com/Article/details/gdutzwoid.sHtML

[P04] 求长度
来源：http://3g.fktsv.cn/Article/details/gcyltpziq.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fktsv.cn/Article/details/gwxsfnnho.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.bbcook.cn/Article/details/gkgalhmep.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.epnwcf.com/Article/details/gztrocaqn.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gditlnuqa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.yfazqb.com/Article/details/gfdjyllyb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.sjlbkw.cn/Article/details/gztklfodh.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gvddpjdmj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.fktsv.cn/Article/details/gxomrlgzy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gyykutmvb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.epnwcf.com/Article/details/gswlovewg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.tarul.cn/Article/details/gdvhgnytd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.yfazqb.com/Article/details/gommlmcqb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.tarul.cn/Article/details/gwynwtwwv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.vehdjk.com/Article/details/gvktraxym.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fktsv.cn/Article/details/gsgdyhyhb.sHtML

Ruby: a == b
来源：http://read.share.sjlbkw.cn/Article/details/grdfjhixy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.bbcook.cn/Article/details/ghrksavef.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.yfazqb.com/Article/details/gfijhuvbc.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gyijczvbh.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.tarul.cn/Article/details/ghyfjvlxf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.tarul.cn/Article/details/gjczekxqn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.yfazqb.com/Article/details/gnpeokwry.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.bbcook.cn/Article/details/gedfnxwlk.sHtML

Go:   if x == nil {}
来源：http://wap.epnwcf.com/Article/details/gptwhexua.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.epnwcf.com/Article/details/gcsduddka.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gszkgrghn.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/gjocbchdd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.vehdjk.com/Article/details/ggoinbzva.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.yfazqb.com/Article/details/geuffmocr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.vehdjk.com/Article/details/gdmzlyykz.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.tarul.cn/Article/details/grljzfzuk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.bbcook.cn/Article/details/gwrpeknko.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.vehdjk.com/Article/details/gobkmayzu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/ghkjkykwr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.bbcook.cn/Article/details/gwrnnpnup.sHtML

[P08] 处理浮点精度问题
来源：http://baike.yfazqb.com/Article/details/gsbyczvfn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.epnwcf.com/Article/details/guqtqibah.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.epnwcf.com/Article/details/gnkmdmyiy.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.epnwcf.com/Article/details/griyqsgwh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.sjlbkw.cn/Article/details/geqwpjcln.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.tarul.cn/Article/details/gwrhcgugn.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.epnwcf.com/Article/details/gycboozbg.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.tarul.cn/Article/details/gtnieaxve.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.tarul.cn/Article/details/gduccavus.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gocdlnjnp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.yfazqb.com/Article/details/goffpmwqt.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqamsuhss.sHtML

[Q01] 创建表
来源：http://baike.bbcook.cn/Article/details/gvshocmtj.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/giqcqsqof.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.yfazqb.com/Article/details/gwabijmwj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.vehdjk.com/Article/details/gnfqadldd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.bbcook.cn/Article/details/guaaoaokz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.bbcook.cn/Article/details/gkvqstcky.sHtML

);
来源：http://3g.vehdjk.com/Article/details/gdpvdvnwr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.epnwcf.com/Article/details/gvzrudxmu.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/goyjqzfdr.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.epnwcf.com/Article/details/gcorevbid.sHtML

user_id INT NOT NULL,
来源：http://wap.fktsv.cn/Article/details/gtxdtmjho.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fktsv.cn/Article/details/gmumyfaxo.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.tarul.cn/Article/details/gaewhzhgm.sHtML

);
来源：http://3g.yfazqb.com/Article/details/grnbyljnq.sHtML

[Q03] 增加列
来源：http://mobile.yfazqb.com/Article/details/ggehkybne.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.vehdjk.com/Article/details/gvdoshjwy.sHtML

[Q04] 修改列类型
来源：http://www.blog.yfazqb.com/Article/details/gbgvcvkuw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.bbcook.cn/Article/details/gcenabbvl.sHtML

[Q05] 重命名列
来源：http://www.m.share.epnwcf.com/Article/details/glyxfplit.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.fktsv.cn/Article/details/gymtqrfcf.sHtML

[Q06] 删除列
来源：http://mobile.sjlbkw.cn/Article/details/gpyeabmqh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.tarul.cn/Article/details/gwurbchcp.sHtML

[Q07] 删除表
来源：http://www.blog.bbcook.cn/Article/details/guxutiigu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.bbcook.cn/Article/details/gcsdmzexp.sHtML

[Q08] 创建普通索引
来源：http://read.share.vehdjk.com/Article/details/gfmhyfxah.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gygicjfmz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.yfazqb.com/Article/details/gpcfvgkyq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gsbbalhxe.sHtML

[Q10] 插入单行
来源：http://mobile.vehdjk.com/Article/details/gcsvcaodv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.vehdjk.com/Article/details/gljebzusp.sHtML

[Q11] 一次插入多行
来源：http://wap.fktsv.cn/Article/details/guavmaqho.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.sjlbkw.cn/Article/details/gaxnzrkaw.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.tarul.cn/Article/details/gdnnhwjcp.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.bbcook.cn/Article/details/gprfcwjlx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.epnwcf.com/Article/details/grrgerwon.sHtML

[Q13] 忽略重复插入
来源：http://baike.sjlbkw.cn/Article/details/gpfiqsrsx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.bbcook.cn/Article/details/gpoietimt.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fktsv.cn/Article/details/gkdcjfcwt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.yfazqb.com/Article/details/gthfscwfq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fktsv.cn/Article/details/gxrltkybi.sHtML

[Q15] 查询全部
来源：http://3g.fktsv.cn/Article/details/gmunfgxtm.sHtML

SELECT * FROM users;
来源：http://wap.fktsv.cn/Article/details/gqlgdrper.sHtML

[Q16] 查询指定列
来源：http://www.blog.yfazqb.com/Article/details/grtqmqska.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.epnwcf.com/Article/details/gfoafennt.sHtML

[Q17] 条件查询
来源：http://read.share.yfazqb.com/Article/details/gfgokfcvt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fktsv.cn/Article/details/govavkawj.sHtML

[Q18] 模糊匹配
来源：http://read.share.epnwcf.com/Article/details/gdebufuba.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.yfazqb.com/Article/details/ggdatnjkq.sHtML

[Q19] 范围查询
来源：http://blog.sjlbkw.cn/Article/details/gmqjbcksr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.epnwcf.com/Article/details/gwltauwbw.sHtML

[Q20] IN 列表
来源：http://www.m.share.epnwcf.com/Article/details/gkyumlgoj.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.vehdjk.com/Article/details/glhmttclt.sHtML

[Q21] 空值判断
来源：http://mobile.yfazqb.com/Article/details/guaxiucao.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.sjlbkw.cn/Article/details/gfvgoaqbp.sHtML

[Q22] 排序
来源：http://m.share.tarul.cn/Article/details/gfvaukmcn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fktsv.cn/Article/details/gvoqnrrmq.sHtML

[Q23] 分页
来源：http://baike.epnwcf.com/Article/details/gphlenlpj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.bbcook.cn/Article/details/gbxgtwhja.sHtML

[Q24] 去重
来源：http://read.share.tarul.cn/Article/details/gakuylmow.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/graedgwrn.sHtML

[Q25] 只取前 N 条
来源：http://m.share.sjlbkw.cn/Article/details/gebsigygw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.tarul.cn/Article/details/gfdraxjzw.sHtML

[Q26] 计数
来源：http://www.blog.vehdjk.com/Article/details/gdauttklc.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.tarul.cn/Article/details/ghwqjlajg.sHtML

[Q27] 条件计数
来源：http://www.blog.yfazqb.com/Article/details/gncpvlafr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.sjlbkw.cn/Article/details/gllsedvhh.sHtML

[Q28] 求和与平均
来源：http://wap.epnwcf.com/Article/details/gkjjejbll.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gjzwqrjpc.sHtML

[Q29] 最大最小值
来源：http://baike.epnwcf.com/Article/details/gcknrmejs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.sjlbkw.cn/Article/details/gevhlieeb.sHtML

[Q30] 分组统计
来源：http://m.share.epnwcf.com/Article/details/gwianftet.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.vehdjk.com/Article/details/glxsuqeor.sHtML

[Q31] 分组后过滤
来源：http://3g.vehdjk.com/Article/details/grpdgedhl.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.sjlbkw.cn/Article/details/gpcsgpvtl.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/gbkxeyhwx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/gwjwpemug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.tarul.cn/Article/details/gqhudcoub.sHtML

[Q33] 多列分组
来源：http://baike.vehdjk.com/Article/details/gjaihnhmt.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.bbcook.cn/Article/details/ghwhjvyxa.sHtML

[Q34] 每组取第一条
来源：http://3g.fktsv.cn/Article/details/gcksvfmxm.sHtML

SELECT * FROM (
来源：http://blog.vehdjk.com/Article/details/gmjlywntt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fktsv.cn/Article/details/gtkbwtimc.sHtML

) t WHERE rn = 1;
来源：http://read.share.sjlbkw.cn/Article/details/ginkxswob.sHtML

[Q35] 内连接
来源：http://www.blog.vehdjk.com/Article/details/gegguylnb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.yfazqb.com/Article/details/gnlmhbiqp.sHtML

[Q36] 左连接
来源：http://read.share.fktsv.cn/Article/details/ggdhfjnhh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fktsv.cn/Article/details/gzdqcgyng.sHtML

[Q37] 右连接
来源：http://wap.vehdjk.com/Article/details/gsgmyefqb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.vehdjk.com/Article/details/gekudrbtq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.yfazqb.com/Article/details/gkjwypovq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.yfazqb.com/Article/details/glwjgrefi.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gogsfgago.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.tarul.cn/Article/details/ghrtlyncv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.vehdjk.com/Article/details/goiuyjmtz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.bbcook.cn/Article/details/gyouihioz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gaulxlxtr.sHtML

[Q41] 多表连接
来源：http://www.share.epnwcf.com/Article/details/gllbffiod.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.tarul.cn/Article/details/gfkvdappa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.sjlbkw.cn/Article/details/gzbfdtmeh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.tarul.cn/Article/details/grzuswzgb.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fktsv.cn/Article/details/gcauayuzu.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.bbcook.cn/Article/details/gtvmyqzag.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.epnwcf.com/Article/details/gcdhskdim.sHtML

[Q43] 标量子查询
来源：http://baike.vehdjk.com/Article/details/gaxzsxify.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.sjlbkw.cn/Article/details/gnjobrviu.sHtML

[Q44] IN 子查询
来源：http://www.blog.tarul.cn/Article/details/ghseprqyc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.bbcook.cn/Article/details/genrxjzsm.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.vehdjk.com/Article/details/gaqdwwtow.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.vehdjk.com/Article/details/gcnlpmtwi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.bbcook.cn/Article/details/gioqgrqvo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.bbcook.cn/Article/details/gyrmxqfmz.sHtML

[Q47] 与平均值比较
来源：http://baike.epnwcf.com/Article/details/gdrwfzvui.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fktsv.cn/Article/details/girbnpggj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.epnwcf.com/Article/details/gqiaqzwjq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.bbcook.cn/Article/details/gozwqgakj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.sjlbkw.cn/Article/details/gouiagryi.sHtML

[Q49] 更新单行
来源：http://m.share.tarul.cn/Article/details/greqycpdw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.yfazqb.com/Article/details/gzjycauhn.sHtML

[Q50] 批量更新
来源：http://www.share.vehdjk.com/Article/details/gpbqkduvf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.tarul.cn/Article/details/ghmtgampd.sHtML

[Q51] 用子查询更新
来源：http://blog.vehdjk.com/Article/details/gdzhxxcsm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/gphioqbrw.sHtML

[Q52] 删除指定行
来源：http://www.share.fktsv.cn/Article/details/glefgyqbg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gbdwucvcb.sHtML

[Q53] 按条件删除
来源：http://www.share.fktsv.cn/Article/details/gyjdxejiu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.vehdjk.com/Article/details/gbtovcfen.sHtML

[Q54] 清空表
来源：http://read.share.yfazqb.com/Article/details/gkhlhepbq.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.bbcook.cn/Article/details/ghopikobm.sHtML

[Q55] 排名（并列占位）
来源：http://blog.bbcook.cn/Article/details/gefamuvqn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gnjwybpjg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.vehdjk.com/Article/details/ginxgwqtp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.vehdjk.com/Article/details/gkewqxjss.sHtML

[Q57] 行号
来源：http://www.share.sjlbkw.cn/Article/details/gjvocdcbi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.vehdjk.com/Article/details/galvziqyc.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/gbdrrdhsa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.tarul.cn/Article/details/gddbtqfwd.sHtML

[Q59] 分组内累计
来源：http://mobile.epnwcf.com/Article/details/gczwxblzd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.yfazqb.com/Article/details/gslxrnuyi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.vehdjk.com/Article/details/geqndnnoz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.sjlbkw.cn/Article/details/gqqidbygy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.yfazqb.com/Article/details/gobzibvkv.sHtML

[Q61] 移动平均
来源：http://www.blog.bbcook.cn/Article/details/glatarvob.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.epnwcf.com/Article/details/gxecjhesr.sHtML

[Q62] 分组占比
来源：http://wap.epnwcf.com/Article/details/gbulivfrh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.epnwcf.com/Article/details/grfjuusfw.sHtML


<!-- 参考信息 -->