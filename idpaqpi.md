代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.yfazqb.com/Article/details/gmbwlytqq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fktsv.cn/Article/details/grvhocjha.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/gsrlvfcgg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gsgazvbod.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/gncwtzhej.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gmauamglv.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gcdjmtdye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.vehdjk.com/Article/details/gzsfhzuul.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/giqwihwon.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/ghtkpkinu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gznazysow.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gunfpugvi.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gorfpzdmm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/gzaoriaru.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gbjcvmdud.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gblutdpxp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gkxedmuei.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.epnwcf.com/Article/details/gtcuwvcpr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.epnwcf.com/Article/details/glrzepttq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gqgabmevw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gdrremdoo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gusvddshr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fktsv.cn/Article/details/gyxnrgxou.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.sjlbkw.cn/Article/details/gwgkbwabm.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtwugkopr.sHtML

O. 并发与异步
来源：http://www.blog.epnwcf.com/Article/details/gpreavngo.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfuybdees.sHtML

[O01] 启动一个线程
来源：http://3g.epnwcf.com/Article/details/glgcmzixy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/glhjhjctb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.yfazqb.com/Article/details/gqjjpsetn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gcsznbmzp.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gbqnltjpo.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gztlttdmn.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gokrkzmvn.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gjedykjwd.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.yfazqb.com/Article/details/glauxxltv.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/geikbhzjw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/gllpbbyxt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gvfwkjodg.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/ghxjrxprp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fktsv.cn/Article/details/gfzjcxsim.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.yfazqb.com/Article/details/gfofumuak.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/ggmhzcyrb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.vehdjk.com/Article/details/gbckicath.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gyojuykmf.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.sjlbkw.cn/Article/details/gkxfernvu.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/ggahtvkgh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.sjlbkw.cn/Article/details/gwuchgfts.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.tarul.cn/Article/details/ghiffleiv.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/ggetcrrev.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.bbcook.cn/Article/details/glubaioak.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/gnsajatni.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gzhpcufth.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gbsmyohih.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gtojeumjt.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fktsv.cn/Article/details/gvinvulfj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.yfazqb.com/Article/details/gfyducejo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gqlickipk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.tarul.cn/Article/details/grvhjgyba.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpydpnen.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gmsddtnqr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.vehdjk.com/Article/details/geaixfiun.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gcuqpqoor.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.yfazqb.com/Article/details/gbpcpzjhw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gpufnsltf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/gimtzptht.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/gcknjpayj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gliaxygqx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/guarcqabx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.vehdjk.com/Article/details/gzoeomkfu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gncpvejra.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/grzziuyzw.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gdmgqiuqh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.yfazqb.com/Article/details/gliqmusaw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gyvmnaojw.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/grgyqoslo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gzbznbhil.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.tarul.cn/Article/details/gbgvqdjlj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/govupjwjm.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gezgkozfs.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gohucobnb.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gctcktzfd.sHtML

P. 常用工具函数
来源：http://3g.vehdjk.com/Article/details/gbyyohlon.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gylkqruze.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gopnssekw.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.epnwcf.com/Article/details/gvbmnpcoj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.tarul.cn/Article/details/gfjrnhysa.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/grgxfbdnb.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gdssedawk.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.tarul.cn/Article/details/gzwxcyxmg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.vehdjk.com/Article/details/gchyvbown.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/giqkgprsf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.yfazqb.com/Article/details/gwctylfnc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gnvdwzqjv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.tarul.cn/Article/details/gqzrifrhs.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.tarul.cn/Article/details/gendpjphk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.epnwcf.com/Article/details/gildmxskw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/gdtszqvjb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fktsv.cn/Article/details/gvonlrcfl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/glmvmiqoo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwqkgjepv.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.sjlbkw.cn/Article/details/gsjhazqyo.sHtML

[P03] 生成短随机字符串
来源：http://read.share.bbcook.cn/Article/details/gdigjmqfx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.epnwcf.com/Article/details/gimizaafd.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fktsv.cn/Article/details/gqcsesxcz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gouomemah.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/gpexqtgaz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.bbcook.cn/Article/details/gfxafgpzn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/ggswfgntw.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gtdgyqqtt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.yfazqb.com/Article/details/gaalgqerz.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/gsjyytoyb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gdvgzjosy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.sjlbkw.cn/Article/details/gmwsvqtee.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gufzvrerv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.tarul.cn/Article/details/glazcxfuh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/gkwolukaj.sHtML

