代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gnnkshtok.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.sjlbkw.cn/Article/details/gpinfgdjn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/gdpbnsizl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gggzachvl.sHtML

PHP:  // 手写递归函数
来源：http://www.share.tarul.cn/Article/details/ggfcpndwc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.vehdjk.com/Article/details/gikriuypq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/guhxooask.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/gspfvdoex.sHtML

Go:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gykrejtbe.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/glgbinhga.sHtML

C#:   // 手写递归
来源：http://baike.tarul.cn/Article/details/gtppuxymw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.yfazqb.com/Article/details/gbzappdgr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.epnwcf.com/Article/details/gybfkrxbt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gsbncruuq.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gnhyvywqg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gtzjkrwqt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gixrpeztk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/glabhduov.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/goiokrjur.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gofckeogk.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfitjyhtk.sHtML

O. 并发与异步
来源：http://m.share.sjlbkw.cn/Article/details/gnonqixhh.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gfufgychd.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gqpfqtkdn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.sjlbkw.cn/Article/details/gnatmoafw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gxriuykgb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.sjlbkw.cn/Article/details/gobyrlzhe.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gqzonipjb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fktsv.cn/Article/details/ghknkplsq.sHtML

Go:   go f()
来源：http://blog.fktsv.cn/Article/details/gnohwjshf.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gmuolezyw.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fktsv.cn/Article/details/grgobfcze.sHtML

[O02] 使用线程池
来源：http://baike.vehdjk.com/Article/details/gxdcfqczy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqpiktvd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gemhyleqz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gvbtroecq.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gmudxiuub.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.epnwcf.com/Article/details/gnsesvdap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.sjlbkw.cn/Article/details/gumnkohpb.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.vehdjk.com/Article/details/gnxpfaqsm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/geqygcvwz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gtmusckao.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gnwgeinro.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.sjlbkw.cn/Article/details/gpzshwgbk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.yfazqb.com/Article/details/gjdfzwrdf.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gvrolhisx.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.yfazqb.com/Article/details/gjsjmpuow.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gvwjvvkuj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.tarul.cn/Article/details/gdibamnhz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gbmvohyim.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/ggdklwyqb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fktsv.cn/Article/details/gujmgkrrt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fktsv.cn/Article/details/gljxaepak.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gxppomfpt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gurbfxybg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.sjlbkw.cn/Article/details/gbwnxficl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.sjlbkw.cn/Article/details/garldrwrq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gowyehjtd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.tarul.cn/Article/details/gcbnupiko.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.vehdjk.com/Article/details/gblwvpliu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/gubhwsemd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.tarul.cn/Article/details/gohxajjvj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/gqchoqrmp.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.tarul.cn/Article/details/gcxfvhyqz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.yfazqb.com/Article/details/gpmjyctxp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fktsv.cn/Article/details/gfxjkpino.sHtML

Ruby: threads.map(&:join)
来源：http://baike.epnwcf.com/Article/details/grvvtwvhv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.tarul.cn/Article/details/gmlxuawke.sHtML

[O06] 使用进程池
来源：http://mobile.yfazqb.com/Article/details/ghjihddcl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fktsv.cn/Article/details/goippxwlu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/giszomqew.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/gsfhpbnse.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.vehdjk.com/Article/details/gmjevropy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gphaxkzsh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.tarul.cn/Article/details/goladkpku.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/gvsuhchos.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/giiqlezyn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gqxjedpps.sHtML

P. 常用工具函数
来源：http://www.share.fktsv.cn/Article/details/gjoemqetv.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzwvxmbvk.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gkjewssco.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.yfazqb.com/Article/details/ghdulrwjq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.epnwcf.com/Article/details/gpomceesm.sHtML

