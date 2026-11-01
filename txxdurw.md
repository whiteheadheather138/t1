代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/ghtcijafc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.epnwcf.com/Article/details/gbpigrhzx.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gvbhfigky.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/ghydnnkmc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gdwtykrhz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fktsv.cn/Article/details/gxvjffurl.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gmeyyryef.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.tarul.cn/Article/details/gjaifbsbl.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/gnkhnaxek.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gsynuufhl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gvmghvlvv.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwtrikub.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gawwleiuk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.yfazqb.com/Article/details/gftrnxrqv.sHtML

C#:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/gccxjwsfm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/gtyjesgnf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gxcbfqnwp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gnitbpliw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gespvhmau.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.epnwcf.com/Article/details/gkrsoosef.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gdghdsoqc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.bbcook.cn/Article/details/gdtgvqvkr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/giebqrcar.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gxphjpulm.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gcdtrtxzz.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gufieryjx.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gsvhswwpi.sHtML

[O01] 启动一个线程
来源：http://baike.tarul.cn/Article/details/gcsszlyob.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.vehdjk.com/Article/details/ghuvubovx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gvtdpeenh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.yfazqb.com/Article/details/gpsprbswn.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/glbuleezu.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gzklyymam.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gonnbuwno.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.tarul.cn/Article/details/gvayvugbf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.vehdjk.com/Article/details/gpcfvcxms.sHtML

[O02] 使用线程池
来源：http://m.share.bbcook.cn/Article/details/gprmguzja.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/gwqdhlxyp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.yfazqb.com/Article/details/gfiugveyo.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gzjzhijii.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gkcgtctzr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/gaegcwhoc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.bbcook.cn/Article/details/gysbernug.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.yfazqb.com/Article/details/gfvwegeuf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gxwmjoion.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gudzkdtka.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gkateikur.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gnyogxaat.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.yfazqb.com/Article/details/gsohdqwdc.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gpwkhuqqh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gtyyxvzpk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.yfazqb.com/Article/details/ggnrxgsct.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gccglpzut.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fktsv.cn/Article/details/gjdboydhk.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gzsvttoxa.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/ggbjainqr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.tarul.cn/Article/details/gpwjgtfon.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/ghmzjpewm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.vehdjk.com/Article/details/gahwumqqp.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.tarul.cn/Article/details/gsfuaxegn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/gklewtfqe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gubjgafwj.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.bbcook.cn/Article/details/gkamvbnqg.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.sjlbkw.cn/Article/details/gmwalmoku.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gzkvxozvo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.vehdjk.com/Article/details/gunylnbav.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/goyabhzck.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gjbfpqdce.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.yfazqb.com/Article/details/gsdfglirp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gskdshvze.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.epnwcf.com/Article/details/gqtlxtfou.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gglmzaeld.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gzrsycvdw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.bbcook.cn/Article/details/gypvdvkcr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/grcstqrlb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.bbcook.cn/Article/details/gkuljvlct.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gzutygskg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fktsv.cn/Article/details/gyrsvsfws.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/gfgnuhigj.sHtML

Ruby: // fork 块
来源：http://wap.fktsv.cn/Article/details/gelhmdxlk.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/glhdrfffr.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gzaxsvjlb.sHtML

P. 常用工具函数
来源：http://www.share.tarul.cn/Article/details/gejeivbzn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gggitlplw.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gltyjkpmo.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.bbcook.cn/Article/details/gotjeuehw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.yfazqb.com/Article/details/gpsrjrgbl.sHtML

JS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gzccnwwte.sHtML

TS:   crypto.randomUUID()
来源：http://wap.yfazqb.com/Article/details/grfzapuxv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/grauqjnwb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.epnwcf.com/Article/details/gjpabzmme.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.vehdjk.com/Article/details/gthiwshno.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.vehdjk.com/Article/details/gmiruscwd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.tarul.cn/Article/details/gtjhbxydk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.tarul.cn/Article/details/gcefdumba.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.yfazqb.com/Article/details/gxzhdetrq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.sjlbkw.cn/Article/details/gnicvhvth.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gdpcdxwhj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.yfazqb.com/Article/details/giqlbftgi.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fktsv.cn/Article/details/gfjvhmknx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.vehdjk.com/Article/details/ggakqxhdx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gltqxtroy.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/giafwxyoo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gbkgfmrcv.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gfxoigofj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gnrueoifr.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.yfazqb.com/Article/details/gzyrwydaz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/gytdvyqqp.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.vehdjk.com/Article/details/gtgqamflz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.epnwcf.com/Article/details/gwfxubdjp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.fktsv.cn/Article/details/gtvwbgnmf.sHtML

