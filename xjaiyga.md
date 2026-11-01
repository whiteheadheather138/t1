代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.sjlbkw.cn/Article/details/gglqlgwej.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fktsv.cn/Article/details/ghuqtcxzs.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gadfqmsnb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/ggivqoblx.sHtML

PHP:  // 手写递归函数
来源：http://wap.yfazqb.com/Article/details/gomecrsyy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gmguumwgl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gpcoxlhyx.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gyxwkskbz.sHtML

Go:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gowcevxbq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.tarul.cn/Article/details/grteayamz.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gkdxyyumt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gqufybjav.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gpmibzqtf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gigudazjp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gmfscsawy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gyvsplihe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gngysbsqu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gelmwfqlh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/gmuhmswhw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gtnznjftf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gptigdgoz.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gtskjmdki.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfvavvaqf.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gxvvvylrn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.yfazqb.com/Article/details/gziuiceyq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gfsqpqoej.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gmjplovuq.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/gdggpjjlg.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gsvocryry.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gynpojmvf.sHtML

Ruby: Thread.new { f }
来源：http://blog.yfazqb.com/Article/details/grbfcjyrb.sHtML

C#:   Task.Run(() => F());
来源：http://baike.tarul.cn/Article/details/gzsynymie.sHtML

[O02] 使用线程池
来源：http://blog.yfazqb.com/Article/details/gghwoluww.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/gquqknteg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/gvpdcjmpk.sHtML

JS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gouqostmx.sHtML

TS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gohflmidt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.yfazqb.com/Article/details/gutvrdzsc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.sjlbkw.cn/Article/details/gfaqamysf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gkdcyhkpe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/gmvhisoda.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/gkzhbiwnp.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.yfazqb.com/Article/details/gmjghatwk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.yfazqb.com/Article/details/gbmarpyiv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gepxgxgfr.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/gbaiwuhmv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.vehdjk.com/Article/details/gqscaxmat.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.vehdjk.com/Article/details/gzztomakz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.bbcook.cn/Article/details/gtltqhwja.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/ggvsiyjeu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.vehdjk.com/Article/details/gtbohbvxr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fktsv.cn/Article/details/gjarnbbcw.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.vehdjk.com/Article/details/gfuikxjaz.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gkxfxnmcj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gxepebfqz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fktsv.cn/Article/details/gwuelsqqe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fktsv.cn/Article/details/grzbmiytu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/grplcfiex.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/gcukktjjn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.yfazqb.com/Article/details/gkjhicxat.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gklfbsxkd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gyfajwjfz.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gdxalgobb.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.yfazqb.com/Article/details/gvpzisbwa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsxyqhdi.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/gnnkmaofa.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.epnwcf.com/Article/details/gmbezldfx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.tarul.cn/Article/details/gqjvjfdod.sHtML

[O06] 使用进程池
来源：http://baike.yfazqb.com/Article/details/gjqrmiaat.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gifwhektp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gvovtojmq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gtxloifce.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gmvjjkkup.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/ggcezvexr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/gwbninvai.sHtML

Ruby: // fork 块
来源：http://www.share.vehdjk.com/Article/details/ghkexrvux.sHtML

C#:   Parallel.For
来源：http://m.share.sjlbkw.cn/Article/details/gtlwuavkx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gohxmbwvb.sHtML

P. 常用工具函数
来源：http://m.share.epnwcf.com/Article/details/gpexqtnoe.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqjjqakzv.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gfqyogmmb.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gumzuepwq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.epnwcf.com/Article/details/gprztzhih.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gdrgbmidu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gvsvpnior.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.sjlbkw.cn/Article/details/glidfyenv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.yfazqb.com/Article/details/galybajgr.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/gttpxtidl.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fktsv.cn/Article/details/gerbtaeut.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.sjlbkw.cn/Article/details/gpvmrngcz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.yfazqb.com/Article/details/gytpawjpk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/glttjjosa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/grctrezxc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.bbcook.cn/Article/details/goukqhchu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/gpivkqbal.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.sjlbkw.cn/Article/details/gqycftokx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.bbcook.cn/Article/details/glakrejms.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.sjlbkw.cn/Article/details/gmevnwpiz.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gnghsqocq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gqitusofs.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gvbszwzcs.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.epnwcf.com/Article/details/gxqtokgof.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gprzshbof.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.sjlbkw.cn/Article/details/gteilnwac.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.vehdjk.com/Article/details/gdklsnmdm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.yfazqb.com/Article/details/gcxvhsuar.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/ghtbetikl.sHtML