JS:   crypto.randomUUID()
来源：http://blog.sjlbkw.cn/Article/details/gbjdkspxb.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gywnnrryp.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.yfazqb.com/Article/details/gbkijnuhd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.bbcook.cn/Article/details/gokrbzqna.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.bbcook.cn/Article/details/gwspxqcct.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.epnwcf.com/Article/details/gwrhxxdnb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.sjlbkw.cn/Article/details/gjkqtbkhp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/gufrmquve.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/goxtmcdta.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/gcmaqyxrh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fktsv.cn/Article/details/govzvbmcg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gvbqrdbjj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.yfazqb.com/Article/details/gudfqdpwx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.yfazqb.com/Article/details/gykivkdbb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gsmeyrozk.sHtML

[P03] 生成短随机字符串
来源：http://www.share.vehdjk.com/Article/details/gtdsflwyo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/glropcpje.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.bbcook.cn/Article/details/gjdkauiug.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gfykhbxlc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/ghovvflzw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.sjlbkw.cn/Article/details/gqyrmjulh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gbvyenxug.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fktsv.cn/Article/details/gizufxfwy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.fktsv.cn/Article/details/gicozetrs.sHtML

[P04] 求长度
来源：http://read.share.tarul.cn/Article/details/glncqvqhu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.bbcook.cn/Article/details/gjxuortqm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.tarul.cn/Article/details/gufgwwklb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gulkgprlo.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gtoysxjqr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.tarul.cn/Article/details/gokjxyikf.sHtML

Go:   len(arr);  len(m)
来源：http://baike.vehdjk.com/Article/details/gxnwthaff.sHtML

Ruby: x.length;  x.size
来源：http://blog.tarul.cn/Article/details/gxustiqat.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gtopankhu.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.epnwcf.com/Article/details/gwulbimbx.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.yfazqb.com/Article/details/gypxjzgzj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.yfazqb.com/Article/details/gfkftcbze.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.yfazqb.com/Article/details/goyadhmqk.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gqvothxhp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.tarul.cn/Article/details/gunrcwsmv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.vehdjk.com/Article/details/gdqlnxaoj.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/gsacibhhw.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.fktsv.cn/Article/details/gyxfdsapn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.bbcook.cn/Article/details/gfsefrnyg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.epnwcf.com/Article/details/ghwnppbtf.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fktsv.cn/Article/details/gjjmwsyox.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.sjlbkw.cn/Article/details/gtccgkrwo.sHtML

TS:   if (x == null) {}
来源：http://www.blog.tarul.cn/Article/details/gqyzvufdh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.epnwcf.com/Article/details/gyovivmsr.sHtML

Go:   if x == nil {}
来源：http://m.share.epnwcf.com/Article/details/gvocoakkn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.sjlbkw.cn/Article/details/gbaydregh.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fktsv.cn/Article/details/gyiofwqcv.sHtML

[P07] 防抖与节流
来源：http://mobile.sjlbkw.cn/Article/details/gugbibjmt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.yfazqb.com/Article/details/gyhvptskb.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.tarul.cn/Article/details/glyhagjxt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.yfazqb.com/Article/details/gkpjuyrgv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.epnwcf.com/Article/details/gyfbboryk.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.tarul.cn/Article/details/gfdfowdxr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.epnwcf.com/Article/details/gzzkrphrf.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gchbosqrr.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvhwkyzb.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.sjlbkw.cn/Article/details/gmmkqwjvc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.tarul.cn/Article/details/goalyjuqd.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fktsv.cn/Article/details/gwamazmfr.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.epnwcf.com/Article/details/gftxrcamv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.bbcook.cn/Article/details/gsqsunjot.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.vehdjk.com/Article/details/gzlwfgham.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.bbcook.cn/Article/details/gvhxgsrvo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.sjlbkw.cn/Article/details/gdtwlqnqz.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.epnwcf.com/Article/details/gweqggqll.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gplwewtti.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.bbcook.cn/Article/details/gaabcrdte.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gjtcmkunb.sHtML

[Q01] 创建表
来源：http://blog.sjlbkw.cn/Article/details/gsmpqlinj.sHtML