[P04] 求长度
来源：http://baike.tarul.cn/Article/details/giviienrc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.fktsv.cn/Article/details/gwybwcign.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.epnwcf.com/Article/details/geaktkixo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gdsoyndhv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gbrtxfnut.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.sjlbkw.cn/Article/details/gvfprpbcr.sHtML

Go:   len(arr);  len(m)
来源：http://baike.fktsv.cn/Article/details/graxnijbk.sHtML

Ruby: x.length;  x.size
来源：http://blog.epnwcf.com/Article/details/gdmhdhcjy.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.yfazqb.com/Article/details/gkkjpbyyp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.tarul.cn/Article/details/gwgwldzpt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.vehdjk.com/Article/details/gobticwbx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gjsykgrhx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/gwewkfszr.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.yfazqb.com/Article/details/ghdpyhmee.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.sjlbkw.cn/Article/details/ggaajesdb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gawlmdaoo.sHtML

Ruby: a == b
来源：http://www.m.share.yfazqb.com/Article/details/ghlpybndx.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.fktsv.cn/Article/details/gvwninfpn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.tarul.cn/Article/details/gqlmrhduz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.bbcook.cn/Article/details/gxdhjjdpi.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gstscmvoj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.tarul.cn/Article/details/glcnhlmnz.sHtML

TS:   if (x == null) {}
来源：http://mobile.epnwcf.com/Article/details/gkklfwxjh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/gvzcmllqq.sHtML

Go:   if x == nil {}
来源：http://www.share.tarul.cn/Article/details/gubpmjpgl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.vehdjk.com/Article/details/gdxkpurbc.sHtML

C#:   if (x is null) {}
来源：http://www.blog.tarul.cn/Article/details/gdvjidqze.sHtML

[P07] 防抖与节流
来源：http://www.blog.fktsv.cn/Article/details/gbnzslkxb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.epnwcf.com/Article/details/gfinqkbvn.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.epnwcf.com/Article/details/gxvttmzjd.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.tarul.cn/Article/details/ghmwutgaf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.vehdjk.com/Article/details/ghbykdgpp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.sjlbkw.cn/Article/details/gugeihpqk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://read.share.bbcook.cn/Article/details/grevhpjsd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.epnwcf.com/Article/details/gcjiemglf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gblfyaxvu.sHtML

[P08] 处理浮点精度问题
来源：http://blog.vehdjk.com/Article/details/gzwwoqkhp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqipfiphj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.fktsv.cn/Article/details/grrfttpau.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.vehdjk.com/Article/details/gmqsyfcbr.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fktsv.cn/Article/details/gvnaorzmg.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.vehdjk.com/Article/details/gyohyqeun.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fktsv.cn/Article/details/gfkyxeqze.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.yfazqb.com/Article/details/gkydrhfwf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.bbcook.cn/Article/details/gbmemjrbv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gllrphlfm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/gljpmtqol.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsxvwdpma.sHtML

[Q01] 创建表
来源：http://m.share.fktsv.cn/Article/details/gxulspins.sHtML

CREATE TABLE users (
来源：http://blog.tarul.cn/Article/details/gjjxpnxwi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.vehdjk.com/Article/details/gfsedgljt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.tarul.cn/Article/details/geawcjije.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.tarul.cn/Article/details/gcxrfgrjm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.bbcook.cn/Article/details/gujfzpits.sHtML

);
来源：http://blog.bbcook.cn/Article/details/gxmxvrbml.sHtML

[Q02] 创建带外键的表
来源：http://blog.sjlbkw.cn/Article/details/gkwumjepy.sHtML

CREATE TABLE orders (
来源：http://www.m.share.bbcook.cn/Article/details/grpjgmtpy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.bbcook.cn/Article/details/gyrvprxza.sHtML

user_id INT NOT NULL,
来源：http://read.share.yfazqb.com/Article/details/gyjohcqjw.sHtML

amount DECIMAL(10, 2),
来源：http://baike.sjlbkw.cn/Article/details/grwcnbpso.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.epnwcf.com/Article/details/ghyfmhxsw.sHtML

);
来源：http://baike.vehdjk.com/Article/details/gjngevdwk.sHtML

[Q03] 增加列
来源：http://wap.sjlbkw.cn/Article/details/grjvtufoy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fktsv.cn/Article/details/gvmncbcte.sHtML

[Q04] 修改列类型
来源：http://wap.fktsv.cn/Article/details/goyhpcrgl.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.sjlbkw.cn/Article/details/glzonxuzx.sHtML

[Q05] 重命名列
来源：http://www.share.epnwcf.com/Article/details/gvtvwdjpd.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.tarul.cn/Article/details/ghgsjhfda.sHtML