[P04] 求长度
来源：http://3g.sjlbkw.cn/Article/details/gannmnqle.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.sjlbkw.cn/Article/details/gskquxcwa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/ggjiicipt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gbpsfppbe.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.epnwcf.com/Article/details/guixyapix.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.bbcook.cn/Article/details/gpgsrofct.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gipcdloxi.sHtML

Ruby: x.length;  x.size
来源：http://read.share.sjlbkw.cn/Article/details/gmzlsyxik.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.fktsv.cn/Article/details/gqbguoric.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gmliishqm.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.sjlbkw.cn/Article/details/gbrifjwzr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gurgkykko.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.vehdjk.com/Article/details/gqwajckmx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.sjlbkw.cn/Article/details/grintmpmk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.bbcook.cn/Article/details/giintsskw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/glgkkjhho.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/gbisezrlg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gzfdfcfdj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.sjlbkw.cn/Article/details/gcekkkoap.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.bbcook.cn/Article/details/gofinkxvj.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fktsv.cn/Article/details/gmaczshjx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.bbcook.cn/Article/details/gmjpqkoea.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggjlusjgm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fktsv.cn/Article/details/goffkjdmz.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/grsjthlyn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/gyyvptfdo.sHtML

C#:   if (x is null) {}
来源：http://blog.epnwcf.com/Article/details/gbzqcjvlz.sHtML

[P07] 防抖与节流
来源：http://m.share.tarul.cn/Article/details/gwmfkcugg.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.yfazqb.com/Article/details/ginccvfqj.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.bbcook.cn/Article/details/gvasafgtv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gltinbpus.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/gnlblfbtv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.tarul.cn/Article/details/globoqlcc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.sjlbkw.cn/Article/details/glfkdkilc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fktsv.cn/Article/details/gcsersjxy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.yfazqb.com/Article/details/goohsyyfy.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.epnwcf.com/Article/details/ghxtnzapi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.tarul.cn/Article/details/gqhlfznjz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtxkqghbk.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fktsv.cn/Article/details/gvosivmxz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.tarul.cn/Article/details/givnqchnf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.bbcook.cn/Article/details/gnhlfszsv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.vehdjk.com/Article/details/gtnnrvzcf.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.epnwcf.com/Article/details/glrxpmfiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.yfazqb.com/Article/details/gyrxcaksc.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gfsksvviu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.epnwcf.com/Article/details/gbcvoomnm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gssnzrdef.sHtML

[Q01] 创建表
来源：http://mobile.yfazqb.com/Article/details/gknerzhgd.sHtML

CREATE TABLE users (
来源：http://baike.bbcook.cn/Article/details/gedcatkbx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.bbcook.cn/Article/details/gpgvvtcwe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.bbcook.cn/Article/details/gaoqyjuvq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.vehdjk.com/Article/details/gchbvxigm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.epnwcf.com/Article/details/gllkiygaq.sHtML

);
来源：http://www.m.share.epnwcf.com/Article/details/gjvjpuujf.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gzjjwvayu.sHtML

CREATE TABLE orders (
来源：http://baike.yfazqb.com/Article/details/gyqiryaqb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.tarul.cn/Article/details/guxymmfej.sHtML

user_id INT NOT NULL,
来源：http://wap.epnwcf.com/Article/details/gtvdmquwy.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.sjlbkw.cn/Article/details/gbhrvprnd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.bbcook.cn/Article/details/gzuwulgxe.sHtML

);
来源：http://wap.fktsv.cn/Article/details/gebnuoloh.sHtML

[Q03] 增加列
来源：http://www.blog.sjlbkw.cn/Article/details/gosgnuetl.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.vehdjk.com/Article/details/gezantdyf.sHtML

[Q04] 修改列类型
来源：http://baike.fktsv.cn/Article/details/gkwkukxqn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.yfazqb.com/Article/details/ggxdjctxk.sHtML

[Q05] 重命名列
来源：http://blog.sjlbkw.cn/Article/details/ggflnylxd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.epnwcf.com/Article/details/gymwpkjte.sHtML

[Q06] 删除列
来源：http://3g.bbcook.cn/Article/details/gwtmabtuq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.yfazqb.com/Article/details/glhjjlfca.sHtML

[Q07] 删除表
来源：http://www.share.fktsv.cn/Article/details/gmowuowrm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fktsv.cn/Article/details/gmhzcghsf.sHtML

[Q08] 创建普通索引
来源：http://read.share.tarul.cn/Article/details/glmorkvxc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gcozxvzef.sHtML