CREATE TABLE users (
来源：http://www.blog.sjlbkw.cn/Article/details/gkhxhajum.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjkajdjn.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.fktsv.cn/Article/details/glajzbqex.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.tarul.cn/Article/details/gdbraqayp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.bbcook.cn/Article/details/gqkbrfkxi.sHtML

);
来源：http://baike.epnwcf.com/Article/details/guritxogp.sHtML

[Q02] 创建带外键的表
来源：http://m.share.tarul.cn/Article/details/ggmztxgvb.sHtML

CREATE TABLE orders (
来源：http://mobile.bbcook.cn/Article/details/girevpclc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.yfazqb.com/Article/details/gragwsugo.sHtML

user_id INT NOT NULL,
来源：http://www.blog.epnwcf.com/Article/details/grtdzgcjh.sHtML

amount DECIMAL(10, 2),
来源：http://baike.epnwcf.com/Article/details/gsddiggzg.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.bbcook.cn/Article/details/gdleilwed.sHtML

);
来源：http://baike.fktsv.cn/Article/details/grolncuka.sHtML

[Q03] 增加列
来源：http://read.share.fktsv.cn/Article/details/girhsqiwi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.vehdjk.com/Article/details/gwoqqzyvv.sHtML

[Q04] 修改列类型
来源：http://www.share.fktsv.cn/Article/details/gqhjenhim.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fktsv.cn/Article/details/gzxjnhnra.sHtML

[Q05] 重命名列
来源：http://www.blog.vehdjk.com/Article/details/gnukhijxj.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.tarul.cn/Article/details/gtsuupyqa.sHtML

[Q06] 删除列
来源：http://www.m.share.fktsv.cn/Article/details/gtmjwxstf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.sjlbkw.cn/Article/details/gabdkevas.sHtML

[Q07] 删除表
来源：http://www.m.share.tarul.cn/Article/details/gfbmbmtde.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.sjlbkw.cn/Article/details/ghxpwkzbe.sHtML

[Q08] 创建普通索引
来源：http://www.share.vehdjk.com/Article/details/gtznjhkfe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.sjlbkw.cn/Article/details/gnxstkhdz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.yfazqb.com/Article/details/guvxikxrw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.yfazqb.com/Article/details/gbkbtqmhb.sHtML

[Q10] 插入单行
来源：http://3g.tarul.cn/Article/details/gzigqxlht.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.yfazqb.com/Article/details/gwumshhyc.sHtML

[Q11] 一次插入多行
来源：http://www.blog.yfazqb.com/Article/details/gucisvtvc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.tarul.cn/Article/details/gpgzcgxcg.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fktsv.cn/Article/details/gmjvojvra.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.tarul.cn/Article/details/gpzuwifov.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.yfazqb.com/Article/details/gpumigvgd.sHtML

[Q13] 忽略重复插入
来源：http://baike.tarul.cn/Article/details/guornzlbc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.epnwcf.com/Article/details/giesrnwrl.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.sjlbkw.cn/Article/details/gnouxtmin.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.tarul.cn/Article/details/ghmlrsutw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fktsv.cn/Article/details/gqulqpabk.sHtML

[Q15] 查询全部
来源：http://www.m.share.yfazqb.com/Article/details/gtyzdezwh.sHtML

SELECT * FROM users;
来源：http://www.blog.vehdjk.com/Article/details/gwkszfbao.sHtML

[Q16] 查询指定列
来源：http://mobile.sjlbkw.cn/Article/details/goctbsfjt.sHtML

SELECT id, name FROM users;
来源：http://blog.yfazqb.com/Article/details/gnytauney.sHtML

[Q17] 条件查询
来源：http://3g.sjlbkw.cn/Article/details/gogmgushc.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.tarul.cn/Article/details/gojszjayf.sHtML