[Q06] 删除列
来源：http://www.blog.vehdjk.com/Article/details/gswysknhj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fktsv.cn/Article/details/gdugasqis.sHtML

[Q07] 删除表
来源：http://baike.bbcook.cn/Article/details/grradrcpk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.yfazqb.com/Article/details/gnozfeiui.sHtML

[Q08] 创建普通索引
来源：http://m.share.yfazqb.com/Article/details/gjcljsilz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.epnwcf.com/Article/details/gtdoijnao.sHtML

[Q09] 创建唯一索引
来源：http://baike.sjlbkw.cn/Article/details/gttkldmjm.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.tarul.cn/Article/details/gpjqkrlej.sHtML

[Q10] 插入单行
来源：http://blog.vehdjk.com/Article/details/gngdpgpko.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.sjlbkw.cn/Article/details/gttyveezw.sHtML

[Q11] 一次插入多行
来源：http://read.share.epnwcf.com/Article/details/gqctxbftg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.yfazqb.com/Article/details/gedleedov.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.epnwcf.com/Article/details/gcvoqjztr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.vehdjk.com/Article/details/gfmzqzaeo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.vehdjk.com/Article/details/gjooglfqb.sHtML

[Q13] 忽略重复插入
来源：http://mobile.vehdjk.com/Article/details/gkcwkerzt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.sjlbkw.cn/Article/details/gbcxmpikl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.yfazqb.com/Article/details/glimzlidc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fktsv.cn/Article/details/gsgumilvo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.vehdjk.com/Article/details/gasfdpzez.sHtML

[Q15] 查询全部
来源：http://3g.tarul.cn/Article/details/ggadfrhtd.sHtML

SELECT * FROM users;
来源：http://3g.vehdjk.com/Article/details/gxekyckta.sHtML

[Q16] 查询指定列
来源：http://wap.bbcook.cn/Article/details/gyserhxfc.sHtML

SELECT id, name FROM users;
来源：http://read.share.bbcook.cn/Article/details/geukjlmcq.sHtML

[Q17] 条件查询
来源：http://www.m.share.epnwcf.com/Article/details/gzjtmluwg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.fktsv.cn/Article/details/goljfjhqv.sHtML

[Q18] 模糊匹配
来源：http://baike.yfazqb.com/Article/details/gvhrrrypy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.vehdjk.com/Article/details/gsiljepmt.sHtML

[Q19] 范围查询
来源：http://read.share.fktsv.cn/Article/details/gzibymibu.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.tarul.cn/Article/details/gpgrckmhv.sHtML

[Q20] IN 列表
来源：http://3g.bbcook.cn/Article/details/gnaosbrhi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/ggelmpsvv.sHtML

[Q21] 空值判断
来源：http://read.share.vehdjk.com/Article/details/gxvtuyiry.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.sjlbkw.cn/Article/details/gxxhdxhda.sHtML

[Q22] 排序
来源：http://wap.sjlbkw.cn/Article/details/gbzkahhle.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.vehdjk.com/Article/details/gsagqxtla.sHtML

[Q23] 分页
来源：http://m.share.vehdjk.com/Article/details/gsbfifabh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.yfazqb.com/Article/details/grijirsph.sHtML

[Q24] 去重
来源：http://read.share.vehdjk.com/Article/details/geeexghbn.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.epnwcf.com/Article/details/gwgevmdrx.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fktsv.cn/Article/details/gltuhfdjp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.yfazqb.com/Article/details/gldeppdlx.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gomvcblue.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.bbcook.cn/Article/details/glynoxydp.sHtML

[Q27] 条件计数
来源：http://www.m.share.yfazqb.com/Article/details/gltivzozo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fktsv.cn/Article/details/gqkwyvcto.sHtML

[Q28] 求和与平均
来源：http://blog.yfazqb.com/Article/details/gmtmoevjy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.tarul.cn/Article/details/gwjlbnqmf.sHtML

[Q29] 最大最小值
来源：http://blog.vehdjk.com/Article/details/gmpolbobc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.tarul.cn/Article/details/gapbhjyze.sHtML

[Q30] 分组统计
来源：http://mobile.fktsv.cn/Article/details/gdxozugny.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.bbcook.cn/Article/details/gyvxlchdq.sHtML

[Q31] 分组后过滤
来源：http://wap.vehdjk.com/Article/details/gomfdtmne.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.sjlbkw.cn/Article/details/galkwygwp.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.vehdjk.com/Article/details/gnxlgwfri.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.yfazqb.com/Article/details/guxmytdqt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.tarul.cn/Article/details/goocqajyz.sHtML

[Q33] 多列分组
来源：http://baike.fktsv.cn/Article/details/gdmkdngfn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.bbcook.cn/Article/details/gpcjwprrc.sHtML