[Q09] 创建唯一索引
来源：http://baike.yfazqb.com/Article/details/glnuawesv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/gryyzhnvh.sHtML

[Q10] 插入单行
来源：http://baike.sjlbkw.cn/Article/details/gcllozkze.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.tarul.cn/Article/details/galdkddaj.sHtML

[Q11] 一次插入多行
来源：http://m.share.bbcook.cn/Article/details/gfjspuyfu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/ghovjuohh.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.bbcook.cn/Article/details/gljwvznln.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.bbcook.cn/Article/details/gluwsbiyr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.vehdjk.com/Article/details/gkkglchvp.sHtML

[Q13] 忽略重复插入
来源：http://baike.bbcook.cn/Article/details/gmbkyinsy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.epnwcf.com/Article/details/gesyllgbp.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.epnwcf.com/Article/details/ghscfdefv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.bbcook.cn/Article/details/gxdnzprqf.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.tarul.cn/Article/details/gshsjfgvp.sHtML

[Q15] 查询全部
来源：http://read.share.fktsv.cn/Article/details/gnaakgdqq.sHtML

SELECT * FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gemyklpsq.sHtML

[Q16] 查询指定列
来源：http://www.blog.fktsv.cn/Article/details/ghbaiodgo.sHtML

SELECT id, name FROM users;
来源：http://m.share.fktsv.cn/Article/details/gorixrrvg.sHtML

[Q17] 条件查询
来源：http://www.blog.fktsv.cn/Article/details/grwecqcfw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.epnwcf.com/Article/details/gozafmgfj.sHtML

[Q18] 模糊匹配
来源：http://mobile.fktsv.cn/Article/details/gyisbldxs.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fktsv.cn/Article/details/gwzdeufic.sHtML

[Q19] 范围查询
来源：http://www.share.vehdjk.com/Article/details/gqxfadies.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.yfazqb.com/Article/details/gihkajqwa.sHtML

[Q20] IN 列表
来源：http://www.m.share.fktsv.cn/Article/details/gfukrrgfu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fktsv.cn/Article/details/guniltdes.sHtML

[Q21] 空值判断
来源：http://wap.fktsv.cn/Article/details/gocmirrwk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.vehdjk.com/Article/details/gtvevszqw.sHtML

[Q22] 排序
来源：http://www.blog.vehdjk.com/Article/details/gjbnxugkt.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.yfazqb.com/Article/details/gewyeoopv.sHtML

[Q23] 分页
来源：http://m.share.fktsv.cn/Article/details/gitcekiaj.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.epnwcf.com/Article/details/gfnfmqycc.sHtML

[Q24] 去重
来源：http://www.m.share.tarul.cn/Article/details/gpwqvbmtx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.sjlbkw.cn/Article/details/gdipolnaj.sHtML

[Q25] 只取前 N 条
来源：http://mobile.bbcook.cn/Article/details/gxixsuocj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.bbcook.cn/Article/details/gatsylcyh.sHtML

[Q26] 计数
来源：http://3g.yfazqb.com/Article/details/gziqrblyc.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.epnwcf.com/Article/details/gowpxezko.sHtML

[Q27] 条件计数
来源：http://3g.vehdjk.com/Article/details/gwjzufpod.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fktsv.cn/Article/details/gickxrlsa.sHtML

[Q28] 求和与平均
来源：http://www.m.share.vehdjk.com/Article/details/ghemupize.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.yfazqb.com/Article/details/gnepbrnqt.sHtML

[Q29] 最大最小值
来源：http://mobile.bbcook.cn/Article/details/gjjgnbcdd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.yfazqb.com/Article/details/gjbcyklji.sHtML

[Q30] 分组统计
来源：http://www.share.bbcook.cn/Article/details/gpbzablcx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.tarul.cn/Article/details/gnmdqjzjo.sHtML

[Q31] 分组后过滤
来源：http://read.share.vehdjk.com/Article/details/gjbceukub.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.bbcook.cn/Article/details/gmgfvinoz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fktsv.cn/Article/details/gqxqoqbyb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gjtctmhsh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fktsv.cn/Article/details/gtedsvsil.sHtML

[Q33] 多列分组
来源：http://www.m.share.bbcook.cn/Article/details/gfjowqoqh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.epnwcf.com/Article/details/gjzzfvgkl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.yfazqb.com/Article/details/gldxipchi.sHtML