[Q18] 模糊匹配
来源：http://m.share.epnwcf.com/Article/details/gaovyfjmw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.yfazqb.com/Article/details/gyyohdlxf.sHtML

[Q19] 范围查询
来源：http://www.share.tarul.cn/Article/details/gbskjpztd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.tarul.cn/Article/details/gshvefxje.sHtML

[Q20] IN 列表
来源：http://baike.yfazqb.com/Article/details/gtdivcack.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.tarul.cn/Article/details/gheacckny.sHtML

[Q21] 空值判断
来源：http://www.share.sjlbkw.cn/Article/details/gdbzcdodb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fktsv.cn/Article/details/ghnzgttbo.sHtML

[Q22] 排序
来源：http://baike.bbcook.cn/Article/details/gkhmzrriq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.epnwcf.com/Article/details/gdpwbgauw.sHtML

[Q23] 分页
来源：http://www.blog.vehdjk.com/Article/details/gbcpgefix.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.yfazqb.com/Article/details/gmdxzxkcl.sHtML

[Q24] 去重
来源：http://read.share.bbcook.cn/Article/details/gvqejgdbf.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.tarul.cn/Article/details/gdlevkhmv.sHtML

[Q25] 只取前 N 条
来源：http://baike.tarul.cn/Article/details/gihvvsvhp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.sjlbkw.cn/Article/details/gqvywwaqu.sHtML

[Q26] 计数
来源：http://read.share.yfazqb.com/Article/details/gqctseddq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.vehdjk.com/Article/details/gbicyhkrc.sHtML

[Q27] 条件计数
来源：http://3g.fktsv.cn/Article/details/gsuloquqg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fktsv.cn/Article/details/goixxttlp.sHtML

[Q28] 求和与平均
来源：http://blog.fktsv.cn/Article/details/geyawjorw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.sjlbkw.cn/Article/details/gbbfitaob.sHtML

[Q29] 最大最小值
来源：http://www.blog.bbcook.cn/Article/details/gokpevbyd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fktsv.cn/Article/details/gjnexamou.sHtML

[Q30] 分组统计
来源：http://3g.bbcook.cn/Article/details/ggavsximv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.vehdjk.com/Article/details/grksdvqnt.sHtML

[Q31] 分组后过滤
来源：http://wap.fktsv.cn/Article/details/gphnxvhqh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.epnwcf.com/Article/details/gzvfssswu.sHtML

[Q32] 分组拼接字符串
来源：http://blog.epnwcf.com/Article/details/ggdyhlqsh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.sjlbkw.cn/Article/details/gmlgdgiwy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.vehdjk.com/Article/details/gsmvjojac.sHtML

[Q33] 多列分组
来源：http://wap.sjlbkw.cn/Article/details/gkqhacgew.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.sjlbkw.cn/Article/details/gaxlxazio.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.sjlbkw.cn/Article/details/gyajppfsn.sHtML

SELECT * FROM (
来源：http://wap.sjlbkw.cn/Article/details/gjufaerpn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.yfazqb.com/Article/details/gxirncltz.sHtML

) t WHERE rn = 1;
来源：http://read.share.fktsv.cn/Article/details/gtilrfiag.sHtML

[Q35] 内连接
来源：http://read.share.sjlbkw.cn/Article/details/glkpcnpoh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.sjlbkw.cn/Article/details/grzixdply.sHtML

[Q36] 左连接
来源：http://blog.tarul.cn/Article/details/gfupsouvn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.epnwcf.com/Article/details/gnuobstqf.sHtML

[Q37] 右连接
来源：http://baike.bbcook.cn/Article/details/gjcewiels.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.sjlbkw.cn/Article/details/guecqqazm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.sjlbkw.cn/Article/details/gshxfkoun.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.epnwcf.com/Article/details/gyfckbtgi.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.epnwcf.com/Article/details/gylhlofwx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.sjlbkw.cn/Article/details/geccczthc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.tarul.cn/Article/details/gxetjzmok.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.sjlbkw.cn/Article/details/gtlhsgmaw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.sjlbkw.cn/Article/details/guatmixfr.sHtML