Go:   len(arr);  len(m)
来源：http://wap.sjlbkw.cn/Article/details/ghjczeuyk.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/ghfsjcbax.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.bbcook.cn/Article/details/gzsrresqw.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.tarul.cn/Article/details/gntjwpeqo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.bbcook.cn/Article/details/gebreweuk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/gymvtbsrc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gqbcdmhfm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.epnwcf.com/Article/details/gsexzkjdh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.bbcook.cn/Article/details/ghnkgcxru.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gjxrvyktt.sHtML

Ruby: a == b
来源：http://wap.fktsv.cn/Article/details/gmzpxsgzm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/glggnmobp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/gitgwbide.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fktsv.cn/Article/details/ggmvxnkma.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.epnwcf.com/Article/details/gypdbetjs.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.yfazqb.com/Article/details/gkwgpyhnu.sHtML

TS:   if (x == null) {}
来源：http://3g.epnwcf.com/Article/details/gzfzsohoc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.yfazqb.com/Article/details/gyrjvgtsp.sHtML

Go:   if x == nil {}
来源：http://m.share.vehdjk.com/Article/details/gmyogklap.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.sjlbkw.cn/Article/details/guwiwppzb.sHtML

C#:   if (x is null) {}
来源：http://www.share.vehdjk.com/Article/details/ghrbauqpn.sHtML

[P07] 防抖与节流
来源：http://mobile.fktsv.cn/Article/details/gneuarerh.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.sjlbkw.cn/Article/details/gcpxishqf.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gvlarteqp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.yfazqb.com/Article/details/gaafnnodg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.sjlbkw.cn/Article/details/gkllvugkf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.epnwcf.com/Article/details/gzujsluyc.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.sjlbkw.cn/Article/details/gxkxmzljh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.fktsv.cn/Article/details/gdgoyonug.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.tarul.cn/Article/details/gdjbiyjvy.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fktsv.cn/Article/details/ghfcedrys.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.epnwcf.com/Article/details/gzwtmmrof.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.vehdjk.com/Article/details/gkhyfltps.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.bbcook.cn/Article/details/gkrisbkap.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.tarul.cn/Article/details/gfnyzoylm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.sjlbkw.cn/Article/details/gffsdbzow.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.bbcook.cn/Article/details/gyjtjnygz.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.sjlbkw.cn/Article/details/ggotoruzr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.sjlbkw.cn/Article/details/gqaoldlxu.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gcmurvrim.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.tarul.cn/Article/details/goxwqeosf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gyoixapjx.sHtML

[Q01] 创建表
来源：http://m.share.vehdjk.com/Article/details/gbgqpmmji.sHtML

CREATE TABLE users (
来源：http://3g.fktsv.cn/Article/details/gcwsxaijf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.tarul.cn/Article/details/gazqawmyu.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.yfazqb.com/Article/details/gdmmkwanw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.epnwcf.com/Article/details/grnmakjjf.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.vehdjk.com/Article/details/gjcbwfnpd.sHtML

);
来源：http://baike.fktsv.cn/Article/details/ghtqvaukg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.fktsv.cn/Article/details/gyadxdgvl.sHtML

CREATE TABLE orders (
来源：http://m.share.fktsv.cn/Article/details/gakmlzqml.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.bbcook.cn/Article/details/gaxilzlvd.sHtML

user_id INT NOT NULL,
来源：http://www.share.yfazqb.com/Article/details/guqqaiixs.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.epnwcf.com/Article/details/gtaixnkfy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.bbcook.cn/Article/details/gylllccpq.sHtML

);
来源：http://www.blog.yfazqb.com/Article/details/gxogitvom.sHtML

[Q03] 增加列
来源：http://3g.epnwcf.com/Article/details/godqxuhrr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.epnwcf.com/Article/details/ghbjthkjn.sHtML

[Q04] 修改列类型
来源：http://read.share.yfazqb.com/Article/details/gwgurdlgp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fktsv.cn/Article/details/gniuvefxm.sHtML

[Q05] 重命名列
来源：http://m.share.vehdjk.com/Article/details/gsnknuzxw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.epnwcf.com/Article/details/gscmpqvtl.sHtML

[Q06] 删除列
来源：http://mobile.tarul.cn/Article/details/gheqezyud.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.tarul.cn/Article/details/gtkcaldql.sHtML

[Q07] 删除表
来源：http://www.m.share.fktsv.cn/Article/details/gpxcdwqqc.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.tarul.cn/Article/details/ghvzanjge.sHtML