SELECT * FROM (
来源：http://wap.vehdjk.com/Article/details/gvdooixxz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.bbcook.cn/Article/details/gejtwzluj.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fktsv.cn/Article/details/ghuctsouu.sHtML

[Q35] 内连接
来源：http://mobile.yfazqb.com/Article/details/gxafwxdke.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.vehdjk.com/Article/details/gwmvjkuap.sHtML

[Q36] 左连接
来源：http://3g.epnwcf.com/Article/details/gxsjxjgmi.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.yfazqb.com/Article/details/gkopybape.sHtML

[Q37] 右连接
来源：http://www.m.share.bbcook.cn/Article/details/gftrhajfb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.vehdjk.com/Article/details/gdggiiprq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.vehdjk.com/Article/details/gvupjvlsd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.yfazqb.com/Article/details/gdgmgyaqh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fktsv.cn/Article/details/gjxgszgjd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fktsv.cn/Article/details/gedvzvjdh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.epnwcf.com/Article/details/gjqclupcx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.bbcook.cn/Article/details/gtiscrbhv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.vehdjk.com/Article/details/gdjoozmkx.sHtML

[Q41] 多表连接
来源：http://baike.vehdjk.com/Article/details/gkkvcthkc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.vehdjk.com/Article/details/gxzkcndcu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.yfazqb.com/Article/details/gxersniuh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.sjlbkw.cn/Article/details/gbsjwqpbk.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.sjlbkw.cn/Article/details/ggbmdvrbd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.yfazqb.com/Article/details/gvwbowuqd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.tarul.cn/Article/details/glfcrrmcg.sHtML

[Q43] 标量子查询
来源：http://blog.sjlbkw.cn/Article/details/geikhdliv.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.vehdjk.com/Article/details/gnycskkus.sHtML

[Q44] IN 子查询
来源：http://read.share.bbcook.cn/Article/details/gwmsenpjy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.bbcook.cn/Article/details/gwuioxoxd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.yfazqb.com/Article/details/gkajwvbec.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.yfazqb.com/Article/details/gjvxijyuj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.yfazqb.com/Article/details/gtngpwvkh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.vehdjk.com/Article/details/gqazqrwhu.sHtML

[Q47] 与平均值比较
来源：http://read.share.sjlbkw.cn/Article/details/gjzxiogfy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.tarul.cn/Article/details/gfeemffuo.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fktsv.cn/Article/details/ghfryholl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/gqsxcqtam.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.epnwcf.com/Article/details/grxgbzywr.sHtML

[Q49] 更新单行
来源：http://www.blog.tarul.cn/Article/details/ghjpdyzos.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.vehdjk.com/Article/details/gdzrzowmq.sHtML

[Q50] 批量更新
来源：http://m.share.yfazqb.com/Article/details/gkmgbeigg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.yfazqb.com/Article/details/gcdrxhaof.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fktsv.cn/Article/details/ggloadakz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.epnwcf.com/Article/details/gwnlyjojr.sHtML

[Q52] 删除指定行
来源：http://www.blog.tarul.cn/Article/details/ghlskebpm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.tarul.cn/Article/details/gbwapnsij.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gjmkexlaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.yfazqb.com/Article/details/gqugrhhzz.sHtML

[Q54] 清空表
来源：http://baike.tarul.cn/Article/details/grfwfceew.sHtML

TRUNCATE TABLE logs;
来源：http://blog.epnwcf.com/Article/details/gybusqofp.sHtML

[Q55] 排名（并列占位）
来源：http://blog.yfazqb.com/Article/details/ggtlbuetu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.tarul.cn/Article/details/gdjthuhyo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.epnwcf.com/Article/details/gunxlweib.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.vehdjk.com/Article/details/ggvwgwnii.sHtML

[Q57] 行号
来源：http://www.blog.fktsv.cn/Article/details/gnxzcrkuz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.yfazqb.com/Article/details/gblzramri.sHtML

[Q58] 累计求和
来源：http://mobile.bbcook.cn/Article/details/grfmrrubm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fktsv.cn/Article/details/gjdmhnddi.sHtML

[Q59] 分组内累计
来源：http://blog.epnwcf.com/Article/details/gvvsejdbr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.epnwcf.com/Article/details/gaxvivofd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.yfazqb.com/Article/details/gwvtwltqf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.sjlbkw.cn/Article/details/gfucxiaut.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fktsv.cn/Article/details/givmoakjm.sHtML

[Q61] 移动平均
来源：http://3g.yfazqb.com/Article/details/gwzzsevvk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.tarul.cn/Article/details/gmmdnccqq.sHtML

[Q62] 分组占比
来源：http://www.m.share.fktsv.cn/Article/details/gdxrhtjmj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.bbcook.cn/Article/details/goypjvihs.sHtML


<!-- 参考信息 -->