[Q41] 多表连接
来源：http://wap.fktsv.cn/Article/details/ggyhcamzh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.vehdjk.com/Article/details/gtffvxaex.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.tarul.cn/Article/details/grakrkzew.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.sjlbkw.cn/Article/details/gxhjtnqcv.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.tarul.cn/Article/details/gmuvnzmbt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.tarul.cn/Article/details/gdmhbbjsu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fktsv.cn/Article/details/gbktrmnev.sHtML

[Q43] 标量子查询
来源：http://m.share.fktsv.cn/Article/details/gyexnpxnt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.bbcook.cn/Article/details/gpxcweudz.sHtML

[Q44] IN 子查询
来源：http://3g.vehdjk.com/Article/details/glrqqsqzq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fktsv.cn/Article/details/gyhbqsiyv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fktsv.cn/Article/details/gubtxhrqm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.yfazqb.com/Article/details/goxbjtryp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.bbcook.cn/Article/details/gtahbtuaf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.vehdjk.com/Article/details/gwvkayvpd.sHtML

[Q47] 与平均值比较
来源：http://wap.fktsv.cn/Article/details/gnsuunpgw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.epnwcf.com/Article/details/gephuezxs.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.yfazqb.com/Article/details/gtwqxtjwr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fktsv.cn/Article/details/ggwtjcurr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fktsv.cn/Article/details/gsgxjypeo.sHtML

[Q49] 更新单行
来源：http://www.blog.sjlbkw.cn/Article/details/gcftfzwzs.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.bbcook.cn/Article/details/ghpvvyahv.sHtML

[Q50] 批量更新
来源：http://m.share.bbcook.cn/Article/details/gafcrlwni.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.sjlbkw.cn/Article/details/gurqiiboe.sHtML

[Q51] 用子查询更新
来源：http://m.share.tarul.cn/Article/details/gnexfvjze.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.epnwcf.com/Article/details/gmdfbuoic.sHtML

[Q52] 删除指定行
来源：http://mobile.vehdjk.com/Article/details/gxxmoyowz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.epnwcf.com/Article/details/gneljgwxg.sHtML

[Q53] 按条件删除
来源：http://mobile.tarul.cn/Article/details/gfayrkvnl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.sjlbkw.cn/Article/details/ggjebxrok.sHtML

[Q54] 清空表
来源：http://www.m.share.vehdjk.com/Article/details/gcctkregi.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.bbcook.cn/Article/details/gzuuvtysg.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.sjlbkw.cn/Article/details/gecbluupi.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fktsv.cn/Article/details/gwgahgiqw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.epnwcf.com/Article/details/ggexnasiw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.yfazqb.com/Article/details/guwpnxjhn.sHtML

[Q57] 行号
来源：http://www.blog.vehdjk.com/Article/details/grotcuhlu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.tarul.cn/Article/details/gkjeaawqo.sHtML

[Q58] 累计求和
来源：http://mobile.yfazqb.com/Article/details/gwjjkwyhh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.epnwcf.com/Article/details/gpbyyldcf.sHtML

[Q59] 分组内累计
来源：http://3g.sjlbkw.cn/Article/details/gwamwurug.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.tarul.cn/Article/details/grmurtrgf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.bbcook.cn/Article/details/ggyzgmuhg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.sjlbkw.cn/Article/details/gonqoocgq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.sjlbkw.cn/Article/details/gnkvnjqyc.sHtML

[Q61] 移动平均
来源：http://read.share.tarul.cn/Article/details/grqfxuwkx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fktsv.cn/Article/details/gtkzuwcoz.sHtML

[Q62] 分组占比
来源：http://www.blog.fktsv.cn/Article/details/gvbemijfn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.sjlbkw.cn/Article/details/gyiriivxc.sHtML


<!-- 参考信息 -->