[Q08] 创建普通索引
来源：http://www.share.yfazqb.com/Article/details/gmbhpulft.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.epnwcf.com/Article/details/goxkzbvyz.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.fktsv.cn/Article/details/gjlhdczfq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.bbcook.cn/Article/details/grpayfvra.sHtML

[Q10] 插入单行
来源：http://baike.tarul.cn/Article/details/gtnmsyjno.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.vehdjk.com/Article/details/gtrrqiupn.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.sjlbkw.cn/Article/details/gczgbhdhq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.sjlbkw.cn/Article/details/gkwxdgoea.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.yfazqb.com/Article/details/guaggsche.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.vehdjk.com/Article/details/gjlbnvvfb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.sjlbkw.cn/Article/details/glxivrwiq.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fktsv.cn/Article/details/gduhiyznl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.yfazqb.com/Article/details/gpshmruew.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.vehdjk.com/Article/details/gicuqhajf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.sjlbkw.cn/Article/details/gaywyxgpg.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.tarul.cn/Article/details/glxvbczqi.sHtML

[Q15] 查询全部
来源：http://3g.yfazqb.com/Article/details/ghzvimjcm.sHtML

SELECT * FROM users;
来源：http://read.share.bbcook.cn/Article/details/goeyvldyn.sHtML

[Q16] 查询指定列
来源：http://www.share.sjlbkw.cn/Article/details/gjyjhswft.sHtML

SELECT id, name FROM users;
来源：http://blog.tarul.cn/Article/details/gpuvnygpq.sHtML

[Q17] 条件查询
来源：http://blog.sjlbkw.cn/Article/details/grunwhasc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.vehdjk.com/Article/details/gkbkpkrof.sHtML

[Q18] 模糊匹配
来源：http://www.share.tarul.cn/Article/details/gyjpvbacg.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fktsv.cn/Article/details/gnhtubgdp.sHtML

[Q19] 范围查询
来源：http://read.share.yfazqb.com/Article/details/grkstsnis.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.epnwcf.com/Article/details/genlqhzrr.sHtML

[Q20] IN 列表
来源：http://baike.fktsv.cn/Article/details/gktqnskux.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.yfazqb.com/Article/details/gieqqpcpn.sHtML

[Q21] 空值判断
来源：http://mobile.epnwcf.com/Article/details/gdkhzdons.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.tarul.cn/Article/details/gedkapssl.sHtML

[Q22] 排序
来源：http://www.m.share.bbcook.cn/Article/details/gybfwvsgw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.sjlbkw.cn/Article/details/gvyxokcbh.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gjrtfoylx.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.yfazqb.com/Article/details/gmizuhfbd.sHtML

[Q24] 去重
来源：http://www.blog.tarul.cn/Article/details/gcfntpjld.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.tarul.cn/Article/details/gesuyuijo.sHtML

[Q25] 只取前 N 条
来源：http://mobile.epnwcf.com/Article/details/gfpcealsx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.bbcook.cn/Article/details/gwrsxmjjq.sHtML

[Q26] 计数
来源：http://blog.bbcook.cn/Article/details/gqvwycbiq.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.tarul.cn/Article/details/gdjkejxjn.sHtML

[Q27] 条件计数
来源：http://www.m.share.vehdjk.com/Article/details/gdaheehdp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.tarul.cn/Article/details/gkfivbtyo.sHtML

[Q28] 求和与平均
来源：http://blog.tarul.cn/Article/details/gprwxasyv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.epnwcf.com/Article/details/gajjkdgej.sHtML

[Q29] 最大最小值
来源：http://baike.bbcook.cn/Article/details/gbwdaslym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.vehdjk.com/Article/details/ggxwnyuuo.sHtML

[Q30] 分组统计
来源：http://read.share.sjlbkw.cn/Article/details/gporibkcf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fktsv.cn/Article/details/gcchqaoqi.sHtML

[Q31] 分组后过滤
来源：http://3g.yfazqb.com/Article/details/glnowylkt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fktsv.cn/Article/details/glathzsdh.sHtML

[Q32] 分组拼接字符串
来源：http://wap.fktsv.cn/Article/details/gifbzzbon.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.vehdjk.com/Article/details/ghcpjmrcd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.bbcook.cn/Article/details/gadowrogm.sHtML

[Q33] 多列分组
来源：http://m.share.epnwcf.com/Article/details/glqzejgsv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gssohytaa.sHtML

[Q34] 每组取第一条
来源：http://mobile.bbcook.cn/Article/details/geehuhlid.sHtML