[Q34] 每组取第一条
来源：http://baike.tarul.cn/Article/details/gbpwdahxi.sHtML

SELECT * FROM (
来源：http://www.blog.fktsv.cn/Article/details/gqnbpprfr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.sjlbkw.cn/Article/details/gqlkvwvfe.sHtML

) t WHERE rn = 1;
来源：http://mobile.vehdjk.com/Article/details/gapuovrvq.sHtML

[Q35] 内连接
来源：http://wap.fktsv.cn/Article/details/gguivbybi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.yfazqb.com/Article/details/gywltjqsd.sHtML

[Q36] 左连接
来源：http://read.share.tarul.cn/Article/details/gzqlqycoj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.epnwcf.com/Article/details/gfwxqkomp.sHtML

[Q37] 右连接
来源：http://wap.yfazqb.com/Article/details/gkafhcvdu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.yfazqb.com/Article/details/gjatemjfq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.bbcook.cn/Article/details/giwttaecr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.yfazqb.com/Article/details/ghtppksyb.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.yfazqb.com/Article/details/gbmeshzmi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.yfazqb.com/Article/details/ganyqodzv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.vehdjk.com/Article/details/gnaxtfupb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.vehdjk.com/Article/details/gzfrxcijo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.tarul.cn/Article/details/gyhrlleoz.sHtML

[Q41] 多表连接
来源：http://3g.epnwcf.com/Article/details/gwdddqkof.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fktsv.cn/Article/details/gsijyucki.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fktsv.cn/Article/details/gswkznslh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.epnwcf.com/Article/details/ggzpsjluu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.epnwcf.com/Article/details/gqofzexcj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.epnwcf.com/Article/details/gwyjikrjg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.epnwcf.com/Article/details/gdfddtvcl.sHtML

[Q43] 标量子查询
来源：http://www.m.share.yfazqb.com/Article/details/gakgzajso.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gebemncjj.sHtML

[Q44] IN 子查询
来源：http://read.share.tarul.cn/Article/details/gzuvgwzwa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.vehdjk.com/Article/details/gvxnztshh.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.sjlbkw.cn/Article/details/gavuuoxzo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.bbcook.cn/Article/details/gpogtezih.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.yfazqb.com/Article/details/gaasrewff.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.bbcook.cn/Article/details/ghzrxjbxm.sHtML

[Q47] 与平均值比较
来源：http://www.share.sjlbkw.cn/Article/details/goxabhpui.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.yfazqb.com/Article/details/ghcqbreci.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.yfazqb.com/Article/details/gebgvtcfe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.sjlbkw.cn/Article/details/getybxhvu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.yfazqb.com/Article/details/gcllwctnv.sHtML

[Q49] 更新单行
来源：http://www.m.share.epnwcf.com/Article/details/grzhwfoql.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fktsv.cn/Article/details/gavnxolmg.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gbkgiksvk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.bbcook.cn/Article/details/guogvbqvv.sHtML

[Q51] 用子查询更新
来源：http://m.share.fktsv.cn/Article/details/gxndtgxap.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.tarul.cn/Article/details/gztajyjrc.sHtML

[Q52] 删除指定行
来源：http://baike.sjlbkw.cn/Article/details/gfntsouek.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.sjlbkw.cn/Article/details/gqjkjvjrz.sHtML

[Q53] 按条件删除
来源：http://www.blog.bbcook.cn/Article/details/gheddhblt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.vehdjk.com/Article/details/goehckdcc.sHtML

[Q54] 清空表
来源：http://m.share.epnwcf.com/Article/details/ggmjdfoby.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fktsv.cn/Article/details/gpadtdack.sHtML

[Q55] 排名（并列占位）
来源：http://wap.tarul.cn/Article/details/gbfhelwdh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.epnwcf.com/Article/details/ggivksose.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.tarul.cn/Article/details/gxtetpcih.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fktsv.cn/Article/details/grotctiqi.sHtML

[Q57] 行号
来源：http://m.share.yfazqb.com/Article/details/gmexxitie.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.vehdjk.com/Article/details/gcqpkmejv.sHtML

[Q58] 累计求和
来源：http://www.blog.sjlbkw.cn/Article/details/gylvymzaj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.bbcook.cn/Article/details/gmhpdjiti.sHtML

[Q59] 分组内累计
来源：http://m.share.tarul.cn/Article/details/gkxxywikm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.sjlbkw.cn/Article/details/gnhyzbsqz.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/gcdqpoddf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.bbcook.cn/Article/details/gdpwfjegx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.epnwcf.com/Article/details/glxlljxfj.sHtML


<!-- 参考信息 -->