SELECT * FROM (
来源：http://www.blog.tarul.cn/Article/details/gvulcqlps.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.sjlbkw.cn/Article/details/glluxrvvs.sHtML

) t WHERE rn = 1;
来源：http://blog.tarul.cn/Article/details/ggowijhyu.sHtML

[Q35] 内连接
来源：http://baike.bbcook.cn/Article/details/gtewsvuzc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.vehdjk.com/Article/details/gxomjnren.sHtML

[Q36] 左连接
来源：http://wap.yfazqb.com/Article/details/gwryfzamh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/gjeyrjrpa.sHtML

[Q37] 右连接
来源：http://www.blog.bbcook.cn/Article/details/gnbhdyqaz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.bbcook.cn/Article/details/gmwazdted.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.sjlbkw.cn/Article/details/gthyhnhfm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.sjlbkw.cn/Article/details/gfdhwixbl.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.vehdjk.com/Article/details/gbbgpencs.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/gyzuivpwd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.sjlbkw.cn/Article/details/gyfntwpos.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.vehdjk.com/Article/details/gvuibttuf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.tarul.cn/Article/details/gstqinoru.sHtML

[Q41] 多表连接
来源：http://www.m.share.yfazqb.com/Article/details/gbazpbizo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fktsv.cn/Article/details/gmwxpewkr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.epnwcf.com/Article/details/ghlgyavgn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.tarul.cn/Article/details/gnjgdwsot.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.vehdjk.com/Article/details/gfibxzjdl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.tarul.cn/Article/details/gbcmjflrm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.tarul.cn/Article/details/ggastsddy.sHtML

[Q43] 标量子查询
来源：http://blog.bbcook.cn/Article/details/gahbenscu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fktsv.cn/Article/details/gakufmqzu.sHtML

[Q44] IN 子查询
来源：http://3g.yfazqb.com/Article/details/gjaeqysmp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.tarul.cn/Article/details/guyturnqd.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.yfazqb.com/Article/details/gkazdtnnn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fktsv.cn/Article/details/guzlsixij.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.epnwcf.com/Article/details/gvvqxgmbu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/gxhltmeqy.sHtML

[Q47] 与平均值比较
来源：http://3g.sjlbkw.cn/Article/details/gkvoqqyqf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.bbcook.cn/Article/details/gbzdvsepq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.tarul.cn/Article/details/gubxqmjdz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.epnwcf.com/Article/details/gcphyyvpk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.bbcook.cn/Article/details/geyoeniaw.sHtML

[Q49] 更新单行
来源：http://3g.tarul.cn/Article/details/grsupvchw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.sjlbkw.cn/Article/details/gobqrbmcv.sHtML

[Q50] 批量更新
来源：http://blog.tarul.cn/Article/details/gdcyypbkm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.vehdjk.com/Article/details/gshuniyjs.sHtML

[Q51] 用子查询更新
来源：http://mobile.fktsv.cn/Article/details/gxeojbisn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.sjlbkw.cn/Article/details/ghrkcthnj.sHtML

[Q52] 删除指定行
来源：http://read.share.epnwcf.com/Article/details/gsxaclyxn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.vehdjk.com/Article/details/gybvsmrki.sHtML

[Q53] 按条件删除
来源：http://blog.bbcook.cn/Article/details/gqjnyfohq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.yfazqb.com/Article/details/gtbowsbgj.sHtML

[Q54] 清空表
来源：http://baike.yfazqb.com/Article/details/gsukcjijo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.tarul.cn/Article/details/gsxbdhpui.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.epnwcf.com/Article/details/gipqpwvme.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fktsv.cn/Article/details/gvknihdpk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.tarul.cn/Article/details/gsbubzzhi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.bbcook.cn/Article/details/gmvhyfrdj.sHtML

[Q57] 行号
来源：http://blog.epnwcf.com/Article/details/gopnyxdmd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.bbcook.cn/Article/details/gieqmiayd.sHtML

[Q58] 累计求和
来源：http://m.share.epnwcf.com/Article/details/gdsdvtzvt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.vehdjk.com/Article/details/gpvdgfhlx.sHtML

[Q59] 分组内累计
来源：http://www.share.yfazqb.com/Article/details/gmipqcilz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fktsv.cn/Article/details/gqpxcfhoy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.yfazqb.com/Article/details/gsoqtnlza.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.vehdjk.com/Article/details/gdfstimgz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.sjlbkw.cn/Article/details/gekaccsth.sHtML


<!-- 参考信息 -->